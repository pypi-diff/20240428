# Comparing `tmp/portage-3.0.63.tar.gz` & `tmp/portage-3.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portage-3.0.63.tar", last modified: Sun Feb 25 08:31:18 2024, max compression
+gzip compressed data, was "portage-3.0.64.tar", last modified: Sun Apr 28 00:35:13 2024, max compression
```

## Comparing `portage-3.0.63.tar` & `portage-3.0.64.tar`

### file list

```diff
@@ -1,998 +1,997 @@
--rw-r--r--   0        0        0     1857 2024-02-25 08:29:43.000000 portage-3.0.63/.builds/ci.yml
--rw-r--r--   0        0        0     1071 2024-02-25 08:29:43.000000 portage-3.0.63/.builds/lint.yml
--rwxr-xr-x   0        0        0      766 2024-02-25 08:29:43.000000 portage-3.0.63/.builds/setup-python.sh
--rw-r--r--   0        0        0      294 2024-02-25 08:29:43.000000 portage-3.0.63/.editorconfig
--rw-r--r--   0        0        0      618 2024-02-25 08:29:43.000000 portage-3.0.63/.git-blame-ignore-revs
--rw-r--r--   0        0        0     3778 2024-02-25 08:29:43.000000 portage-3.0.63/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1257 2024-02-25 08:29:43.000000 portage-3.0.63/.github/workflows/lint.yml
--rw-r--r--   0        0        0      231 2024-02-25 08:29:43.000000 portage-3.0.63/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      116 2024-02-25 08:29:43.000000 portage-3.0.63/.gitignore
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/.portage_not_installed
--rw-r--r--   0        0        0      456 2024-02-25 08:29:43.000000 portage-3.0.63/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1840 2024-02-25 08:29:43.000000 portage-3.0.63/COPYING
--rw-r--r--   0        0        0     7201 2024-02-25 08:29:43.000000 portage-3.0.63/DEVELOPING
--rw-r--r--   0        0        0    18092 2024-02-25 08:29:43.000000 portage-3.0.63/LICENSE
--rw-r--r--   0        0        0    71724 2024-02-25 08:29:43.000000 portage-3.0.63/NEWS
--rw-r--r--   0        0        0     3559 2024-02-25 08:29:43.000000 portage-3.0.63/README.md
--rw-r--r--   0        0        0    84461 2024-02-25 08:29:43.000000 portage-3.0.63/RELEASE-NOTES
--rw-r--r--   0        0        0     1848 2024-02-25 08:29:43.000000 portage-3.0.63/TEST-NOTES
--rwxr-xr-x   0        0        0     3262 2024-02-25 08:29:43.000000 portage-3.0.63/bin/archive-conf
--rw-r--r--   0        0        0     1443 2024-02-25 08:29:43.000000 portage-3.0.63/bin/bashrc-functions.sh
--rwxr-xr-x   0        0        0     4457 2024-02-25 08:29:43.000000 portage-3.0.63/bin/binhost-snapshot
--rwxr-xr-x   0        0        0      618 2024-02-25 08:31:17.195731 portage-3.0.63/bin/chmod-lite
--rwxr-xr-x   0        0        0      951 2024-02-25 08:29:43.000000 portage-3.0.63/bin/chmod-lite.py
--rwxr-xr-x   0        0        0     5891 2024-02-25 08:29:43.000000 portage-3.0.63/bin/chpathtool.py
--rwxr-xr-x   0        0        0     1421 2024-02-25 08:29:43.000000 portage-3.0.63/bin/clean_locks
--rwxr-xr-x   0        0        0    20957 2024-02-25 08:29:43.000000 portage-3.0.63/bin/dispatch-conf
--rwxr-xr-x   0        0        0     8895 2024-02-25 08:29:43.000000 portage-3.0.63/bin/dohtml.py
--rw-r--r--   0        0        0    20007 2024-02-25 08:29:43.000000 portage-3.0.63/bin/doins.py
--rw-r--r--   0        0        0     6078 2024-02-25 08:29:43.000000 portage-3.0.63/bin/eapi.sh
--rw-r--r--   0        0        0     4310 2024-02-25 08:29:43.000000 portage-3.0.63/bin/eapi7-ver-funcs.sh
--rwxr-xr-x   0        0        0    15402 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild
--rwxr-xr-x   0        0        0      639 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/bsd/sed
--rwxr-xr-x   0        0        0      200 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/die
--rwxr-xr-x   0        0        0     1049 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dobin
--rwxr-xr-x   0        0        0      515 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/doconfd
--rwxr-xr-x   0        0        0      359 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dodir
--rwxr-xr-x   0        0        0      885 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dodoc
--rwxr-xr-x   0        0        0      513 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/doenvd
--rwxr-xr-x   0        0        0      952 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/doexe
--rwxr-xr-x   0        0        0      531 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dohard
--rwxr-xr-x   0        0        0      632 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/doheader
--rwxr-xr-x   0        0        0      793 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dohtml
--rwxr-xr-x   0        0        0      722 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/doinfo
--rwxr-xr-x   0        0        0      485 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/doinitd
--rwxr-xr-x   0        0        0     3034 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/doins
--rwxr-xr-x   0        0        0     1333 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dolib
--rwxr-xr-x   0        0        0      189 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dolib.a
--rwxr-xr-x   0        0        0      189 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dolib.so
--rwxr-xr-x   0        0        0     1553 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/doman
--rwxr-xr-x   0        0        0     1216 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/domo
--rwxr-xr-x   0        0        0     1053 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dosbin
--rwxr-xr-x   0        0        0      818 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dosed
--rwxr-xr-x   0        0        0     2411 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/dosym
--rwxr-xr-x   0        0        0      204 2024-02-25 08:31:17.197731 portage-3.0.63/bin/ebuild-helpers/eerror
--rwxr-xr-x   0        0        0      204 2024-02-25 08:31:17.197731 portage-3.0.63/bin/ebuild-helpers/einfo
--rwxr-xr-x   0        0        0      204 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/elog
--rwxr-xr-x   0        0        0      894 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/emake
--rwxr-xr-x   0        0        0      204 2024-02-25 08:31:17.197731 portage-3.0.63/bin/ebuild-helpers/eqawarn
--rwxr-xr-x   0        0        0      204 2024-02-25 08:31:17.197731 portage-3.0.63/bin/ebuild-helpers/ewarn
--rwxr-xr-x   0        0        0      882 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/fowners
--rwxr-xr-x   0        0        0      949 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/fperms
--rwxr-xr-x   0        0        0      490 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/keepdir
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newbin
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newconfd
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newdoc
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newenvd
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newexe
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newheader
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newinitd
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/newins
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newlib.a
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newlib.so
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newman
--rwxr-xr-x   0        0        0     1201 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/newsbin
--rwxr-xr-x   0        0        0      359 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/nonfatal
--rwxr-xr-x   0        0        0      242 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/prepall
--rwxr-xr-x   0        0        0      242 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/prepalldocs
--rwxr-xr-x   0        0        0      242 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/prepallinfo
--rwxr-xr-x   0        0        0      242 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/prepallman
--rwxr-xr-x   0        0        0      242 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/prepallstrip
--rwxr-xr-x   0        0        0      242 2024-02-25 08:31:17.198732 portage-3.0.63/bin/ebuild-helpers/prepinfo
--rwxr-xr-x   0        0        0      242 2024-02-25 08:31:17.199731 portage-3.0.63/bin/ebuild-helpers/prepman
--rwxr-xr-x   0        0        0      242 2024-02-25 08:31:17.199731 portage-3.0.63/bin/ebuild-helpers/prepstrip
--rwxr-xr-x   0        0        0     1178 2024-02-25 08:31:17.199731 portage-3.0.63/bin/ebuild-helpers/unprivileged/chgrp
--rwxr-xr-x   0        0        0     1178 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/unprivileged/chown
--rwxr-xr-x   0        0        0     1369 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-helpers/xattr/install
--rwxr-xr-x   0        0        0      618 2024-02-25 08:31:17.199731 portage-3.0.63/bin/ebuild-ipc
--rwxr-xr-x   0        0        0    10684 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-ipc.py
--rwxr-xr-x   0        0        0      618 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild-pyhelper
--rwxr-xr-x   0        0        0    26179 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ebuild.sh
--rwxr-xr-x   0        0        0     6481 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ecompress
--rwxr-xr-x   0        0        0     1746 2024-02-25 08:29:43.000000 portage-3.0.63/bin/ecompress-file
--rwxr-xr-x   0        0        0    53990 2024-02-25 08:29:43.000000 portage-3.0.63/bin/egencache
--rwxr-xr-x   0        0        0     2151 2024-02-25 08:29:43.000000 portage-3.0.63/bin/emaint
--rwxr-xr-x   0        0        0     3297 2024-02-25 08:29:43.000000 portage-3.0.63/bin/emerge
--rwxr-xr-x   0        0        0    21009 2024-02-25 08:29:43.000000 portage-3.0.63/bin/emerge-webrsync
--rwxr-xr-x   0        0        0      634 2024-02-25 08:29:43.000000 portage-3.0.63/bin/emirrordist
--rwxr-xr-x   0        0        0     1107 2024-02-25 08:29:43.000000 portage-3.0.63/bin/env-update
--rwxr-xr-x   0        0        0    18168 2024-02-25 08:29:43.000000 portage-3.0.63/bin/estrip
--rwxr-xr-x   0        0        0    23706 2024-02-25 08:29:43.000000 portage-3.0.63/bin/etc-update
--rwxr-xr-x   0        0        0     6045 2024-02-25 08:29:43.000000 portage-3.0.63/bin/filter-bash-environment.py
--rwxr-xr-x   0        0        0     1754 2024-02-25 08:29:43.000000 portage-3.0.63/bin/fixpackages
--rwxr-xr-x   0        0        0    15636 2024-02-25 08:29:43.000000 portage-3.0.63/bin/glsa-check
--rwxr-xr-x   0        0        0     2166 2024-02-25 08:29:43.000000 portage-3.0.63/bin/gpkg-helper.py
--rwxr-xr-x   0        0        0     2476 2024-02-25 08:29:43.000000 portage-3.0.63/bin/gpkg-sign
--rw-r--r--   0        0        0     2918 2024-02-25 08:29:43.000000 portage-3.0.63/bin/helper-functions.sh
--rw-r--r--   0        0        0      443 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/05double-D
--rw-r--r--   0        0        0     4376 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/05prefix
--rw-r--r--   0        0        0     5559 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/10executable-issues
--rw-r--r--   0        0        0     3591 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/10ignored-flags
--rw-r--r--   0        0        0      406 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/20deprecated-directories
--rw-r--r--   0        0        0      835 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/20runtime-directories
--rw-r--r--   0        0        0     3328 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/60bash-completion
--rw-r--r--   0        0        0     1450 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/60openrc
--rw-r--r--   0        0        0     5508 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/60pkgconfig
--rw-r--r--   0        0        0      668 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/60pngfix
--rw-r--r--   0        0        0      687 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/60systemd
--rw-r--r--   0        0        0      442 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/60udev
--rw-r--r--   0        0        0     5556 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/80libraries
--rw-r--r--   0        0        0     1417 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/80multilib-strict
--rw-r--r--   0        0        0     1929 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/90bad-bin-group-write
--rw-r--r--   0        0        0     1577 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/90bad-bin-owner
--rw-r--r--   0        0        0      665 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/90cmake-warnings
--rw-r--r--   0        0        0     3995 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/90config-impl-decl
--rw-r--r--   0        0        0     1277 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/90cython-dep
--rw-r--r--   0        0        0     8742 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/90gcc-warnings
--rw-r--r--   0        0        0     1033 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/90world-writable
--rw-r--r--   0        0        0     1529 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install-qa-check.d/95empty-dirs
--rwxr-xr-x   0        0        0     6314 2024-02-25 08:29:43.000000 portage-3.0.63/bin/install.py
--rw-r--r--   0        0        0    18552 2024-02-25 08:29:43.000000 portage-3.0.63/bin/isolated-functions.sh
--rwxr-xr-x   0        0        0      903 2024-02-25 08:29:43.000000 portage-3.0.63/bin/lock-helper.py
--rw-r--r--   0        0        0     1633 2024-02-25 08:29:43.000000 portage-3.0.63/bin/meson.build
--rwxr-xr-x   0        0        0    19740 2024-02-25 08:29:43.000000 portage-3.0.63/bin/misc-functions.sh
--rw-r--r--   0        0        0    34672 2024-02-25 08:29:43.000000 portage-3.0.63/bin/phase-functions.sh
--rw-r--r--   0        0        0    33960 2024-02-25 08:29:43.000000 portage-3.0.63/bin/phase-helpers.sh
--rw-r--r--   0        0        0     5723 2024-02-25 08:29:43.000000 portage-3.0.63/bin/pid-ns-init
--rwxr-xr-x   0        0        0    51197 2024-02-25 08:29:43.000000 portage-3.0.63/bin/portageq
--rwxr-xr-x   0        0        0      550 2024-02-25 08:29:43.000000 portage-3.0.63/bin/portageq-wrapper
--rw-r--r--   0        0        0     5236 2024-02-25 08:29:43.000000 portage-3.0.63/bin/postinst-qa-check.d/50xdg-utils
--rw-r--r--   0        0        0     5236 2024-02-25 08:31:17.202731 portage-3.0.63/bin/preinst-qa-check.d/50xdg-utils
--rwxr-xr-x   0        0        0    16797 2024-02-25 08:29:43.000000 portage-3.0.63/bin/quickpkg
--rwxr-xr-x   0        0        0     4992 2024-02-25 08:29:43.000000 portage-3.0.63/bin/regenworld
--rw-r--r--   0        0        0     4642 2024-02-25 08:29:43.000000 portage-3.0.63/bin/save-ebuild-env.sh
--rwxr-xr-x   0        0        0     1339 2024-02-25 08:29:43.000000 portage-3.0.63/bin/shelve-utils
--rw-r--r--   0        0        0     8037 2024-02-25 08:29:43.000000 portage-3.0.63/bin/socks5-server.py
--rwxr-xr-x   0        0        0     4784 2024-02-25 08:29:43.000000 portage-3.0.63/bin/xattr-helper.py
--rwxr-xr-x   0        0        0     1825 2024-02-25 08:29:43.000000 portage-3.0.63/bin/xpak-helper.py
--rw-r--r--   0        0        0     2314 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/dispatch-conf.conf
--rw-r--r--   0        0        0     2000 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/etc-update.conf
--rw-r--r--   0        0        0      272 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/logrotate.d/elog-save-summary
--rw-r--r--   0        0        0    20487 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example
--rw-r--r--   0        0        0     1718 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.alpha.diff
--rw-r--r--   0        0        0     2319 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.amd64-fbsd.diff
--rw-r--r--   0        0        0     2309 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.amd64.diff
--rw-r--r--   0        0        0     1425 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.arc.diff
--rw-r--r--   0        0        0     1592 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.arm.diff
--rw-r--r--   0        0        0     1580 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.arm64.diff
--rw-r--r--   0        0        0     2465 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.hppa.diff
--rw-r--r--   0        0        0      663 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.ia64.diff
--rw-r--r--   0        0        0     2192 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.loong.diff
--rw-r--r--   0        0        0      900 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.m68k.diff
--rw-r--r--   0        0        0     1383 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.mips.diff
--rw-r--r--   0        0        0     3541 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.ppc.diff
--rw-r--r--   0        0        0     2361 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.ppc64.diff
--rw-r--r--   0        0        0     2332 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.riscv.diff
--rw-r--r--   0        0        0      656 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.s390.diff
--rw-r--r--   0        0        0     1257 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.sh.diff
--rw-r--r--   0        0        0      728 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.sparc-fbsd.diff
--rw-r--r--   0        0        0     2129 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.sparc.diff
--rw-r--r--   0        0        0     2507 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.x86-fbsd.diff
--rw-r--r--   0        0        0     3759 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.conf.example.x86.diff
--rw-r--r--   0        0        0     7661 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/make.globals
--rw-r--r--   0        0        0     3193 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/meson.build
--rw-r--r--   0        0        0     2311 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/repo.postsync.d/example
--rw-r--r--   0        0        0      640 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/repos.conf
--rw-r--r--   0        0        0     4164 2024-02-25 08:29:43.000000 portage-3.0.63/cnf/sets/portage.conf
--rw-r--r--   0        0        0        7 2024-02-25 08:29:43.000000 portage-3.0.63/doc/api/.gitignore
--rw-r--r--   0        0        0     1141 2024-02-25 08:29:43.000000 portage-3.0.63/doc/api/Makefile
--rw-r--r--   0        0        0     2372 2024-02-25 08:29:43.000000 portage-3.0.63/doc/api/conf.py
--rw-r--r--   0        0        0      217 2024-02-25 08:29:43.000000 portage-3.0.63/doc/api/index.rst
--rw-r--r--   0        0        0     1544 2024-02-25 08:29:43.000000 portage-3.0.63/doc/api/meson.build
--rw-r--r--   0        0        0     1900 2024-02-25 08:29:43.000000 portage-3.0.63/doc/config/bashrc.docbook
--rw-r--r--   0        0        0    26217 2024-02-25 08:29:43.000000 portage-3.0.63/doc/config/sets.docbook
--rw-r--r--   0        0        0       85 2024-02-25 08:29:43.000000 portage-3.0.63/doc/config.docbook
--rw-r--r--   0        0        0      257 2024-02-25 08:29:43.000000 portage-3.0.63/doc/custom.xsl
--rw-r--r--   0        0        0     3281 2024-02-25 08:29:43.000000 portage-3.0.63/doc/dependency_resolution/decision_making.docbook
--rw-r--r--   0        0        0     4154 2024-02-25 08:29:43.000000 portage-3.0.63/doc/dependency_resolution/package_modeling.docbook
--rw-r--r--   0        0        0     3451 2024-02-25 08:29:43.000000 portage-3.0.63/doc/dependency_resolution/task_scheduling.docbook
--rw-r--r--   0        0        0      200 2024-02-25 08:29:43.000000 portage-3.0.63/doc/dependency_resolution.docbook
--rw-r--r--   0        0        0      121 2024-02-25 08:29:43.000000 portage-3.0.63/doc/fragment/meson.build
--rw-r--r--   0        0        0       37 2024-02-25 08:29:43.000000 portage-3.0.63/doc/fragment/version.in
--rw-r--r--   0        0        0     2039 2024-02-25 08:29:43.000000 portage-3.0.63/doc/meson.build
--rw-r--r--   0        0        0      487 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/eapi/0.docbook
--rw-r--r--   0        0        0     1598 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/eapi/1.docbook
--rw-r--r--   0        0        0     8299 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/eapi/2.docbook
--rw-r--r--   0        0        0     2938 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/eapi/3.docbook
--rw-r--r--   0        0        0     3112 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/eapi/4-slot-abi.docbook
--rw-r--r--   0        0        0    14689 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/eapi/4.docbook
--rw-r--r--   0        0        0     8044 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/eapi/5.docbook
--rw-r--r--   0        0        0     1725 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/helper_functions.docbook
--rw-r--r--   0        0        0     2780 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild/phases.docbook
--rw-r--r--   0        0        0      364 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package/ebuild.docbook
--rw-r--r--   0        0        0       76 2024-02-25 08:29:43.000000 portage-3.0.63/doc/package.docbook
--rw-r--r--   0        0        0     2147 2024-02-25 08:29:43.000000 portage-3.0.63/doc/portage.docbook
--rw-r--r--   0        0        0    19581 2024-02-25 08:29:43.000000 portage-3.0.63/doc/qa.docbook
--rw-r--r--   0        0        0      836 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/AbstractDepPriority.py
--rw-r--r--   0        0        0    14502 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/AbstractEbuildProcess.py
--rw-r--r--   0        0        0     3723 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/AbstractPollTask.py
--rw-r--r--   0        0        0     9829 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/AsynchronousLock.py
--rw-r--r--   0        0        0     7098 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/AsynchronousTask.py
--rw-r--r--   0        0        0      473 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/AtomArg.py
--rw-r--r--   0        0        0    22225 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/Binpkg.py
--rw-r--r--   0        0        0     2329 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/BinpkgEnvExtractor.py
--rw-r--r--   0        0        0     5399 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/BinpkgExtractorAsync.py
--rw-r--r--   0        0        0    11117 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/BinpkgFetcher.py
--rw-r--r--   0        0        0     2298 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/BinpkgPrefetcher.py
--rw-r--r--   0        0        0     4908 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/BinpkgVerifier.py
--rw-r--r--   0        0        0      483 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/Blocker.py
--rw-r--r--   0        0        0     6827 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/BlockerCache.py
--rw-r--r--   0        0        0     5325 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/BlockerDB.py
--rw-r--r--   0        0        0      355 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/BlockerDepPriority.py
--rw-r--r--   0        0        0     4228 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/CompositeTask.py
--rw-r--r--   0        0        0     1843 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/DepPriority.py
--rw-r--r--   0        0        0     1856 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/DepPriorityNormalRange.py
--rw-r--r--   0        0        0     4024 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/DepPrioritySatisfiedRange.py
--rw-r--r--   0        0        0      878 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/Dependency.py
--rw-r--r--   0        0        0     1056 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/DependencyArg.py
--rw-r--r--   0        0        0     2663 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildBinpkg.py
--rw-r--r--   0        0        0    23601 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildBuild.py
--rw-r--r--   0        0        0     5749 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildBuildDir.py
--rw-r--r--   0        0        0     2961 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildExecuter.py
--rw-r--r--   0        0        0    14596 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildFetcher.py
--rw-r--r--   0        0        0     1181 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildFetchonly.py
--rw-r--r--   0        0        0     4716 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildIpcDaemon.py
--rw-r--r--   0        0        0     3239 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildMerge.py
--rw-r--r--   0        0        0     8795 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildMetadataPhase.py
--rw-r--r--   0        0        0    23719 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildPhase.py
--rw-r--r--   0        0        0      872 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildProcess.py
--rw-r--r--   0        0        0      679 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/EbuildSpawnProcess.py
--rw-r--r--   0        0        0    12786 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/FakeVartree.py
--rw-r--r--   0        0        0     1774 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/FifoIpcDaemon.py
--rw-r--r--   0        0        0     9142 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/JobStatusDisplay.py
--rw-r--r--   0        0        0     4816 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/MergeListItem.py
--rw-r--r--   0        0        0     6606 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/MetadataRegen.py
--rw-r--r--   0        0        0     2424 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/MiscFunctionsProcess.py
--rw-r--r--   0        0        0    30872 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/Package.py
--rw-r--r--   0        0        0      735 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/PackageArg.py
--rw-r--r--   0        0        0     2626 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/PackageMerge.py
--rw-r--r--   0        0        0     4333 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/PackagePhase.py
--rw-r--r--   0        0        0     5870 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/PackageUninstall.py
--rw-r--r--   0        0        0     4651 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/PackageVirtualDbapi.py
--rw-r--r--   0        0        0     2680 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/PipeReader.py
--rw-r--r--   0        0        0     6709 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/PollScheduler.py
--rw-r--r--   0        0        0      603 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/ProgressHandler.py
--rw-r--r--   0        0        0     1227 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/RootConfig.py
--rw-r--r--   0        0        0    88020 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/Scheduler.py
--rw-r--r--   0        0        0     2648 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/SequentialTaskQueue.py
--rw-r--r--   0        0        0      421 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/SetArg.py
--rw-r--r--   0        0        0     9356 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/SpawnProcess.py
--rw-r--r--   0        0        0     3246 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/SubProcess.py
--rw-r--r--   0        0        0     1478 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/Task.py
--rw-r--r--   0        0        0     1538 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/TaskSequence.py
--rw-r--r--   0        0        0      455 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/UninstallFailure.py
--rw-r--r--   0        0        0     1531 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/UnmergeDepPriority.py
--rw-r--r--   0        0        0     3547 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/UseFlagDisplay.py
--rw-r--r--   0        0        0     2915 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/UserQuery.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/__init__.py
--rw-r--r--   0        0        0     1165 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/_find_deep_system_runtime_deps.py
--rw-r--r--   0        0        0      442 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/_flush_elog_mod_echo.py
--rw-r--r--   0        0        0   149252 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/actions.py
--rw-r--r--   0        0        0     1952 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/chk_updated_cfg_files.py
--rw-r--r--   0        0        0      498 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/clear_caches.py
--rw-r--r--   0        0        0      579 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/countdown.py
--rw-r--r--   0        0        0     9008 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/create_depgraph_params.py
--rw-r--r--   0        0        0     5191 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/create_world_atom.py
--rw-r--r--   0        0        0   516527 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/depgraph.py
--rw-r--r--   0        0        0     1814 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/emergelog.py
--rw-r--r--   0        0        0      958 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/getloadavg.py
--rw-r--r--   0        0        0     3425 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/help.py
--rw-r--r--   0        0        0      785 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/is_valid_package_atom.py
--rw-r--r--   0        0        0    42796 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/main.py
--rw-r--r--   0        0        0     2787 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/meson.build
--rw-r--r--   0        0        0     5614 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/post_emerge.py
--rw-r--r--   0        0        0     3198 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/DbapiProvidesIndex.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/__init__.py
--rw-r--r--   0        0        0    11328 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/backtracking.py
--rw-r--r--   0        0        0    12441 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/circular_dependency.py
--rw-r--r--   0        0        0      310 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/meson.build
--rw-r--r--   0        0        0    39524 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/output.py
--rw-r--r--   0        0        0    20748 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/output_helpers.py
--rw-r--r--   0        0        0    15636 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/package_tracker.py
--rw-r--r--   0        0        0    58875 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/resolver/slot_collision.py
--rw-r--r--   0        0        0    20639 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/search.py
--rw-r--r--   0        0        0     1573 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/show_invalid_depstring_notice.py
--rw-r--r--   0        0        0     3196 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/stdout_spinner.py
--rw-r--r--   0        0        0    26360 2024-02-25 08:29:43.000000 portage-3.0.63/lib/_emerge/unmerge.py
--rw-r--r--   0        0        0       36 2024-02-25 08:29:43.000000 portage-3.0.63/lib/meson.build
--rw-r--r--   0        0        0    26045 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_compat_upgrade/__init__.py
--rw-r--r--   0        0        0     1666 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_compat_upgrade/binpkg_compression.py
--rw-r--r--   0        0        0     1641 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_compat_upgrade/binpkg_format.py
--rw-r--r--   0        0        0     1240 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_compat_upgrade/binpkg_multi_instance.py
--rw-r--r--   0        0        0     4288 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_compat_upgrade/default_locations.py
--rw-r--r--   0        0        0      260 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_compat_upgrade/meson.build
--rw-r--r--   0        0        0     5376 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/Config.py
--rw-r--r--   0        0        0     7215 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/ContentDB.py
--rw-r--r--   0        0        0     4679 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/DeletionIterator.py
--rw-r--r--   0        0        0     5030 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/DeletionTask.py
--rw-r--r--   0        0        0    11319 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/FetchIterator.py
--rw-r--r--   0        0        0    25403 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/FetchTask.py
--rw-r--r--   0        0        0     8831 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/MirrorDistTask.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/__init__.py
--rw-r--r--   0        0        0    15993 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/main.py
--rw-r--r--   0        0        0      331 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_emirrordist/meson.build
--rw-r--r--   0        0        0    10327 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_global_updates.py
--rw-r--r--   0        0        0     2550 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_legacy_globals.py
--rw-r--r--   0        0        0     4819 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_selinux.py
--rw-r--r--   0        0        0     1719 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/ProfilePackageSet.py
--rw-r--r--   0        0        0    14423 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/__init__.py
--rw-r--r--   0        0        0     8205 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/base.py
--rw-r--r--   0        0        0    22046 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/dbapi.py
--rw-r--r--   0        0        0    15995 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/files.py
--rw-r--r--   0        0        0     3602 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/libs.py
--rw-r--r--   0        0        0      297 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/meson.build
--rw-r--r--   0        0        0     2406 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/profiles.py
--rw-r--r--   0        0        0     3535 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/security.py
--rw-r--r--   0        0        0     1442 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/_sets/shell.py
--rw-r--r--   0        0        0     2578 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/binpkg.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/binrepo/__init__.py
--rw-r--r--   0        0        0     4553 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/binrepo/config.py
--rw-r--r--   0        0        0      144 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/binrepo/meson.build
--rw-r--r--   0        0        0      101 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/__init__.py
--rw-r--r--   0        0        0     3710 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/anydbm.py
--rw-r--r--   0        0        0     2139 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/cache_errors.py
--rw-r--r--   0        0        0     5226 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/ebuild_xattr.py
--rw-r--r--   0        0        0     5286 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/flat_hash.py
--rw-r--r--   0        0        0     3197 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/fs_template.py
--rw-r--r--   0        0        0      562 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/index/IndexStreamIterator.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/index/__init__.py
--rw-r--r--   0        0        0      190 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/index/meson.build
--rw-r--r--   0        0        0     1394 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/index/pkg_desc_index.py
--rw-r--r--   0        0        0    11883 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/mappings.py
--rw-r--r--   0        0        0      403 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/meson.build
--rw-r--r--   0        0        0     5844 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/metadata.py
--rw-r--r--   0        0        0    11821 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/sql_template.py
--rw-r--r--   0        0        0    13804 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/sqlite.py
--rw-r--r--   0        0        0    13275 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/template.py
--rw-r--r--   0        0        0      789 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cache/volatile.py
--rw-r--r--   0        0        0    16566 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/checksum.py
--rw-r--r--   0        0        0     9647 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/const.py
--rw-r--r--   0        0        0    11470 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/cvstree.py
--rw-r--r--   0        0        0    11537 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/data.py
--rw-r--r--   0        0        0      643 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/DummyTree.py
--rw-r--r--   0        0        0     5690 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/IndexedPortdb.py
--rw-r--r--   0        0        0     3743 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/IndexedVardb.py
--rw-r--r--   0        0        0     2991 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/_ContentsCaseSensitivityManager.py
--rw-r--r--   0        0        0    11209 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/_MergeProcess.py
--rw-r--r--   0        0        0     1686 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/_SyncfsProcess.py
--rw-r--r--   0        0        0     6019 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/_VdbMetadataDelta.py
--rw-r--r--   0        0        0    17596 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/__init__.py
--rw-r--r--   0        0        0     2545 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/_expand_new_virt.py
--rw-r--r--   0        0        0     1685 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/_similar_name_search.py
--rw-r--r--   0        0        0    97477 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/bintree.py
--rw-r--r--   0        0        0     4184 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/cpv_expand.py
--rw-r--r--   0        0        0     1889 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/dep_expand.py
--rw-r--r--   0        0        0      540 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/meson.build
--rw-r--r--   0        0        0    67024 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/porttree.py
--rw-r--r--   0        0        0   254525 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/vartree.py
--rw-r--r--   0        0        0     7587 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dbapi/virtual.py
--rw-r--r--   0        0        0     3956 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/debug.py
--rw-r--r--   0        0        0   108089 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/__init__.py
--rw-r--r--   0        0        0     3780 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/_dnf.py
--rw-r--r--   0        0        0     4605 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/_slot_operator.py
--rw-r--r--   0        0        0    43041 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/dep_check.py
--rw-r--r--   0        0        0     2612 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/libc.py
--rw-r--r--   0        0        0      228 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/meson.build
--rw-r--r--   0        0        0     2110 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/soname/SonameAtom.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/soname/__init__.py
--rw-r--r--   0        0        0      203 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/soname/meson.build
--rw-r--r--   0        0        0     5311 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/soname/multilib_category.py
--rw-r--r--   0        0        0     1491 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dep/soname/parse.py
--rw-r--r--   0        0        0    14093 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/dispatch_conf.py
--rw-r--r--   0        0        0     8092 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/eapi.py
--rw-r--r--   0        0        0     6757 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/eclass_cache.py
--rw-r--r--   0        0        0     6879 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/__init__.py
--rw-r--r--   0        0        0      613 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/filtering.py
--rw-r--r--   0        0        0      348 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/meson.build
--rw-r--r--   0        0        0     6065 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/messages.py
--rw-r--r--   0        0        0      968 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/mod_custom.py
--rw-r--r--   0        0        0     2401 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/mod_echo.py
--rw-r--r--   0        0        0     1660 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/mod_mail.py
--rw-r--r--   0        0        0     3183 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/mod_mail_summary.py
--rw-r--r--   0        0        0     3396 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/mod_save.py
--rw-r--r--   0        0        0     3580 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/mod_save_summary.py
--rw-r--r--   0        0        0      974 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/elog/mod_syslog.py
--rw-r--r--   0        0        0      163 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/__init__.py
--rw-r--r--   0        0        0      762 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/defaults.py
--rw-r--r--   0        0        0     8705 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/main.py
--rw-r--r--   0        0        0      183 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/meson.build
--rw-r--r--   0        0        0      173 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/__init__.py
--rw-r--r--   0        0        0      524 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/binhost/__init__.py
--rw-r--r--   0        0        0     6358 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/binhost/binhost.py
--rw-r--r--   0        0        0      160 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/binhost/meson.build
--rw-r--r--   0        0        0      534 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/config/__init__.py
--rw-r--r--   0        0        0     2520 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/config/config.py
--rw-r--r--   0        0        0      158 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/config/meson.build
--rw-r--r--   0        0        0     1629 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/logs/__init__.py
--rw-r--r--   0        0        0     3535 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/logs/logs.py
--rw-r--r--   0        0        0      154 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/logs/meson.build
--rw-r--r--   0        0        0     1417 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/merges/__init__.py
--rw-r--r--   0        0        0     9897 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/merges/merges.py
--rw-r--r--   0        0        0      158 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/merges/meson.build
--rw-r--r--   0        0        0      261 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/meson.build
--rw-r--r--   0        0        0      851 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/move/__init__.py
--rw-r--r--   0        0        0      154 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/move/meson.build
--rw-r--r--   0        0        0     7693 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/move/move.py
--rw-r--r--   0        0        0      566 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/resume/__init__.py
--rw-r--r--   0        0        0      158 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/resume/meson.build
--rw-r--r--   0        0        0     1900 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/resume/resume.py
--rw-r--r--   0        0        0     2145 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/sync/__init__.py
--rw-r--r--   0        0        0      154 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/sync/meson.build
--rw-r--r--   0        0        0    18470 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/sync/sync.py
--rw-r--r--   0        0        0      502 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/world/__init__.py
--rw-r--r--   0        0        0      156 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/world/meson.build
--rw-r--r--   0        0        0     3109 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/emaint/modules/world/world.py
--rw-r--r--   0        0        0       52 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/env/__init__.py
--rw-r--r--   0        0        0     3054 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/env/config.py
--rw-r--r--   0        0        0    10311 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/env/loaders.py
--rw-r--r--   0        0        0      187 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/env/meson.build
--rw-r--r--   0        0        0      578 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/env/validators.py
--rw-r--r--   0        0        0     6867 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/exception.py
--rw-r--r--   0        0        0    31465 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/getbinpkg.py
--rw-r--r--   0        0        0    31427 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/glsa.py
--rw-r--r--   0        0        0     3819 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/gpg.py
--rw-r--r--   0        0        0    78541 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/gpkg.py
--rw-r--r--   0        0        0      579 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/installation.py
--rw-r--r--   0        0        0     1550 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/localization.py
--rw-r--r--   0        0        0    28609 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/locks.py
--rw-r--r--   0        0        0     6187 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/mail.py
--rw-r--r--   0        0        0    31108 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/manifest.py
--rw-r--r--   0        0        0     1449 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/meson.build
--rw-r--r--   0        0        0     8221 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/metadata.py
--rw-r--r--   0        0        0     8568 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/module.py
--rw-r--r--   0        0        0    18469 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/news.py
--rw-r--r--   0        0        0    30107 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/output.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/__init__.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/__init__.py
--rw-r--r--   0        0        0    13005 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/KeywordsManager.py
--rw-r--r--   0        0        0     9192 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/LicenseManager.py
--rw-r--r--   0        0        0    16684 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/LocationsManager.py
--rw-r--r--   0        0        0    13915 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/MaskManager.py
--rw-r--r--   0        0        0    21565 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/UseManager.py
--rw-r--r--   0        0        0     8445 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/VirtualsManager.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/__init__.py
--rw-r--r--   0        0        0      771 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/env_var_validation.py
--rw-r--r--   0        0        0     4694 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/features_set.py
--rw-r--r--   0        0        0     2273 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/helper.py
--rw-r--r--   0        0        0      421 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/meson.build
--rw-r--r--   0        0        0     9512 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_config/special_env_vars.py
--rw-r--r--   0        0        0      829 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_ipc/ExitCommand.py
--rw-r--r--   0        0        0      212 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_ipc/IpcCommand.py
--rw-r--r--   0        0        0     5193 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_ipc/QueryCommand.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_ipc/__init__.py
--rw-r--r--   0        0        0      213 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_ipc/meson.build
--rw-r--r--   0        0        0     1405 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_metadata_invalid.py
--rw-r--r--   0        0        0     1815 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py
--rw-r--r--   0        0        0     3768 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py
--rw-r--r--   0        0        0     7859 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_parallel_manifest/__init__.py
--rw-r--r--   0        0        0      238 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_parallel_manifest/meson.build
--rw-r--r--   0        0        0     4987 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/_spawn_nofetch.py
--rw-r--r--   0        0        0   133980 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/config.py
--rw-r--r--   0        0        0     4195 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/deprecated_profile_check.py
--rw-r--r--   0        0        0     6732 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/digestcheck.py
--rw-r--r--   0        0        0     9417 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/digestgen.py
--rw-r--r--   0        0        0   114236 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/doebuild.py
--rw-r--r--   0        0        0    79562 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/fetch.py
--rw-r--r--   0        0        0     4689 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/getmaskingreason.py
--rw-r--r--   0        0        0     6556 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/getmaskingstatus.py
--rw-r--r--   0        0        0      529 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/meson.build
--rw-r--r--   0        0        0    19287 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/prepare_build_dirs.py
--rw-r--r--   0        0        0     1004 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/ebuild/profile_iuse.py
--rw-r--r--   0        0        0      141 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/package/meson.build
--rw-r--r--   0        0        0    51466 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/process.py
--rw-r--r--   0        0        0     1573 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/progress.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/proxy/__init__.py
--rw-r--r--   0        0        0     7762 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/proxy/lazyimport.py
--rw-r--r--   0        0        0      172 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/proxy/meson.build
--rw-r--r--   0        0        0     2856 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/proxy/objectproxy.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/__init__.py
--rw-r--r--   0        0        0    62134 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/config.py
--rw-r--r--   0        0        0      166 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/meson.build
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/storage/__init__.py
--rw-r--r--   0        0        0     3950 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/storage/hardlink_quarantine.py
--rw-r--r--   0        0        0    10937 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/storage/hardlink_rcu.py
--rw-r--r--   0        0        0     1153 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/storage/inplace.py
--rw-r--r--   0        0        0     2675 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/storage/interface.py
--rw-r--r--   0        0        0      241 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/repository/storage/meson.build
--rw-r--r--   0        0        0     1589 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/__init__.py
--rw-r--r--   0        0        0     3015 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/config_checks.py
--rw-r--r--   0        0        0    14873 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/controller.py
--rw-r--r--   0        0        0      696 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/getaddrinfo_validate.py
--rw-r--r--   0        0        0      283 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/meson.build
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/__init__.py
--rw-r--r--   0        0        0     1650 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/cvs/__init__.py
--rw-r--r--   0        0        0     2341 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/cvs/cvs.py
--rw-r--r--   0        0        0      150 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/cvs/meson.build
--rw-r--r--   0        0        0     2770 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/git/__init__.py
--rw-r--r--   0        0        0    24957 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/git/git.py
--rw-r--r--   0        0        0      150 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/git/meson.build
--rw-r--r--   0        0        0     1403 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/mercurial/__init__.py
--rw-r--r--   0        0        0     6125 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/mercurial/mercurial.py
--rw-r--r--   0        0        0      162 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/mercurial/meson.build
--rw-r--r--   0        0        0      226 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/meson.build
--rw-r--r--   0        0        0     1287 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/rsync/__init__.py
--rw-r--r--   0        0        0      154 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/rsync/meson.build
--rw-r--r--   0        0        0    34132 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/rsync/rsync.py
--rw-r--r--   0        0        0     1037 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/svn/__init__.py
--rw-r--r--   0        0        0      150 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/svn/meson.build
--rw-r--r--   0        0        0     2759 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/svn/svn.py
--rw-r--r--   0        0        0     1650 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/webrsync/__init__.py
--rw-r--r--   0        0        0      160 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/webrsync/meson.build
--rw-r--r--   0        0        0     4983 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/modules/webrsync/webrsync.py
--rw-r--r--   0        0        0     2485 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/old_tree_timestamp.py
--rw-r--r--   0        0        0    13378 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/sync/syncbase.py
--rw-r--r--   0        0        0     1850 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev
--rw-r--r--   0        0        0     1852 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev
--rw-r--r--   0        0        0     2055 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key
--rw-r--r--   0        0        0     2055 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key
--rw-r--r--   0        0        0     2774 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/.gnupg/pubring.kbx
--rw-r--r--   0        0        0     1360 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/.gnupg/trustdb.gpg
--rw-r--r--   0        0        0     3786 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/__test__.py
--rw-r--r--   0        0        0      317 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/meson.build
--rw-r--r--   0        0        0     2602 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/setup_env.py
--rw-r--r--   0        0        0      547 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/test_dobin.py
--rw-r--r--   0        0        0      565 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/test_dodir.py
--rw-r--r--   0        0        0    13017 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/test_doins.py
--rw-r--r--   0        0        0     9192 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/test_eapi7_ver_funcs.py
--rw-r--r--   0        0        0     3083 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/bin/test_filter_bash_env.py
--rw-r--r--   0        0        0     2454 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/conftest.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dbapi/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dbapi/__test__.py
--rw-r--r--   0        0        0      263 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dbapi/meson.build
--rw-r--r--   0        0        0     4867 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dbapi/test_auxdb.py
--rw-r--r--   0        0        0     8553 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dbapi/test_bintree.py
--rw-r--r--   0        0        0     3973 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dbapi/test_fakedbapi.py
--rw-r--r--   0        0        0     9479 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dbapi/test_portdb_cache.py
--rw-r--r--   0        0        0      169 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/__test__.py
--rw-r--r--   0        0        0      839 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/meson.build
--rw-r--r--   0        0        0    24520 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_atom.py
--rw-r--r--   0        0        0     4452 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_best_match_to_list.py
--rw-r--r--   0        0        0     9752 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_check_required_use.py
--rw-r--r--   0        0        0     1149 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_dep_getcpv.py
--rw-r--r--   0        0        0      988 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_dep_getrepo.py
--rw-r--r--   0        0        0      934 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_dep_getslot.py
--rw-r--r--   0        0        0     1402 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_dep_getusedeps.py
--rw-r--r--   0        0        0     2077 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_dnf_convert.py
--rw-r--r--   0        0        0      779 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_extended_atom_dict.py
--rw-r--r--   0        0        0     3769 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_extract_affecting_use.py
--rw-r--r--   0        0        0     1237 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_get_operator.py
--rw-r--r--   0        0        0     1778 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_get_required_use_flags.py
--rw-r--r--   0        0        0     1009 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_isjustname.py
--rw-r--r--   0        0        0    11660 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_isvalidatom.py
--rw-r--r--   0        0        0     2406 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_libc.py
--rw-r--r--   0        0        0    11132 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_match_from_list.py
--rw-r--r--   0        0        0     3245 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_overlap_dnf.py
--rw-r--r--   0        0        0     2661 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_paren_reduce.py
--rw-r--r--   0        0        0      790 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_soname_atom_pickle.py
--rw-r--r--   0        0        0     1652 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_standalone.py
--rw-r--r--   0        0        0    27656 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/dep/test_use_reduce.py
--rw-r--r--   0        0        0      107 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/__test__.py
--rw-r--r--   0        0        0      439 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/meson.build
--rw-r--r--   0        0        0     1387 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_array_fromfile_eof.py
--rw-r--r--   0        0        0    14001 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_config.py
--rw-r--r--   0        0        0     6009 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py
--rw-r--r--   0        0        0     5238 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_doebuild_spawn.py
--rw-r--r--   0        0        0    35301 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_fetch.py
--rw-r--r--   0        0        0     7065 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_ipc_daemon.py
--rw-r--r--   0        0        0     5211 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_shell_quote.py
--rw-r--r--   0        0        0     1920 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_spawn.py
--rw-r--r--   0        0        0     4479 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/ebuild/test_use_expand_incremental.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/__test__.py
--rw-r--r--   0        0        0    25096 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/conftest.py
--rw-r--r--   0        0        0      425 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/meson.build
--rw-r--r--   0        0        0     2617 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/test_actions.py
--rw-r--r--   0        0        0     6946 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/test_baseline.py
--rw-r--r--   0        0        0     7552 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/test_binpkg_fetch.py
--rw-r--r--   0        0        0    10436 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/test_config_protect.py
--rw-r--r--   0        0        0     6503 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py
--rw-r--r--   0        0        0     6847 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/test_emerge_slot_abi.py
--rw-r--r--   0        0        0     1320 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/test_global_updates.py
--rw-r--r--   0        0        0    19102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/emerge/test_libc_dep_inject.py
--rw-r--r--   0        0        0      169 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/__test__.py
--rw-r--r--   0        0        0      176 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/config/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/config/__test__.py
--rw-r--r--   0        0        0      301 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/config/meson.build
--rw-r--r--   0        0        0     1164 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/config/test_PackageKeywordsFile.py
--rw-r--r--   0        0        0      818 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/config/test_PackageMaskFile.py
--rw-r--r--   0        0        0     1077 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/config/test_PackageUseFile.py
--rw-r--r--   0        0        0     1149 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/config/test_PortageModulesFile.py
--rw-r--r--   0        0        0      166 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/env/meson.build
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/glsa/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/glsa/__test__.py
--rw-r--r--   0        0        0      181 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/glsa/meson.build
--rw-r--r--   0        0        0     8021 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/glsa/test_security_set.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/__test__.py
--rw-r--r--   0        0        0      376 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/meson.build
--rw-r--r--   0        0        0    13834 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_checksum.py
--rw-r--r--   0        0        0    16272 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_gpg.py
--rw-r--r--   0        0        0     1929 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_metadata_update.py
--rw-r--r--   0        0        0     5277 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_metadata_url.py
--rw-r--r--   0        0        0    14781 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_path.py
--rw-r--r--   0        0        0     1869 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_size.py
--rw-r--r--   0        0        0     3306 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_stream.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lafilefixer/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lafilefixer/__test__.py
--rw-r--r--   0        0        0      187 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lafilefixer/meson.build
--rw-r--r--   0        0        0     6338 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lafilefixer/test_lafilefixer.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lazyimport/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lazyimport/__test__.py
--rw-r--r--   0        0        0      249 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lazyimport/meson.build
--rw-r--r--   0        0        0     2860 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py
--rw-r--r--   0        0        0      596 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lazyimport/test_preload_portage_submodules.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lint/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lint/__test__.py
--rw-r--r--   0        0        0      272 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lint/meson.build
--rw-r--r--   0        0        0      214 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lint/metadata.py
--rw-r--r--   0        0        0     2345 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lint/test_bash_syntax.py
--rw-r--r--   0        0        0     3031 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lint/test_compile_modules.py
--rw-r--r--   0        0        0     1516 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/lint/test_import_modules.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/locks/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/locks/__test__.py
--rw-r--r--   0        0        0      220 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/locks/meson.build
--rw-r--r--   0        0        0     7546 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/locks/test_asynchronous_lock.py
--rw-r--r--   0        0        0     2552 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/locks/test_lock_nonblock.py
--rw-r--r--   0        0        0      507 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/meson.build
--rw-r--r--   0        0        0      170 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/news/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/news/__test__.py
--rw-r--r--   0        0        0      177 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/news/meson.build
--rw-r--r--   0        0        0    14381 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/news/test_NewsItem.py
--rw-r--r--   0        0        0      107 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/__test__.py
--rw-r--r--   0        0        0      513 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/meson.build
--rw-r--r--   0        0        0     4144 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_AsyncFunction.py
--rw-r--r--   0        0        0     1545 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_ForkProcess.py
--rw-r--r--   0        0        0     2332 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_PipeLogger.py
--rw-r--r--   0        0        0     3121 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_PopenProcess.py
--rw-r--r--   0        0        0     2061 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_PopenProcessBlockingIO.py
--rw-r--r--   0        0        0     1684 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_pickle.py
--rw-r--r--   0        0        0     3811 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_poll.py
--rw-r--r--   0        0        0      987 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_spawn_fail_e2big.py
--rw-r--r--   0        0        0     1195 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_spawn_returnproc.py
--rw-r--r--   0        0        0     1341 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_spawn_warn_large_env.py
--rw-r--r--   0        0        0     1229 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/process/test_unshare_net.py
--rw-r--r--   0        0        0    43872 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/ResolverPlayground.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/__test__.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/binpkg_multi_instance/__init__.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/binpkg_multi_instance/__test__.py
--rw-r--r--   0        0        0      254 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/binpkg_multi_instance/meson.build
--rw-r--r--   0        0        0     5585 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py
--rw-r--r--   0        0        0     3747 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py
--rw-r--r--   0        0        0     3664 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/meson.build
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/__init__.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/__test__.py
--rw-r--r--   0        0        0      519 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/meson.build
--rw-r--r--   0        0        0     3931 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_autounmask.py
--rw-r--r--   0        0        0     1755 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_depclean.py
--rw-r--r--   0        0        0     8528 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_downgrade.py
--rw-r--r--   0        0        0     3840 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_or_choices.py
--rw-r--r--   0        0        0     3305 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_reinstall.py
--rw-r--r--   0        0        0     4521 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_skip_update.py
--rw-r--r--   0        0        0    12877 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py
--rw-r--r--   0        0        0     3971 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_slot_conflict_update.py
--rw-r--r--   0        0        0     2944 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_soname_provided.py
--rw-r--r--   0        0        0     2778 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_unsatisfiable.py
--rw-r--r--   0        0        0     3354 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/soname/test_unsatisfied.py
--rw-r--r--   0        0        0     2824 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py
--rw-r--r--   0        0        0     9576 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_alternatives_gzip.py
--rw-r--r--   0        0        0    28432 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_autounmask.py
--rw-r--r--   0        0        0     2731 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_autounmask_binpkg_use.py
--rw-r--r--   0        0        0     2176 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_autounmask_keep_keywords.py
--rw-r--r--   0        0        0     3118 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_autounmask_multilib_use.py
--rw-r--r--   0        0        0     1279 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_autounmask_parent.py
--rw-r--r--   0        0        0     2573 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_autounmask_use_backtrack.py
--rw-r--r--   0        0        0     3743 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_autounmask_use_breakage.py
--rw-r--r--   0        0        0     1850 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py
--rw-r--r--   0        0        0     5786 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_backtracking.py
--rw-r--r--   0        0        0     6805 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_bdeps.py
--rw-r--r--   0        0        0     4927 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py
--rw-r--r--   0        0        0     4231 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_blocker.py
--rw-r--r--   0        0        0     2459 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_broken_deps.py
--rw-r--r--   0        0        0     4330 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_changed_deps.py
--rw-r--r--   0        0        0     7899 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_circular_choices.py
--rw-r--r--   0        0        0     3341 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_circular_choices_rust.py
--rw-r--r--   0        0        0     4832 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_circular_dependencies.py
--rw-r--r--   0        0        0     4948 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_complete_graph.py
--rw-r--r--   0        0        0     2910 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py
--rw-r--r--   0        0        0     5605 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_cross_dep_priority.py
--rw-r--r--   0        0        0     9959 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_depclean.py
--rw-r--r--   0        0        0     5070 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_depclean_order.py
--rw-r--r--   0        0        0     2444 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_depclean_slot_unavailable.py
--rw-r--r--   0        0        0    13377 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_depth.py
--rw-r--r--   0        0        0     3329 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_disjunctive_depend_order.py
--rw-r--r--   0        0        0     9971 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_eapi.py
--rw-r--r--   0        0        0     4323 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_emptytree_reinstall_unsatisfiability.py
--rw-r--r--   0        0        0     2658 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_features_test_use.py
--rw-r--r--   0        0        0     3379 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py
--rw-r--r--   0        0        0     3457 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_installkernel.py
--rw-r--r--   0        0        0    11063 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_keywords.py
--rw-r--r--   0        0        0    31277 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_merge_order.py
--rw-r--r--   0        0        0     1234 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py
--rw-r--r--   0        0        0    15920 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_multirepo.py
--rw-r--r--   0        0        0     1772 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_multislot.py
--rw-r--r--   0        0        0     1554 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_old_dep_chain_display.py
--rw-r--r--   0        0        0     1142 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_onlydeps.py
--rw-r--r--   0        0        0     1527 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_onlydeps_circular.py
--rw-r--r--   0        0        0     5933 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_onlydeps_ideps.py
--rw-r--r--   0        0        0     2552 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_onlydeps_minimal.py
--rw-r--r--   0        0        0    25128 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_or_choices.py
--rw-r--r--   0        0        0     2716 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_or_downgrade_installed.py
--rw-r--r--   0        0        0     6850 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_or_upgrade_installed.py
--rw-r--r--   0        0        0     3911 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_output.py
--rw-r--r--   0        0        0     9049 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_package_tracker.py
--rw-r--r--   0        0        0     4296 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_perl_rebuild_bug.py
--rw-r--r--   0        0        0     4568 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_profile_default_eapi.py
--rw-r--r--   0        0        0     3353 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_profile_package_set.py
--rw-r--r--   0        0        0     6911 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_rebuild.py
--rw-r--r--   0        0        0     5847 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_rebuild_ghostscript.py
--rw-r--r--   0        0        0     2409 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py
--rw-r--r--   0        0        0    11792 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_required_use.py
--rw-r--r--   0        0        0     7177 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py
--rw-r--r--   0        0        0     3500 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_simple.py
--rw-r--r--   0        0        0    18128 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_abi.py
--rw-r--r--   0        0        0     8790 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_abi_downgrade.py
--rw-r--r--   0        0        0     3488 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_change_without_revbump.py
--rw-r--r--   0        0        0    13393 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_collisions.py
--rw-r--r--   0        0        0     2528 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_blocked_prune.py
--rw-r--r--   0        0        0     1990 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py
--rw-r--r--   0        0        0     1432 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_mask_update.py
--rw-r--r--   0        0        0    14826 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_rebuild.py
--rw-r--r--   0        0        0     7910 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py
--rw-r--r--   0        0        0     2579 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_update.py
--rw-r--r--   0        0        0     2491 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_update_virt.py
--rw-r--r--   0        0        0     5024 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_autounmask.py
--rw-r--r--   0        0        0     7642 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_bdeps.py
--rw-r--r--   0        0        0     4350 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_complete_graph.py
--rw-r--r--   0        0        0     4694 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py
--rw-r--r--   0        0        0     4366 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_missed_update.py
--rw-r--r--   0        0        0     3719 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_rebuild.py
--rw-r--r--   0        0        0     1682 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_required_use.py
--rw-r--r--   0        0        0     9190 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py
--rw-r--r--   0        0        0     3974 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py
--rw-r--r--   0        0        0     2103 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py
--rw-r--r--   0        0        0     3518 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_unsolved.py
--rw-r--r--   0        0        0     2107 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py
--rw-r--r--   0        0        0     1819 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py
--rw-r--r--   0        0        0     3584 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_targetroot.py
--rw-r--r--   0        0        0    11321 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_unmerge_order.py
--rw-r--r--   0        0        0     1571 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_unnecessary_slot_upgrade.py
--rw-r--r--   0        0        0     3843 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_update.py
--rw-r--r--   0        0        0     1827 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_use_dep_defaults.py
--rw-r--r--   0        0        0    10931 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_useflags.py
--rw-r--r--   0        0        0     9976 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_virtual_minimize_children.py
--rw-r--r--   0        0        0     9326 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_virtual_slot.py
--rw-r--r--   0        0        0     2910 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/resolver/test_with_test_deps.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/__test__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/base/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/base/__test__.py
--rw-r--r--   0        0        0      226 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/base/meson.build
--rw-r--r--   0        0        0     2051 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/base/test_internal_package_set.py
--rw-r--r--   0        0        0     1324 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/base/test_variable_set.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/files/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/files/__test__.py
--rw-r--r--   0        0        0      225 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/files/meson.build
--rw-r--r--   0        0        0     1018 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/files/test_config_file_set.py
--rw-r--r--   0        0        0      855 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/files/test_static_file_set.py
--rw-r--r--   0        0        0      197 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/meson.build
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/shell/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/shell/__test__.py
--rw-r--r--   0        0        0      180 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/shell/meson.build
--rw-r--r--   0        0        0      801 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sets/shell/test_shell.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sync/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sync/__test__.py
--rw-r--r--   0        0        0      179 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sync/meson.build
--rw-r--r--   0        0        0    16350 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/sync/test_sync_local.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/unicode/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/unicode/__test__.py
--rw-r--r--   0        0        0      185 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/unicode/meson.build
--rw-r--r--   0        0        0     2293 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/unicode/test_string_format.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/update/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/update/__test__.py
--rw-r--r--   0        0        0      246 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/update/meson.build
--rw-r--r--   0        0        0    11839 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/update/test_move_ent.py
--rw-r--r--   0        0        0    11094 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/update/test_move_slot_ent.py
--rw-r--r--   0        0        0    20527 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/update/test_update_dbentry.py
--rw-r--r--   0        0        0      170 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/__test__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/dyn_libs/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/dyn_libs/__test__.py
--rw-r--r--   0        0        0      226 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/dyn_libs/meson.build
--rw-r--r--   0        0        0     2695 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/dyn_libs/test_installed_dynlibs.py
--rw-r--r--   0        0        0     1389 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/dyn_libs/test_soname_deps.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/eventloop/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/eventloop/__test__.py
--rw-r--r--   0        0        0      193 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/eventloop/meson.build
--rw-r--r--   0        0        0      826 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/eventloop/test_call_soon_fifo.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/file_copy/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/file_copy/__test__.py
--rw-r--r--   0        0        0      187 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/file_copy/meson.build
--rw-r--r--   0        0        0     2179 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/file_copy/test_copyfile.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/__test__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/__test__.py
--rw-r--r--   0        0        0      388 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/meson.build
--rw-r--r--   0        0        0     2025 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py
--rw-r--r--   0        0        0     5396 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py
--rw-r--r--   0        0        0      795 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py
--rw-r--r--   0        0        0     1394 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py
--rw-r--r--   0        0        0     6914 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py
--rw-r--r--   0        0        0     2344 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py
--rw-r--r--   0        0        0      348 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/meson.build
--rw-r--r--   0        0        0     7135 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/test_compat_coroutine.py
--rw-r--r--   0        0        0     1274 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/test_done_callback.py
--rw-r--r--   0        0        0     1565 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/test_done_callback_after_exit.py
--rw-r--r--   0        0        0     2933 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/test_iter_completed.py
--rw-r--r--   0        0        0    11301 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/futures/test_retry.py
--rw-r--r--   0        0        0      750 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/meson.build
--rw-r--r--   0        0        0     5805 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_checksum.py
--rw-r--r--   0        0        0    11345 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_digraph.py
--rw-r--r--   0        0        0     1824 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_file_copier.py
--rw-r--r--   0        0        0     3539 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_getconfig.py
--rw-r--r--   0        0        0      315 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_grabdict.py
--rw-r--r--   0        0        0     5805 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_install_mask.py
--rw-r--r--   0        0        0     1211 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_manifest.py
--rw-r--r--   0        0        0    10489 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_mtimedb.py
--rw-r--r--   0        0        0      440 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_normalizedPath.py
--rw-r--r--   0        0        0     1735 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_shelve.py
--rw-r--r--   0        0        0     8330 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_socks5.py
--rw-r--r--   0        0        0      832 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_stackDictList.py
--rw-r--r--   0        0        0     1185 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_stackDicts.py
--rw-r--r--   0        0        0      715 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_stackLists.py
--rw-r--r--   0        0        0      864 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_uniqueArray.py
--rw-r--r--   0        0        0     3347 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_varExpand.py
--rw-r--r--   0        0        0     1681 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_whirlpool.py
--rw-r--r--   0        0        0     6243 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/util/test_xattr.py
--rw-r--r--   0        0        0      174 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/versions/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/versions/__test__.py
--rw-r--r--   0        0        0      211 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/versions/meson.build
--rw-r--r--   0        0        0      555 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/versions/test_cpv_sort_key.py
--rw-r--r--   0        0        0     3026 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/versions/test_vercmp.py
--rw-r--r--   0        0        0      169 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/xpak/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/xpak/__test__.py
--rw-r--r--   0        0        0      178 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/xpak/meson.build
--rw-r--r--   0        0        0      427 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/tests/xpak/test_decodeint.py
--rw-r--r--   0        0        0    17014 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/update.py
--rw-r--r--   0        0        0     2929 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/ExtractKernelVersion.py
--rw-r--r--   0        0        0     2141 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/SlotObject.py
--rw-r--r--   0        0        0    68950 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/__init__.py
--rw-r--r--   0        0        0     2683 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/AsyncFunction.py
--rw-r--r--   0        0        0     3393 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/AsyncScheduler.py
--rw-r--r--   0        0        0     1165 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/AsyncTaskFuture.py
--rw-r--r--   0        0        0     5892 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/BuildLogger.py
--rw-r--r--   0        0        0     1220 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/FileCopier.py
--rw-r--r--   0        0        0      801 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/FileDigester.py
--rw-r--r--   0        0        0    13101 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/ForkProcess.py
--rw-r--r--   0        0        0     7527 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/PipeLogger.py
--rw-r--r--   0        0        0     2587 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/PipeReaderBlockingIO.py
--rw-r--r--   0        0        0     1118 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/PopenProcess.py
--rw-r--r--   0        0        0     4649 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/SchedulerInterface.py
--rw-r--r--   0        0        0      643 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/TaskScheduler.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/__init__.py
--rw-r--r--   0        0        0      499 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/meson.build
--rw-r--r--   0        0        0     1360 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_async/run_main_scheduler.py
--rw-r--r--   0        0        0     4347 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_compare_files.py
--rw-r--r--   0        0        0     1219 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_ctypes.py
--rw-r--r--   0        0        0     2654 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_desktop_entry.py
--rw-r--r--   0        0        0    41422 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/LinkageMapELF.py
--rw-r--r--   0        0        0     2877 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/NeededEntry.py
--rw-r--r--   0        0        0     9385 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/__init__.py
--rw-r--r--   0        0        0     3834 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/display_preserved_libs.py
--rw-r--r--   0        0        0     2743 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/dyn_libs.py
--rw-r--r--   0        0        0      335 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/meson.build
--rw-r--r--   0        0        0     6203 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/soname_deps.py
--rw-r--r--   0        0        0     3722 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_dyn_libs/soname_deps_qa.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_eventloop/__init__.py
--rw-r--r--   0        0        0     7640 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_eventloop/asyncio_event_loop.py
--rw-r--r--   0        0        0      213 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_eventloop/global_event_loop.py
--rw-r--r--   0        0        0      196 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_eventloop/meson.build
--rw-r--r--   0        0        0     3029 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_get_vm_info.py
--rw-r--r--   0        0        0     5956 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_info_files.py
--rw-r--r--   0        0        0      692 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_path.py
--rw-r--r--   0        0        0     2530 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_pty.py
--rw-r--r--   0        0        0     4032 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_urlopen.py
--rw-r--r--   0        0        0     7063 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/_xattr.py
--rw-r--r--   0        0        0     1528 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/backoff.py
--rw-r--r--   0        0        0      784 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/bin_entry_point.py
--rw-r--r--   0        0        0     2189 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/changelog.py
--rw-r--r--   0        0        0     3464 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/compression_probe.py
--rw-r--r--   0        0        0     2403 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/configparser.py
--rw-r--r--   0        0        0     2180 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/cpuinfo.py
--rw-r--r--   0        0        0    12975 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/digraph.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/elf/__init__.py
--rw-r--r--   0        0        0     1446 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/elf/constants.py
--rw-r--r--   0        0        0     1889 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/elf/header.py
--rw-r--r--   0        0        0      169 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/elf/meson.build
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/endian/__init__.py
--rw-r--r--   0        0        0     1303 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/endian/decode.py
--rw-r--r--   0        0        0      148 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/endian/meson.build
--rw-r--r--   0        0        0    17055 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/env_update.py
--rw-r--r--   0        0        0      920 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/file_copy/__init__.py
--rw-r--r--   0        0        0      130 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/file_copy/meson.build
--rw-r--r--   0        0        0     2118 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/formatter.py
--rw-r--r--   0        0        0      180 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/__init__.py
--rw-r--r--   0        0        0    11282 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/_asyncio/__init__.py
--rw-r--r--   0        0        0      159 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/_asyncio/meson.build
--rw-r--r--   0        0        0     3016 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/_asyncio/streams.py
--rw-r--r--   0        0        0     1886 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/_sync_decorator.py
--rw-r--r--   0        0        0     4942 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/compat_coroutine.py
--rw-r--r--   0        0        0        0 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/executor/__init__.py
--rw-r--r--   0        0        0     4424 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/executor/fork.py
--rw-r--r--   0        0        0      156 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/executor/meson.build
--rw-r--r--   0        0        0     2830 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/extendedfutures.py
--rw-r--r--   0        0        0      516 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/futures.py
--rw-r--r--   0        0        0     6868 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/iter_completed.py
--rw-r--r--   0        0        0      355 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/meson.build
--rw-r--r--   0        0        0     6298 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/retry.py
--rw-r--r--   0        0        0     2237 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/futures/unix_events.py
--rw-r--r--   0        0        0     1584 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/hooks.py
--rw-r--r--   0        0        0     6549 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/install_mask.py
--rw-r--r--   0        0        0     2996 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/iterators/MultiIterGroupBy.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/iterators/__init__.py
--rw-r--r--   0        0        0      161 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/iterators/meson.build
--rw-r--r--   0        0        0     7350 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/lafilefixer.py
--rw-r--r--   0        0        0     4814 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/listdir.py
--rw-r--r--   0        0        0     4901 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/locale.py
--rw-r--r--   0        0        0     1070 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/meson.build
--rw-r--r--   0        0        0    14876 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/movefile.py
--rw-r--r--   0        0        0     4258 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/mtimedb.py
--rw-r--r--   0        0        0     2990 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/netlink.py
--rw-r--r--   0        0        0     1336 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/path.py
--rw-r--r--   0        0        0     1527 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/shelve.py
--rw-r--r--   0        0        0     4707 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/socks5.py
--rw-r--r--   0        0        0    58416 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/whirlpool.py
--rw-r--r--   0        0        0     4506 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/util/writeable_check.py
--rw-r--r--   0        0        0    20265 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/versions.py
--rw-r--r--   0        0        0      102 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/xml/__init__.py
--rw-r--r--   0        0        0      142 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/xml/meson.build
--rw-r--r--   0        0        0    16789 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/xml/metadata.py
--rw-r--r--   0        0        0    19634 2024-02-25 08:29:43.000000 portage-3.0.63/lib/portage/xpak.py
--rwxr-xr-x   0        0        0     1280 2024-02-25 08:29:43.000000 portage-3.0.63/make.conf.example-repatch.sh
--rw-r--r--   0        0        0     4275 2024-02-25 08:29:43.000000 portage-3.0.63/man/color.map.5
--rw-r--r--   0        0        0     3634 2024-02-25 08:29:43.000000 portage-3.0.63/man/dispatch-conf.1
--rw-r--r--   0        0        0    10769 2024-02-25 08:29:43.000000 portage-3.0.63/man/ebuild.1
--rw-r--r--   0        0        0    61555 2024-02-25 08:29:43.000000 portage-3.0.63/man/ebuild.5
--rw-r--r--   0        0        0     7452 2024-02-25 08:29:43.000000 portage-3.0.63/man/egencache.1
--rw-r--r--   0        0        0     3507 2024-02-25 08:29:43.000000 portage-3.0.63/man/emaint.1
--rw-r--r--   0        0        0    71807 2024-02-25 08:29:43.000000 portage-3.0.63/man/emerge.1
--rw-r--r--   0        0        0     4778 2024-02-25 08:29:43.000000 portage-3.0.63/man/emirrordist.1
--rw-r--r--   0        0        0     1062 2024-02-25 08:29:43.000000 portage-3.0.63/man/env-update.1
--rw-r--r--   0        0        0     1733 2024-02-25 08:29:43.000000 portage-3.0.63/man/etc-update.1
--rw-r--r--   0        0        0      458 2024-02-25 08:29:43.000000 portage-3.0.63/man/fixpackages.1
--rw-r--r--   0        0        0     2341 2024-02-25 08:29:43.000000 portage-3.0.63/man/glsa-check.1
--rw-r--r--   0        0        0    59644 2024-02-25 08:29:43.000000 portage-3.0.63/man/make.conf.5
--rw-r--r--   0        0        0      549 2024-02-25 08:29:43.000000 portage-3.0.63/man/meson.build
--rw-r--r--   0        0        0    64193 2024-02-25 08:29:43.000000 portage-3.0.63/man/portage.5
--rw-r--r--   0        0        0     2339 2024-02-25 08:29:43.000000 portage-3.0.63/man/quickpkg.1
--rw-r--r--   0        0        0     8221 2024-02-25 08:29:43.000000 portage-3.0.63/man/ru/color.map.5
--rw-r--r--   0        0        0     6046 2024-02-25 08:29:43.000000 portage-3.0.63/man/ru/dispatch-conf.1
--rw-r--r--   0        0        0    18214 2024-02-25 08:29:43.000000 portage-3.0.63/man/ru/ebuild.1
--rw-r--r--   0        0        0     1862 2024-02-25 08:29:43.000000 portage-3.0.63/man/ru/env-update.1
--rw-r--r--   0        0        0     3116 2024-02-25 08:29:43.000000 portage-3.0.63/man/ru/etc-update.1
--rw-r--r--   0        0        0      860 2024-02-25 08:29:43.000000 portage-3.0.63/man/ru/fixpackages.1
--rw-r--r--   0        0        0      374 2024-02-25 08:29:43.000000 portage-3.0.63/man/ru/meson.build
--rw-r--r--   0        0        0     6382 2024-02-25 08:29:43.000000 portage-3.0.63/man/xpak.5
--rw-r--r--   0        0        0     3087 2024-02-25 08:29:43.000000 portage-3.0.63/meson.build
--rw-r--r--   0        0        0     1806 2024-02-25 08:29:43.000000 portage-3.0.63/meson_options.txt
--rwxr-xr-x   0        0        0    29089 2024-02-25 08:29:43.000000 portage-3.0.63/misc/emerge-delta-webrsync
--rw-r--r--   0        0        0    15189 2024-02-25 08:29:43.000000 portage-3.0.63/pylintrc
--rw-r--r--   0        0        0     1650 2024-02-25 08:29:43.000000 portage-3.0.63/pyproject.toml
--rwxr-xr-x   0        0        0       81 2024-02-25 08:29:43.000000 portage-3.0.63/run-pylint
--rw-r--r--   0        0        0     1303 2024-02-25 08:29:43.000000 portage-3.0.63/src/meson.build
--rw-r--r--   0        0        0    71291 2024-02-25 08:29:43.000000 portage-3.0.63/src/portage_util__whirlpool.c
--rw-r--r--   0        0        0    13398 2024-02-25 08:29:43.000000 portage-3.0.63/src/portage_util_file_copy_reflink_linux.c
--rw-r--r--   0        0        0     1276 2024-02-25 08:29:43.000000 portage-3.0.63/src/portage_util_libc.c
--rw-r--r--   0        0        0      571 2024-02-25 08:29:43.000000 portage-3.0.63/testpath
--rw-r--r--   0        0        0      543 2024-02-25 08:29:43.000000 portage-3.0.63/tox.ini
--rw-r--r--   0        0        0    24629 2024-02-25 08:31:19.368024 portage-3.0.63/PKG-INFO
+-rw-r--r--   0        0        0     1857 2024-04-28 00:34:23.000000 portage-3.0.64/.builds/ci.yml
+-rw-r--r--   0        0        0     1071 2024-04-28 00:34:23.000000 portage-3.0.64/.builds/lint.yml
+-rwxr-xr-x   0        0        0      766 2024-04-28 00:34:23.000000 portage-3.0.64/.builds/setup-python.sh
+-rw-r--r--   0        0        0      294 2024-04-28 00:34:23.000000 portage-3.0.64/.editorconfig
+-rw-r--r--   0        0        0      618 2024-04-28 00:34:23.000000 portage-3.0.64/.git-blame-ignore-revs
+-rw-r--r--   0        0        0     3774 2024-04-28 00:34:23.000000 portage-3.0.64/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1203 2024-04-28 00:34:23.000000 portage-3.0.64/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      273 2024-04-28 00:34:23.000000 portage-3.0.64/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      116 2024-04-28 00:34:23.000000 portage-3.0.64/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/.portage_not_installed
+-rw-r--r--   0        0        0      454 2024-04-28 00:34:23.000000 portage-3.0.64/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1840 2024-04-28 00:34:23.000000 portage-3.0.64/COPYING
+-rw-r--r--   0        0        0     7201 2024-04-28 00:34:23.000000 portage-3.0.64/DEVELOPING
+-rw-r--r--   0        0        0    18092 2024-04-28 00:34:23.000000 portage-3.0.64/LICENSE
+-rw-r--r--   0        0        0    75128 2024-04-28 00:34:23.000000 portage-3.0.64/NEWS
+-rw-r--r--   0        0        0     3559 2024-04-28 00:34:23.000000 portage-3.0.64/README.md
+-rw-r--r--   0        0        0    84461 2024-04-28 00:34:23.000000 portage-3.0.64/RELEASE-NOTES
+-rw-r--r--   0        0        0     1848 2024-04-28 00:34:23.000000 portage-3.0.64/TEST-NOTES
+-rwxr-xr-x   0        0        0     3262 2024-04-28 00:34:23.000000 portage-3.0.64/bin/archive-conf
+-rw-r--r--   0        0        0     1443 2024-04-28 00:34:23.000000 portage-3.0.64/bin/bashrc-functions.sh
+-rwxr-xr-x   0        0        0     4457 2024-04-28 00:34:23.000000 portage-3.0.64/bin/binhost-snapshot
+-rwxr-xr-x   0        0        0      618 2024-04-28 00:35:10.017311 portage-3.0.64/bin/chmod-lite
+-rwxr-xr-x   0        0        0      951 2024-04-28 00:34:23.000000 portage-3.0.64/bin/chmod-lite.py
+-rwxr-xr-x   0        0        0     5891 2024-04-28 00:34:23.000000 portage-3.0.64/bin/chpathtool.py
+-rwxr-xr-x   0        0        0     1421 2024-04-28 00:34:23.000000 portage-3.0.64/bin/clean_locks
+-rwxr-xr-x   0        0        0    20957 2024-04-28 00:34:23.000000 portage-3.0.64/bin/dispatch-conf
+-rwxr-xr-x   0        0        0     8895 2024-04-28 00:34:23.000000 portage-3.0.64/bin/dohtml.py
+-rw-r--r--   0        0        0    20007 2024-04-28 00:34:23.000000 portage-3.0.64/bin/doins.py
+-rw-r--r--   0        0        0     6078 2024-04-28 00:34:23.000000 portage-3.0.64/bin/eapi.sh
+-rw-r--r--   0        0        0     4310 2024-04-28 00:34:23.000000 portage-3.0.64/bin/eapi7-ver-funcs.sh
+-rwxr-xr-x   0        0        0    15586 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild
+-rwxr-xr-x   0        0        0      639 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/bsd/sed
+-rwxr-xr-x   0        0        0      200 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/die
+-rwxr-xr-x   0        0        0     1049 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dobin
+-rwxr-xr-x   0        0        0      515 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/doconfd
+-rwxr-xr-x   0        0        0      359 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dodir
+-rwxr-xr-x   0        0        0      885 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dodoc
+-rwxr-xr-x   0        0        0      513 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/doenvd
+-rwxr-xr-x   0        0        0      952 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/doexe
+-rwxr-xr-x   0        0        0      531 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dohard
+-rwxr-xr-x   0        0        0      632 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/doheader
+-rwxr-xr-x   0        0        0      793 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dohtml
+-rwxr-xr-x   0        0        0      722 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/doinfo
+-rwxr-xr-x   0        0        0      485 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/doinitd
+-rwxr-xr-x   0        0        0     3034 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/doins
+-rwxr-xr-x   0        0        0     1333 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dolib
+-rwxr-xr-x   0        0        0      189 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dolib.a
+-rwxr-xr-x   0        0        0      189 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dolib.so
+-rwxr-xr-x   0        0        0     1553 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/doman
+-rwxr-xr-x   0        0        0     1216 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/domo
+-rwxr-xr-x   0        0        0     1053 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dosbin
+-rwxr-xr-x   0        0        0      818 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dosed
+-rwxr-xr-x   0        0        0     2411 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/dosym
+-rwxr-xr-x   0        0        0      204 2024-04-28 00:35:10.023311 portage-3.0.64/bin/ebuild-helpers/eerror
+-rwxr-xr-x   0        0        0      204 2024-04-28 00:35:10.023311 portage-3.0.64/bin/ebuild-helpers/einfo
+-rwxr-xr-x   0        0        0      204 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/elog
+-rwxr-xr-x   0        0        0      894 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/emake
+-rwxr-xr-x   0        0        0      204 2024-04-28 00:35:10.024311 portage-3.0.64/bin/ebuild-helpers/eqawarn
+-rwxr-xr-x   0        0        0      204 2024-04-28 00:35:10.024311 portage-3.0.64/bin/ebuild-helpers/ewarn
+-rwxr-xr-x   0        0        0      882 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/fowners
+-rwxr-xr-x   0        0        0      949 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/fperms
+-rwxr-xr-x   0        0        0      490 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/keepdir
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.024311 portage-3.0.64/bin/ebuild-helpers/newbin
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newconfd
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newdoc
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newenvd
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newexe
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newheader
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newinitd
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/newins
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newlib.a
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newlib.so
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newman
+-rwxr-xr-x   0        0        0     1201 2024-04-28 00:35:10.025311 portage-3.0.64/bin/ebuild-helpers/newsbin
+-rwxr-xr-x   0        0        0      359 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/nonfatal
+-rwxr-xr-x   0        0        0      242 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/prepall
+-rwxr-xr-x   0        0        0      242 2024-04-28 00:35:10.026311 portage-3.0.64/bin/ebuild-helpers/prepalldocs
+-rwxr-xr-x   0        0        0      242 2024-04-28 00:35:10.026311 portage-3.0.64/bin/ebuild-helpers/prepallinfo
+-rwxr-xr-x   0        0        0      242 2024-04-28 00:35:10.026311 portage-3.0.64/bin/ebuild-helpers/prepallman
+-rwxr-xr-x   0        0        0      242 2024-04-28 00:35:10.026311 portage-3.0.64/bin/ebuild-helpers/prepallstrip
+-rwxr-xr-x   0        0        0      242 2024-04-28 00:35:10.026311 portage-3.0.64/bin/ebuild-helpers/prepinfo
+-rwxr-xr-x   0        0        0      242 2024-04-28 00:35:10.026311 portage-3.0.64/bin/ebuild-helpers/prepman
+-rwxr-xr-x   0        0        0      242 2024-04-28 00:35:10.026311 portage-3.0.64/bin/ebuild-helpers/prepstrip
+-rwxr-xr-x   0        0        0     1178 2024-04-28 00:35:10.027311 portage-3.0.64/bin/ebuild-helpers/unprivileged/chgrp
+-rwxr-xr-x   0        0        0     1178 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/unprivileged/chown
+-rwxr-xr-x   0        0        0     1369 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-helpers/xattr/install
+-rwxr-xr-x   0        0        0      618 2024-04-28 00:35:10.027311 portage-3.0.64/bin/ebuild-ipc
+-rwxr-xr-x   0        0        0    10684 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-ipc.py
+-rwxr-xr-x   0        0        0      618 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild-pyhelper
+-rwxr-xr-x   0        0        0    26179 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ebuild.sh
+-rwxr-xr-x   0        0        0     6481 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ecompress
+-rwxr-xr-x   0        0        0     1746 2024-04-28 00:34:23.000000 portage-3.0.64/bin/ecompress-file
+-rwxr-xr-x   0        0        0    53990 2024-04-28 00:34:23.000000 portage-3.0.64/bin/egencache
+-rwxr-xr-x   0        0        0     2151 2024-04-28 00:34:23.000000 portage-3.0.64/bin/emaint
+-rwxr-xr-x   0        0        0     3297 2024-04-28 00:34:23.000000 portage-3.0.64/bin/emerge
+-rwxr-xr-x   0        0        0    21009 2024-04-28 00:34:23.000000 portage-3.0.64/bin/emerge-webrsync
+-rwxr-xr-x   0        0        0      634 2024-04-28 00:34:23.000000 portage-3.0.64/bin/emirrordist
+-rwxr-xr-x   0        0        0     1107 2024-04-28 00:34:23.000000 portage-3.0.64/bin/env-update
+-rwxr-xr-x   0        0        0    18168 2024-04-28 00:34:23.000000 portage-3.0.64/bin/estrip
+-rwxr-xr-x   0        0        0    23706 2024-04-28 00:34:23.000000 portage-3.0.64/bin/etc-update
+-rwxr-xr-x   0        0        0     6045 2024-04-28 00:34:23.000000 portage-3.0.64/bin/filter-bash-environment.py
+-rwxr-xr-x   0        0        0     1754 2024-04-28 00:34:23.000000 portage-3.0.64/bin/fixpackages
+-rwxr-xr-x   0        0        0    15636 2024-04-28 00:34:23.000000 portage-3.0.64/bin/glsa-check
+-rwxr-xr-x   0        0        0     2166 2024-04-28 00:34:23.000000 portage-3.0.64/bin/gpkg-helper.py
+-rwxr-xr-x   0        0        0     2476 2024-04-28 00:34:23.000000 portage-3.0.64/bin/gpkg-sign
+-rw-r--r--   0        0        0     2918 2024-04-28 00:34:23.000000 portage-3.0.64/bin/helper-functions.sh
+-rw-r--r--   0        0        0      443 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/05double-D
+-rw-r--r--   0        0        0     4376 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/05prefix
+-rw-r--r--   0        0        0     5559 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/10executable-issues
+-rw-r--r--   0        0        0     3591 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/10ignored-flags
+-rw-r--r--   0        0        0      406 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/20deprecated-directories
+-rw-r--r--   0        0        0      835 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/20runtime-directories
+-rw-r--r--   0        0        0     3233 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/60bash-completion
+-rw-r--r--   0        0        0     1450 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/60openrc
+-rw-r--r--   0        0        0     5508 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/60pkgconfig
+-rw-r--r--   0        0        0      668 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/60pngfix
+-rw-r--r--   0        0        0      687 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/60systemd
+-rw-r--r--   0        0        0      442 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/60udev
+-rw-r--r--   0        0        0     5556 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/80libraries
+-rw-r--r--   0        0        0     1417 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/80multilib-strict
+-rw-r--r--   0        0        0     1929 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/90bad-bin-group-write
+-rw-r--r--   0        0        0     1577 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/90bad-bin-owner
+-rw-r--r--   0        0        0      665 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/90cmake-warnings
+-rw-r--r--   0        0        0     3995 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/90config-impl-decl
+-rw-r--r--   0        0        0     1277 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/90cython-dep
+-rw-r--r--   0        0        0     8742 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/90gcc-warnings
+-rw-r--r--   0        0        0     1033 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/90world-writable
+-rw-r--r--   0        0        0     1529 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install-qa-check.d/95empty-dirs
+-rwxr-xr-x   0        0        0     6314 2024-04-28 00:34:23.000000 portage-3.0.64/bin/install.py
+-rw-r--r--   0        0        0    18552 2024-04-28 00:34:23.000000 portage-3.0.64/bin/isolated-functions.sh
+-rwxr-xr-x   0        0        0      903 2024-04-28 00:34:23.000000 portage-3.0.64/bin/lock-helper.py
+-rw-r--r--   0        0        0     1633 2024-04-28 00:34:23.000000 portage-3.0.64/bin/meson.build
+-rwxr-xr-x   0        0        0    20217 2024-04-28 00:34:23.000000 portage-3.0.64/bin/misc-functions.sh
+-rw-r--r--   0        0        0    34761 2024-04-28 00:34:23.000000 portage-3.0.64/bin/phase-functions.sh
+-rw-r--r--   0        0        0    33960 2024-04-28 00:34:23.000000 portage-3.0.64/bin/phase-helpers.sh
+-rw-r--r--   0        0        0     5723 2024-04-28 00:34:23.000000 portage-3.0.64/bin/pid-ns-init
+-rwxr-xr-x   0        0        0    51197 2024-04-28 00:34:23.000000 portage-3.0.64/bin/portageq
+-rwxr-xr-x   0        0        0      550 2024-04-28 00:34:23.000000 portage-3.0.64/bin/portageq-wrapper
+-rw-r--r--   0        0        0     5236 2024-04-28 00:34:23.000000 portage-3.0.64/bin/postinst-qa-check.d/50xdg-utils
+-rw-r--r--   0        0        0     5236 2024-04-28 00:35:10.034311 portage-3.0.64/bin/preinst-qa-check.d/50xdg-utils
+-rwxr-xr-x   0        0        0    16797 2024-04-28 00:34:23.000000 portage-3.0.64/bin/quickpkg
+-rwxr-xr-x   0        0        0     4992 2024-04-28 00:34:23.000000 portage-3.0.64/bin/regenworld
+-rw-r--r--   0        0        0     4642 2024-04-28 00:34:23.000000 portage-3.0.64/bin/save-ebuild-env.sh
+-rwxr-xr-x   0        0        0     1339 2024-04-28 00:34:23.000000 portage-3.0.64/bin/shelve-utils
+-rw-r--r--   0        0        0     8037 2024-04-28 00:34:23.000000 portage-3.0.64/bin/socks5-server.py
+-rwxr-xr-x   0        0        0     4784 2024-04-28 00:34:23.000000 portage-3.0.64/bin/xattr-helper.py
+-rwxr-xr-x   0        0        0     1825 2024-04-28 00:34:23.000000 portage-3.0.64/bin/xpak-helper.py
+-rw-r--r--   0        0        0       55 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/METADATA
+-rw-r--r--   0        0        0     2314 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/dispatch-conf.conf
+-rw-r--r--   0        0        0     2000 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/etc-update.conf
+-rw-r--r--   0        0        0      272 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/logrotate.d/elog-save-summary
+-rw-r--r--   0        0        0    20487 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example
+-rw-r--r--   0        0        0     1718 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.alpha.diff
+-rw-r--r--   0        0        0     2319 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.amd64-fbsd.diff
+-rw-r--r--   0        0        0     2309 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.amd64.diff
+-rw-r--r--   0        0        0     1425 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.arc.diff
+-rw-r--r--   0        0        0     1592 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.arm.diff
+-rw-r--r--   0        0        0     1580 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.arm64.diff
+-rw-r--r--   0        0        0     2465 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.hppa.diff
+-rw-r--r--   0        0        0      663 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.ia64.diff
+-rw-r--r--   0        0        0     2192 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.loong.diff
+-rw-r--r--   0        0        0      900 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.m68k.diff
+-rw-r--r--   0        0        0     1383 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.mips.diff
+-rw-r--r--   0        0        0     3541 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.ppc.diff
+-rw-r--r--   0        0        0     2361 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.ppc64.diff
+-rw-r--r--   0        0        0     2332 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.riscv.diff
+-rw-r--r--   0        0        0      656 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.s390.diff
+-rw-r--r--   0        0        0     1257 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.sh.diff
+-rw-r--r--   0        0        0      728 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.sparc-fbsd.diff
+-rw-r--r--   0        0        0     2129 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.sparc.diff
+-rw-r--r--   0        0        0     2507 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.x86-fbsd.diff
+-rw-r--r--   0        0        0     3759 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.conf.example.x86.diff
+-rw-r--r--   0        0        0     7661 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/make.globals
+-rw-r--r--   0        0        0     3193 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/meson.build
+-rw-r--r--   0        0        0     2311 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/repo.postsync.d/example
+-rw-r--r--   0        0        0      640 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/repos.conf
+-rw-r--r--   0        0        0     4000 2024-04-28 00:34:23.000000 portage-3.0.64/cnf/sets/portage.conf
+-rw-r--r--   0        0        0        7 2024-04-28 00:34:23.000000 portage-3.0.64/doc/api/.gitignore
+-rw-r--r--   0        0        0     1141 2024-04-28 00:34:23.000000 portage-3.0.64/doc/api/Makefile
+-rw-r--r--   0        0        0     2372 2024-04-28 00:34:23.000000 portage-3.0.64/doc/api/conf.py
+-rw-r--r--   0        0        0      217 2024-04-28 00:34:23.000000 portage-3.0.64/doc/api/index.rst
+-rw-r--r--   0        0        0     1544 2024-04-28 00:34:23.000000 portage-3.0.64/doc/api/meson.build
+-rw-r--r--   0        0        0     1900 2024-04-28 00:34:23.000000 portage-3.0.64/doc/config/bashrc.docbook
+-rw-r--r--   0        0        0    26217 2024-04-28 00:34:23.000000 portage-3.0.64/doc/config/sets.docbook
+-rw-r--r--   0        0        0       85 2024-04-28 00:34:23.000000 portage-3.0.64/doc/config.docbook
+-rw-r--r--   0        0        0      257 2024-04-28 00:34:23.000000 portage-3.0.64/doc/custom.xsl
+-rw-r--r--   0        0        0     3281 2024-04-28 00:34:23.000000 portage-3.0.64/doc/dependency_resolution/decision_making.docbook
+-rw-r--r--   0        0        0     4154 2024-04-28 00:34:23.000000 portage-3.0.64/doc/dependency_resolution/package_modeling.docbook
+-rw-r--r--   0        0        0     3451 2024-04-28 00:34:23.000000 portage-3.0.64/doc/dependency_resolution/task_scheduling.docbook
+-rw-r--r--   0        0        0      200 2024-04-28 00:34:23.000000 portage-3.0.64/doc/dependency_resolution.docbook
+-rw-r--r--   0        0        0      121 2024-04-28 00:34:23.000000 portage-3.0.64/doc/fragment/meson.build
+-rw-r--r--   0        0        0       37 2024-04-28 00:34:23.000000 portage-3.0.64/doc/fragment/version.in
+-rw-r--r--   0        0        0     2039 2024-04-28 00:34:23.000000 portage-3.0.64/doc/meson.build
+-rw-r--r--   0        0        0      487 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/eapi/0.docbook
+-rw-r--r--   0        0        0     1598 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/eapi/1.docbook
+-rw-r--r--   0        0        0     8299 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/eapi/2.docbook
+-rw-r--r--   0        0        0     2938 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/eapi/3.docbook
+-rw-r--r--   0        0        0     3112 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/eapi/4-slot-abi.docbook
+-rw-r--r--   0        0        0    14689 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/eapi/4.docbook
+-rw-r--r--   0        0        0     8044 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/eapi/5.docbook
+-rw-r--r--   0        0        0     1725 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/helper_functions.docbook
+-rw-r--r--   0        0        0     2780 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild/phases.docbook
+-rw-r--r--   0        0        0      364 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package/ebuild.docbook
+-rw-r--r--   0        0        0       76 2024-04-28 00:34:23.000000 portage-3.0.64/doc/package.docbook
+-rw-r--r--   0        0        0     2147 2024-04-28 00:34:23.000000 portage-3.0.64/doc/portage.docbook
+-rw-r--r--   0        0        0    19581 2024-04-28 00:34:23.000000 portage-3.0.64/doc/qa.docbook
+-rw-r--r--   0        0        0      836 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/AbstractDepPriority.py
+-rw-r--r--   0        0        0    14502 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/AbstractEbuildProcess.py
+-rw-r--r--   0        0        0     3723 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/AbstractPollTask.py
+-rw-r--r--   0        0        0     9829 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/AsynchronousLock.py
+-rw-r--r--   0        0        0     7098 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/AsynchronousTask.py
+-rw-r--r--   0        0        0      473 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/AtomArg.py
+-rw-r--r--   0        0        0    22225 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/Binpkg.py
+-rw-r--r--   0        0        0     2329 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/BinpkgEnvExtractor.py
+-rw-r--r--   0        0        0     5399 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/BinpkgExtractorAsync.py
+-rw-r--r--   0        0        0    11147 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/BinpkgFetcher.py
+-rw-r--r--   0        0        0     3341 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/BinpkgPrefetcher.py
+-rw-r--r--   0        0        0     4908 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/BinpkgVerifier.py
+-rw-r--r--   0        0        0      483 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/Blocker.py
+-rw-r--r--   0        0        0     6827 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/BlockerCache.py
+-rw-r--r--   0        0        0     5325 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/BlockerDB.py
+-rw-r--r--   0        0        0      355 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/BlockerDepPriority.py
+-rw-r--r--   0        0        0     4228 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/CompositeTask.py
+-rw-r--r--   0        0        0     1843 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/DepPriority.py
+-rw-r--r--   0        0        0     1856 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/DepPriorityNormalRange.py
+-rw-r--r--   0        0        0     4024 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/DepPrioritySatisfiedRange.py
+-rw-r--r--   0        0        0      878 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/Dependency.py
+-rw-r--r--   0        0        0     1056 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/DependencyArg.py
+-rw-r--r--   0        0        0     2728 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildBinpkg.py
+-rw-r--r--   0        0        0    23601 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildBuild.py
+-rw-r--r--   0        0        0     5749 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildBuildDir.py
+-rw-r--r--   0        0        0     2961 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildExecuter.py
+-rw-r--r--   0        0        0    14626 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildFetcher.py
+-rw-r--r--   0        0        0     1181 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildFetchonly.py
+-rw-r--r--   0        0        0     4716 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildIpcDaemon.py
+-rw-r--r--   0        0        0     3239 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildMerge.py
+-rw-r--r--   0        0        0     8795 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildMetadataPhase.py
+-rw-r--r--   0        0        0    25490 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildPhase.py
+-rw-r--r--   0        0        0      872 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildProcess.py
+-rw-r--r--   0        0        0      679 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/EbuildSpawnProcess.py
+-rw-r--r--   0        0        0    12786 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/FakeVartree.py
+-rw-r--r--   0        0        0     1774 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/FifoIpcDaemon.py
+-rw-r--r--   0        0        0     9142 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/JobStatusDisplay.py
+-rw-r--r--   0        0        0     4816 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/MergeListItem.py
+-rw-r--r--   0        0        0     6606 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/MetadataRegen.py
+-rw-r--r--   0        0        0     2424 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/MiscFunctionsProcess.py
+-rw-r--r--   0        0        0    30872 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/Package.py
+-rw-r--r--   0        0        0      735 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/PackageArg.py
+-rw-r--r--   0        0        0     2640 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/PackageMerge.py
+-rw-r--r--   0        0        0     4333 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/PackagePhase.py
+-rw-r--r--   0        0        0     5870 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/PackageUninstall.py
+-rw-r--r--   0        0        0     4651 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/PackageVirtualDbapi.py
+-rw-r--r--   0        0        0     2680 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/PipeReader.py
+-rw-r--r--   0        0        0     6709 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/PollScheduler.py
+-rw-r--r--   0        0        0      603 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/ProgressHandler.py
+-rw-r--r--   0        0        0     1227 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/RootConfig.py
+-rw-r--r--   0        0        0    89303 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/Scheduler.py
+-rw-r--r--   0        0        0     2648 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/SequentialTaskQueue.py
+-rw-r--r--   0        0        0      421 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/SetArg.py
+-rw-r--r--   0        0        0     9861 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/SpawnProcess.py
+-rw-r--r--   0        0        0     3246 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/SubProcess.py
+-rw-r--r--   0        0        0     1478 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/Task.py
+-rw-r--r--   0        0        0     1538 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/TaskSequence.py
+-rw-r--r--   0        0        0      455 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/UninstallFailure.py
+-rw-r--r--   0        0        0     1531 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/UnmergeDepPriority.py
+-rw-r--r--   0        0        0     3547 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/UseFlagDisplay.py
+-rw-r--r--   0        0        0     2915 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/UserQuery.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/_find_deep_system_runtime_deps.py
+-rw-r--r--   0        0        0      442 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/_flush_elog_mod_echo.py
+-rw-r--r--   0        0        0   149252 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/actions.py
+-rw-r--r--   0        0        0     1952 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/chk_updated_cfg_files.py
+-rw-r--r--   0        0        0      498 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/clear_caches.py
+-rw-r--r--   0        0        0      579 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/countdown.py
+-rw-r--r--   0        0        0     9008 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/create_depgraph_params.py
+-rw-r--r--   0        0        0     5191 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/create_world_atom.py
+-rw-r--r--   0        0        0   516527 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/depgraph.py
+-rw-r--r--   0        0        0     1814 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/emergelog.py
+-rw-r--r--   0        0        0      958 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/getloadavg.py
+-rw-r--r--   0        0        0     3425 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/help.py
+-rw-r--r--   0        0        0      785 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/is_valid_package_atom.py
+-rw-r--r--   0        0        0    42796 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/main.py
+-rw-r--r--   0        0        0     2787 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/meson.build
+-rw-r--r--   0        0        0     5614 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/post_emerge.py
+-rw-r--r--   0        0        0     3198 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/DbapiProvidesIndex.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/__init__.py
+-rw-r--r--   0        0        0    11328 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/backtracking.py
+-rw-r--r--   0        0        0    12441 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/circular_dependency.py
+-rw-r--r--   0        0        0      310 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/meson.build
+-rw-r--r--   0        0        0    39524 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/output.py
+-rw-r--r--   0        0        0    20748 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/output_helpers.py
+-rw-r--r--   0        0        0    15636 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/package_tracker.py
+-rw-r--r--   0        0        0    58875 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/resolver/slot_collision.py
+-rw-r--r--   0        0        0    20639 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/search.py
+-rw-r--r--   0        0        0     1573 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/show_invalid_depstring_notice.py
+-rw-r--r--   0        0        0     3196 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/stdout_spinner.py
+-rw-r--r--   0        0        0    26360 2024-04-28 00:34:23.000000 portage-3.0.64/lib/_emerge/unmerge.py
+-rw-r--r--   0        0        0       36 2024-04-28 00:34:23.000000 portage-3.0.64/lib/meson.build
+-rw-r--r--   0        0        0    24470 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_compat_upgrade/__init__.py
+-rw-r--r--   0        0        0     1666 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_compat_upgrade/binpkg_compression.py
+-rw-r--r--   0        0        0     1641 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_compat_upgrade/binpkg_format.py
+-rw-r--r--   0        0        0     1240 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_compat_upgrade/binpkg_multi_instance.py
+-rw-r--r--   0        0        0     4288 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_compat_upgrade/default_locations.py
+-rw-r--r--   0        0        0      260 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_compat_upgrade/meson.build
+-rw-r--r--   0        0        0     5376 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/Config.py
+-rw-r--r--   0        0        0     7215 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/ContentDB.py
+-rw-r--r--   0        0        0     4679 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/DeletionIterator.py
+-rw-r--r--   0        0        0     5030 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/DeletionTask.py
+-rw-r--r--   0        0        0    11319 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/FetchIterator.py
+-rw-r--r--   0        0        0    25403 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/FetchTask.py
+-rw-r--r--   0        0        0     8831 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/MirrorDistTask.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/__init__.py
+-rw-r--r--   0        0        0    15993 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/main.py
+-rw-r--r--   0        0        0      331 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_emirrordist/meson.build
+-rw-r--r--   0        0        0    10327 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_global_updates.py
+-rw-r--r--   0        0        0     2550 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_legacy_globals.py
+-rw-r--r--   0        0        0     4819 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_selinux.py
+-rw-r--r--   0        0        0     1719 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/ProfilePackageSet.py
+-rw-r--r--   0        0        0    14423 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/__init__.py
+-rw-r--r--   0        0        0     8205 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/base.py
+-rw-r--r--   0        0        0    22046 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/dbapi.py
+-rw-r--r--   0        0        0    15995 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/files.py
+-rw-r--r--   0        0        0     3602 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/libs.py
+-rw-r--r--   0        0        0      297 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/meson.build
+-rw-r--r--   0        0        0     2406 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/profiles.py
+-rw-r--r--   0        0        0     3535 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/security.py
+-rw-r--r--   0        0        0     1442 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/_sets/shell.py
+-rw-r--r--   0        0        0     2580 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/binpkg.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/binrepo/__init__.py
+-rw-r--r--   0        0        0     4553 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/binrepo/config.py
+-rw-r--r--   0        0        0      144 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/binrepo/meson.build
+-rw-r--r--   0        0        0      101 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/__init__.py
+-rw-r--r--   0        0        0     3710 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/anydbm.py
+-rw-r--r--   0        0        0     2139 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/cache_errors.py
+-rw-r--r--   0        0        0     5226 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/ebuild_xattr.py
+-rw-r--r--   0        0        0     5286 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/flat_hash.py
+-rw-r--r--   0        0        0     3197 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/fs_template.py
+-rw-r--r--   0        0        0      562 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/index/IndexStreamIterator.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/index/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/index/meson.build
+-rw-r--r--   0        0        0     1394 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/index/pkg_desc_index.py
+-rw-r--r--   0        0        0    11883 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/mappings.py
+-rw-r--r--   0        0        0      403 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/meson.build
+-rw-r--r--   0        0        0     5844 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/metadata.py
+-rw-r--r--   0        0        0    11821 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/sql_template.py
+-rw-r--r--   0        0        0    13804 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/sqlite.py
+-rw-r--r--   0        0        0    13275 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/template.py
+-rw-r--r--   0        0        0      789 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cache/volatile.py
+-rw-r--r--   0        0        0    16566 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/checksum.py
+-rw-r--r--   0        0        0     9647 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/const.py
+-rw-r--r--   0        0        0    11470 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/cvstree.py
+-rw-r--r--   0        0        0    11537 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/data.py
+-rw-r--r--   0        0        0      643 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/DummyTree.py
+-rw-r--r--   0        0        0     5690 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/IndexedPortdb.py
+-rw-r--r--   0        0        0     3743 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/IndexedVardb.py
+-rw-r--r--   0        0        0     2991 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/_ContentsCaseSensitivityManager.py
+-rw-r--r--   0        0        0    11200 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/_MergeProcess.py
+-rw-r--r--   0        0        0     1502 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/_SyncfsProcess.py
+-rw-r--r--   0        0        0     6019 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/_VdbMetadataDelta.py
+-rw-r--r--   0        0        0    17596 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/__init__.py
+-rw-r--r--   0        0        0     2545 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/_expand_new_virt.py
+-rw-r--r--   0        0        0     1685 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/_similar_name_search.py
+-rw-r--r--   0        0        0    97795 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/bintree.py
+-rw-r--r--   0        0        0     4184 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/cpv_expand.py
+-rw-r--r--   0        0        0     1889 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/dep_expand.py
+-rw-r--r--   0        0        0      540 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/meson.build
+-rw-r--r--   0        0        0    67024 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/porttree.py
+-rw-r--r--   0        0        0   254525 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/vartree.py
+-rw-r--r--   0        0        0     7587 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dbapi/virtual.py
+-rw-r--r--   0        0        0     3956 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/debug.py
+-rw-r--r--   0        0        0   108089 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/__init__.py
+-rw-r--r--   0        0        0     3780 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/_dnf.py
+-rw-r--r--   0        0        0     4605 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/_slot_operator.py
+-rw-r--r--   0        0        0    43041 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/dep_check.py
+-rw-r--r--   0        0        0     2612 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/libc.py
+-rw-r--r--   0        0        0      228 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/meson.build
+-rw-r--r--   0        0        0     2110 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/soname/SonameAtom.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/soname/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/soname/meson.build
+-rw-r--r--   0        0        0     5311 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/soname/multilib_category.py
+-rw-r--r--   0        0        0     1491 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dep/soname/parse.py
+-rw-r--r--   0        0        0    14093 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/dispatch_conf.py
+-rw-r--r--   0        0        0     8092 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/eapi.py
+-rw-r--r--   0        0        0     6757 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/eclass_cache.py
+-rw-r--r--   0        0        0     6879 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/filtering.py
+-rw-r--r--   0        0        0      348 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/meson.build
+-rw-r--r--   0        0        0     6065 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/messages.py
+-rw-r--r--   0        0        0     3378 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/mod_custom.py
+-rw-r--r--   0        0        0     2401 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/mod_echo.py
+-rw-r--r--   0        0        0     1660 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/mod_mail.py
+-rw-r--r--   0        0        0     3183 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/mod_mail_summary.py
+-rw-r--r--   0        0        0     3396 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/mod_save.py
+-rw-r--r--   0        0        0     3580 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/mod_save_summary.py
+-rw-r--r--   0        0        0      974 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/elog/mod_syslog.py
+-rw-r--r--   0        0        0      163 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/__init__.py
+-rw-r--r--   0        0        0      762 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/defaults.py
+-rw-r--r--   0        0        0     8705 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/main.py
+-rw-r--r--   0        0        0      183 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/meson.build
+-rw-r--r--   0        0        0      173 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/__init__.py
+-rw-r--r--   0        0        0      524 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/binhost/__init__.py
+-rw-r--r--   0        0        0     6358 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/binhost/binhost.py
+-rw-r--r--   0        0        0      160 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/binhost/meson.build
+-rw-r--r--   0        0        0      534 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/config/__init__.py
+-rw-r--r--   0        0        0     2520 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/config/config.py
+-rw-r--r--   0        0        0      158 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/config/meson.build
+-rw-r--r--   0        0        0     1629 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/logs/__init__.py
+-rw-r--r--   0        0        0     3535 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/logs/logs.py
+-rw-r--r--   0        0        0      154 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/logs/meson.build
+-rw-r--r--   0        0        0     1417 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/merges/__init__.py
+-rw-r--r--   0        0        0     9897 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/merges/merges.py
+-rw-r--r--   0        0        0      158 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/merges/meson.build
+-rw-r--r--   0        0        0      261 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/meson.build
+-rw-r--r--   0        0        0      851 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/move/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/move/meson.build
+-rw-r--r--   0        0        0     7693 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/move/move.py
+-rw-r--r--   0        0        0      566 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/resume/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/resume/meson.build
+-rw-r--r--   0        0        0     1900 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/resume/resume.py
+-rw-r--r--   0        0        0     2145 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/sync/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/sync/meson.build
+-rw-r--r--   0        0        0    18470 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/sync/sync.py
+-rw-r--r--   0        0        0      502 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/world/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/world/meson.build
+-rw-r--r--   0        0        0     3109 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/emaint/modules/world/world.py
+-rw-r--r--   0        0        0       52 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/env/__init__.py
+-rw-r--r--   0        0        0     3054 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/env/config.py
+-rw-r--r--   0        0        0    10311 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/env/loaders.py
+-rw-r--r--   0        0        0      187 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/env/meson.build
+-rw-r--r--   0        0        0      578 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/env/validators.py
+-rw-r--r--   0        0        0     6867 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/exception.py
+-rw-r--r--   0        0        0    31465 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/getbinpkg.py
+-rw-r--r--   0        0        0    31427 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/glsa.py
+-rw-r--r--   0        0        0     3819 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/gpg.py
+-rw-r--r--   0        0        0    78613 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/gpkg.py
+-rw-r--r--   0        0        0      579 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/installation.py
+-rw-r--r--   0        0        0     1550 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/localization.py
+-rw-r--r--   0        0        0    28609 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/locks.py
+-rw-r--r--   0        0        0     6187 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/mail.py
+-rw-r--r--   0        0        0    31108 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/manifest.py
+-rw-r--r--   0        0        0     1449 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/meson.build
+-rw-r--r--   0        0        0     8221 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/metadata.py
+-rw-r--r--   0        0        0     8568 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/module.py
+-rw-r--r--   0        0        0    18469 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/news.py
+-rw-r--r--   0        0        0    30358 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/output.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/__init__.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/__init__.py
+-rw-r--r--   0        0        0    13005 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/KeywordsManager.py
+-rw-r--r--   0        0        0     9192 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/LicenseManager.py
+-rw-r--r--   0        0        0    16684 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/LocationsManager.py
+-rw-r--r--   0        0        0    13915 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/MaskManager.py
+-rw-r--r--   0        0        0    21565 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/UseManager.py
+-rw-r--r--   0        0        0     8445 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/VirtualsManager.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/env_var_validation.py
+-rw-r--r--   0        0        0     4694 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/features_set.py
+-rw-r--r--   0        0        0     2273 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/helper.py
+-rw-r--r--   0        0        0      421 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/meson.build
+-rw-r--r--   0        0        0     9546 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_config/special_env_vars.py
+-rw-r--r--   0        0        0      829 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_ipc/ExitCommand.py
+-rw-r--r--   0        0        0      212 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_ipc/IpcCommand.py
+-rw-r--r--   0        0        0     5193 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_ipc/QueryCommand.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_ipc/__init__.py
+-rw-r--r--   0        0        0      213 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_ipc/meson.build
+-rw-r--r--   0        0        0     1405 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_metadata_invalid.py
+-rw-r--r--   0        0        0     1815 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py
+-rw-r--r--   0        0        0     3768 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py
+-rw-r--r--   0        0        0     7859 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_parallel_manifest/__init__.py
+-rw-r--r--   0        0        0      238 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_parallel_manifest/meson.build
+-rw-r--r--   0        0        0     4987 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/_spawn_nofetch.py
+-rw-r--r--   0        0        0   134026 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/config.py
+-rw-r--r--   0        0        0     4195 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/deprecated_profile_check.py
+-rw-r--r--   0        0        0     6732 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/digestcheck.py
+-rw-r--r--   0        0        0     9417 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/digestgen.py
+-rw-r--r--   0        0        0   115330 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/doebuild.py
+-rw-r--r--   0        0        0    79562 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/fetch.py
+-rw-r--r--   0        0        0     4689 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/getmaskingreason.py
+-rw-r--r--   0        0        0     6556 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/getmaskingstatus.py
+-rw-r--r--   0        0        0      529 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/meson.build
+-rw-r--r--   0        0        0    19287 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/prepare_build_dirs.py
+-rw-r--r--   0        0        0     1004 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/ebuild/profile_iuse.py
+-rw-r--r--   0        0        0      141 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/package/meson.build
+-rw-r--r--   0        0        0    52283 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/process.py
+-rw-r--r--   0        0        0     1573 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/progress.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/proxy/__init__.py
+-rw-r--r--   0        0        0     7762 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/proxy/lazyimport.py
+-rw-r--r--   0        0        0      172 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/proxy/meson.build
+-rw-r--r--   0        0        0     2856 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/proxy/objectproxy.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/__init__.py
+-rw-r--r--   0        0        0    62134 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/config.py
+-rw-r--r--   0        0        0      166 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/meson.build
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/storage/__init__.py
+-rw-r--r--   0        0        0     3950 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/storage/hardlink_quarantine.py
+-rw-r--r--   0        0        0    10937 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/storage/hardlink_rcu.py
+-rw-r--r--   0        0        0     1153 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/storage/inplace.py
+-rw-r--r--   0        0        0     2675 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/storage/interface.py
+-rw-r--r--   0        0        0      241 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/repository/storage/meson.build
+-rw-r--r--   0        0        0     1589 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/__init__.py
+-rw-r--r--   0        0        0     3015 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/config_checks.py
+-rw-r--r--   0        0        0    14873 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/controller.py
+-rw-r--r--   0        0        0      696 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/getaddrinfo_validate.py
+-rw-r--r--   0        0        0      283 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/meson.build
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/__init__.py
+-rw-r--r--   0        0        0     1650 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/cvs/__init__.py
+-rw-r--r--   0        0        0     2341 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/cvs/cvs.py
+-rw-r--r--   0        0        0      150 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/cvs/meson.build
+-rw-r--r--   0        0        0     2770 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/git/__init__.py
+-rw-r--r--   0        0        0    24957 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/git/git.py
+-rw-r--r--   0        0        0      150 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/git/meson.build
+-rw-r--r--   0        0        0     1403 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/mercurial/__init__.py
+-rw-r--r--   0        0        0     6125 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/mercurial/mercurial.py
+-rw-r--r--   0        0        0      162 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/mercurial/meson.build
+-rw-r--r--   0        0        0      226 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/meson.build
+-rw-r--r--   0        0        0     1287 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/rsync/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/rsync/meson.build
+-rw-r--r--   0        0        0    34132 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/rsync/rsync.py
+-rw-r--r--   0        0        0     1037 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/svn/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/svn/meson.build
+-rw-r--r--   0        0        0     2759 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/svn/svn.py
+-rw-r--r--   0        0        0     1650 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/webrsync/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/webrsync/meson.build
+-rw-r--r--   0        0        0     4983 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/webrsync/webrsync.py
+-rw-r--r--   0        0        0      975 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/zipfile/__init__.py
+-rw-r--r--   0        0        0     4452 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/modules/zipfile/zipfile.py
+-rw-r--r--   0        0        0     2485 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/old_tree_timestamp.py
+-rw-r--r--   0        0        0    13378 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/sync/syncbase.py
+-rw-r--r--   0        0        0     1850 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev
+-rw-r--r--   0        0        0     1852 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev
+-rw-r--r--   0        0        0     2055 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key
+-rw-r--r--   0        0        0     2055 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key
+-rw-r--r--   0        0        0     2774 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/.gnupg/pubring.kbx
+-rw-r--r--   0        0        0     1360 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/.gnupg/trustdb.gpg
+-rw-r--r--   0        0        0     3786 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/__test__.py
+-rw-r--r--   0        0        0      317 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/meson.build
+-rw-r--r--   0        0        0     2602 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/setup_env.py
+-rw-r--r--   0        0        0      547 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/test_dobin.py
+-rw-r--r--   0        0        0      565 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/test_dodir.py
+-rw-r--r--   0        0        0    13017 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/test_doins.py
+-rw-r--r--   0        0        0     9192 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/test_eapi7_ver_funcs.py
+-rw-r--r--   0        0        0     3083 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/bin/test_filter_bash_env.py
+-rw-r--r--   0        0        0     2454 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/conftest.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dbapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dbapi/__test__.py
+-rw-r--r--   0        0        0      263 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dbapi/meson.build
+-rw-r--r--   0        0        0     4867 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dbapi/test_auxdb.py
+-rw-r--r--   0        0        0     9211 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dbapi/test_bintree.py
+-rw-r--r--   0        0        0     3973 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dbapi/test_fakedbapi.py
+-rw-r--r--   0        0        0     9479 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dbapi/test_portdb_cache.py
+-rw-r--r--   0        0        0      169 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/__test__.py
+-rw-r--r--   0        0        0      839 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/meson.build
+-rw-r--r--   0        0        0    24520 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_atom.py
+-rw-r--r--   0        0        0     4452 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_best_match_to_list.py
+-rw-r--r--   0        0        0     9752 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_check_required_use.py
+-rw-r--r--   0        0        0     1149 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_dep_getcpv.py
+-rw-r--r--   0        0        0      988 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_dep_getrepo.py
+-rw-r--r--   0        0        0      934 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_dep_getslot.py
+-rw-r--r--   0        0        0     1402 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_dep_getusedeps.py
+-rw-r--r--   0        0        0     2077 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_dnf_convert.py
+-rw-r--r--   0        0        0      779 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_extended_atom_dict.py
+-rw-r--r--   0        0        0     3769 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_extract_affecting_use.py
+-rw-r--r--   0        0        0     1237 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_get_operator.py
+-rw-r--r--   0        0        0     1778 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_get_required_use_flags.py
+-rw-r--r--   0        0        0     1009 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_isjustname.py
+-rw-r--r--   0        0        0    11660 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_isvalidatom.py
+-rw-r--r--   0        0        0     2406 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_libc.py
+-rw-r--r--   0        0        0    11132 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_match_from_list.py
+-rw-r--r--   0        0        0     3245 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_overlap_dnf.py
+-rw-r--r--   0        0        0     2661 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_paren_reduce.py
+-rw-r--r--   0        0        0      790 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_soname_atom_pickle.py
+-rw-r--r--   0        0        0     1652 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_standalone.py
+-rw-r--r--   0        0        0    27656 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/dep/test_use_reduce.py
+-rw-r--r--   0        0        0      107 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/__test__.py
+-rw-r--r--   0        0        0      439 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/meson.build
+-rw-r--r--   0        0        0     1387 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_array_fromfile_eof.py
+-rw-r--r--   0        0        0    14001 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_config.py
+-rw-r--r--   0        0        0     7900 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py
+-rw-r--r--   0        0        0     5238 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_doebuild_spawn.py
+-rw-r--r--   0        0        0    35301 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_fetch.py
+-rw-r--r--   0        0        0     7065 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_ipc_daemon.py
+-rw-r--r--   0        0        0     5211 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_shell_quote.py
+-rw-r--r--   0        0        0     1920 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_spawn.py
+-rw-r--r--   0        0        0     4479 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/ebuild/test_use_expand_incremental.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/__test__.py
+-rw-r--r--   0        0        0    25096 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/conftest.py
+-rw-r--r--   0        0        0      425 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/meson.build
+-rw-r--r--   0        0        0     2617 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/test_actions.py
+-rw-r--r--   0        0        0     6946 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/test_baseline.py
+-rw-r--r--   0        0        0     7552 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/test_binpkg_fetch.py
+-rw-r--r--   0        0        0    10436 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/test_config_protect.py
+-rw-r--r--   0        0        0     6503 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py
+-rw-r--r--   0        0        0     6847 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/test_emerge_slot_abi.py
+-rw-r--r--   0        0        0     1320 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/test_global_updates.py
+-rw-r--r--   0        0        0    19102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/emerge/test_libc_dep_inject.py
+-rw-r--r--   0        0        0      169 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/__test__.py
+-rw-r--r--   0        0        0      176 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/config/__test__.py
+-rw-r--r--   0        0        0      301 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/config/meson.build
+-rw-r--r--   0        0        0     1164 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/config/test_PackageKeywordsFile.py
+-rw-r--r--   0        0        0      818 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/config/test_PackageMaskFile.py
+-rw-r--r--   0        0        0     1077 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/config/test_PackageUseFile.py
+-rw-r--r--   0        0        0     1149 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/config/test_PortageModulesFile.py
+-rw-r--r--   0        0        0      166 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/env/meson.build
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/glsa/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/glsa/__test__.py
+-rw-r--r--   0        0        0      181 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/glsa/meson.build
+-rw-r--r--   0        0        0     8021 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/glsa/test_security_set.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/__test__.py
+-rw-r--r--   0        0        0      376 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/meson.build
+-rw-r--r--   0        0        0    13834 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_checksum.py
+-rw-r--r--   0        0        0    16272 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_gpg.py
+-rw-r--r--   0        0        0     1929 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_metadata_update.py
+-rw-r--r--   0        0        0     5277 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_metadata_url.py
+-rw-r--r--   0        0        0    14781 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_path.py
+-rw-r--r--   0        0        0     1869 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_size.py
+-rw-r--r--   0        0        0     3306 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_stream.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lafilefixer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lafilefixer/__test__.py
+-rw-r--r--   0        0        0      187 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lafilefixer/meson.build
+-rw-r--r--   0        0        0     6338 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lafilefixer/test_lafilefixer.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lazyimport/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lazyimport/__test__.py
+-rw-r--r--   0        0        0      249 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lazyimport/meson.build
+-rw-r--r--   0        0        0     2860 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py
+-rw-r--r--   0        0        0      596 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lazyimport/test_preload_portage_submodules.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lint/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lint/__test__.py
+-rw-r--r--   0        0        0      272 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lint/meson.build
+-rw-r--r--   0        0        0      214 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lint/metadata.py
+-rw-r--r--   0        0        0     2345 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lint/test_bash_syntax.py
+-rw-r--r--   0        0        0     3031 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lint/test_compile_modules.py
+-rw-r--r--   0        0        0     1516 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/lint/test_import_modules.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/locks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/locks/__test__.py
+-rw-r--r--   0        0        0      220 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/locks/meson.build
+-rw-r--r--   0        0        0     7546 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/locks/test_asynchronous_lock.py
+-rw-r--r--   0        0        0     2552 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/locks/test_lock_nonblock.py
+-rw-r--r--   0        0        0      507 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/meson.build
+-rw-r--r--   0        0        0      170 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/news/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/news/__test__.py
+-rw-r--r--   0        0        0      177 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/news/meson.build
+-rw-r--r--   0        0        0    14381 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/news/test_NewsItem.py
+-rw-r--r--   0        0        0      107 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/__test__.py
+-rw-r--r--   0        0        0      513 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/meson.build
+-rw-r--r--   0        0        0     4144 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_AsyncFunction.py
+-rw-r--r--   0        0        0     1545 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_ForkProcess.py
+-rw-r--r--   0        0        0     2332 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_PipeLogger.py
+-rw-r--r--   0        0        0     3121 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_PopenProcess.py
+-rw-r--r--   0        0        0     2061 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_PopenProcessBlockingIO.py
+-rw-r--r--   0        0        0     1684 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_pickle.py
+-rw-r--r--   0        0        0     3811 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_poll.py
+-rw-r--r--   0        0        0      987 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_spawn_fail_e2big.py
+-rw-r--r--   0        0        0     1195 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_spawn_returnproc.py
+-rw-r--r--   0        0        0     1341 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_spawn_warn_large_env.py
+-rw-r--r--   0        0        0     1504 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/process/test_unshare_net.py
+-rw-r--r--   0        0        0    44218 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/ResolverPlayground.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/__test__.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/binpkg_multi_instance/__init__.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/binpkg_multi_instance/__test__.py
+-rw-r--r--   0        0        0      254 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/binpkg_multi_instance/meson.build
+-rw-r--r--   0        0        0     5585 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py
+-rw-r--r--   0        0        0     3747 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py
+-rw-r--r--   0        0        0     3664 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/meson.build
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/__init__.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/__test__.py
+-rw-r--r--   0        0        0      519 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/meson.build
+-rw-r--r--   0        0        0     3931 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_autounmask.py
+-rw-r--r--   0        0        0     1755 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_depclean.py
+-rw-r--r--   0        0        0     8528 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_downgrade.py
+-rw-r--r--   0        0        0     3840 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_or_choices.py
+-rw-r--r--   0        0        0     3305 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_reinstall.py
+-rw-r--r--   0        0        0     4521 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_skip_update.py
+-rw-r--r--   0        0        0    12877 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py
+-rw-r--r--   0        0        0     3971 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_slot_conflict_update.py
+-rw-r--r--   0        0        0     2944 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_soname_provided.py
+-rw-r--r--   0        0        0     2778 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_unsatisfiable.py
+-rw-r--r--   0        0        0     3354 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/soname/test_unsatisfied.py
+-rw-r--r--   0        0        0     2824 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py
+-rw-r--r--   0        0        0     9576 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_alternatives_gzip.py
+-rw-r--r--   0        0        0    28432 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_autounmask.py
+-rw-r--r--   0        0        0     2731 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_autounmask_binpkg_use.py
+-rw-r--r--   0        0        0     2176 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_autounmask_keep_keywords.py
+-rw-r--r--   0        0        0     3118 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_autounmask_multilib_use.py
+-rw-r--r--   0        0        0     1279 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_autounmask_parent.py
+-rw-r--r--   0        0        0     2573 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_autounmask_use_backtrack.py
+-rw-r--r--   0        0        0     3743 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_autounmask_use_breakage.py
+-rw-r--r--   0        0        0     1850 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py
+-rw-r--r--   0        0        0     5786 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_backtracking.py
+-rw-r--r--   0        0        0     6805 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_bdeps.py
+-rw-r--r--   0        0        0     4927 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py
+-rw-r--r--   0        0        0     4231 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_blocker.py
+-rw-r--r--   0        0        0     2459 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_broken_deps.py
+-rw-r--r--   0        0        0     4330 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_changed_deps.py
+-rw-r--r--   0        0        0     7899 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_circular_choices.py
+-rw-r--r--   0        0        0     3341 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_circular_choices_rust.py
+-rw-r--r--   0        0        0     4832 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_circular_dependencies.py
+-rw-r--r--   0        0        0     4948 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_complete_graph.py
+-rw-r--r--   0        0        0     2910 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py
+-rw-r--r--   0        0        0     5605 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_cross_dep_priority.py
+-rw-r--r--   0        0        0     9959 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_depclean.py
+-rw-r--r--   0        0        0     5070 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_depclean_order.py
+-rw-r--r--   0        0        0     2444 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_depclean_slot_unavailable.py
+-rw-r--r--   0        0        0    13377 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_depth.py
+-rw-r--r--   0        0        0     3329 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_disjunctive_depend_order.py
+-rw-r--r--   0        0        0     9971 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_eapi.py
+-rw-r--r--   0        0        0     4323 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_emptytree_reinstall_unsatisfiability.py
+-rw-r--r--   0        0        0     2658 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_features_test_use.py
+-rw-r--r--   0        0        0     3379 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py
+-rw-r--r--   0        0        0     3457 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_installkernel.py
+-rw-r--r--   0        0        0    11063 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_keywords.py
+-rw-r--r--   0        0        0    31277 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_merge_order.py
+-rw-r--r--   0        0        0     1234 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py
+-rw-r--r--   0        0        0    15920 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_multirepo.py
+-rw-r--r--   0        0        0     1772 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_multislot.py
+-rw-r--r--   0        0        0     1554 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_old_dep_chain_display.py
+-rw-r--r--   0        0        0     1142 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_onlydeps.py
+-rw-r--r--   0        0        0     1527 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_onlydeps_circular.py
+-rw-r--r--   0        0        0     5933 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_onlydeps_ideps.py
+-rw-r--r--   0        0        0     2552 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_onlydeps_minimal.py
+-rw-r--r--   0        0        0    25128 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_or_choices.py
+-rw-r--r--   0        0        0     2716 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_or_downgrade_installed.py
+-rw-r--r--   0        0        0     6850 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_or_upgrade_installed.py
+-rw-r--r--   0        0        0     3911 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_output.py
+-rw-r--r--   0        0        0     9049 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_package_tracker.py
+-rw-r--r--   0        0        0     4296 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_perl_rebuild_bug.py
+-rw-r--r--   0        0        0     4568 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_profile_default_eapi.py
+-rw-r--r--   0        0        0     3353 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_profile_package_set.py
+-rw-r--r--   0        0        0     6911 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_rebuild.py
+-rw-r--r--   0        0        0     5847 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_rebuild_ghostscript.py
+-rw-r--r--   0        0        0     2409 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py
+-rw-r--r--   0        0        0    11792 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_required_use.py
+-rw-r--r--   0        0        0     7177 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py
+-rw-r--r--   0        0        0     3500 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_simple.py
+-rw-r--r--   0        0        0    18128 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_abi.py
+-rw-r--r--   0        0        0     8790 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_abi_downgrade.py
+-rw-r--r--   0        0        0     3488 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_change_without_revbump.py
+-rw-r--r--   0        0        0    13393 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_collisions.py
+-rw-r--r--   0        0        0     2528 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_blocked_prune.py
+-rw-r--r--   0        0        0     1990 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py
+-rw-r--r--   0        0        0     1432 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_mask_update.py
+-rw-r--r--   0        0        0    14826 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_rebuild.py
+-rw-r--r--   0        0        0     7910 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py
+-rw-r--r--   0        0        0     2579 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_update.py
+-rw-r--r--   0        0        0     2491 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_update_virt.py
+-rw-r--r--   0        0        0     5024 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_autounmask.py
+-rw-r--r--   0        0        0     7642 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_bdeps.py
+-rw-r--r--   0        0        0     4350 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_complete_graph.py
+-rw-r--r--   0        0        0     4694 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py
+-rw-r--r--   0        0        0     4366 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_missed_update.py
+-rw-r--r--   0        0        0     3719 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_rebuild.py
+-rw-r--r--   0        0        0     1682 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_required_use.py
+-rw-r--r--   0        0        0     9190 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py
+-rw-r--r--   0        0        0     3974 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py
+-rw-r--r--   0        0        0     2103 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py
+-rw-r--r--   0        0        0     3518 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_unsolved.py
+-rw-r--r--   0        0        0     2107 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py
+-rw-r--r--   0        0        0     1819 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py
+-rw-r--r--   0        0        0     3584 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_targetroot.py
+-rw-r--r--   0        0        0    11321 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_unmerge_order.py
+-rw-r--r--   0        0        0     1571 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_unnecessary_slot_upgrade.py
+-rw-r--r--   0        0        0     3843 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_update.py
+-rw-r--r--   0        0        0     1827 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_use_dep_defaults.py
+-rw-r--r--   0        0        0    10931 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_useflags.py
+-rw-r--r--   0        0        0     9976 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_virtual_minimize_children.py
+-rw-r--r--   0        0        0     9326 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_virtual_slot.py
+-rw-r--r--   0        0        0     2910 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/resolver/test_with_test_deps.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/__test__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/base/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/base/__test__.py
+-rw-r--r--   0        0        0      226 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/base/meson.build
+-rw-r--r--   0        0        0     2051 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/base/test_internal_package_set.py
+-rw-r--r--   0        0        0     1555 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/base/test_variable_set.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/files/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/files/__test__.py
+-rw-r--r--   0        0        0      225 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/files/meson.build
+-rw-r--r--   0        0        0     1018 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/files/test_config_file_set.py
+-rw-r--r--   0        0        0      855 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/files/test_static_file_set.py
+-rw-r--r--   0        0        0      197 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/meson.build
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/shell/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/shell/__test__.py
+-rw-r--r--   0        0        0      180 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/shell/meson.build
+-rw-r--r--   0        0        0      801 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sets/shell/test_shell.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sync/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sync/__test__.py
+-rw-r--r--   0        0        0      211 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sync/meson.build
+-rw-r--r--   0        0        0    16350 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sync/test_sync_local.py
+-rw-r--r--   0        0        0     3087 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/sync/test_sync_zipfile.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/unicode/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/unicode/__test__.py
+-rw-r--r--   0        0        0      185 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/unicode/meson.build
+-rw-r--r--   0        0        0     2293 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/unicode/test_string_format.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/update/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/update/__test__.py
+-rw-r--r--   0        0        0      246 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/update/meson.build
+-rw-r--r--   0        0        0    11839 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/update/test_move_ent.py
+-rw-r--r--   0        0        0    11094 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/update/test_move_slot_ent.py
+-rw-r--r--   0        0        0    20527 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/update/test_update_dbentry.py
+-rw-r--r--   0        0        0      170 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/__test__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/dyn_libs/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/dyn_libs/__test__.py
+-rw-r--r--   0        0        0      226 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/dyn_libs/meson.build
+-rw-r--r--   0        0        0     2695 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/dyn_libs/test_installed_dynlibs.py
+-rw-r--r--   0        0        0     1389 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/dyn_libs/test_soname_deps.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/eventloop/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/eventloop/__test__.py
+-rw-r--r--   0        0        0      193 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/eventloop/meson.build
+-rw-r--r--   0        0        0      826 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/eventloop/test_call_soon_fifo.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/file_copy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/file_copy/__test__.py
+-rw-r--r--   0        0        0      187 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/file_copy/meson.build
+-rw-r--r--   0        0        0     2646 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/file_copy/test_copyfile.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/__test__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/__test__.py
+-rw-r--r--   0        0        0      388 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/meson.build
+-rw-r--r--   0        0        0     2025 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py
+-rw-r--r--   0        0        0     5396 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py
+-rw-r--r--   0        0        0      795 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py
+-rw-r--r--   0        0        0     1394 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py
+-rw-r--r--   0        0        0     6914 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py
+-rw-r--r--   0        0        0     2344 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py
+-rw-r--r--   0        0        0      312 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/meson.build
+-rw-r--r--   0        0        0     1274 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/test_done_callback.py
+-rw-r--r--   0        0        0     1565 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/test_done_callback_after_exit.py
+-rw-r--r--   0        0        0     2933 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/test_iter_completed.py
+-rw-r--r--   0        0        0    11301 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/futures/test_retry.py
+-rw-r--r--   0        0        0      750 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/meson.build
+-rw-r--r--   0        0        0     5805 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_checksum.py
+-rw-r--r--   0        0        0    11345 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_digraph.py
+-rw-r--r--   0        0        0     1824 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_file_copier.py
+-rw-r--r--   0        0        0     3539 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_getconfig.py
+-rw-r--r--   0        0        0      315 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_grabdict.py
+-rw-r--r--   0        0        0     5805 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_install_mask.py
+-rw-r--r--   0        0        0     1211 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_manifest.py
+-rw-r--r--   0        0        0    10489 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_mtimedb.py
+-rw-r--r--   0        0        0      440 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_normalizedPath.py
+-rw-r--r--   0        0        0     1735 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_shelve.py
+-rw-r--r--   0        0        0     8314 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_socks5.py
+-rw-r--r--   0        0        0      832 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_stackDictList.py
+-rw-r--r--   0        0        0     1185 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_stackDicts.py
+-rw-r--r--   0        0        0      715 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_stackLists.py
+-rw-r--r--   0        0        0      864 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_uniqueArray.py
+-rw-r--r--   0        0        0     3347 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_varExpand.py
+-rw-r--r--   0        0        0     1681 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_whirlpool.py
+-rw-r--r--   0        0        0     6243 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/util/test_xattr.py
+-rw-r--r--   0        0        0      174 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/versions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/versions/__test__.py
+-rw-r--r--   0        0        0      211 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/versions/meson.build
+-rw-r--r--   0        0        0      555 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/versions/test_cpv_sort_key.py
+-rw-r--r--   0        0        0     3026 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/versions/test_vercmp.py
+-rw-r--r--   0        0        0      169 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/xpak/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/xpak/__test__.py
+-rw-r--r--   0        0        0      178 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/xpak/meson.build
+-rw-r--r--   0        0        0      427 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/tests/xpak/test_decodeint.py
+-rw-r--r--   0        0        0    17014 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/update.py
+-rw-r--r--   0        0        0     2929 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/ExtractKernelVersion.py
+-rw-r--r--   0        0        0     2141 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/SlotObject.py
+-rw-r--r--   0        0        0    68950 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/__init__.py
+-rw-r--r--   0        0        0     2683 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/AsyncFunction.py
+-rw-r--r--   0        0        0     3393 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/AsyncScheduler.py
+-rw-r--r--   0        0        0     1165 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/AsyncTaskFuture.py
+-rw-r--r--   0        0        0     5892 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/BuildLogger.py
+-rw-r--r--   0        0        0     1220 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/FileCopier.py
+-rw-r--r--   0        0        0      801 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/FileDigester.py
+-rw-r--r--   0        0        0    12867 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/ForkProcess.py
+-rw-r--r--   0        0        0     7527 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/PipeLogger.py
+-rw-r--r--   0        0        0     2587 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/PipeReaderBlockingIO.py
+-rw-r--r--   0        0        0     1118 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/PopenProcess.py
+-rw-r--r--   0        0        0     4649 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/SchedulerInterface.py
+-rw-r--r--   0        0        0      643 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/TaskScheduler.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/meson.build
+-rw-r--r--   0        0        0     1360 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_async/run_main_scheduler.py
+-rw-r--r--   0        0        0     4347 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_compare_files.py
+-rw-r--r--   0        0        0     1640 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_ctypes.py
+-rw-r--r--   0        0        0     2654 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_desktop_entry.py
+-rw-r--r--   0        0        0    41422 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/LinkageMapELF.py
+-rw-r--r--   0        0        0     2877 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/NeededEntry.py
+-rw-r--r--   0        0        0     9385 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/__init__.py
+-rw-r--r--   0        0        0     3834 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/display_preserved_libs.py
+-rw-r--r--   0        0        0     2743 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/dyn_libs.py
+-rw-r--r--   0        0        0      335 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/meson.build
+-rw-r--r--   0        0        0     6203 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/soname_deps.py
+-rw-r--r--   0        0        0     3722 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_dyn_libs/soname_deps_qa.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_eventloop/__init__.py
+-rw-r--r--   0        0        0     7395 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_eventloop/asyncio_event_loop.py
+-rw-r--r--   0        0        0      213 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_eventloop/global_event_loop.py
+-rw-r--r--   0        0        0      196 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_eventloop/meson.build
+-rw-r--r--   0        0        0     3029 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_get_vm_info.py
+-rw-r--r--   0        0        0     5956 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_info_files.py
+-rw-r--r--   0        0        0      692 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_path.py
+-rw-r--r--   0        0        0     3001 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_pty.py
+-rw-r--r--   0        0        0     4078 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_urlopen.py
+-rw-r--r--   0        0        0     7063 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/_xattr.py
+-rw-r--r--   0        0        0     1528 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/backoff.py
+-rw-r--r--   0        0        0      784 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/bin_entry_point.py
+-rw-r--r--   0        0        0     2189 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/changelog.py
+-rw-r--r--   0        0        0     3464 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/compression_probe.py
+-rw-r--r--   0        0        0     2403 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/configparser.py
+-rw-r--r--   0        0        0     2180 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/cpuinfo.py
+-rw-r--r--   0        0        0    12975 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/digraph.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/elf/__init__.py
+-rw-r--r--   0        0        0     1446 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/elf/constants.py
+-rw-r--r--   0        0        0     1889 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/elf/header.py
+-rw-r--r--   0        0        0      169 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/elf/meson.build
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/endian/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/endian/decode.py
+-rw-r--r--   0        0        0      148 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/endian/meson.build
+-rw-r--r--   0        0        0    17055 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/env_update.py
+-rw-r--r--   0        0        0     4055 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/file_copy.py
+-rw-r--r--   0        0        0     2118 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/formatter.py
+-rw-r--r--   0        0        0      180 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/__init__.py
+-rw-r--r--   0        0        0    10853 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/_asyncio/__init__.py
+-rw-r--r--   0        0        0      159 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/_asyncio/meson.build
+-rw-r--r--   0        0        0     3016 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/_asyncio/streams.py
+-rw-r--r--   0        0        0     1886 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/_sync_decorator.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/executor/__init__.py
+-rw-r--r--   0        0        0     4424 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/executor/fork.py
+-rw-r--r--   0        0        0      156 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/executor/meson.build
+-rw-r--r--   0        0        0     2830 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/extendedfutures.py
+-rw-r--r--   0        0        0      516 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/futures.py
+-rw-r--r--   0        0        0     6868 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/iter_completed.py
+-rw-r--r--   0        0        0      324 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/meson.build
+-rw-r--r--   0        0        0     6298 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/retry.py
+-rw-r--r--   0        0        0     2237 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/futures/unix_events.py
+-rw-r--r--   0        0        0     1584 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/hooks.py
+-rw-r--r--   0        0        0     6549 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/install_mask.py
+-rw-r--r--   0        0        0     2996 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/iterators/MultiIterGroupBy.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/iterators/__init__.py
+-rw-r--r--   0        0        0      161 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/iterators/meson.build
+-rw-r--r--   0        0        0     7350 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/lafilefixer.py
+-rw-r--r--   0        0        0     4814 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/listdir.py
+-rw-r--r--   0        0        0     4710 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/locale.py
+-rw-r--r--   0        0        0     1074 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/meson.build
+-rw-r--r--   0        0        0    14876 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/movefile.py
+-rw-r--r--   0        0        0     4258 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/mtimedb.py
+-rw-r--r--   0        0        0     2990 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/netlink.py
+-rw-r--r--   0        0        0     1336 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/path.py
+-rw-r--r--   0        0        0     1527 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/shelve.py
+-rw-r--r--   0        0        0     3718 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/socks5.py
+-rw-r--r--   0        0        0    58416 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/whirlpool.py
+-rw-r--r--   0        0        0     4541 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/util/writeable_check.py
+-rw-r--r--   0        0        0    20265 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/versions.py
+-rw-r--r--   0        0        0      102 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/xml/__init__.py
+-rw-r--r--   0        0        0      142 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/xml/meson.build
+-rw-r--r--   0        0        0    16789 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/xml/metadata.py
+-rw-r--r--   0        0        0    19634 2024-04-28 00:34:23.000000 portage-3.0.64/lib/portage/xpak.py
+-rwxr-xr-x   0        0        0     1280 2024-04-28 00:34:23.000000 portage-3.0.64/make.conf.example-repatch.sh
+-rw-r--r--   0        0        0     4275 2024-04-28 00:34:23.000000 portage-3.0.64/man/color.map.5
+-rw-r--r--   0        0        0     3634 2024-04-28 00:34:23.000000 portage-3.0.64/man/dispatch-conf.1
+-rw-r--r--   0        0        0    10769 2024-04-28 00:34:23.000000 portage-3.0.64/man/ebuild.1
+-rw-r--r--   0        0        0    61555 2024-04-28 00:34:23.000000 portage-3.0.64/man/ebuild.5
+-rw-r--r--   0        0        0     7452 2024-04-28 00:34:23.000000 portage-3.0.64/man/egencache.1
+-rw-r--r--   0        0        0     3507 2024-04-28 00:34:23.000000 portage-3.0.64/man/emaint.1
+-rw-r--r--   0        0        0    71865 2024-04-28 00:34:23.000000 portage-3.0.64/man/emerge.1
+-rw-r--r--   0        0        0     4778 2024-04-28 00:34:23.000000 portage-3.0.64/man/emirrordist.1
+-rw-r--r--   0        0        0     1062 2024-04-28 00:34:23.000000 portage-3.0.64/man/env-update.1
+-rw-r--r--   0        0        0     1733 2024-04-28 00:34:23.000000 portage-3.0.64/man/etc-update.1
+-rw-r--r--   0        0        0      458 2024-04-28 00:34:23.000000 portage-3.0.64/man/fixpackages.1
+-rw-r--r--   0        0        0     2341 2024-04-28 00:34:23.000000 portage-3.0.64/man/glsa-check.1
+-rw-r--r--   0        0        0    59822 2024-04-28 00:34:23.000000 portage-3.0.64/man/make.conf.5
+-rw-r--r--   0        0        0      549 2024-04-28 00:34:23.000000 portage-3.0.64/man/meson.build
+-rw-r--r--   0        0        0    64475 2024-04-28 00:34:23.000000 portage-3.0.64/man/portage.5
+-rw-r--r--   0        0        0     2339 2024-04-28 00:34:23.000000 portage-3.0.64/man/quickpkg.1
+-rw-r--r--   0        0        0     8221 2024-04-28 00:34:23.000000 portage-3.0.64/man/ru/color.map.5
+-rw-r--r--   0        0        0     6046 2024-04-28 00:34:23.000000 portage-3.0.64/man/ru/dispatch-conf.1
+-rw-r--r--   0        0        0    18214 2024-04-28 00:34:23.000000 portage-3.0.64/man/ru/ebuild.1
+-rw-r--r--   0        0        0     1862 2024-04-28 00:34:23.000000 portage-3.0.64/man/ru/env-update.1
+-rw-r--r--   0        0        0     3116 2024-04-28 00:34:23.000000 portage-3.0.64/man/ru/etc-update.1
+-rw-r--r--   0        0        0      860 2024-04-28 00:34:23.000000 portage-3.0.64/man/ru/fixpackages.1
+-rw-r--r--   0        0        0      374 2024-04-28 00:34:23.000000 portage-3.0.64/man/ru/meson.build
+-rw-r--r--   0        0        0     6382 2024-04-28 00:34:23.000000 portage-3.0.64/man/xpak.5
+-rw-r--r--   0        0        0     3352 2024-04-28 00:34:23.000000 portage-3.0.64/meson.build
+-rw-r--r--   0        0        0     1806 2024-04-28 00:34:23.000000 portage-3.0.64/meson_options.txt
+-rwxr-xr-x   0        0        0    29089 2024-04-28 00:34:23.000000 portage-3.0.64/misc/emerge-delta-webrsync
+-rw-r--r--   0        0        0    15198 2024-04-28 00:34:23.000000 portage-3.0.64/pylintrc
+-rw-r--r--   0        0        0     1650 2024-04-28 00:34:23.000000 portage-3.0.64/pyproject.toml
+-rwxr-xr-x   0        0        0       81 2024-04-28 00:34:23.000000 portage-3.0.64/run-pylint
+-rw-r--r--   0        0        0      595 2024-04-28 00:34:23.000000 portage-3.0.64/src/meson.build
+-rw-r--r--   0        0        0    71291 2024-04-28 00:34:23.000000 portage-3.0.64/src/portage_util__whirlpool.c
+-rw-r--r--   0        0        0      571 2024-04-28 00:34:23.000000 portage-3.0.64/testpath
+-rw-r--r--   0        0        0      543 2024-04-28 00:34:23.000000 portage-3.0.64/tox.ini
+-rw-r--r--   0        0        0    24629 2024-04-28 00:35:14.891370 portage-3.0.64/PKG-INFO
```

### Comparing `portage-3.0.63/.builds/ci.yml` & `portage-3.0.64/.builds/ci.yml`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/.builds/lint.yml` & `portage-3.0.64/.builds/lint.yml`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/.builds/setup-python.sh` & `portage-3.0.64/.builds/setup-python.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/.git-blame-ignore-revs` & `portage-3.0.64/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/.github/workflows/ci.yml` & `portage-3.0.64/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         start-method:
           - 'fork'
           - 'spawn'
         python-version:
           - '3.9'
           - '3.10'
           - '3.11'
-          - '3.12-dev'
+          - '3.12'
           - '3.13-dev'
           - 'pypy-3.10'
         exclude:
           - python-version: '3.9'
             start-method: 'spawn'
           - python-version: '3.10'
             start-method: 'spawn'
@@ -30,17 +30,17 @@
             start-method: 'spawn'
           - python-version: '3.13-dev'
             start-method: 'spawn'
           - python-version: 'pypy-3.10'
             start-method: 'spawn'
       fail-fast: false
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           set -xe
           echo "force-unsafe-io" | sudo tee /etc/dpkg/dpkg.cfg.d/force-unsafe-io
           sudo apt-get update -q
```

### Comparing `portage-3.0.63/.github/workflows/lint.yml` & `portage-3.0.64/.github/workflows/lint.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 
 on: [ push, pull_request ]
 
 jobs:
   black:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: "Collect stragglers that Black misses"
         id: stragglers
         run: |
-          echo "::set-output name=missed::$(
+          echo "missed=$(
           find bin -type f -not -name '*.py' -not -name '*.sh' | \
-          xargs grep -l '#!/usr/bin/env python' | tr $'\n' ' ')"
+          xargs grep -l '#!/usr/bin/env python' | tr $'\n' ' ')" >> $GITHUB_OUTPUT
       - uses: psf/black@24.1.1
         with:
             src: . ${{ steps.stragglers.outputs.missed }}
 
   pylint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version:
           - '3.9'
           - '3.10'
           - '3.11'
-          # pylint currently broken under 3.12
-          # - '3.12-dev'
+          - '3.12'
       fail-fast: false
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install python dependencies
         run: |
           set -xe
           python -VV
           python -m site
```

### Comparing `portage-3.0.63/COPYING` & `portage-3.0.64/COPYING`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/DEVELOPING` & `portage-3.0.64/DEVELOPING`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/LICENSE` & `portage-3.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/NEWS` & `portage-3.0.64/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,120 @@
 [Optional short blurb/summary]
 * Breaking changes
 * Security
 * Features
 * Bug fixes
 * Cleanups
 
+portage-3.0.65 (UNRELEASED)
+--------------
+
+TODO
+
+portage-3.0.64 (2024-04-28)
+--------------
+
+Features:
+* Scheduler: Support parallel-install with merge-wait (bug #256616, bug #925213).
+
+  This makes the (future) improvement mentioned in portage-3.0.62's NEWS.
+
+* phase-functions: prematurely delete WORKDIR if FEATURES=merge-wait
+
+  The 'merge-wait' feature could lead to running out of disk space on
+  PORTAGE_TMPDIR's filesystem because many more workdirs were kept around
+  until merging was queued up. We now purge the workdirs but keep the image
+  around until merging.
+
+* Start to record REPO_REVISIONS in build-info in VDB (bug #924772).
+
+  Ultimately the intention is to expose this information in binhost
+  metadata so that clients can select consistent revisions of source
+  repositories.
+
+* util: file_copy: Support btrfs's FICLONE ioctl for fast file clones.
+
+  Added when implementing the below 'src: Drop linux_reflink C module.'
+  cleanup.
+
+* sync: Add new 'zipfile' sync-type.
+
+  This allows fetching ebuild repositories via snapshots from e.g. GitHub,
+  gitweb, cgit.
+
+Bug fixes:
+* ctypes: Add workaround for loading libc on musl.
+
+* util: set a timeout for urlopen calls (bug #926221).
+
+* SpawnProcess: Fix noise / warnings caused by set_term_size (bug #923750, bug #925456).
+
+* binpkg, gpkg: Add missing newlines to error messages.
+
+* writable_check: Improve whitespace handling when parsing /proc/self/mountinfo (bug #925888).
+
+* doebuild: Call _setup_locale (bug #925863).
+
+  This is needed to more robustly handle invalid or inappropriate locale settings.
+
+* binarytree._populate_remote: Fix UnboundLocalError for binpkg-request-signature (bug #926048).
+
+* elog/mod_custom: Spawn processes in background (bug #925907).
+
+  Fixes a noisy crash on exit.
+
+* Fix REQUIRED_USE error with --fetchonly --pretend but not --fetchonly (bug #675748).
+
+* socks5: Fix exit with FEATURES="network-sandbox-proxy" or FEATURES="distcc" (bug #925240).
+
+* meson.build: Install dist-info METADATA (bug #920330).
+
+  This is needed for 'pip' to not be confused when Portage is installed system-wide.
+
+* EbuildPhase/EbuildBinpkg: Ensure PKGDIR subdirectory permissions (bug #712222).
+
+  A warning (failure) was observed with FEATURES="installsources" otherwise.
+
+* config: Sort FEATURES to avoid non-determinism (bug #914441).
+
+* man: Document autoenabled options by --getbinpkgonly.
+
+* BinpkgPrefetcher: Use eerror for binarytree inject failures (bug #927632).
+
+  This improves the readability of the error substantially.
+
+* install-qa-check.d: Remove QA warning when no bash completions are found  (bug #928599, bug #928869).
+
+  This check had too many false positives.
+
+* lib: use more pure git-describe output for --version (bug #912209).
+
+  This makes 'emerge --version' info far nicer when using portage-9999.
+
+* lib: adhere to python package version conventions (bug #926966).
+
+  (Note that this needed fixing even before the change for bug #912209).
+
+Cleanups:
+* cnf: sets: Migrate @golang-rebuild to dev-lang/go (removed from Portage) (bug #919751).
+
+* src: Drop libc C module.
+
+  This was only used for `find_library` on musl. We've now implemented
+  an alternative workaround for this.
+
+* src: Drop linux_reflink C module.
+
+  This is now implemented in pure Python, which also means PyPy can
+  benefit.
+
+  Testsuite coverage was also improved for this area.
+
+* Delete compat_coroutine module.
+
 portage-3.0.63 (2024-02-25)
 --------------
 
 Bug fixes:
 * emerge: Skip installed packages with emptytree in depgraph selection (bug #651018).
 
 * bin/install-qa-check.d: 90gcc-warnings: drop warnings with too many FPs (bug #925460).
```

### Comparing `portage-3.0.63/README.md` & `portage-3.0.64/README.md`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/RELEASE-NOTES` & `portage-3.0.64/RELEASE-NOTES`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/TEST-NOTES` & `portage-3.0.64/TEST-NOTES`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/archive-conf` & `portage-3.0.64/bin/archive-conf`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/bashrc-functions.sh` & `portage-3.0.64/bin/bashrc-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/binhost-snapshot` & `portage-3.0.64/bin/binhost-snapshot`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/chmod-lite` & `portage-3.0.64/bin/chmod-lite`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/chmod-lite.py` & `portage-3.0.64/bin/chmod-lite.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/chpathtool.py` & `portage-3.0.64/bin/chpathtool.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/clean_locks` & `portage-3.0.64/bin/clean_locks`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/dispatch-conf` & `portage-3.0.64/bin/dispatch-conf`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/dohtml.py` & `portage-3.0.64/bin/dohtml.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/doins.py` & `portage-3.0.64/bin/doins.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/eapi.sh` & `portage-3.0.64/bin/eapi.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/eapi7-ver-funcs.sh` & `portage-3.0.64/bin/eapi7-ver-funcs.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild` & `portage-3.0.64/bin/ebuild`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,18 @@
         tmpsettings["EBUILD_FORCE_TEST"] = "1"
         tmpsettings.backup_changes("EBUILD_FORCE_TEST")
         tmpsettings.features.add("test")
         portage.writemsg(_("Forcing test.\n"), noiselevel=-1)
 
     tmpsettings.features.discard("fail-clean")
 
+    # We don't implement merge-wait for the ebuild command, so discard
+    # it from FEATURES. This prevents premature WORKDIR removal.
+    tmpsettings.features.discard("merge-wait")
+
     if "merge" in pargs and "noauto" in tmpsettings.features:
         print("Disabling noauto in features... merge disables it. (qmerge doesn't)")
         tmpsettings.features.discard("noauto")
 
     if "digest" in tmpsettings.features:
         if pargs and pargs[0] not in ("digest", "manifest"):
             pargs = ["digest"] + pargs
```

### Comparing `portage-3.0.63/bin/ebuild-helpers/bsd/sed` & `portage-3.0.64/bin/ebuild-helpers/bsd/sed`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/dobin` & `portage-3.0.64/bin/ebuild-helpers/dobin`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/doconfd` & `portage-3.0.64/bin/ebuild-helpers/doconfd`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/dodoc` & `portage-3.0.64/bin/ebuild-helpers/dodoc`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/doenvd` & `portage-3.0.64/bin/ebuild-helpers/doenvd`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/doexe` & `portage-3.0.64/bin/ebuild-helpers/doexe`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/dohard` & `portage-3.0.64/bin/ebuild-helpers/dohard`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/doheader` & `portage-3.0.64/bin/ebuild-helpers/doheader`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/dohtml` & `portage-3.0.64/bin/ebuild-helpers/dohtml`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/doinfo` & `portage-3.0.64/bin/ebuild-helpers/doinfo`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/doins` & `portage-3.0.64/bin/ebuild-helpers/doins`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/dolib` & `portage-3.0.64/bin/ebuild-helpers/dolib`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/doman` & `portage-3.0.64/bin/ebuild-helpers/doman`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/domo` & `portage-3.0.64/bin/ebuild-helpers/domo`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/dosbin` & `portage-3.0.64/bin/ebuild-helpers/dosbin`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/dosed` & `portage-3.0.64/bin/ebuild-helpers/dosed`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/dosym` & `portage-3.0.64/bin/ebuild-helpers/dosym`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/emake` & `portage-3.0.64/bin/ebuild-helpers/emake`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/fowners` & `portage-3.0.64/bin/ebuild-helpers/fowners`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/fperms` & `portage-3.0.64/bin/ebuild-helpers/fperms`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newbin` & `portage-3.0.64/bin/ebuild-helpers/newbin`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newconfd` & `portage-3.0.64/bin/ebuild-helpers/newconfd`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newdoc` & `portage-3.0.64/bin/ebuild-helpers/newdoc`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newenvd` & `portage-3.0.64/bin/ebuild-helpers/newenvd`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newexe` & `portage-3.0.64/bin/ebuild-helpers/newexe`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newheader` & `portage-3.0.64/bin/ebuild-helpers/newheader`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newinitd` & `portage-3.0.64/bin/ebuild-helpers/newinitd`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newins` & `portage-3.0.64/bin/ebuild-helpers/newins`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newlib.a` & `portage-3.0.64/bin/ebuild-helpers/newlib.a`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newlib.so` & `portage-3.0.64/bin/ebuild-helpers/newlib.so`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newman` & `portage-3.0.64/bin/ebuild-helpers/newman`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/newsbin` & `portage-3.0.64/bin/ebuild-helpers/newsbin`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/unprivileged/chgrp` & `portage-3.0.64/bin/ebuild-helpers/unprivileged/chgrp`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/unprivileged/chown` & `portage-3.0.64/bin/ebuild-helpers/unprivileged/chown`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-helpers/xattr/install` & `portage-3.0.64/bin/ebuild-helpers/xattr/install`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-ipc` & `portage-3.0.64/bin/ebuild-ipc`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-ipc.py` & `portage-3.0.64/bin/ebuild-ipc.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild-pyhelper` & `portage-3.0.64/bin/ebuild-pyhelper`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ebuild.sh` & `portage-3.0.64/bin/ebuild.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ecompress` & `portage-3.0.64/bin/ecompress`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/ecompress-file` & `portage-3.0.64/bin/ecompress-file`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/egencache` & `portage-3.0.64/bin/egencache`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/emaint` & `portage-3.0.64/bin/emaint`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/emerge` & `portage-3.0.64/bin/emerge`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/emerge-webrsync` & `portage-3.0.64/bin/emerge-webrsync`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/emirrordist` & `portage-3.0.64/bin/emirrordist`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/env-update` & `portage-3.0.64/bin/env-update`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/estrip` & `portage-3.0.64/bin/estrip`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/etc-update` & `portage-3.0.64/bin/etc-update`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/filter-bash-environment.py` & `portage-3.0.64/bin/filter-bash-environment.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/fixpackages` & `portage-3.0.64/bin/fixpackages`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/glsa-check` & `portage-3.0.64/bin/glsa-check`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/gpkg-helper.py` & `portage-3.0.64/bin/gpkg-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/gpkg-sign` & `portage-3.0.64/bin/gpkg-sign`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/helper-functions.sh` & `portage-3.0.64/bin/helper-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/05prefix` & `portage-3.0.64/bin/install-qa-check.d/05prefix`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/10executable-issues` & `portage-3.0.64/bin/install-qa-check.d/10executable-issues`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/10ignored-flags` & `portage-3.0.64/bin/install-qa-check.d/10ignored-flags`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/20runtime-directories` & `portage-3.0.64/bin/install-qa-check.d/20runtime-directories`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/60bash-completion` & `portage-3.0.64/bin/install-qa-check.d/60bash-completion`

 * *Files 6% similar despite different names*

```diff
@@ -73,17 +73,14 @@
 				qa_warnings+=(
 					"${f##*/}: 'have' command is deprecated and must not be used."
 				)
 				unset 'completions[0]'
 			fi
 
 			if [[ -z ${completions[@]} ]]; then
-				qa_warnings+=(
-					"${f##*/}: does not define any completions (failed to source?)."
-				)
 				continue
 			fi
 
 			for c in "${completions[@]}"; do
 				if [[ ${c} == /* ]]; then
 					qa_warnings+=(
 						"${f##*/}: absolute paths can not be used for completions (on '${c}')."
```

### Comparing `portage-3.0.63/bin/install-qa-check.d/60openrc` & `portage-3.0.64/bin/install-qa-check.d/60openrc`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/60pkgconfig` & `portage-3.0.64/bin/install-qa-check.d/60pkgconfig`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/60pngfix` & `portage-3.0.64/bin/install-qa-check.d/60pngfix`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/60systemd` & `portage-3.0.64/bin/install-qa-check.d/60systemd`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/80libraries` & `portage-3.0.64/bin/install-qa-check.d/80libraries`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/80multilib-strict` & `portage-3.0.64/bin/install-qa-check.d/80multilib-strict`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/90bad-bin-group-write` & `portage-3.0.64/bin/install-qa-check.d/90bad-bin-group-write`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/90bad-bin-owner` & `portage-3.0.64/bin/install-qa-check.d/90bad-bin-owner`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/90cmake-warnings` & `portage-3.0.64/bin/install-qa-check.d/90cmake-warnings`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/90config-impl-decl` & `portage-3.0.64/bin/install-qa-check.d/90config-impl-decl`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/90cython-dep` & `portage-3.0.64/bin/install-qa-check.d/90cython-dep`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/90gcc-warnings` & `portage-3.0.64/bin/install-qa-check.d/90gcc-warnings`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/90world-writable` & `portage-3.0.64/bin/install-qa-check.d/90world-writable`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install-qa-check.d/95empty-dirs` & `portage-3.0.64/bin/install-qa-check.d/95empty-dirs`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/install.py` & `portage-3.0.64/bin/install.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/isolated-functions.sh` & `portage-3.0.64/bin/isolated-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/lock-helper.py` & `portage-3.0.64/bin/lock-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/meson.build` & `portage-3.0.64/bin/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/misc-functions.sh` & `portage-3.0.64/bin/misc-functions.sh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2023 Gentoo Authors
+# Copyright 1999-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 #
 # Miscellaneous shell functions that make use of the ebuild env but don't need
 # to be included directly in ebuild.sh.
 #
 # We're sourcing ebuild.sh here so that we inherit all of it's goodness,
 # including bashrc trickery.  This approach allows us to do our miscellaneous
@@ -251,14 +251,21 @@
 			"${PORTAGE_BIN_PATH}"/estrip --queue "${PORTAGE_DOSTRIP[@]}"
 			"${PORTAGE_BIN_PATH}"/estrip --ignore "${PORTAGE_DOSTRIP_SKIP[@]}"
 			"${PORTAGE_BIN_PATH}"/estrip --dequeue
 		else
 			"${PORTAGE_BIN_PATH}"/estrip --prepallstrip
 		fi
 	fi
+
+	# Prematurely delete WORKDIR in case merge-wait is enabled to
+	# decrease the space used by portage build directories until the
+	# packages are merged and cleaned.
+	if has merge-wait ${FEATURES} && ! has keepwork ${FEATURES}; then
+		rm -rf "${WORKDIR}"
+	fi
 }
 
 __dyn_instprep() {
 	if [[ -e ${PORTAGE_BUILDDIR}/.instprepped ]] ; then
 		__vecho ">>> It appears that '${PF}' is already instprepped; skipping."
 		__vecho ">>> Remove '${PORTAGE_BUILDDIR}/.instprepped' to force instprep."
 		return 0
@@ -507,15 +514,19 @@
 	cd "${T}" || die
 
 	# Sandbox is disabled in case the user wants to use a symlink
 	# for ${PKGDIR} and/or ${PKGDIR}/All.
 	export SANDBOX_ON="0"
 	[[ -z "${PORTAGE_BINPKG_TMPFILE}" ]] && \
 		die "PORTAGE_BINPKG_TMPFILE is unset"
-	mkdir -p "${PORTAGE_BINPKG_TMPFILE%/*}" || die "mkdir failed"
+	if [[ ! -d ${PORTAGE_BINPKG_TMPFILE%/*} ]]; then
+		# Warn because we don't set PKGDIR directory permissions here.
+		ewarn "__dyn_package: Creating PORTAGE_BINPKG_TMPFILE parent dir: ${PORTAGE_BINPKG_TMPFILE%/*}"
+		mkdir -p "${PORTAGE_BINPKG_TMPFILE%/*}" || die "mkdir failed"
+	fi
 
 	if [[ ! -z "${BUILD_ID}" ]]; then
 		echo -n "${BUILD_ID}" > "${PORTAGE_BUILDDIR}"/build-info/BUILD_ID
 	fi
 
 	if [[ "${BINPKG_FORMAT}" == "xpak" ]]; then
 		local tar_options=""
```

### Comparing `portage-3.0.63/bin/phase-functions.sh` & `portage-3.0.64/bin/phase-functions.sh`

 * *Files 2% similar despite different names*

```diff
@@ -715,14 +715,15 @@
 	assert "__save_ebuild_env failed"
 	cd "${PORTAGE_BUILDDIR}"/build-info || die
 
 	${PORTAGE_BZIP2_COMMAND} -f9 environment
 
 	cp "${EBUILD}" "${PF}.ebuild"
 	[[ -n "${PORTAGE_REPO_NAME}" ]]  && echo "${PORTAGE_REPO_NAME}" > repository
+	[[ -n ${PORTAGE_REPO_REVISIONS} ]] && echo "${PORTAGE_REPO_REVISIONS}" > REPO_REVISIONS
 	if has nostrip ${FEATURES} ${PORTAGE_RESTRICT} || has strip ${PORTAGE_RESTRICT}; then
 		>> DEBUGBUILD
 	fi
 	trap - SIGINT SIGQUIT
 }
 
 __dyn_help() {
```

### Comparing `portage-3.0.63/bin/phase-helpers.sh` & `portage-3.0.64/bin/phase-helpers.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/pid-ns-init` & `portage-3.0.64/bin/pid-ns-init`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/portageq` & `portage-3.0.64/bin/portageq`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/portageq-wrapper` & `portage-3.0.64/bin/portageq-wrapper`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/postinst-qa-check.d/50xdg-utils` & `portage-3.0.64/bin/postinst-qa-check.d/50xdg-utils`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/preinst-qa-check.d/50xdg-utils` & `portage-3.0.64/bin/preinst-qa-check.d/50xdg-utils`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/quickpkg` & `portage-3.0.64/bin/quickpkg`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/regenworld` & `portage-3.0.64/bin/regenworld`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/save-ebuild-env.sh` & `portage-3.0.64/bin/save-ebuild-env.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/shelve-utils` & `portage-3.0.64/bin/shelve-utils`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/socks5-server.py` & `portage-3.0.64/bin/socks5-server.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/xattr-helper.py` & `portage-3.0.64/bin/xattr-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/bin/xpak-helper.py` & `portage-3.0.64/bin/xpak-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/dispatch-conf.conf` & `portage-3.0.64/cnf/dispatch-conf.conf`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/etc-update.conf` & `portage-3.0.64/cnf/etc-update.conf`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example` & `portage-3.0.64/cnf/make.conf.example`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.alpha.diff` & `portage-3.0.64/cnf/make.conf.example.alpha.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.amd64-fbsd.diff` & `portage-3.0.64/cnf/make.conf.example.amd64-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.amd64.diff` & `portage-3.0.64/cnf/make.conf.example.amd64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.arc.diff` & `portage-3.0.64/cnf/make.conf.example.arc.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.arm.diff` & `portage-3.0.64/cnf/make.conf.example.arm.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.arm64.diff` & `portage-3.0.64/cnf/make.conf.example.arm64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.hppa.diff` & `portage-3.0.64/cnf/make.conf.example.hppa.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.ia64.diff` & `portage-3.0.64/cnf/make.conf.example.ia64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.loong.diff` & `portage-3.0.64/cnf/make.conf.example.loong.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.m68k.diff` & `portage-3.0.64/cnf/make.conf.example.m68k.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.mips.diff` & `portage-3.0.64/cnf/make.conf.example.mips.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.ppc.diff` & `portage-3.0.64/cnf/make.conf.example.ppc.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.ppc64.diff` & `portage-3.0.64/cnf/make.conf.example.ppc64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.riscv.diff` & `portage-3.0.64/cnf/make.conf.example.riscv.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.s390.diff` & `portage-3.0.64/cnf/make.conf.example.s390.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.sh.diff` & `portage-3.0.64/cnf/make.conf.example.sh.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.sparc-fbsd.diff` & `portage-3.0.64/cnf/make.conf.example.sparc-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.sparc.diff` & `portage-3.0.64/cnf/make.conf.example.sparc.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.x86-fbsd.diff` & `portage-3.0.64/cnf/make.conf.example.x86-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.conf.example.x86.diff` & `portage-3.0.64/cnf/make.conf.example.x86.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/make.globals` & `portage-3.0.64/cnf/make.globals`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/meson.build` & `portage-3.0.64/cnf/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/repo.postsync.d/example` & `portage-3.0.64/cnf/repo.postsync.d/example`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/repos.conf` & `portage-3.0.64/cnf/repos.conf`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/cnf/sets/portage.conf` & `portage-3.0.64/cnf/sets/portage.conf`

 * *Files 4% similar despite different names*

```diff
@@ -106,18 +106,12 @@
 class = portage.sets.dbapi.UnavailableBinaries
 
 # Installed packages for which vdb *DEPEND entries are outdated compared
 # to the matching portdb entry.
 [changed-deps]
 class = portage.sets.dbapi.ChangedDepsSet
 
-# Installed packages for which vdb *DEPEND includes dev-lang/go.
-[golang-rebuild]
-class = portage.sets.dbapi.VariableSet
-variable = BDEPEND
-includes = dev-lang/go
-
 # Installed packages for which vdb *DEPEND includes virtual/rust
 [rust-rebuild]
 class = portage.sets.dbapi.VariableSet
 variable = BDEPEND
 includes = virtual/rust
```

### Comparing `portage-3.0.63/doc/api/Makefile` & `portage-3.0.64/doc/api/Makefile`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/api/conf.py` & `portage-3.0.64/doc/api/conf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/api/meson.build` & `portage-3.0.64/doc/api/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/config/bashrc.docbook` & `portage-3.0.64/doc/config/bashrc.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/config/sets.docbook` & `portage-3.0.64/doc/config/sets.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/dependency_resolution/decision_making.docbook` & `portage-3.0.64/doc/dependency_resolution/decision_making.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/dependency_resolution/package_modeling.docbook` & `portage-3.0.64/doc/dependency_resolution/package_modeling.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/dependency_resolution/task_scheduling.docbook` & `portage-3.0.64/doc/dependency_resolution/task_scheduling.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/meson.build` & `portage-3.0.64/doc/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/package/ebuild/eapi/1.docbook` & `portage-3.0.64/doc/package/ebuild/eapi/1.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/package/ebuild/eapi/2.docbook` & `portage-3.0.64/doc/package/ebuild/eapi/2.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/package/ebuild/eapi/3.docbook` & `portage-3.0.64/doc/package/ebuild/eapi/3.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/package/ebuild/eapi/4-slot-abi.docbook` & `portage-3.0.64/doc/package/ebuild/eapi/4-slot-abi.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/package/ebuild/eapi/4.docbook` & `portage-3.0.64/doc/package/ebuild/eapi/4.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/package/ebuild/eapi/5.docbook` & `portage-3.0.64/doc/package/ebuild/eapi/5.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/package/ebuild/helper_functions.docbook` & `portage-3.0.64/doc/package/ebuild/helper_functions.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/package/ebuild/phases.docbook` & `portage-3.0.64/doc/package/ebuild/phases.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/portage.docbook` & `portage-3.0.64/doc/portage.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/doc/qa.docbook` & `portage-3.0.64/doc/qa.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/AbstractDepPriority.py` & `portage-3.0.64/lib/_emerge/AbstractDepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/AbstractEbuildProcess.py` & `portage-3.0.64/lib/_emerge/AbstractEbuildProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/AbstractPollTask.py` & `portage-3.0.64/lib/_emerge/AbstractPollTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/AsynchronousLock.py` & `portage-3.0.64/lib/_emerge/AsynchronousLock.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/AsynchronousTask.py` & `portage-3.0.64/lib/_emerge/AsynchronousTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/Binpkg.py` & `portage-3.0.64/lib/_emerge/Binpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/BinpkgEnvExtractor.py` & `portage-3.0.64/lib/_emerge/BinpkgEnvExtractor.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/BinpkgExtractorAsync.py` & `portage-3.0.64/lib/_emerge/BinpkgExtractorAsync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/BinpkgFetcher.py` & `portage-3.0.64/lib/_emerge/BinpkgFetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 1999-2023 Gentoo Authors
+# Copyright 1999-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 from _emerge.AsynchronousLock import AsynchronousLock
 from _emerge.CompositeTask import CompositeTask
 from _emerge.SpawnProcess import SpawnProcess
 from urllib.parse import urlparse as urllib_parse_urlparse
 import stat
@@ -229,15 +229,17 @@
         if self.background or not sys.__stdout__.isatty():
             # When the output only goes to a log file,
             # there's no point in creating a pty.
             return os.pipe()
         stdout_pipe = None
         if not self.background:
             stdout_pipe = fd_pipes.get(1)
-        got_pty, master_fd, slave_fd = _create_pty_or_pipe(copy_term_size=stdout_pipe)
+        self._pty_ready, master_fd, slave_fd = _create_pty_or_pipe(
+            copy_term_size=stdout_pipe
+        )
         return (master_fd, slave_fd)
 
     def sync_timestamp(self):
         # If possible, update the mtime to match the remote package if
         # the fetcher didn't already do it automatically.
         bintree = self.pkg.root_config.trees["bintree"]
         if bintree._remote_has_index:
```

### Comparing `portage-3.0.63/lib/_emerge/BinpkgVerifier.py` & `portage-3.0.64/lib/_emerge/BinpkgVerifier.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/BlockerCache.py` & `portage-3.0.64/lib/_emerge/BlockerCache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/BlockerDB.py` & `portage-3.0.64/lib/_emerge/BlockerDB.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/CompositeTask.py` & `portage-3.0.64/lib/_emerge/CompositeTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/DepPriority.py` & `portage-3.0.64/lib/_emerge/DepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/DepPriorityNormalRange.py` & `portage-3.0.64/lib/_emerge/DepPriorityNormalRange.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/DepPrioritySatisfiedRange.py` & `portage-3.0.64/lib/_emerge/DepPrioritySatisfiedRange.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/Dependency.py` & `portage-3.0.64/lib/_emerge/Dependency.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/DependencyArg.py` & `portage-3.0.64/lib/_emerge/DependencyArg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildBinpkg.py` & `portage-3.0.64/lib/_emerge/EbuildBinpkg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 1999-2023 Gentoo Authors
+# Copyright 1999-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import io
 import sys
 
 from _emerge.CompositeTask import CompositeTask
 from _emerge.EbuildPhase import EbuildPhase
@@ -25,14 +25,15 @@
     def _start(self):
         pkg = self.pkg
         root_config = pkg.root_config
         bintree = root_config.trees["bintree"]
         pkg_allocated_path, build_id = bintree.getname_build_id(
             pkg.cpv, allocate_new=True
         )
+        bintree._ensure_dir(os.path.dirname(pkg_allocated_path))
 
         self.pkg_allocated_path = pkg_allocated_path
         self._binpkg_tmpfile = self.pkg_allocated_path + "." + str(portage.getpid())
         self.settings["PORTAGE_BINPKG_TMPFILE"] = self._binpkg_tmpfile
 
         if "binpkg-multi-instance" in self.settings.features:
             self.settings["BUILD_ID"] = str(build_id)
```

### Comparing `portage-3.0.63/lib/_emerge/EbuildBuild.py` & `portage-3.0.64/lib/_emerge/EbuildBuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildBuildDir.py` & `portage-3.0.64/lib/_emerge/EbuildBuildDir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildExecuter.py` & `portage-3.0.64/lib/_emerge/EbuildExecuter.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildFetcher.py` & `portage-3.0.64/lib/_emerge/EbuildFetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 1999-2023 Gentoo Authors
+# Copyright 1999-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import copy
 import functools
 import io
 import sys
 
@@ -390,15 +390,17 @@
         if self.background or not sys.stdout.isatty():
             # When the output only goes to a log file,
             # there's no point in creating a pty.
             return os.pipe()
         stdout_pipe = None
         if not self.background:
             stdout_pipe = fd_pipes.get(1)
-        got_pty, master_fd, slave_fd = _create_pty_or_pipe(copy_term_size=stdout_pipe)
+        self._pty_ready, master_fd, slave_fd = _create_pty_or_pipe(
+            copy_term_size=stdout_pipe
+        )
         return (master_fd, slave_fd)
 
     def _eerror(self, lines):
         out = io.StringIO()
         for line in lines:
             eerror(line, phase="unpack", key=self.pkg.cpv, out=out)
         msg = out.getvalue()
```

### Comparing `portage-3.0.63/lib/_emerge/EbuildFetchonly.py` & `portage-3.0.64/lib/_emerge/EbuildFetchonly.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildIpcDaemon.py` & `portage-3.0.64/lib/_emerge/EbuildIpcDaemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildMerge.py` & `portage-3.0.64/lib/_emerge/EbuildMerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildMetadataPhase.py` & `portage-3.0.64/lib/_emerge/EbuildMetadataPhase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildPhase.py` & `portage-3.0.64/lib/_emerge/EbuildPhase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 1999-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import functools
 import gzip
 import io
+import json
 import sys
 import tempfile
 
 from _emerge.AsynchronousLock import AsynchronousLock
 from _emerge.BinpkgEnvExtractor import BinpkgEnvExtractor
 from _emerge.MiscFunctionsProcess import MiscFunctionsProcess
 from _emerge.EbuildProcess import EbuildProcess
@@ -79,14 +80,51 @@
                     #     % self.settings["LC_CTYPE"]
                     # )
                     break
             else:
                 raise AssertionError("C locale did not pass the test!")
 
 
+async def _setup_repo_revisions(settings):
+    repo_name = settings.configdict["pkg"].get("PORTAGE_REPO_NAME")
+    db = getattr(settings.mycpv, "_db", None)
+    if (
+        isinstance(db, portage.portdbapi)
+        and repo_name
+        and "PORTAGE_REPO_REVISIONS" not in settings.configdict["pkg"]
+    ):
+        repo = db.repositories[repo_name]
+        ec_dict = repo.eclass_db.get_eclass_data(
+            settings.configdict["pkg"]["INHERITED"].split()
+        )
+        referenced_repos = {repo.name: repo}
+        for ec_info in ec_dict.values():
+            ec_repo = db.repositories.get_repo_for_location(
+                os.path.dirname(os.path.dirname(ec_info.location))
+            )
+            referenced_repos.setdefault(ec_repo.name, ec_repo)
+        repo_revisions = {}
+        for repo_ref in referenced_repos.values():
+            if repo_ref.sync_type:
+                sync = portage.sync.module_controller.get_class(repo_ref.sync_type)()
+                try:
+                    # TODO: Wait for subprocesses asynchronously here.
+                    status, repo_revision = sync.retrieve_head(
+                        options={"repo": repo_ref}
+                    )
+                except NotImplementedError:
+                    pass
+                else:
+                    if status == os.EX_OK:
+                        repo_revisions[repo_ref.name] = repo_revision.strip()
+        settings.configdict["pkg"]["PORTAGE_REPO_REVISIONS"] = json.dumps(
+            repo_revisions, ensure_ascii=False, sort_keys=True
+        )
+
+
 class EbuildPhase(CompositeTask):
     __slots__ = ("actionmap", "fd_pipes", "phase", "settings") + ("_ebuild_lock",)
 
     # FEATURES displayed prior to setup phase
     _features_display = (
         "ccache",
         "compressdebug",
@@ -116,14 +154,15 @@
     def _start(self):
         future = asyncio.ensure_future(self._async_start(), loop=self.scheduler)
         self._start_task(AsyncTaskFuture(future=future), self._async_start_exit)
 
     async def _async_start(self):
 
         await _setup_locale(self.settings)
+        await _setup_repo_revisions(self.settings)
 
         need_builddir = self.phase not in EbuildProcess._phases_without_builddir
 
         if need_builddir:
             phase_completed_file = os.path.join(
                 self.settings["PORTAGE_BUILDDIR"], f".{self.phase.rstrip('e')}ed"
             )
@@ -204,14 +243,17 @@
                             self.settings["CATEGORY"],
                             self.settings["PF"],
                         )
                         + ".gpkg.tar"
                     )
                 else:
                     raise InvalidBinaryPackageFormat(binpkg_format)
+                self.settings.mycpv._db.bintree._ensure_dir(
+                    os.path.dirname(self.settings["PORTAGE_BINPKG_TMPFILE"])
+                )
 
     def _async_start_exit(self, task):
         task.future.cancelled() or task.future.result()
         if self._default_exit(task) != os.EX_OK:
             self.wait()
             return
```

### Comparing `portage-3.0.63/lib/_emerge/EbuildProcess.py` & `portage-3.0.64/lib/_emerge/EbuildProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/EbuildSpawnProcess.py` & `portage-3.0.64/lib/_emerge/EbuildSpawnProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/FakeVartree.py` & `portage-3.0.64/lib/_emerge/FakeVartree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/FifoIpcDaemon.py` & `portage-3.0.64/lib/_emerge/FifoIpcDaemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/JobStatusDisplay.py` & `portage-3.0.64/lib/_emerge/JobStatusDisplay.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/MergeListItem.py` & `portage-3.0.64/lib/_emerge/MergeListItem.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/MetadataRegen.py` & `portage-3.0.64/lib/_emerge/MetadataRegen.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/MiscFunctionsProcess.py` & `portage-3.0.64/lib/_emerge/MiscFunctionsProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/Package.py` & `portage-3.0.64/lib/_emerge/Package.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/PackageArg.py` & `portage-3.0.64/lib/_emerge/PackageArg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/PackageMerge.py` & `portage-3.0.64/lib/_emerge/PackageMerge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright 1999-2014 Gentoo Foundation
+# Copyright 1999-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 from _emerge.CompositeTask import CompositeTask
 from portage.dep import _repo_separator
 from portage.output import colorize
 
 
 class PackageMerge(CompositeTask):
-    __slots__ = ("merge", "postinst_failure")
+    __slots__ = ("is_system_pkg", "merge", "postinst_failure")
 
     def _should_show_status(self):
         return (
             not self.merge.build_opts.fetchonly
             and not self.merge.build_opts.pretend
             and not self.merge.build_opts.buildpkgonly
         )
```

### Comparing `portage-3.0.63/lib/_emerge/PackagePhase.py` & `portage-3.0.64/lib/_emerge/PackagePhase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/PackageUninstall.py` & `portage-3.0.64/lib/_emerge/PackageUninstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/PackageVirtualDbapi.py` & `portage-3.0.64/lib/_emerge/PackageVirtualDbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/PipeReader.py` & `portage-3.0.64/lib/_emerge/PipeReader.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/PollScheduler.py` & `portage-3.0.64/lib/_emerge/PollScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/ProgressHandler.py` & `portage-3.0.64/lib/_emerge/ProgressHandler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/RootConfig.py` & `portage-3.0.64/lib/_emerge/RootConfig.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/Scheduler.py` & `portage-3.0.64/lib/_emerge/Scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1515,25 +1515,28 @@
         if build.returncode == os.EX_OK and self._terminated_tasks:
             # We've been interrupted, so we won't
             # add this to the merge queue.
             self.curval += 1
             self._deallocate_config(build.settings)
         elif build.returncode == os.EX_OK:
             self.curval += 1
-            merge = PackageMerge(merge=build, scheduler=self._sched_iface)
+            merge = PackageMerge(
+                is_system_pkg=(build.pkg in self._deep_system_deps),
+                merge=build,
+                scheduler=self._sched_iface,
+            )
             self._running_tasks[id(merge)] = merge
             # By default, merge-wait only allows merge when no builds are executing.
             # As a special exception, dependencies on system packages are frequently
             # unspecified and will therefore force merge-wait.
-            is_system_pkg = build.pkg in self._deep_system_deps
             if not build.build_opts.buildpkgonly and (
-                "merge-wait" in build.settings.features or is_system_pkg
+                "merge-wait" in build.settings.features or merge.is_system_pkg
             ):
                 self._merge_wait_queue.append(merge)
-                if is_system_pkg:
+                if merge.is_system_pkg:
                     merge.addStartListener(self._system_merge_started)
             else:
                 self._task_queues.merge.add(merge)
                 merge.addExitListener(self._merge_exit)
                 self._status_display.merges = len(self._task_queues.merge)
         else:
             settings = build.settings
@@ -1800,21 +1803,40 @@
             # parallel-install does not cause more than one of
             # them to install at the same time.
             if (
                 self._merge_wait_queue
                 and not self._jobs
                 and not self._task_queues.merge
             ):
-                task = self._merge_wait_queue.popleft()
-                task.scheduler = self._sched_iface
-                self._merge_wait_scheduled.append(task)
-                self._task_queues.merge.add(task)
-                task.addExitListener(self._merge_wait_exit_handler)
-                self._status_display.merges = len(self._task_queues.merge)
-                state_change += 1
+                while self._merge_wait_queue:
+                    # If we added non-system packages to the merge queue in a
+                    # previous iteration of this loop, then for system packages we
+                    # need to come back later when the merge queue is empty.
+                    # TODO: Maybe promote non-system packages to the front of the
+                    # queue and process them within the current loop, though that
+                    # causes merge order to differ from the order builds finish.
+                    if (
+                        self._task_queues.merge
+                        and self._merge_wait_queue[0].is_system_pkg
+                    ):
+                        break
+                    task = self._merge_wait_queue.popleft()
+                    task.scheduler = self._sched_iface
+                    self._merge_wait_scheduled.append(task)
+                    self._task_queues.merge.add(task)
+                    task.addExitListener(self._merge_wait_exit_handler)
+                    self._status_display.merges = len(self._task_queues.merge)
+                    state_change += 1
+                    # For system packages, always serialize install regardless of
+                    # parallel-install, in order to mitigate failures triggered
+                    # by fragile states as in bug 256616. For other packages,
+                    # continue to populate self._task_queues.merge, which will
+                    # serialize install unless parallel-install is enabled.
+                    if task.is_system_pkg:
+                        break
 
             if self._schedule_tasks_imp():
                 state_change += 1
 
             self._status_display.display()
 
             # Cancel prefetchers if they're the only reason
```

### Comparing `portage-3.0.63/lib/_emerge/SequentialTaskQueue.py` & `portage-3.0.64/lib/_emerge/SequentialTaskQueue.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/SpawnProcess.py` & `portage-3.0.64/lib/_emerge/SpawnProcess.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
     __slots__ = (
         ("args", "create_pipe", "log_filter_file")
         + _spawn_kwarg_names
         + (
             "_main_task",
             "_main_task_cancel",
+            "_pty_ready",
             "_selinux_type",
         )
     )
 
     # Max number of attempts to kill the processes listed in cgroup.procs,
     # given that processes may fork before they can be killed.
     _CGROUP_CLEANUP_RETRY_MAX = 8
@@ -74,18 +75,15 @@
                     raise NotImplementedError(
                         "logfile conflicts with create_pipe=False"
                     )
                 # When called via process.spawn and ForkProcess._start,
                 # SpawnProcess will have created a pipe earlier, so it
                 # would be redundant to do it here (it could also trigger
                 # spawn recursion via set_term_size as in bug 923750).
-                # Use /dev/null for master_fd, triggering early return
-                # of _main, followed by _async_waitpid.
-                # TODO: Optimize away the need for master_fd here.
-                master_fd = os.open(os.devnull, os.O_RDONLY)
+                master_fd = None
                 slave_fd = None
                 can_log = False
 
             null_input = None
             if not self.background or 0 in fd_pipes:
                 # Subclasses such as AbstractEbuildProcess may have already passed
                 # in a null file descriptor in fd_pipes, so use that when given.
@@ -161,55 +159,62 @@
 
         self._start_main_task(
             master_fd, log_file_path=log_file_path, stdout_fd=stdout_fd
         )
         self._registered = True
 
     def _start_main_task(self, pr, log_file_path=None, stdout_fd=None):
-        build_logger = BuildLogger(
-            env=self.env,
-            log_path=log_file_path,
-            log_filter_file=self.log_filter_file,
-            scheduler=self.scheduler,
-        )
-        build_logger.start()
-
-        pipe_logger = PipeLogger(
-            background=self.background,
-            scheduler=self.scheduler,
-            input_fd=pr,
-            log_file_path=build_logger.stdin,
-            stdout_fd=stdout_fd,
-        )
+        if pr is None:
+            build_logger = None
+            pipe_logger = None
+        else:
+            build_logger = BuildLogger(
+                env=self.env,
+                log_path=log_file_path,
+                log_filter_file=self.log_filter_file,
+                scheduler=self.scheduler,
+            )
+            build_logger.start()
+
+            pipe_logger = PipeLogger(
+                background=self.background,
+                scheduler=self.scheduler,
+                input_fd=pr,
+                log_file_path=build_logger.stdin,
+                stdout_fd=stdout_fd,
+            )
 
-        pipe_logger.start()
+            pipe_logger.start()
 
         self._main_task_cancel = functools.partial(
             self._main_cancel, build_logger, pipe_logger
         )
         self._main_task = asyncio.ensure_future(
             self._main(build_logger, pipe_logger, loop=self.scheduler),
             loop=self.scheduler,
         )
         self._main_task.add_done_callback(self._main_exit)
 
     async def _main(self, build_logger, pipe_logger, loop=None):
+        if isinstance(self._pty_ready, asyncio.Future):
+            await self._pty_ready
+            self._pty_ready = None
         try:
-            if pipe_logger.poll() is None:
+            if pipe_logger is not None and pipe_logger.poll() is None:
                 await pipe_logger.async_wait()
-            if build_logger.poll() is None:
+            if build_logger is not None and build_logger.poll() is None:
                 await build_logger.async_wait()
         except asyncio.CancelledError:
             self._main_cancel(build_logger, pipe_logger)
             raise
 
     def _main_cancel(self, build_logger, pipe_logger):
-        if pipe_logger.poll() is None:
+        if pipe_logger is not None and pipe_logger.poll() is None:
             pipe_logger.cancel()
-        if build_logger.poll() is None:
+        if build_logger is not None and build_logger.poll() is None:
             build_logger.cancel()
 
     def _main_exit(self, main_task):
         self._main_task = None
         self._main_task_cancel = None
         try:
             main_task.result()
@@ -234,15 +239,17 @@
         """
         @type fd_pipes: dict
         @param fd_pipes: pipes from which to copy terminal size if desired.
         """
         stdout_pipe = None
         if not self.background:
             stdout_pipe = fd_pipes.get(1)
-        got_pty, master_fd, slave_fd = _create_pty_or_pipe(copy_term_size=stdout_pipe)
+        self._pty_ready, master_fd, slave_fd = _create_pty_or_pipe(
+            copy_term_size=stdout_pipe
+        )
         return (master_fd, slave_fd)
 
     def _spawn(
         self, args: list[str], **kwargs
     ) -> portage.process.MultiprocessingProcess:
         spawn_func = portage.process.spawn
 
@@ -254,14 +261,20 @@
 
         return spawn_func(args, **kwargs)
 
     def _unregister(self):
         SubProcess._unregister(self)
         if self._main_task is not None:
             self._main_task.done() or self._main_task.cancel()
+        if isinstance(self._pty_ready, asyncio.Future):
+            (
+                self._pty_ready.done()
+                and (self._pty_ready.cancelled() or self._pty_ready.result() or True)
+            ) or self._pty_ready.cancel()
+            self._pty_ready = None
 
     def _cancel(self):
         if self._main_task is not None:
             if not self._main_task.done():
                 if self._main_task_cancel is not None:
                     self._main_task_cancel()
                     self._main_task_cancel = None
```

### Comparing `portage-3.0.63/lib/_emerge/SubProcess.py` & `portage-3.0.64/lib/_emerge/SubProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/Task.py` & `portage-3.0.64/lib/_emerge/Task.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/TaskSequence.py` & `portage-3.0.64/lib/_emerge/TaskSequence.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/UnmergeDepPriority.py` & `portage-3.0.64/lib/_emerge/UnmergeDepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/UseFlagDisplay.py` & `portage-3.0.64/lib/_emerge/UseFlagDisplay.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/UserQuery.py` & `portage-3.0.64/lib/_emerge/UserQuery.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/_find_deep_system_runtime_deps.py` & `portage-3.0.64/lib/_emerge/_find_deep_system_runtime_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/actions.py` & `portage-3.0.64/lib/_emerge/actions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/chk_updated_cfg_files.py` & `portage-3.0.64/lib/_emerge/chk_updated_cfg_files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/countdown.py` & `portage-3.0.64/lib/_emerge/countdown.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/create_depgraph_params.py` & `portage-3.0.64/lib/_emerge/create_depgraph_params.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/create_world_atom.py` & `portage-3.0.64/lib/_emerge/create_world_atom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/depgraph.py` & `portage-3.0.64/lib/_emerge/depgraph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/emergelog.py` & `portage-3.0.64/lib/_emerge/emergelog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/getloadavg.py` & `portage-3.0.64/lib/_emerge/getloadavg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/help.py` & `portage-3.0.64/lib/_emerge/help.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/is_valid_package_atom.py` & `portage-3.0.64/lib/_emerge/is_valid_package_atom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/main.py` & `portage-3.0.64/lib/_emerge/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/meson.build` & `portage-3.0.64/lib/_emerge/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/post_emerge.py` & `portage-3.0.64/lib/_emerge/post_emerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/resolver/DbapiProvidesIndex.py` & `portage-3.0.64/lib/_emerge/resolver/DbapiProvidesIndex.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/resolver/backtracking.py` & `portage-3.0.64/lib/_emerge/resolver/backtracking.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/resolver/circular_dependency.py` & `portage-3.0.64/lib/_emerge/resolver/circular_dependency.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/resolver/output.py` & `portage-3.0.64/lib/_emerge/resolver/output.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/resolver/output_helpers.py` & `portage-3.0.64/lib/_emerge/resolver/output_helpers.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/resolver/package_tracker.py` & `portage-3.0.64/lib/_emerge/resolver/package_tracker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/resolver/slot_collision.py` & `portage-3.0.64/lib/_emerge/resolver/slot_collision.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/search.py` & `portage-3.0.64/lib/_emerge/search.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/show_invalid_depstring_notice.py` & `portage-3.0.64/lib/_emerge/show_invalid_depstring_notice.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/stdout_spinner.py` & `portage-3.0.64/lib/_emerge/stdout_spinner.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/_emerge/unmerge.py` & `portage-3.0.64/lib/_emerge/unmerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/__init__.py` & `portage-3.0.64/lib/portage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -716,56 +716,29 @@
                 return VERSION
             if os.path.isdir(os.path.join(PORTAGE_BASE_PATH, ".git")):
                 encoding = _encodings["fs"]
                 cmd = [
                     BASH_BINARY,
                     "-c",
                     (
-                        f"cd {_shell_quote(PORTAGE_BASE_PATH)} ; git describe --match 'portage-*' || exit $? ; "
-                        'if [ -n "`git diff-index --name-only --diff-filter=M HEAD`" ] ; '
-                        "then echo modified ; git rev-list --format=%%ct -n 1 HEAD ; fi ; "
-                        "exit 0"
+                        f"cd {_shell_quote(PORTAGE_BASE_PATH)} ; git describe --dirty --match 'portage-*' || exit $? ; "
                     ),
                 ]
                 cmd = [
                     _unicode_encode(x, encoding=encoding, errors="strict") for x in cmd
                 ]
                 proc = subprocess.Popen(
                     cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
                 )
                 output = _unicode_decode(proc.communicate()[0], encoding=encoding)
                 status = proc.wait()
                 if os.WIFEXITED(status) and os.WEXITSTATUS(status) == os.EX_OK:
-                    output_lines = output.splitlines()
-                    if output_lines:
-                        version_split = output_lines[0].split("-")
-                        if len(version_split) > 1:
-                            VERSION = version_split[1]
-                            patchlevel = False
-                            if len(version_split) > 2:
-                                patchlevel = True
-                                VERSION = f"{VERSION}_p{version_split[2]}"
-                            if len(output_lines) > 1 and output_lines[1] == "modified":
-                                head_timestamp = None
-                                if len(output_lines) > 3:
-                                    try:
-                                        head_timestamp = int(output_lines[3])
-                                    except ValueError:
-                                        pass
-                                timestamp = int(time.time())
-                                if (
-                                    head_timestamp is not None
-                                    and timestamp > head_timestamp
-                                ):
-                                    timestamp = timestamp - head_timestamp
-                                if not patchlevel:
-                                    VERSION = f"{VERSION}_p0"
-                                VERSION = f"{VERSION}_p{timestamp}"
-                            return VERSION
-            VERSION = "HEAD"
+                    VERSION = output.lstrip("portage-").strip().replace("-g", "+g")
+            else:
+                VERSION = "HEAD"
             return VERSION
 
     VERSION = _LazyVersion()
 
 else:
     VERSION = "@VERSION@"
```

### Comparing `portage-3.0.63/lib/portage/_compat_upgrade/binpkg_compression.py` & `portage-3.0.64/lib/portage/_compat_upgrade/binpkg_compression.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_compat_upgrade/binpkg_format.py` & `portage-3.0.64/lib/portage/_compat_upgrade/binpkg_format.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_compat_upgrade/binpkg_multi_instance.py` & `portage-3.0.64/lib/portage/_compat_upgrade/binpkg_multi_instance.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_compat_upgrade/default_locations.py` & `portage-3.0.64/lib/portage/_compat_upgrade/default_locations.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_emirrordist/Config.py` & `portage-3.0.64/lib/portage/_emirrordist/Config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_emirrordist/ContentDB.py` & `portage-3.0.64/lib/portage/_emirrordist/ContentDB.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_emirrordist/DeletionIterator.py` & `portage-3.0.64/lib/portage/_emirrordist/DeletionIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_emirrordist/DeletionTask.py` & `portage-3.0.64/lib/portage/_emirrordist/DeletionTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_emirrordist/FetchIterator.py` & `portage-3.0.64/lib/portage/_emirrordist/FetchIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_emirrordist/FetchTask.py` & `portage-3.0.64/lib/portage/_emirrordist/FetchTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_emirrordist/MirrorDistTask.py` & `portage-3.0.64/lib/portage/_emirrordist/MirrorDistTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_emirrordist/main.py` & `portage-3.0.64/lib/portage/_emirrordist/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_global_updates.py` & `portage-3.0.64/lib/portage/_global_updates.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_legacy_globals.py` & `portage-3.0.64/lib/portage/_legacy_globals.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_selinux.py` & `portage-3.0.64/lib/portage/_selinux.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/ProfilePackageSet.py` & `portage-3.0.64/lib/portage/_sets/ProfilePackageSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/__init__.py` & `portage-3.0.64/lib/portage/_sets/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/base.py` & `portage-3.0.64/lib/portage/_sets/base.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/dbapi.py` & `portage-3.0.64/lib/portage/_sets/dbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/files.py` & `portage-3.0.64/lib/portage/_sets/files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/libs.py` & `portage-3.0.64/lib/portage/_sets/libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/profiles.py` & `portage-3.0.64/lib/portage/_sets/profiles.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/security.py` & `portage-3.0.64/lib/portage/_sets/security.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/_sets/shell.py` & `portage-3.0.64/lib/portage/_sets/shell.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/binpkg.py` & `portage-3.0.64/lib/portage/binpkg.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             except tarfile.TarError:
                 pass
 
     except Exception as err:
         # We got many different exceptions here, so have to catch all of them.
         file_format = None
         writemsg(
-            colorize("ERR", f"Error reading binpkg '{binpkg_path}': {err}"),
+            colorize("ERR", f"Error reading binpkg '{binpkg_path}': {err}\n"),
         )
         raise InvalidBinaryPackageFormat(f"Error reading binpkg '{binpkg_path}': {err}")
 
     if file_format is None:
         raise InvalidBinaryPackageFormat(
             f"Unsupported binary package format from '{binpkg_path}'"
         )
```

### Comparing `portage-3.0.63/lib/portage/binrepo/config.py` & `portage-3.0.64/lib/portage/binrepo/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/anydbm.py` & `portage-3.0.64/lib/portage/cache/anydbm.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/cache_errors.py` & `portage-3.0.64/lib/portage/cache/cache_errors.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/ebuild_xattr.py` & `portage-3.0.64/lib/portage/cache/ebuild_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/flat_hash.py` & `portage-3.0.64/lib/portage/cache/flat_hash.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/fs_template.py` & `portage-3.0.64/lib/portage/cache/fs_template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/index/IndexStreamIterator.py` & `portage-3.0.64/lib/portage/cache/index/IndexStreamIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/index/pkg_desc_index.py` & `portage-3.0.64/lib/portage/cache/index/pkg_desc_index.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/mappings.py` & `portage-3.0.64/lib/portage/cache/mappings.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/metadata.py` & `portage-3.0.64/lib/portage/cache/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/sql_template.py` & `portage-3.0.64/lib/portage/cache/sql_template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/sqlite.py` & `portage-3.0.64/lib/portage/cache/sqlite.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/template.py` & `portage-3.0.64/lib/portage/cache/template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cache/volatile.py` & `portage-3.0.64/lib/portage/cache/volatile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/checksum.py` & `portage-3.0.64/lib/portage/checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/const.py` & `portage-3.0.64/lib/portage/const.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/cvstree.py` & `portage-3.0.64/lib/portage/cvstree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/data.py` & `portage-3.0.64/lib/portage/data.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/DummyTree.py` & `portage-3.0.64/lib/portage/dbapi/DummyTree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/IndexedPortdb.py` & `portage-3.0.64/lib/portage/dbapi/IndexedPortdb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/IndexedVardb.py` & `portage-3.0.64/lib/portage/dbapi/IndexedVardb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/_ContentsCaseSensitivityManager.py` & `portage-3.0.64/lib/portage/dbapi/_ContentsCaseSensitivityManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/_MergeProcess.py` & `portage-3.0.64/lib/portage/dbapi/_MergeProcess.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import multiprocessing
 import platform
 
 import fcntl
 import portage
 from portage import os, _unicode_decode
 from portage.package.ebuild._ipc.QueryCommand import QueryCommand
-from portage.util._ctypes import find_library
+from portage.util._ctypes import load_libc
 import portage.elog.messages
 from portage.util._async.ForkProcess import ForkProcess
 from portage.util import no_color
 
 
 class MergeProcess(ForkProcess):
     """
@@ -60,15 +60,15 @@
             settings.reset()
             settings.setcpv(cpv, mydb=self.mydbapi)
 
         # This caches the libc library lookup in the current
         # process, so that it's only done once rather than
         # for each child process.
         if platform.system() == "Linux" and "merge-sync" in settings.features:
-            find_library("c")
+            load_libc()
 
         # Inherit stdin by default, so that the pdb SIGUSR1
         # handler is usable for the subprocess.
         if self.fd_pipes is None:
             self.fd_pipes = {}
         else:
             self.fd_pipes = self.fd_pipes.copy()
```

### Comparing `portage-3.0.63/lib/portage/dbapi/_SyncfsProcess.py` & `portage-3.0.64/lib/portage/dbapi/_SyncfsProcess.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2012-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import functools
 
 from portage import os
-from portage.util._ctypes import find_library, LoadLibrary
+from portage.util._ctypes import load_libc
 from portage.util._async.ForkProcess import ForkProcess
 
 
 class SyncfsProcess(ForkProcess):
     """
     Isolate ctypes usage in a subprocess, in order to avoid
     potential problems with stale cached libraries as
@@ -20,23 +20,17 @@
 
     def _start(self):
         self.target = functools.partial(self._target, self._get_syncfs, self.paths)
         super()._start()
 
     @staticmethod
     def _get_syncfs():
-        filename = find_library("c")
-        if filename is not None:
-            library = LoadLibrary(filename)
-            if library is not None:
-                try:
-                    return library.syncfs
-                except AttributeError:
-                    pass
-
+        (libc, _) = load_libc()
+        if libc is not None:
+            return getattr(libc, "syncfs", None)
         return None
 
     @staticmethod
     def _target(get_syncfs, paths):
         syncfs_failed = False
         syncfs = get_syncfs()
```

### Comparing `portage-3.0.63/lib/portage/dbapi/_VdbMetadataDelta.py` & `portage-3.0.64/lib/portage/dbapi/_VdbMetadataDelta.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/__init__.py` & `portage-3.0.64/lib/portage/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/_expand_new_virt.py` & `portage-3.0.64/lib/portage/dbapi/_expand_new_virt.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/_similar_name_search.py` & `portage-3.0.64/lib/portage/dbapi/_similar_name_search.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/bintree.py` & `portage-3.0.64/lib/portage/dbapi/bintree.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 import tempfile
 import textwrap
 import time
 import traceback
 import warnings
 from gzip import GzipFile
 from itertools import chain
+from pathlib import PurePath
 from urllib.parse import urlparse
 
 
 class UseCachedCopyOfRemoteIndex(Exception):
     # If the local copy is recent enough
     # then fetching the remote index can be skipped.
     pass
@@ -835,19 +836,26 @@
         try:
             pkgdir_st = os.stat(self.pkgdir)
         except OSError:
             ensure_dirs(path)
             return
         pkgdir_gid = pkgdir_st.st_gid
         pkgdir_grp_mode = 0o2070 & pkgdir_st.st_mode
-        try:
-            ensure_dirs(path, gid=pkgdir_gid, mode=pkgdir_grp_mode, mask=0)
-        except PortageException:
-            if not os.path.isdir(path):
-                raise
+
+        components = []
+        for component in PurePath(path).relative_to(self.pkgdir).parts:
+            components.append(component)
+            component_path = os.path.join(self.pkgdir, *components)
+            try:
+                ensure_dirs(
+                    component_path, gid=pkgdir_gid, mode=pkgdir_grp_mode, mask=0
+                )
+            except PortageException:
+                if not os.path.isdir(component_path):
+                    raise
 
     def _file_permissions(self, path):
         try:
             pkgdir_st = os.stat(self.pkgdir)
         except OSError:
             pass
         else:
@@ -1620,15 +1628,15 @@
                         continue
 
                     if gpkg_only:
                         try:
                             binpkg_format = get_binpkg_format(
                                 d.get("PATH"), remote=True
                             )
-                        except InvalidBinaryPackageFormat:
+                        except InvalidBinaryPackageFormat as e:
                             writemsg(
                                 colorize(
                                     "WARN",
                                     f"{e}\n",
                                 ),
                                 noiselevel=-1,
                             )
```

### Comparing `portage-3.0.63/lib/portage/dbapi/cpv_expand.py` & `portage-3.0.64/lib/portage/dbapi/cpv_expand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/dep_expand.py` & `portage-3.0.64/lib/portage/dbapi/dep_expand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/meson.build` & `portage-3.0.64/lib/portage/dbapi/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/porttree.py` & `portage-3.0.64/lib/portage/dbapi/porttree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/vartree.py` & `portage-3.0.64/lib/portage/dbapi/vartree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dbapi/virtual.py` & `portage-3.0.64/lib/portage/dbapi/virtual.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/debug.py` & `portage-3.0.64/lib/portage/debug.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dep/__init__.py` & `portage-3.0.64/lib/portage/dep/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dep/_dnf.py` & `portage-3.0.64/lib/portage/dep/_dnf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dep/_slot_operator.py` & `portage-3.0.64/lib/portage/dep/_slot_operator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dep/dep_check.py` & `portage-3.0.64/lib/portage/dep/dep_check.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dep/libc.py` & `portage-3.0.64/lib/portage/dep/libc.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dep/soname/SonameAtom.py` & `portage-3.0.64/lib/portage/dep/soname/SonameAtom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dep/soname/multilib_category.py` & `portage-3.0.64/lib/portage/dep/soname/multilib_category.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dep/soname/parse.py` & `portage-3.0.64/lib/portage/dep/soname/parse.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/dispatch_conf.py` & `portage-3.0.64/lib/portage/dispatch_conf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/eapi.py` & `portage-3.0.64/lib/portage/eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/eclass_cache.py` & `portage-3.0.64/lib/portage/eclass_cache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/__init__.py` & `portage-3.0.64/lib/portage/elog/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/filtering.py` & `portage-3.0.64/lib/portage/elog/filtering.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/messages.py` & `portage-3.0.64/lib/portage/elog/messages.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/mod_echo.py` & `portage-3.0.64/lib/portage/elog/mod_echo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/mod_mail.py` & `portage-3.0.64/lib/portage/elog/mod_mail.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/mod_mail_summary.py` & `portage-3.0.64/lib/portage/elog/mod_mail_summary.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/mod_save.py` & `portage-3.0.64/lib/portage/elog/mod_save.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/mod_save_summary.py` & `portage-3.0.64/lib/portage/elog/mod_save_summary.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/elog/mod_syslog.py` & `portage-3.0.64/lib/portage/elog/mod_syslog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/defaults.py` & `portage-3.0.64/lib/portage/emaint/defaults.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/main.py` & `portage-3.0.64/lib/portage/emaint/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/binhost/__init__.py` & `portage-3.0.64/lib/portage/emaint/modules/binhost/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/binhost/binhost.py` & `portage-3.0.64/lib/portage/emaint/modules/binhost/binhost.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/config/__init__.py` & `portage-3.0.64/lib/portage/emaint/modules/config/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/config/config.py` & `portage-3.0.64/lib/portage/emaint/modules/config/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/logs/__init__.py` & `portage-3.0.64/lib/portage/emaint/modules/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/logs/logs.py` & `portage-3.0.64/lib/portage/emaint/modules/logs/logs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/merges/__init__.py` & `portage-3.0.64/lib/portage/emaint/modules/merges/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/merges/merges.py` & `portage-3.0.64/lib/portage/emaint/modules/merges/merges.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/move/__init__.py` & `portage-3.0.64/lib/portage/emaint/modules/move/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/move/move.py` & `portage-3.0.64/lib/portage/emaint/modules/move/move.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/resume/__init__.py` & `portage-3.0.64/lib/portage/emaint/modules/resume/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/resume/resume.py` & `portage-3.0.64/lib/portage/emaint/modules/resume/resume.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/sync/__init__.py` & `portage-3.0.64/lib/portage/emaint/modules/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/sync/sync.py` & `portage-3.0.64/lib/portage/emaint/modules/sync/sync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/emaint/modules/world/world.py` & `portage-3.0.64/lib/portage/emaint/modules/world/world.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/env/config.py` & `portage-3.0.64/lib/portage/env/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/env/loaders.py` & `portage-3.0.64/lib/portage/env/loaders.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/env/validators.py` & `portage-3.0.64/lib/portage/env/validators.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/exception.py` & `portage-3.0.64/lib/portage/exception.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/getbinpkg.py` & `portage-3.0.64/lib/portage/getbinpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/glsa.py` & `portage-3.0.64/lib/portage/glsa.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/gpg.py` & `portage-3.0.64/lib/portage/gpg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/gpkg.py` & `portage-3.0.64/lib/portage/gpkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         self.closed = True
 
         if self.proc is not None:
             self.thread.join()
             try:
                 if self.proc.wait() != os.EX_OK:
                     if not self.killed:
-                        writemsg(colorize("BAD", f"GPKG external program failed."))
+                        writemsg(colorize("BAD", f"GPKG external program failed.\n"))
                         raise CompressorOperationFailed("decompression failed")
             finally:
                 self.proc.stdout.close()
 
 
 class checksum_helper:
     """
@@ -414,25 +414,25 @@
             try:
                 drop_user = self.settings.get("GPG_VERIFY_USER_DROP", "nobody")
                 if drop_user == "":
                     self.uid = None
                 else:
                     self.uid = pwd.getpwnam(drop_user).pw_uid
             except KeyError:
-                writemsg(colorize("BAD", f"!!! Failed to find user {drop_user}."))
+                writemsg(colorize("BAD", f"!!! Failed to find user {drop_user}.\n"))
                 raise
 
             try:
                 drop_group = self.settings.get("GPG_VERIFY_GROUP_DROP", "nogroup")
                 if drop_group == "":
                     self.gid = None
                 else:
                     self.gid = grp.getgrnam(drop_group).gr_gid
             except KeyError:
-                writemsg(colorize("BAD", f"!!! Failed to find group {drop_group}."))
+                writemsg(colorize("BAD", f"!!! Failed to find group {drop_group}.\n"))
                 raise
         else:
             self.uid = None
             self.gid = None
 
         # Initialize the hash libs
         self.libs = {}
@@ -632,41 +632,43 @@
                 if member is None:
                     break
                 if (member.name in self.file_list) or (
                     os.path.join(".", member.name) in self.file_list
                 ):
                     writemsg(
                         colorize(
-                            "BAD", f"Danger: duplicate files detected: {member.name}"
+                            "BAD", f"Danger: duplicate files detected: {member.name}\n"
                         )
                     )
                     raise ValueError("Duplicate files detected.")
                 if member.name.startswith("/"):
                     writemsg(
                         colorize(
-                            "BAD", f"Danger: absolute path detected: {member.name}"
+                            "BAD", f"Danger: absolute path detected: {member.name}\n"
                         )
                     )
                     raise ValueError("Absolute path detected.")
                 if member.name.startswith("../") or ("/../" in member.name):
                     writemsg(
                         colorize(
-                            "BAD", f"Danger: path traversal detected: {member.name}"
+                            "BAD", f"Danger: path traversal detected: {member.name}\n"
                         )
                     )
                     raise ValueError("Path traversal detected.")
                 if member.isdev():
                     writemsg(
-                        colorize("BAD", f"Danger: device file detected: {member.name}")
+                        colorize(
+                            "BAD", f"Danger: device file detected: {member.name}\n"
+                        )
                     )
                     raise ValueError("Device file detected.")
                 if member.islnk() and (member.linkname not in self.file_list):
                     writemsg(
                         colorize(
-                            "BAD", f"Danger: hardlink escape detected: {member.name}"
+                            "BAD", f"Danger: hardlink escape detected: {member.name}\n"
                         )
                     )
                     raise ValueError("Hardlink escape detected.")
 
                 self.file_list.append(member.name)
                 self.tar.extract(member, path=temp_dir.name)
 
@@ -991,15 +993,15 @@
             ) as image_tar:
                 with tarfile.open(mode="r|", fileobj=image_tar) as image:
                     try:
                         image_safe = tar_safe_extract(image, "image")
                         image_safe.extractall(decompress_dir)
                         image_tar.close()
                     except Exception as ex:
-                        writemsg(colorize("BAD", "!!!Extract failed."))
+                        writemsg(colorize("BAD", "!!!Extract failed.\n"))
                         raise
                     finally:
                         if not image_tar.closed:
                             image_tar.kill()
 
     def update_metadata(self, metadata, new_basename=None, force=False):
         """
```

### Comparing `portage-3.0.63/lib/portage/installation.py` & `portage-3.0.64/lib/portage/installation.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/localization.py` & `portage-3.0.64/lib/portage/localization.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/locks.py` & `portage-3.0.64/lib/portage/locks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/mail.py` & `portage-3.0.64/lib/portage/mail.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/manifest.py` & `portage-3.0.64/lib/portage/manifest.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/meson.build` & `portage-3.0.64/lib/portage/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/metadata.py` & `portage-3.0.64/lib/portage/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/module.py` & `portage-3.0.64/lib/portage/module.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/news.py` & `portage-3.0.64/lib/portage/news.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/output.py` & `portage-3.0.64/lib/portage/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 __docformat__ = "epytext"
 
 import errno
 import itertools
 import re
 import subprocess
 import sys
+from typing import Optional
 
 import portage
 
 portage.proxy.lazyimport.lazyimport(
     globals(),
     "portage.process:spawn",
     "portage.util:writemsg",
@@ -550,31 +551,35 @@
                 pass
             else:
                 if val[0] >= 0 and val[1] >= 0:
                     return val
     return (0, 0)
 
 
-def set_term_size(lines, columns, fd):
+def set_term_size(lines: int, columns: int, fd: int) -> Optional[asyncio.Future]:
     """
     Set the number of lines and columns for the tty that is connected to fd.
     For portability, this simply calls `stty rows $lines columns $columns`.
+
+    If spawn succeeds and the event loop is running then an instance of
+    asyncio.Future is returned and the caller should wait for it in order
+    to prevent possible error messages like this:
+
+    [ERROR] Task was destroyed but it is pending!
     """
 
     cmd = ["stty", "rows", str(lines), "columns", str(columns)]
     try:
         proc = spawn(cmd, env=os.environ, fd_pipes={0: fd}, returnproc=True)
     except CommandNotFound:
         writemsg(_("portage: stty: command not found\n"), noiselevel=-1)
     else:
         loop = asyncio.get_event_loop()
         if loop.is_running():
-            asyncio.ensure_future(proc.wait(), loop).add_done_callback(
-                lambda future: future.result()
-            )
+            return asyncio.ensure_future(proc.wait(), loop=loop)
         else:
             loop.run_until_complete(proc.wait())
 
 
 class EOutput:
     """
     Performs fancy terminal formatting for status and informational messages.
```

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/KeywordsManager.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/KeywordsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/LicenseManager.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/LicenseManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/LocationsManager.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/LocationsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/MaskManager.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/MaskManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/UseManager.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/UseManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/VirtualsManager.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/VirtualsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/env_var_validation.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/env_var_validation.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/features_set.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/features_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/helper.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_config/special_env_vars.py` & `portage-3.0.64/lib/portage/package/ebuild/_config/special_env_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
         "PORTAGE_OVERRIDE_EPREFIX",
         "PORTAGE_PIPE_FD",
         "PORTAGE_PROPERTIES",
         "PORTAGE_PYM_PATH",
         "PORTAGE_PYTHON",
         "PORTAGE_PYTHONPATH",
         "PORTAGE_QUIET",
+        "PORTAGE_REPO_REVISIONS",
         "PORTAGE_REPO_NAME",
         "PORTAGE_REPOSITORIES",
         "PORTAGE_RESTRICT",
         "PORTAGE_SIGPIPE_STATUS",
         "PORTAGE_SOCKS5_PROXY",
         "PORTAGE_TMPDIR",
         "PORTAGE_UPDATE_ENV",
```

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_ipc/ExitCommand.py` & `portage-3.0.64/lib/portage/package/ebuild/_ipc/ExitCommand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_ipc/QueryCommand.py` & `portage-3.0.64/lib/portage/package/ebuild/_ipc/QueryCommand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_metadata_invalid.py` & `portage-3.0.64/lib/portage/package/ebuild/_metadata_invalid.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py` & `portage-3.0.64/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py` & `portage-3.0.64/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py` & `portage-3.0.64/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/_spawn_nofetch.py` & `portage-3.0.64/lib/portage/package/ebuild/_spawn_nofetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/config.py` & `portage-3.0.64/lib/portage/package/ebuild/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2202,15 +2202,17 @@
             if "test" in self.features:
                 if ebuild_force_test and "test" in self.usemask:
                     self.usemask = frozenset(x for x in self.usemask if x != "test")
             if restrict_test or ("test" in self.usemask and not ebuild_force_test):
                 # "test" is in IUSE and USE=test is masked, so execution
                 # of src_test() probably is not reliable. Therefore,
                 # temporarily disable FEATURES=test just for this package.
-                self["FEATURES"] = " ".join(x for x in self.features if x != "test")
+                self["FEATURES"] = " ".join(
+                    x for x in sorted(self.features) if x != "test"
+                )
 
         # Allow _* flags from USE_EXPAND wildcards to pass through here.
         use.difference_update(
             [
                 x
                 for x in use
                 if (x not in explicit_iuse and not iuse_implicit_match(x))
```

### Comparing `portage-3.0.63/lib/portage/package/ebuild/deprecated_profile_check.py` & `portage-3.0.64/lib/portage/package/ebuild/deprecated_profile_check.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/digestcheck.py` & `portage-3.0.64/lib/portage/package/ebuild/digestcheck.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/digestgen.py` & `portage-3.0.64/lib/portage/package/ebuild/digestgen.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/doebuild.py` & `portage-3.0.64/lib/portage/package/ebuild/doebuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "portage.dep.soname.multilib_category:compute_multilib_category",
     "portage.util._desktop_entry:validate_desktop_entry",
     "portage.util._dyn_libs.NeededEntry:NeededEntry",
     "portage.util._dyn_libs.soname_deps:SonameDepsProcessor",
     "portage.util._async.SchedulerInterface:SchedulerInterface",
     "portage.util._eventloop.global_event_loop:global_event_loop",
     "portage.util.ExtractKernelVersion:ExtractKernelVersion",
+    "_emerge.EbuildPhase:_setup_locale",
 )
 
 from portage import (
     bsd_chflags,
     eapi_is_supported,
     merge,
     os,
@@ -1030,14 +1031,21 @@
             tmpdir_orig = mysettings["PORTAGE_TMPDIR"]
             mysettings["PORTAGE_TMPDIR"] = tmpdir
 
         doebuild_environment(
             myebuild, mydo, myroot, mysettings, debug, use_cache, mydbapi
         )
 
+        # For returnproc or returnpid assume that the event loop is running
+        # so we can't run the event loop to call _setup_locale in this case
+        # and we have to assume the caller took care of it (otherwise
+        # config.environ() will raise AssertionError).
+        if not (returnproc or returnpid):
+            asyncio.run(_setup_locale(mysettings))
+
         if mydo in clean_phases:
             builddir_lock = None
             if not returnpid and "PORTAGE_BUILDDIR_LOCKED" not in mysettings:
                 builddir_lock = EbuildBuildDir(
                     scheduler=asyncio._safe_loop(), settings=mysettings
                 )
                 builddir_lock.scheduler.run_until_complete(builddir_lock.async_lock())
@@ -1801,14 +1809,22 @@
     return actionmap
 
 
 def _validate_deps(mysettings, myroot, mydo, mydbapi):
     invalid_dep_exempt_phases = {"clean", "cleanrm", "help", "prerm", "postrm"}
     all_keys = set(Package.metadata_keys)
     all_keys.add("SRC_URI")
+    # Since configdict["pkg"]["USE"] may contain package.use settings
+    # from config.setcpv, it is inappropriate to use here (bug 675748),
+    # so discard it. This is only an issue because configdict["pkg"] is
+    # a sub-optimal place to extract metadata from. This issue does not
+    # necessarily indicate a flaw in the Package constructor, since
+    # passing in precalculated USE can be valid for things like
+    # autounmask USE changes.
+    all_keys.discard("USE")
     all_keys = tuple(all_keys)
     metadata = mysettings.configdict["pkg"]
     if all(k in metadata for k in ("PORTAGE_REPO_NAME", "SRC_URI")):
         metadata = dict(
             ((k, metadata[k]) for k in all_keys if k in metadata),
             repository=metadata["PORTAGE_REPO_NAME"],
         )
@@ -1826,14 +1842,18 @@
 
     class FakeTree:
         def __init__(self, mydb):
             self.dbapi = mydb
 
     root_config = RootConfig(mysettings, {"porttree": FakeTree(mydbapi)}, None)
 
+    # A USE calculation from setcpv should always be available here because
+    # mysettings.mycpv is not None, so use it to prevent redundant setcpv calls.
+    metadata["USE"] = mysettings["PORTAGE_USE"]
+
     pkg = Package(
         built=False,
         cpv=mysettings.mycpv,
         metadata=metadata,
         root_config=root_config,
         type_name="ebuild",
     )
```

### Comparing `portage-3.0.63/lib/portage/package/ebuild/fetch.py` & `portage-3.0.64/lib/portage/package/ebuild/fetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/getmaskingreason.py` & `portage-3.0.64/lib/portage/package/ebuild/getmaskingreason.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/getmaskingstatus.py` & `portage-3.0.64/lib/portage/package/ebuild/getmaskingstatus.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/meson.build` & `portage-3.0.64/lib/portage/package/ebuild/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/prepare_build_dirs.py` & `portage-3.0.64/lib/portage/package/ebuild/prepare_build_dirs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/package/ebuild/profile_iuse.py` & `portage-3.0.64/lib/portage/package/ebuild/profile_iuse.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/process.py` & `portage-3.0.64/lib/portage/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright 1998-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 
 import atexit
 import errno
 import fcntl
+import io
 import logging
 import multiprocessing
 import platform
 import signal
 import socket
 import subprocess
 import sys
@@ -33,15 +34,15 @@
     "portage.util.futures:asyncio",
     "portage.util:dump_traceback,writemsg,writemsg_level",
 )
 
 from portage.const import BASH_BINARY, SANDBOX_BINARY, FAKEROOT_BINARY
 from portage.exception import CommandNotFound
 from portage.proxy.objectproxy import ObjectProxy
-from portage.util._ctypes import find_library, LoadLibrary, ctypes
+from portage.util._ctypes import load_libc, LoadLibrary, ctypes
 
 try:
     from portage.util.netlink import RtNetlink
 except ImportError:
     if platform.system() == "Linux":
         raise
     RtNetlink = None
@@ -222,14 +223,42 @@
             dump_traceback("Error in portage.process.run_exitfuncs", noiselevel=0)
             exc_info = sys.exc_info()
 
     if exc_info is not None:
         raise exc_info[0](exc_info[1]).with_traceback(exc_info[2])
 
 
+async def run_coroutine_exitfuncs():
+    """
+    This is the same as run_exitfuncs but it uses asyncio.iscoroutinefunction
+    to check which functions to run. It is called by the AsyncioEventLoop
+    _close_main method just before the loop is closed.
+    """
+    tasks = []
+    for index, (func, targs, kargs) in reversed(list(enumerate(_exithandlers))):
+        if asyncio.iscoroutinefunction(func):
+            del _exithandlers[index]
+            tasks.append(asyncio.ensure_future(func(*targs, **kargs)))
+    tracebacks = []
+    exc_info = None
+    for task in tasks:
+        try:
+            await task
+        except Exception:
+            file = io.StringIO()
+            traceback.print_exc(file=file)
+            tracebacks.append(file.getvalue())
+            exc_info = sys.exc_info()
+    if len(tracebacks) > 1:
+        for tb in tracebacks[:-1]:
+            print(tb, file=sys.stderr, flush=True)
+    if exc_info is not None:
+        raise exc_info[1].with_traceback(exc_info[2])
+
+
 atexit.register(run_exitfuncs)
 
 # It used to be necessary for API consumers to remove pids from spawned_pids,
 # since otherwise it would accumulate a pids endlessly. Now, spawned_pids is
 # just an empty dummy list, so for backward compatibility, ignore ValueError
 # for removal on non-existent items.
 
@@ -956,19 +985,17 @@
     # the parent process (see bug #289486).
     signal.signal(signal.SIGQUIT, signal.SIG_DFL)
 
     # Unshare (while still uid==0)
     have_unshare = False
     libc = None
     if unshare_net or unshare_ipc or unshare_mount or unshare_pid:
-        filename = find_library("c")
-        if filename is not None:
-            libc = LoadLibrary(filename)
-            if libc is not None:
-                have_unshare = hasattr(libc, "unshare")
+        (libc, _) = load_libc()
+        if libc is not None:
+            have_unshare = hasattr(libc, "unshare")
 
     if not have_unshare:
         # unshare() may not be supported by libc
         unshare_net = False
         unshare_ipc = False
         unshare_mount = False
         unshare_pid = False
@@ -1208,19 +1235,15 @@
         @param flags: unshare flags
         @type flags: int
         @rtype: int
         @returns: errno value, or 0 if no error occurred.
         """
         # This ctypes library lookup caches the result for use in the
         # subprocess when the multiprocessing start method is fork.
-        filename = find_library("c")
-        if filename is None:
-            return errno.ENOTSUP
-
-        libc = LoadLibrary(filename)
+        (libc, filename) = load_libc()
         if libc is None:
             return errno.ENOTSUP
 
         parent_pipe, subproc_pipe = multiprocessing.Pipe(duplex=False)
 
         proc = multiprocessing.Process(
             target=cls._run_subproc,
```

### Comparing `portage-3.0.63/lib/portage/progress.py` & `portage-3.0.64/lib/portage/progress.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/proxy/lazyimport.py` & `portage-3.0.64/lib/portage/proxy/lazyimport.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/proxy/objectproxy.py` & `portage-3.0.64/lib/portage/proxy/objectproxy.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/repository/config.py` & `portage-3.0.64/lib/portage/repository/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/repository/storage/hardlink_quarantine.py` & `portage-3.0.64/lib/portage/repository/storage/hardlink_quarantine.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/repository/storage/hardlink_rcu.py` & `portage-3.0.64/lib/portage/repository/storage/hardlink_rcu.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/repository/storage/inplace.py` & `portage-3.0.64/lib/portage/repository/storage/inplace.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/repository/storage/interface.py` & `portage-3.0.64/lib/portage/repository/storage/interface.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/__init__.py` & `portage-3.0.64/lib/portage/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/config_checks.py` & `portage-3.0.64/lib/portage/sync/config_checks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/controller.py` & `portage-3.0.64/lib/portage/sync/controller.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/getaddrinfo_validate.py` & `portage-3.0.64/lib/portage/sync/getaddrinfo_validate.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/cvs/__init__.py` & `portage-3.0.64/lib/portage/sync/modules/cvs/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/cvs/cvs.py` & `portage-3.0.64/lib/portage/sync/modules/cvs/cvs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/git/__init__.py` & `portage-3.0.64/lib/portage/sync/modules/git/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/git/git.py` & `portage-3.0.64/lib/portage/sync/modules/git/git.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/mercurial/__init__.py` & `portage-3.0.64/lib/portage/sync/modules/mercurial/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/mercurial/mercurial.py` & `portage-3.0.64/lib/portage/sync/modules/mercurial/mercurial.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/rsync/__init__.py` & `portage-3.0.64/lib/portage/sync/modules/rsync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/rsync/rsync.py` & `portage-3.0.64/lib/portage/sync/modules/rsync/rsync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/svn/__init__.py` & `portage-3.0.64/lib/portage/sync/modules/svn/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/svn/svn.py` & `portage-3.0.64/lib/portage/sync/modules/svn/svn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/webrsync/__init__.py` & `portage-3.0.64/lib/portage/sync/modules/webrsync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/modules/webrsync/webrsync.py` & `portage-3.0.64/lib/portage/sync/modules/webrsync/webrsync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/old_tree_timestamp.py` & `portage-3.0.64/lib/portage/sync/old_tree_timestamp.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/sync/syncbase.py` & `portage-3.0.64/lib/portage/sync/syncbase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev` & `portage-3.0.64/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev` & `portage-3.0.64/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key` & `portage-3.0.64/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key` & `portage-3.0.64/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/.gnupg/pubring.kbx` & `portage-3.0.64/lib/portage/tests/.gnupg/pubring.kbx`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/.gnupg/trustdb.gpg` & `portage-3.0.64/lib/portage/tests/.gnupg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/__init__.py` & `portage-3.0.64/lib/portage/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/bin/setup_env.py` & `portage-3.0.64/lib/portage/tests/bin/setup_env.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/bin/test_dobin.py` & `portage-3.0.64/lib/portage/tests/bin/test_dobin.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/bin/test_dodir.py` & `portage-3.0.64/lib/portage/tests/bin/test_dodir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/bin/test_doins.py` & `portage-3.0.64/lib/portage/tests/bin/test_doins.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/bin/test_eapi7_ver_funcs.py` & `portage-3.0.64/lib/portage/tests/bin/test_eapi7_ver_funcs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/bin/test_filter_bash_env.py` & `portage-3.0.64/lib/portage/tests/bin/test_filter_bash_env.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/conftest.py` & `portage-3.0.64/lib/portage/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dbapi/test_auxdb.py` & `portage-3.0.64/lib/portage/tests/dbapi/test_auxdb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dbapi/test_bintree.py` & `portage-3.0.64/lib/portage/tests/dbapi/test_bintree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,42 @@
-# Copyright 2022 Gentoo Authors
+# Copyright 2022-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 from unittest.mock import MagicMock, patch, call
 import os
 import tempfile
 
 from portage.tests import TestCase
 
 from portage.dbapi.bintree import binarytree
 from portage.localization import _
 from portage.const import BINREPOS_CONF_FILE
 
 
 class BinarytreeTestCase(TestCase):
+    @classmethod
+    def setUpClass(cls):
+        """
+        Create a temporary TMPDIR which prevents test
+        methods of this class from leaving behind an empty
+        /tmp/Packages file if TMPDIR is initially unset.
+        """
+        cls._orig_tmpdir = os.environ.get("TMPDIR")
+        cls._tmpdir = tempfile.TemporaryDirectory()
+        os.environ["TMPDIR"] = cls._tmpdir.name
+
+    @classmethod
+    def tearDownClass(cls):
+        cls._tmpdir.cleanup()
+        if cls._orig_tmpdir is None:
+            os.environ.pop("TMPDIR", None)
+        else:
+            os.environ["TMPDIR"] = cls._orig_tmpdir
+        del cls._orig_tmpdir, cls._tmpdir
+
     def test_required_init_params(self):
         with self.assertRaises(TypeError) as cm:
             binarytree()
         self.assertEqual(str(cm.exception), "pkgdir parameter is required")
         with self.assertRaises(TypeError) as cm:
             binarytree(pkgdir=os.getenv("TMPDIR", "/tmp"))
         self.assertEqual(str(cm.exception), "settings parameter is required")
```

### Comparing `portage-3.0.63/lib/portage/tests/dbapi/test_fakedbapi.py` & `portage-3.0.64/lib/portage/tests/dbapi/test_fakedbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dbapi/test_portdb_cache.py` & `portage-3.0.64/lib/portage/tests/dbapi/test_portdb_cache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/meson.build` & `portage-3.0.64/lib/portage/tests/dep/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_atom.py` & `portage-3.0.64/lib/portage/tests/dep/test_atom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_best_match_to_list.py` & `portage-3.0.64/lib/portage/tests/dep/test_best_match_to_list.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_check_required_use.py` & `portage-3.0.64/lib/portage/tests/dep/test_check_required_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_dep_getcpv.py` & `portage-3.0.64/lib/portage/tests/dep/test_dep_getcpv.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_dep_getrepo.py` & `portage-3.0.64/lib/portage/tests/dep/test_dep_getrepo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_dep_getslot.py` & `portage-3.0.64/lib/portage/tests/dep/test_dep_getslot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_dep_getusedeps.py` & `portage-3.0.64/lib/portage/tests/dep/test_dep_getusedeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_dnf_convert.py` & `portage-3.0.64/lib/portage/tests/dep/test_dnf_convert.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_extended_atom_dict.py` & `portage-3.0.64/lib/portage/tests/dep/test_extended_atom_dict.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_extract_affecting_use.py` & `portage-3.0.64/lib/portage/tests/dep/test_extract_affecting_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_get_operator.py` & `portage-3.0.64/lib/portage/tests/dep/test_get_operator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_get_required_use_flags.py` & `portage-3.0.64/lib/portage/tests/dep/test_get_required_use_flags.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_isjustname.py` & `portage-3.0.64/lib/portage/tests/dep/test_isjustname.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_isvalidatom.py` & `portage-3.0.64/lib/portage/tests/dep/test_isvalidatom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_libc.py` & `portage-3.0.64/lib/portage/tests/dep/test_libc.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_match_from_list.py` & `portage-3.0.64/lib/portage/tests/dep/test_match_from_list.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_overlap_dnf.py` & `portage-3.0.64/lib/portage/tests/dep/test_overlap_dnf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_paren_reduce.py` & `portage-3.0.64/lib/portage/tests/dep/test_paren_reduce.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_soname_atom_pickle.py` & `portage-3.0.64/lib/portage/tests/dep/test_soname_atom_pickle.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_standalone.py` & `portage-3.0.64/lib/portage/tests/dep/test_standalone.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/dep/test_use_reduce.py` & `portage-3.0.64/lib/portage/tests/dep/test_use_reduce.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/ebuild/test_array_fromfile_eof.py` & `portage-3.0.64/lib/portage/tests/ebuild/test_array_fromfile_eof.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/ebuild/test_config.py` & `portage-3.0.64/lib/portage/tests/ebuild/test_config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/ebuild/test_doebuild_spawn.py` & `portage-3.0.64/lib/portage/tests/ebuild/test_doebuild_spawn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/ebuild/test_fetch.py` & `portage-3.0.64/lib/portage/tests/ebuild/test_fetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/ebuild/test_ipc_daemon.py` & `portage-3.0.64/lib/portage/tests/ebuild/test_ipc_daemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/ebuild/test_shell_quote.py` & `portage-3.0.64/lib/portage/tests/ebuild/test_shell_quote.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/ebuild/test_spawn.py` & `portage-3.0.64/lib/portage/tests/ebuild/test_spawn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/ebuild/test_use_expand_incremental.py` & `portage-3.0.64/lib/portage/tests/ebuild/test_use_expand_incremental.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/conftest.py` & `portage-3.0.64/lib/portage/tests/emerge/conftest.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/test_actions.py` & `portage-3.0.64/lib/portage/tests/emerge/test_actions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/test_baseline.py` & `portage-3.0.64/lib/portage/tests/emerge/test_baseline.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/test_binpkg_fetch.py` & `portage-3.0.64/lib/portage/tests/emerge/test_binpkg_fetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/test_config_protect.py` & `portage-3.0.64/lib/portage/tests/emerge/test_config_protect.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py` & `portage-3.0.64/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/test_emerge_slot_abi.py` & `portage-3.0.64/lib/portage/tests/emerge/test_emerge_slot_abi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/test_global_updates.py` & `portage-3.0.64/lib/portage/tests/emerge/test_global_updates.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/emerge/test_libc_dep_inject.py` & `portage-3.0.64/lib/portage/tests/emerge/test_libc_dep_inject.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/env/config/test_PackageKeywordsFile.py` & `portage-3.0.64/lib/portage/tests/env/config/test_PackageKeywordsFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/env/config/test_PackageMaskFile.py` & `portage-3.0.64/lib/portage/tests/env/config/test_PackageMaskFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/env/config/test_PackageUseFile.py` & `portage-3.0.64/lib/portage/tests/env/config/test_PackageUseFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/env/config/test_PortageModulesFile.py` & `portage-3.0.64/lib/portage/tests/env/config/test_PortageModulesFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/glsa/test_security_set.py` & `portage-3.0.64/lib/portage/tests/glsa/test_security_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_checksum.py` & `portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_gpg.py` & `portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_gpg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_metadata_update.py` & `portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_metadata_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_metadata_url.py` & `portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_metadata_url.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_path.py` & `portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_size.py` & `portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_size.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/gpkg/test_gpkg_stream.py` & `portage-3.0.64/lib/portage/tests/gpkg/test_gpkg_stream.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/lafilefixer/test_lafilefixer.py` & `portage-3.0.64/lib/portage/tests/lafilefixer/test_lafilefixer.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py` & `portage-3.0.64/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/lazyimport/test_preload_portage_submodules.py` & `portage-3.0.64/lib/portage/tests/lazyimport/test_preload_portage_submodules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/lint/test_bash_syntax.py` & `portage-3.0.64/lib/portage/tests/lint/test_bash_syntax.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/lint/test_compile_modules.py` & `portage-3.0.64/lib/portage/tests/lint/test_compile_modules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/lint/test_import_modules.py` & `portage-3.0.64/lib/portage/tests/lint/test_import_modules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/locks/test_asynchronous_lock.py` & `portage-3.0.64/lib/portage/tests/locks/test_asynchronous_lock.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/locks/test_lock_nonblock.py` & `portage-3.0.64/lib/portage/tests/locks/test_lock_nonblock.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/news/test_NewsItem.py` & `portage-3.0.64/lib/portage/tests/news/test_NewsItem.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/meson.build` & `portage-3.0.64/lib/portage/tests/process/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_AsyncFunction.py` & `portage-3.0.64/lib/portage/tests/process/test_AsyncFunction.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_ForkProcess.py` & `portage-3.0.64/lib/portage/tests/process/test_ForkProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_PipeLogger.py` & `portage-3.0.64/lib/portage/tests/process/test_PipeLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_PopenProcess.py` & `portage-3.0.64/lib/portage/tests/process/test_PopenProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_PopenProcessBlockingIO.py` & `portage-3.0.64/lib/portage/tests/process/test_PopenProcessBlockingIO.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_pickle.py` & `portage-3.0.64/lib/portage/tests/process/test_pickle.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_poll.py` & `portage-3.0.64/lib/portage/tests/process/test_poll.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_spawn_fail_e2big.py` & `portage-3.0.64/lib/portage/tests/process/test_spawn_fail_e2big.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_spawn_returnproc.py` & `portage-3.0.64/lib/portage/tests/process/test_spawn_returnproc.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/process/test_spawn_warn_large_env.py` & `portage-3.0.64/lib/portage/tests/process/test_spawn_warn_large_env.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/ResolverPlayground.py` & `portage-3.0.64/lib/portage/tests/resolver/ResolverPlayground.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from portage.tests import cnf_path
 from portage.util import ensure_dirs, normalize_path
 from portage.versions import catsplit
 from portage.exception import InvalidBinaryPackageFormat
 from portage.gpg import GPG
 
 import _emerge
-from _emerge.actions import _calc_depclean
+from _emerge.actions import _calc_depclean, expand_set_arguments
 from _emerge.Blocker import Blocker
 from _emerge.create_depgraph_params import create_depgraph_params
 from _emerge.DependencyArg import DependencyArg
 from _emerge.depgraph import (
     _frozen_depgraph_config,
     backtrack_depgraph,
 )
@@ -50,14 +50,15 @@
     config_files = frozenset(
         (
             "eapi",
             "layout.conf",
             "make.conf",
             "modules",
             "package.accept_keywords",
+            "package.env",
             "package.keywords",
             "package.license",
             "package.mask",
             "package.properties",
             "package.provided",
             "packages",
             "package.unmask",
@@ -743,14 +744,22 @@
                 "remove" if action in ("dep_check", "depclean", "prune") else action
             )
             params = create_depgraph_params(options, params_action)
             frozen_config = _frozen_depgraph_config(
                 self.settings, self.trees, options, params, None
             )
 
+            atoms, retval = expand_set_arguments(
+                atoms, action, self.trees[self.eroot]["root_config"]
+            )
+            if retval != os.EX_OK:
+                raise AssertionError(
+                    f"expand_set_arguments failed with retval {retval}"
+                )
+
             if params_action == "remove":
                 depclean_result = _calc_depclean(
                     self.settings,
                     self.trees,
                     None,
                     options,
                     action,
```

### Comparing `portage-3.0.63/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py` & `portage-3.0.64/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py` & `portage-3.0.64/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/meson.build` & `portage-3.0.64/lib/portage/tests/resolver/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/meson.build` & `portage-3.0.64/lib/portage/tests/resolver/soname/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_autounmask.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_depclean.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_depclean.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_downgrade.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_or_choices.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_or_choices.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_reinstall.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_reinstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_skip_update.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_skip_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_slot_conflict_update.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_slot_conflict_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_soname_provided.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_soname_provided.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_unsatisfiable.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_unsatisfiable.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/soname/test_unsatisfied.py` & `portage-3.0.64/lib/portage/tests/resolver/soname/test_unsatisfied.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py` & `portage-3.0.64/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_alternatives_gzip.py` & `portage-3.0.64/lib/portage/tests/resolver/test_alternatives_gzip.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_autounmask.py` & `portage-3.0.64/lib/portage/tests/resolver/test_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_autounmask_binpkg_use.py` & `portage-3.0.64/lib/portage/tests/resolver/test_autounmask_binpkg_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_autounmask_keep_keywords.py` & `portage-3.0.64/lib/portage/tests/resolver/test_autounmask_keep_keywords.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_autounmask_multilib_use.py` & `portage-3.0.64/lib/portage/tests/resolver/test_autounmask_multilib_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_autounmask_parent.py` & `portage-3.0.64/lib/portage/tests/resolver/test_autounmask_parent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_autounmask_use_backtrack.py` & `portage-3.0.64/lib/portage/tests/resolver/test_autounmask_use_backtrack.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_autounmask_use_breakage.py` & `portage-3.0.64/lib/portage/tests/resolver/test_autounmask_use_breakage.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py` & `portage-3.0.64/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_backtracking.py` & `portage-3.0.64/lib/portage/tests/resolver/test_backtracking.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_bdeps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_bdeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py` & `portage-3.0.64/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_blocker.py` & `portage-3.0.64/lib/portage/tests/resolver/test_blocker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_broken_deps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_broken_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_changed_deps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_changed_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_circular_choices.py` & `portage-3.0.64/lib/portage/tests/resolver/test_circular_choices.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_circular_choices_rust.py` & `portage-3.0.64/lib/portage/tests/resolver/test_circular_choices_rust.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_circular_dependencies.py` & `portage-3.0.64/lib/portage/tests/resolver/test_circular_dependencies.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_complete_graph.py` & `portage-3.0.64/lib/portage/tests/resolver/test_complete_graph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py` & `portage-3.0.64/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_cross_dep_priority.py` & `portage-3.0.64/lib/portage/tests/resolver/test_cross_dep_priority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_depclean.py` & `portage-3.0.64/lib/portage/tests/resolver/test_depclean.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_depclean_order.py` & `portage-3.0.64/lib/portage/tests/resolver/test_depclean_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_depclean_slot_unavailable.py` & `portage-3.0.64/lib/portage/tests/resolver/test_depclean_slot_unavailable.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_depth.py` & `portage-3.0.64/lib/portage/tests/resolver/test_depth.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_disjunctive_depend_order.py` & `portage-3.0.64/lib/portage/tests/resolver/test_disjunctive_depend_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_eapi.py` & `portage-3.0.64/lib/portage/tests/resolver/test_eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_emptytree_reinstall_unsatisfiability.py` & `portage-3.0.64/lib/portage/tests/resolver/test_emptytree_reinstall_unsatisfiability.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_features_test_use.py` & `portage-3.0.64/lib/portage/tests/resolver/test_features_test_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py` & `portage-3.0.64/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_installkernel.py` & `portage-3.0.64/lib/portage/tests/resolver/test_installkernel.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_keywords.py` & `portage-3.0.64/lib/portage/tests/resolver/test_keywords.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_merge_order.py` & `portage-3.0.64/lib/portage/tests/resolver/test_merge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py` & `portage-3.0.64/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_multirepo.py` & `portage-3.0.64/lib/portage/tests/resolver/test_multirepo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_multislot.py` & `portage-3.0.64/lib/portage/tests/resolver/test_multislot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_old_dep_chain_display.py` & `portage-3.0.64/lib/portage/tests/resolver/test_old_dep_chain_display.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_onlydeps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_onlydeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_onlydeps_circular.py` & `portage-3.0.64/lib/portage/tests/resolver/test_onlydeps_circular.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_onlydeps_ideps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_onlydeps_ideps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_onlydeps_minimal.py` & `portage-3.0.64/lib/portage/tests/resolver/test_onlydeps_minimal.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_or_choices.py` & `portage-3.0.64/lib/portage/tests/resolver/test_or_choices.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_or_downgrade_installed.py` & `portage-3.0.64/lib/portage/tests/resolver/test_or_downgrade_installed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_or_upgrade_installed.py` & `portage-3.0.64/lib/portage/tests/resolver/test_or_upgrade_installed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_output.py` & `portage-3.0.64/lib/portage/tests/resolver/test_output.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_package_tracker.py` & `portage-3.0.64/lib/portage/tests/resolver/test_package_tracker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_perl_rebuild_bug.py` & `portage-3.0.64/lib/portage/tests/resolver/test_perl_rebuild_bug.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_profile_default_eapi.py` & `portage-3.0.64/lib/portage/tests/resolver/test_profile_default_eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_profile_package_set.py` & `portage-3.0.64/lib/portage/tests/resolver/test_profile_package_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_rebuild.py` & `portage-3.0.64/lib/portage/tests/resolver/test_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_rebuild_ghostscript.py` & `portage-3.0.64/lib/portage/tests/resolver/test_rebuild_ghostscript.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py` & `portage-3.0.64/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_required_use.py` & `portage-3.0.64/lib/portage/tests/resolver/test_required_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py` & `portage-3.0.64/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_simple.py` & `portage-3.0.64/lib/portage/tests/resolver/test_simple.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_abi.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_abi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_abi_downgrade.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_abi_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_change_without_revbump.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_change_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_collisions.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_collisions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_blocked_prune.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_blocked_prune.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_mask_update.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_mask_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_rebuild.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_update.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_conflict_update_virt.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_conflict_update_virt.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_autounmask.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_bdeps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_bdeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_complete_graph.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_complete_graph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_missed_update.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_missed_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_rebuild.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_required_use.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_required_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_unsolved.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_unsolved.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py` & `portage-3.0.64/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py` & `portage-3.0.64/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_targetroot.py` & `portage-3.0.64/lib/portage/tests/resolver/test_targetroot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_unmerge_order.py` & `portage-3.0.64/lib/portage/tests/resolver/test_unmerge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_unnecessary_slot_upgrade.py` & `portage-3.0.64/lib/portage/tests/resolver/test_unnecessary_slot_upgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_update.py` & `portage-3.0.64/lib/portage/tests/resolver/test_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_use_dep_defaults.py` & `portage-3.0.64/lib/portage/tests/resolver/test_use_dep_defaults.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_useflags.py` & `portage-3.0.64/lib/portage/tests/resolver/test_useflags.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_virtual_minimize_children.py` & `portage-3.0.64/lib/portage/tests/resolver/test_virtual_minimize_children.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_virtual_slot.py` & `portage-3.0.64/lib/portage/tests/resolver/test_virtual_slot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/resolver/test_with_test_deps.py` & `portage-3.0.64/lib/portage/tests/resolver/test_with_test_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/sets/base/test_internal_package_set.py` & `portage-3.0.64/lib/portage/tests/sets/base/test_internal_package_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/sets/base/test_variable_set.py` & `portage-3.0.64/lib/portage/tests/sets/base/test_variable_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-# Copyright 2022 Gentoo Authors
+# Copyright 2022-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 from portage.tests import TestCase
 from portage.tests.resolver.ResolverPlayground import (
     ResolverPlayground,
     ResolverPlaygroundTestCase,
 )
 
 
 class VariableSetTestCase(TestCase):
     def testVariableSetEmerge(self):
+
+        # Using local set definition because @golang-rebuild migrated to dev-lang/go since bug 919751.
+        golang_rebuild = "{class=portage.sets.dbapi.VariableSet,variable=BDEPEND,includes=dev-lang/go}"
+
         ebuilds = {
             "dev-go/go-pkg-1": {"BDEPEND": "dev-lang/go"},
             "www-client/firefox-1": {
                 "BDEPEND": "|| ( virtual/rust:0/a virtual/rust:0/b )"
             },
         }
         installed = ebuilds
         playground = ResolverPlayground(ebuilds=ebuilds, installed=installed)
 
         test_cases = (
             ResolverPlaygroundTestCase(
-                ["@golang-rebuild"],
+                [f"@golang-rebuild{golang_rebuild}"],
                 mergelist=["dev-go/go-pkg-1"],
                 success=True,
             ),
             ResolverPlaygroundTestCase(
                 ["@rust-rebuild"],
                 mergelist=["www-client/firefox-1"],
                 success=True,
```

### Comparing `portage-3.0.63/lib/portage/tests/sets/files/test_config_file_set.py` & `portage-3.0.64/lib/portage/tests/sets/files/test_config_file_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/sets/files/test_static_file_set.py` & `portage-3.0.64/lib/portage/tests/sets/files/test_static_file_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/sets/shell/test_shell.py` & `portage-3.0.64/lib/portage/tests/sets/shell/test_shell.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/sync/test_sync_local.py` & `portage-3.0.64/lib/portage/tests/sync/test_sync_local.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/unicode/test_string_format.py` & `portage-3.0.64/lib/portage/tests/unicode/test_string_format.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/update/test_move_ent.py` & `portage-3.0.64/lib/portage/tests/update/test_move_ent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/update/test_move_slot_ent.py` & `portage-3.0.64/lib/portage/tests/update/test_move_slot_ent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/update/test_update_dbentry.py` & `portage-3.0.64/lib/portage/tests/update/test_update_dbentry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/dyn_libs/test_installed_dynlibs.py` & `portage-3.0.64/lib/portage/tests/util/dyn_libs/test_installed_dynlibs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/dyn_libs/test_soname_deps.py` & `portage-3.0.64/lib/portage/tests/util/dyn_libs/test_soname_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/eventloop/test_call_soon_fifo.py` & `portage-3.0.64/lib/portage/tests/util/eventloop/test_call_soon_fifo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/file_copy/test_copyfile.py` & `portage-3.0.64/lib/portage/tests/util/file_copy/test_copyfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright 2017, 2023 Gentoo Foundation
 # Distributed under the terms of the GNU General Public License v2
 
 import shutil
 import tempfile
+from unittest.mock import patch
 
 import pytest
 
 from portage import os
 from portage.tests import TestCase
 from portage.checksum import perform_md5
-from portage.util.file_copy import copyfile
+from portage.util.file_copy import copyfile, _fastcopy
 
 
 class CopyFileTestCase(TestCase):
     def testCopyFile(self):
         tempdir = tempfile.mkdtemp()
         try:
             src_path = os.path.join(tempdir, "src")
@@ -38,29 +39,41 @@
             dest_path = os.path.join(tempdir, "dest")
             content = b"foo"
 
             # Use seek to create some sparse blocks. Don't make these
             # files too big, in case the filesystem doesn't support
             # sparse files.
             with open(src_path, "wb") as f:
+                f.seek(2**16, os.SEEK_SET)
                 f.write(content)
-                f.seek(2**17, 1)
-                f.write(content)
-                f.seek(2**18, 1)
+                f.seek(2**17, os.SEEK_SET)
                 f.write(content)
                 # Test that sparse blocks are handled correctly at
-                # the end of the file (involves seek and truncate).
-                f.seek(2**17, 1)
+                # the end of the file.
+                f.truncate(2**18)
 
-            copyfile(src_path, dest_path)
+            fastcopy_success = False
+
+            def mock_fastcopy(src, dst):
+                nonlocal fastcopy_success
+                _fastcopy(src, dst)
+                fastcopy_success = True
+
+            with patch("portage.util.file_copy._fastcopy", new=mock_fastcopy):
+                copyfile(src_path, dest_path)
 
             self.assertEqual(perform_md5(src_path), perform_md5(dest_path))
 
-            # This last part of the test is expected to fail when sparse
-            # copy is not implemented, so mark it xfail:
-            pytest.xfail(reason="sparse copy is not implemented")
+            src_stat = os.stat(src_path)
+            dest_stat = os.stat(dest_path)
+
+            self.assertEqual(src_stat.st_size, dest_stat.st_size)
 
             # If sparse blocks were preserved, then both files should
             # consume the same number of blocks.
-            self.assertEqual(os.stat(src_path).st_blocks, os.stat(dest_path).st_blocks)
+            # This is expected to fail when sparse copy is not implemented.
+            if src_stat.st_blocks != dest_stat.st_blocks:
+                if fastcopy_success:
+                    pytest.fail(reason="sparse copy failed with _fastcopy")
+                pytest.xfail(reason="sparse copy is not implemented")
         finally:
             shutil.rmtree(tempdir)
```

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py` & `portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py` & `portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py` & `portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py` & `portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py` & `portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py` & `portage-3.0.64/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/test_compat_coroutine.py` & `portage-3.0.64/lib/portage/util/futures/retry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,210 +1,227 @@
-# Copyright 2018 Gentoo Foundation
+# Copyright 2018-2021 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
-from portage.util.futures import asyncio
-from portage.util.futures.compat_coroutine import (
-    coroutine,
-    coroutine_return,
+__all__ = (
+    "RetryError",
+    "retry",
 )
-from portage.util.futures._sync_decorator import _sync_decorator, _sync_methods
-from portage.tests import TestCase
 
+import functools
+
+from portage.exception import PortageException
+from portage.util.futures import asyncio
+
+
+class RetryError(PortageException):
+    """Raised when retry fails."""
+
+    def __init__(self):
+        PortageException.__init__(self, "retry error")
+
+
+def retry(
+    try_max=None,
+    try_timeout=None,
+    overall_timeout=None,
+    delay_func=None,
+    reraise=False,
+    loop=None,
+):
+    """
+    Create and return a retry decorator. The decorator is intended to
+    operate only on a coroutine function.
+
+    @param try_max: maximum number of tries
+    @type try_max: int or None
+    @param try_timeout: number of seconds to wait for a try to succeed
+            before cancelling it, which is only effective if func returns
+            tasks that support cancellation
+    @type try_timeout: float or None
+    @param overall_timeout: number of seconds to wait for retires to
+            succeed before aborting, which is only effective if func returns
+            tasks that support cancellation
+    @type overall_timeout: float or None
+    @param delay_func: function that takes an int argument corresponding
+            to the number of previous tries and returns a number of seconds
+            to wait before the next try
+    @type delay_func: callable
+    @param reraise: Reraise the last exception, instead of RetryError
+    @type reraise: bool
+    @param loop: event loop
+    @type loop: EventLoop
+    @return: func decorated with retry support
+    @rtype: callable
+    """
+    return functools.partial(
+        _retry_wrapper, loop, try_max, try_timeout, overall_timeout, delay_func, reraise
+    )
+
+
+def _retry_wrapper(
+    _loop, try_max, try_timeout, overall_timeout, delay_func, reraise, func, loop=None
+):
+    """
+    Create and return a decorated function.
+    """
+    return functools.partial(
+        _retry,
+        loop or _loop,
+        try_max,
+        try_timeout,
+        overall_timeout,
+        delay_func,
+        reraise,
+        func,
+    )
+
+
+def _retry(
+    loop,
+    try_max,
+    try_timeout,
+    overall_timeout,
+    delay_func,
+    reraise,
+    func,
+    *args,
+    **kwargs,
+):
+    """
+    Retry coroutine, used to implement retry decorator.
+
+    @return: func return value
+    @rtype: asyncio.Future (or compatible)
+    """
+    loop = asyncio._wrap_loop(loop)
+    future = loop.create_future()
+    _Retry(
+        future,
+        loop,
+        try_max,
+        try_timeout,
+        overall_timeout,
+        delay_func,
+        reraise,
+        functools.partial(func, *args, **kwargs),
+    )
+    return future
+
+
+class _Retry:
+    def __init__(
+        self,
+        future,
+        loop,
+        try_max,
+        try_timeout,
+        overall_timeout,
+        delay_func,
+        reraise,
+        func,
+    ):
+        self._future = future
+        self._loop = loop
+        self._try_max = try_max
+        self._try_timeout = try_timeout
+        self._delay_func = delay_func
+        self._reraise = reraise
+        self._func = func
+
+        self._try_timeout_handle = None
+        self._overall_timeout_handle = None
+        self._overall_timeout_expired = None
+        self._tries = 0
+        self._current_task = None
+        self._previous_result = None
+
+        future.add_done_callback(self._cancel_callback)
+        if overall_timeout is not None:
+            self._overall_timeout_handle = loop.call_later(
+                overall_timeout, self._overall_timeout_callback
+            )
+        self._begin_try()
+
+    def _cancel_callback(self, future):
+        if future.cancelled() and self._current_task is not None:
+            self._current_task.cancel()
+
+    def _try_timeout_callback(self):
+        self._try_timeout_handle = None
+        self._current_task.cancel()
+
+    def _overall_timeout_callback(self):
+        self._overall_timeout_handle = None
+        self._overall_timeout_expired = True
+        self._current_task.cancel()
+        self._retry_error()
+
+    def _begin_try(self):
+        self._tries += 1
+        self._current_task = asyncio.ensure_future(self._func(), loop=self._loop)
+        self._current_task.add_done_callback(self._try_done)
+        if self._try_timeout is not None:
+            self._try_timeout_handle = self._loop.call_later(
+                self._try_timeout, self._try_timeout_callback
+            )
+
+    def _try_done(self, future):
+        self._current_task = None
+
+        if self._try_timeout_handle is not None:
+            self._try_timeout_handle.cancel()
+            self._try_timeout_handle = None
+
+        if not future.cancelled():
+            # consume exception, so that the event loop
+            # exception handler does not report it
+            future.exception()
+
+        if self._overall_timeout_expired:
+            return
+
+        try:
+            if self._future.cancelled():
+                return
+
+            self._previous_result = future
+            if not (future.cancelled() or future.exception() is not None):
+                # success
+                self._future.set_result(future.result())
+                return
+        finally:
+            if self._future.done() and self._overall_timeout_handle is not None:
+                self._overall_timeout_handle.cancel()
+                self._overall_timeout_handle = None
+
+        if self._try_max is not None and self._tries >= self._try_max:
+            self._retry_error()
+            return
+
+        if self._delay_func is not None:
+            delay = self._delay_func(self._tries)
+            self._current_task = self._loop.call_later(delay, self._delay_done)
+            return
+
+        self._begin_try()
+
+    def _delay_done(self):
+        self._current_task = None
+
+        if self._future.cancelled() or self._overall_timeout_expired:
+            return
+
+        self._begin_try()
+
+    def _retry_error(self):
+        if self._previous_result is None or self._previous_result.cancelled():
+            cause = asyncio.TimeoutError()
+        else:
+            cause = self._previous_result.exception()
+
+        if self._reraise:
+            e = cause
+        else:
+            e = RetryError()
+            e.__cause__ = cause
 
-class CompatCoroutineTestCase(TestCase):
-    def test_returning_coroutine(self):
-        @coroutine
-        def returning_coroutine(loop=None):
-            yield asyncio.sleep(0, loop=loop)
-            coroutine_return("success")
-
-        loop = asyncio.get_event_loop()
-        self.assertEqual(
-            "success",
-            asyncio.get_event_loop().run_until_complete(returning_coroutine(loop=loop)),
-        )
-
-    def test_raising_coroutine(self):
-        class TestException(Exception):
-            pass
-
-        @coroutine
-        def raising_coroutine(loop=None):
-            yield asyncio.sleep(0, loop=loop)
-            raise TestException("exception")
-
-        loop = asyncio.get_event_loop()
-        self.assertRaises(
-            TestException, loop.run_until_complete, raising_coroutine(loop=loop)
-        )
-
-    def test_catching_coroutine(self):
-        class TestException(Exception):
-            pass
-
-        @coroutine
-        def catching_coroutine(loop=None):
-            loop = asyncio._wrap_loop(loop)
-            future = loop.create_future()
-            loop.call_soon(future.set_exception, TestException("exception"))
-            try:
-                yield future
-            except TestException:
-                self.assertTrue(True)
-            else:
-                self.assertTrue(False)
-            coroutine_return("success")
-
-        loop = asyncio.get_event_loop()
-        self.assertEqual(
-            "success", loop.run_until_complete(catching_coroutine(loop=loop))
-        )
-
-    def test_cancelled_coroutine(self):
-        """
-        Verify that a coroutine can handle (and reraise) asyncio.CancelledError
-        in order to perform any necessary cleanup. Note that the
-        asyncio.CancelledError will only be thrown in the coroutine if there's
-        an opportunity (yield) before the generator raises StopIteration.
-        """
-        loop = asyncio.get_event_loop()
-        ready_for_exception = loop.create_future()
-        exception_in_coroutine = loop.create_future()
-
-        @coroutine
-        def cancelled_coroutine(loop=None):
-            loop = asyncio._wrap_loop(loop)
-            while True:
-                task = loop.create_future()
-                try:
-                    ready_for_exception.set_result(None)
-                    yield task
-                except BaseException as e:
-                    # Since python3.8, asyncio.CancelledError inherits
-                    # from BaseException.
-                    task.done() or task.cancel()
-                    exception_in_coroutine.set_exception(e)
-                    raise
-                else:
-                    exception_in_coroutine.set_result(None)
-
-        future = cancelled_coroutine(loop=loop)
-        loop.run_until_complete(ready_for_exception)
-        future.cancel()
-
-        self.assertRaises(asyncio.CancelledError, loop.run_until_complete, future)
-
-        self.assertRaises(
-            asyncio.CancelledError, loop.run_until_complete, exception_in_coroutine
-        )
-
-    def test_cancelled_future(self):
-        """
-        When a coroutine raises CancelledError, the coroutine's
-        future is cancelled.
-        """
-
-        @coroutine
-        def cancelled_future_coroutine(loop=None):
-            loop = asyncio._wrap_loop(loop)
-            while True:
-                future = loop.create_future()
-                loop.call_soon(future.cancel)
-                yield future
-
-        loop = asyncio.get_event_loop()
-        future = loop.run_until_complete(
-            asyncio.wait([cancelled_future_coroutine(loop=loop)], loop=loop)
-        )[0].pop()
-        self.assertTrue(future.cancelled())
-
-    def test_yield_expression_result(self):
-        @coroutine
-        def yield_expression_coroutine(loop=None):
-            for i in range(3):
-                x = yield asyncio.sleep(0, result=i, loop=loop)
-                self.assertEqual(x, i)
-
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(yield_expression_coroutine(loop=loop))
-
-    def test_method_coroutine(self):
-        class Cubby:
-            _empty = object()
-
-            def __init__(self, loop):
-                self._loop = loop
-                self._value = self._empty
-                self._waiters = []
-
-            def _notify(self):
-                waiters = self._waiters
-                self._waiters = []
-                for waiter in waiters:
-                    waiter.cancelled() or waiter.set_result(None)
-
-            def _wait(self):
-                waiter = self._loop.create_future()
-                self._waiters.append(waiter)
-                return waiter
-
-            @coroutine
-            def read(self, loop=None):
-                while self._value is self._empty:
-                    yield self._wait()
-
-                value = self._value
-                self._value = self._empty
-                self._notify()
-                coroutine_return(value)
-
-            @coroutine
-            def write(self, value, loop=None):
-                while self._value is not self._empty:
-                    yield self._wait()
-
-                self._value = value
-                self._notify()
-
-        @coroutine
-        def writer_coroutine(cubby, values, sentinel, loop=None):
-            for value in values:
-                yield cubby.write(value, loop=loop)
-            yield cubby.write(sentinel, loop=loop)
-
-        @coroutine
-        def reader_coroutine(cubby, sentinel, loop=None):
-            results = []
-            while True:
-                result = yield cubby.read(loop=loop)
-                if result == sentinel:
-                    break
-                results.append(result)
-            coroutine_return(results)
-
-        loop = asyncio.get_event_loop()
-        cubby = Cubby(loop)
-        values = list(range(3))
-        writer = asyncio.ensure_future(
-            writer_coroutine(cubby, values, None, loop=loop), loop=loop
-        )
-        reader = asyncio.ensure_future(
-            reader_coroutine(cubby, None, loop=loop), loop=loop
-        )
-        loop.run_until_complete(asyncio.wait([writer, reader], loop=loop))
-
-        self.assertEqual(reader.result(), values)
-
-        # Test decoration of coroutine methods and functions for
-        # synchronous usage, allowing coroutines to smoothly
-        # blend with synchronous code.
-        sync_cubby = _sync_methods(cubby, loop=loop)
-        sync_reader = _sync_decorator(reader_coroutine, loop=loop)
-        writer = asyncio.ensure_future(
-            writer_coroutine(cubby, values, None, loop=loop), loop=loop
-        )
-        self.assertEqual(sync_reader(cubby, None), values)
-        self.assertTrue(writer.done())
-
-        for i in range(3):
-            sync_cubby.write(i)
-            self.assertEqual(sync_cubby.read(), i)
+        self._future.set_exception(e)
```

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/test_done_callback.py` & `portage-3.0.64/lib/portage/tests/util/futures/test_done_callback.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/test_done_callback_after_exit.py` & `portage-3.0.64/lib/portage/tests/util/futures/test_done_callback_after_exit.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/test_iter_completed.py` & `portage-3.0.64/lib/portage/tests/util/futures/test_iter_completed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/futures/test_retry.py` & `portage-3.0.64/lib/portage/tests/util/futures/test_retry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/meson.build` & `portage-3.0.64/lib/portage/tests/util/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_checksum.py` & `portage-3.0.64/lib/portage/tests/util/test_checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_digraph.py` & `portage-3.0.64/lib/portage/tests/util/test_digraph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_file_copier.py` & `portage-3.0.64/lib/portage/tests/util/test_file_copier.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_getconfig.py` & `portage-3.0.64/lib/portage/tests/util/test_getconfig.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_install_mask.py` & `portage-3.0.64/lib/portage/tests/util/test_install_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_manifest.py` & `portage-3.0.64/lib/portage/tests/util/test_manifest.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_mtimedb.py` & `portage-3.0.64/lib/portage/tests/util/test_mtimedb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_shelve.py` & `portage-3.0.64/lib/portage/tests/util/test_shelve.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_socks5.py` & `portage-3.0.64/lib/portage/tests/util/test_socks5.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,18 +212,17 @@
                     server.server_port,
                     path,
                 )
 
                 self.assertEqual(result, content)
         finally:
             try:
-                # Also run_exitfuncs to test atexit hook cleanup.
-                await socks5.proxy.stop()
+                # Also run_coroutine_exitfuncs to test atexit hook cleanup.
                 self.assertNotEqual(portage.process._exithandlers, [])
-                portage.process.run_exitfuncs()
+                await portage.process.run_coroutine_exitfuncs()
                 self.assertEqual(portage.process._exithandlers, [])
             finally:
                 portage.process._exithandlers = previous_exithandlers
                 shutil.rmtree(tempdir)
 
 
 class Socks5ServerLoopCloseTestCase(TestCase):
```

### Comparing `portage-3.0.63/lib/portage/tests/util/test_stackDictList.py` & `portage-3.0.64/lib/portage/tests/util/test_stackDictList.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_stackDicts.py` & `portage-3.0.64/lib/portage/tests/util/test_stackDicts.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_stackLists.py` & `portage-3.0.64/lib/portage/tests/util/test_stackLists.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_uniqueArray.py` & `portage-3.0.64/lib/portage/tests/util/test_uniqueArray.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_varExpand.py` & `portage-3.0.64/lib/portage/tests/util/test_varExpand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_whirlpool.py` & `portage-3.0.64/lib/portage/tests/util/test_whirlpool.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/util/test_xattr.py` & `portage-3.0.64/lib/portage/tests/util/test_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/versions/test_cpv_sort_key.py` & `portage-3.0.64/lib/portage/tests/versions/test_cpv_sort_key.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/tests/versions/test_vercmp.py` & `portage-3.0.64/lib/portage/tests/versions/test_vercmp.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/update.py` & `portage-3.0.64/lib/portage/update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/ExtractKernelVersion.py` & `portage-3.0.64/lib/portage/util/ExtractKernelVersion.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/SlotObject.py` & `portage-3.0.64/lib/portage/util/SlotObject.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/__init__.py` & `portage-3.0.64/lib/portage/util/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/AsyncFunction.py` & `portage-3.0.64/lib/portage/util/_async/AsyncFunction.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/AsyncScheduler.py` & `portage-3.0.64/lib/portage/util/_async/AsyncScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/AsyncTaskFuture.py` & `portage-3.0.64/lib/portage/util/_async/AsyncTaskFuture.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/BuildLogger.py` & `portage-3.0.64/lib/portage/util/_async/BuildLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/FileCopier.py` & `portage-3.0.64/lib/portage/util/_async/FileCopier.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/FileDigester.py` & `portage-3.0.64/lib/portage/util/_async/FileDigester.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/ForkProcess.py` & `portage-3.0.64/lib/portage/util/_async/ForkProcess.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,19 +87,16 @@
                     if self.logfile:
                         raise NotImplementedError(
                             "logfile conflicts with create_pipe=False"
                         )
                     # When called via process.spawn, SpawnProcess
                     # will have created a pipe earlier, so it would be
                     # redundant to do it here (it could also trigger spawn
-                    # recursion via set_term_size as in bug 923750). Use
-                    # /dev/null for master_fd, triggering early return
-                    # of _main, followed by _async_waitpid.
-                    # TODO: Optimize away the need for master_fd here.
-                    master_fd = os.open(os.devnull, os.O_RDONLY)
+                    # recursion via set_term_size as in bug 923750).
+                    master_fd = None
                     slave_fd = None
 
                 self._files = self._files_dict(connection=connection, slave_fd=slave_fd)
 
                 # Create duplicate file descriptors in self._fd_pipes
                 # so that the caller is free to manage the lifecycle
                 # of the original fd_pipes.
```

### Comparing `portage-3.0.63/lib/portage/util/_async/PipeLogger.py` & `portage-3.0.64/lib/portage/util/_async/PipeLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/PipeReaderBlockingIO.py` & `portage-3.0.64/lib/portage/util/_async/PipeReaderBlockingIO.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/PopenProcess.py` & `portage-3.0.64/lib/portage/util/_async/PopenProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/SchedulerInterface.py` & `portage-3.0.64/lib/portage/util/_async/SchedulerInterface.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/TaskScheduler.py` & `portage-3.0.64/lib/portage/util/_async/TaskScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_async/run_main_scheduler.py` & `portage-3.0.64/lib/portage/util/_async/run_main_scheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_compare_files.py` & `portage-3.0.64/lib/portage/util/_compare_files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_ctypes.py` & `portage-3.0.64/lib/portage/util/_ctypes.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,7 +44,22 @@
     handle = _library_handles.get(name)
 
     if handle is None and ctypes is not None:
         handle = ctypes.CDLL(name, use_errno=True)
         _library_handles[name] = handle
 
     return handle
+
+
+def load_libc():
+    """
+    Loads the C standard library, returns a tuple with the CDLL handle and
+    the filename. Returns (None, None) if unavailable.
+    """
+    filename = find_library("c")
+    if filename is None:
+        # find_library fails for musl where there is no soname
+        filename = "libc.so"
+    try:
+        return (LoadLibrary(filename), filename)
+    except OSError:
+        return (None, None)
```

### Comparing `portage-3.0.63/lib/portage/util/_desktop_entry.py` & `portage-3.0.64/lib/portage/util/_desktop_entry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_dyn_libs/LinkageMapELF.py` & `portage-3.0.64/lib/portage/util/_dyn_libs/LinkageMapELF.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_dyn_libs/NeededEntry.py` & `portage-3.0.64/lib/portage/util/_dyn_libs/NeededEntry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py` & `portage-3.0.64/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_dyn_libs/display_preserved_libs.py` & `portage-3.0.64/lib/portage/util/_dyn_libs/display_preserved_libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_dyn_libs/dyn_libs.py` & `portage-3.0.64/lib/portage/util/_dyn_libs/dyn_libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_dyn_libs/soname_deps.py` & `portage-3.0.64/lib/portage/util/_dyn_libs/soname_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_dyn_libs/soname_deps_qa.py` & `portage-3.0.64/lib/portage/util/_dyn_libs/soname_deps_qa.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_eventloop/asyncio_event_loop.py` & `portage-3.0.64/lib/portage/util/_eventloop/asyncio_event_loop.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 try:
     from asyncio.unix_events import PidfdChildWatcher
 except ImportError:
     PidfdChildWatcher = None
 
 import portage
-from portage.util import socks5
 
 
 class AsyncioEventLoop(_AbstractEventLoop):
     """
     Implementation of asyncio.AbstractEventLoop which wraps asyncio's
     event loop and is minimally compatible with _PortageEventLoop.
     """
@@ -71,20 +70,15 @@
             self._closing = True
             if self._is_main:
                 self.run_until_complete(self._close_main())
             self._loop.close()
             self._closing = False
 
     async def _close_main(self):
-        # Even though this has an exit hook, invoke it here so that
-        # we can properly wait for it and avoid messages like this:
-        # [ERROR] Task was destroyed but it is pending!
-        if socks5.proxy.is_running():
-            await socks5.proxy.stop()
-
+        await portage.process.run_coroutine_exitfuncs()
         portage.process.run_exitfuncs()
 
     @staticmethod
     def _internal_caller_exception_handler(loop, context):
         """
         An exception handler which drops to a pdb shell if std* streams
         refer to a tty, and otherwise kills the process with SIGTERM.
```

### Comparing `portage-3.0.63/lib/portage/util/_get_vm_info.py` & `portage-3.0.64/lib/portage/util/_get_vm_info.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_info_files.py` & `portage-3.0.64/lib/portage/util/_info_files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_path.py` & `portage-3.0.64/lib/portage/util/_path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/_pty.py` & `portage-3.0.64/lib/portage/util/_pty.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# Copyright 2010-2011 Gentoo Foundation
+# Copyright 2010-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
+import asyncio
 import platform
 import pty
 import termios
+from typing import Optional, Union
 
 from portage import os
 from portage.output import get_term_size, set_term_size
 from portage.util import writemsg
 
 # Disable the use of openpty on Solaris as it seems Python's openpty
 # implementation doesn't play nice on Solaris with Portage's
@@ -15,25 +17,29 @@
 # Additional note for the future: on Interix, pipes do NOT work, so
 # _disable_openpty on Interix must *never* be True
 _disable_openpty = platform.system() in ("SunOS",)
 
 _fbsd_test_pty = platform.system() == "FreeBSD"
 
 
-def _create_pty_or_pipe(copy_term_size=None):
+def _create_pty_or_pipe(
+    copy_term_size: Optional[int] = None,
+) -> tuple[Union[asyncio.Future, bool], int, int]:
     """
     Try to create a pty and if then fails then create a normal
-    pipe instead.
+    pipe instead. If a Future is returned for pty_ready, then the
+    caller should wait for it (which comes from set_term_size
+    because it spawns stty).
 
     @param copy_term_size: If a tty file descriptor is given
             then the term size will be copied to the pty.
     @type copy_term_size: int
     @rtype: tuple
-    @return: A tuple of (is_pty, master_fd, slave_fd) where
-            is_pty is True if a pty was successfully allocated, and
+    @return: A tuple of (pty_ready, master_fd, slave_fd) where
+            pty_ready is asyncio.Future or True if a pty was successfully allocated, and
             False if a normal pipe was allocated.
     """
 
     got_pty = False
 
     global _disable_openpty, _fbsd_test_pty
 
@@ -65,12 +71,15 @@
     if got_pty:
         # Disable post-processing of output since otherwise weird
         # things like \n -> \r\n transformations may occur.
         mode = termios.tcgetattr(slave_fd)
         mode[1] &= ~termios.OPOST
         termios.tcsetattr(slave_fd, termios.TCSANOW, mode)
 
+    pty_ready = None
     if got_pty and copy_term_size is not None and os.isatty(copy_term_size):
         rows, columns = get_term_size()
-        set_term_size(rows, columns, slave_fd)
+        pty_ready = set_term_size(rows, columns, slave_fd)
 
-    return (got_pty, master_fd, slave_fd)
+    # The future only exists when got_pty is True, so we can
+    # return the future in lieu of got_pty when it exists.
+    return (got_pty if pty_ready is None else pty_ready, master_fd, slave_fd)
```

### Comparing `portage-3.0.63/lib/portage/util/_urlopen.py` & `portage-3.0.64/lib/portage/util/_urlopen.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
     @returns: bool, True if ssl certificate verification is enabled by
             default
     """
     return hasattr(__import__("ssl"), "_create_unverified_context")
 
 
-def urlopen(url, if_modified_since=None, headers={}, proxies=None):
+def urlopen(url, timeout=10, if_modified_since=None, headers={}, proxies=None):
     parse_result = urllib_parse.urlparse(url)
     if parse_result.scheme not in ("http", "https"):
-        return _urlopen(url)
+        return _urlopen(url, timeout=timeout)
 
     netloc = parse_result.netloc.rpartition("@")[-1]
     url = urllib_parse.urlunparse(
         (
             parse_result.scheme,
             netloc,
             parse_result.path,
@@ -55,15 +55,15 @@
         )
 
     handlers = [CompressedResponseProcessor(password_manager)]
     if proxies:
         handlers.append(urllib_request.ProxyHandler(proxies))
     opener = urllib_request.build_opener(*handlers)
 
-    hdl = opener.open(request)
+    hdl = opener.open(request, timeout=timeout)
     if hdl.headers.get("last-modified", ""):
         try:
             add_header = hdl.headers.add_header
         except AttributeError:
             # Python 2
             add_header = hdl.headers.addheader
         add_header("timestamp", _http_to_timestamp(hdl.headers.get("last-modified")))
```

### Comparing `portage-3.0.63/lib/portage/util/_xattr.py` & `portage-3.0.64/lib/portage/util/_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/backoff.py` & `portage-3.0.64/lib/portage/util/backoff.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/bin_entry_point.py` & `portage-3.0.64/lib/portage/util/bin_entry_point.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/changelog.py` & `portage-3.0.64/lib/portage/util/changelog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/compression_probe.py` & `portage-3.0.64/lib/portage/util/compression_probe.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/configparser.py` & `portage-3.0.64/lib/portage/util/configparser.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/cpuinfo.py` & `portage-3.0.64/lib/portage/util/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/digraph.py` & `portage-3.0.64/lib/portage/util/digraph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/elf/constants.py` & `portage-3.0.64/lib/portage/util/elf/constants.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/elf/header.py` & `portage-3.0.64/lib/portage/util/elf/header.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/endian/decode.py` & `portage-3.0.64/lib/portage/util/endian/decode.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/env_update.py` & `portage-3.0.64/lib/portage/util/env_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/formatter.py` & `portage-3.0.64/lib/portage/util/formatter.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/futures/_asyncio/__init__.py` & `portage-3.0.64/lib/portage/util/futures/_asyncio/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,28 @@
 from asyncio import (
     ALL_COMPLETED,
     CancelledError,
     FIRST_COMPLETED,
     FIRST_EXCEPTION,
     Future,
     InvalidStateError,
+    iscoroutinefunction,
     Lock as _Lock,
     shield,
     TimeoutError,
     wait_for,
 )
 
 import threading
 
 import portage
 
 portage.proxy.lazyimport.lazyimport(
     globals(),
     "portage.util.futures.unix_events:_PortageEventLoopPolicy",
-    "portage.util.futures:compat_coroutine@_compat_coroutine",
 )
 from portage.util._eventloop.asyncio_event_loop import (
     AsyncioEventLoop as _AsyncioEventLoop,
 )
 
 
 _lock = threading.Lock()
@@ -154,27 +154,14 @@
     """
     Wraps asyncio.wait() and omits the loop argument which is not
     supported since python 3.10.
     """
     return _real_asyncio.wait(futures, timeout=timeout, return_when=return_when)
 
 
-def iscoroutinefunction(func):
-    """
-    Return True if func is a decorated coroutine function,
-    supporting both asyncio.coroutine and compat_coroutine since
-    their behavior is identical for all practical purposes.
-    """
-    if _compat_coroutine._iscoroutinefunction(func):
-        return True
-    if _real_asyncio.iscoroutinefunction(func):
-        return True
-    return False
-
-
 class Lock(_Lock):
     """
     Inject loop parameter for python3.9 or less in order to avoid
     "got Future <Future pending> attached to a different loop" errors.
     """
 
     def __init__(self, **kwargs):
```

### Comparing `portage-3.0.63/lib/portage/util/futures/_asyncio/streams.py` & `portage-3.0.64/lib/portage/util/futures/_asyncio/streams.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/futures/_sync_decorator.py` & `portage-3.0.64/lib/portage/util/futures/_sync_decorator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/futures/compat_coroutine.py` & `portage-3.0.64/lib/portage/util/futures/executor/fork.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,142 +1,141 @@
-# Copyright 2018-2021 Gentoo Foundation
+# Copyright 2018-2024 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
-import functools
-
-import portage
-
-portage.proxy.lazyimport.lazyimport(
-    globals(),
-    "portage.util.futures:asyncio",
-)
-
-# A marker for iscoroutinefunction.
-_is_coroutine = object()
-
-
-def _iscoroutinefunction(func):
-    """
-    Return True if func is a decorated coroutine function
-    created with the coroutine decorator for this module.
-    """
-    return getattr(func, "_is_coroutine", None) is _is_coroutine
-
-
-def coroutine(generator_func):
-    """
-    A decorator for a generator function that behaves as coroutine function.
-    The generator should yield a Future instance in order to wait for it,
-    and the result becomes the result of the current yield-expression,
-    via the PEP 342 generator send() method.
-
-    The decorated function returns a Future which is done when the generator
-    is exhausted. The generator can return a value via the coroutine_return
-    function.
-
-    @param generator_func: A generator function that yields Futures, and
-            will receive the result of each Future as the result of the
-            corresponding yield-expression.
-    @type generator_func: function
-    @rtype: function
-    @return: A function which calls the given generator function and
-            returns a Future that is done when the generator is exhausted.
-    """
-
-    # Note that functools.partial does not work for decoration of
-    # methods, since it doesn't implement the descriptor protocol.
-    # This problem is solve by defining a wrapper function.
-    @functools.wraps(generator_func)
-    def wrapped(*args, **kwargs):
-        return _generator_future(generator_func, *args, **kwargs)
-
-    wrapped._is_coroutine = _is_coroutine
-    return wrapped
-
-
-def coroutine_return(result=None):
-    """
-    Terminate the current coroutine and set the result of the associated
-    Future.
-
-    @param result: of the current coroutine's Future
-    @type object
-    """
-    raise _CoroutineReturnValue(result)
-
-
-def _generator_future(generator_func, *args, **kwargs):
-    """
-    Call generator_func with the given arguments, and return a Future
-    that is done when the resulting generation is exhausted. If a
-    keyword argument named 'loop' is given, then it is used instead of
-    the default event loop.
-    """
-    loop = kwargs.get("loop")
-    loop = asyncio._wrap_loop(loop)
-    result = loop.create_future()
-    _GeneratorTask(generator_func(*args, **kwargs), result, loop=loop)
-    return result
+__all__ = ("ForkExecutor",)
 
+import collections
+import functools
+import os
+import traceback
 
-class _CoroutineReturnValue(Exception):
-    def __init__(self, result):
-        self.result = result
+from portage.util._async.AsyncFunction import AsyncFunction
+from portage.util.futures import asyncio
+from portage.util.cpuinfo import get_cpu_count
+
+
+class ForkExecutor:
+    """
+    An implementation of concurrent.futures.Executor that forks a
+    new process for each task, with support for cancellation of tasks.
+
+    This is entirely driven by an event loop.
+    """
+
+    def __init__(self, max_workers=None, loop=None):
+        self._max_workers = max_workers or get_cpu_count()
+        self._loop = asyncio._wrap_loop(loop)
+        self._submit_queue = collections.deque()
+        self._running_tasks = {}
+        self._shutdown = False
+        self._shutdown_future = self._loop.create_future()
+
+    def submit(self, fn, *args, **kwargs):
+        """Submits a callable to be executed with the given arguments.
+
+        Schedules the callable to be executed as fn(*args, **kwargs) and returns
+        a Future instance representing the execution of the callable.
+
+        Returns:
+                A Future representing the given call.
+        """
+        future = self._loop.create_future()
+        proc = AsyncFunction(
+            target=functools.partial(self._guarded_fn_call, fn, args, kwargs),
+            # Directly inherit stdio streams and run in the foreground with no log.
+            create_pipe=False,
+        )
+        self._submit_queue.append((future, proc))
+        self._schedule()
+        return future
+
+    def _schedule(self):
+        while (
+            not self._shutdown
+            and self._submit_queue
+            and (
+                self._max_workers is True
+                or len(self._running_tasks) < self._max_workers
+            )
+        ):
+            future, proc = self._submit_queue.popleft()
+            future.add_done_callback(functools.partial(self._cancel_cb, proc))
+            proc.addExitListener(functools.partial(self._proc_exit, future))
+            proc.scheduler = self._loop
+            proc.start()
+            self._running_tasks[id(proc)] = proc
+
+    def _cancel_cb(self, proc, future):
+        if future.cancelled():
+            # async, handle the rest in _proc_exit
+            proc.cancel()
 
+    @staticmethod
+    def _guarded_fn_call(fn, args, kwargs):
+        try:
+            result = fn(*args, **kwargs)
+            exception = None
+        except Exception as e:
+            result = None
+            exception = _ExceptionWithTraceback(e)
 
-class _GeneratorTask:
-    """
-    Asynchronously executes the generator to completion, waiting for
-    the result of each Future that it yields, and sending the result
-    to the generator.
-    """
+        return result, exception
 
-    def __init__(self, generator, result, loop):
-        self._generator = generator
-        self._result = result
-        self._current_task = None
-        self._loop = loop
-        result.add_done_callback(self._cancel_callback)
-        loop.call_soon(self._next)
-
-    def _cancel_callback(self, result):
-        if result.cancelled() and self._current_task is not None:
-            # The done callback for self._current_task invokes
-            # _next in either case here.
-            self._current_task.done() or self._current_task.cancel()
-
-    def _next(self, previous=None):
-        self._current_task = None
-        if self._result.cancelled():
-            if previous is not None:
-                # Consume exceptions, in order to avoid triggering
-                # the event loop's exception handler.
-                previous.cancelled() or previous.exception()
-
-            # This will throw asyncio.CancelledError in the coroutine if
-            # there's an opportunity (yield) before the generator raises
-            # StopIteration.
-            previous = self._result
-        try:
-            if previous is None:
-                future = next(self._generator)
-            elif previous.cancelled():
-                future = self._generator.throw(asyncio.CancelledError())
-            elif previous.exception() is None:
-                future = self._generator.send(previous.result())
+    def _proc_exit(self, future, proc):
+        if not future.cancelled():
+            if proc.returncode == os.EX_OK:
+                result, exception = proc.result
+                if exception is not None:
+                    future.set_exception(exception)
+                else:
+                    future.set_result(result)
             else:
-                future = self._generator.throw(previous.exception())
-
-        except asyncio.CancelledError:
-            self._result.cancel()
-        except _CoroutineReturnValue as e:
-            if not self._result.cancelled():
-                self._result.set_result(e.result)
-        except StopIteration:
-            if not self._result.cancelled():
-                self._result.set_result(None)
-        except Exception as e:
-            if not self._result.cancelled():
-                self._result.set_exception(e)
-        else:
-            self._current_task = asyncio.ensure_future(future, loop=self._loop)
-            self._current_task.add_done_callback(self._next)
+                # TODO: add special exception class for this, maybe
+                # distinguish between kill and crash
+                future.set_exception(
+                    Exception(
+                        f"pid {proc.pid} crashed or killed, exitcode {proc.returncode}"
+                    )
+                )
+
+        del self._running_tasks[id(proc)]
+        self._schedule()
+        if self._shutdown and not self._running_tasks:
+            self._shutdown_future.set_result(None)
+
+    def shutdown(self, wait=True):
+        self._shutdown = True
+        if not self._running_tasks and not self._shutdown_future.done():
+            self._shutdown_future.set_result(None)
+        if wait:
+            self._loop.run_until_complete(self._shutdown_future)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.shutdown(wait=True)
+        return False
+
+
+class _ExceptionWithTraceback:
+    def __init__(self, exc):
+        tb = traceback.format_exception(type(exc), exc, exc.__traceback__)
+        tb = "".join(tb)
+        self.exc = exc
+        self.tb = f'\n"""\n{tb}"""'
+
+    def __reduce__(self):
+        return _rebuild_exc, (self.exc, self.tb)
+
+
+class _RemoteTraceback(Exception):
+    def __init__(self, tb):
+        self.tb = tb
+
+    def __str__(self):
+        return self.tb
+
+
+def _rebuild_exc(exc, tb):
+    exc.__cause__ = _RemoteTraceback(tb)
+    return exc
```

### Comparing `portage-3.0.63/lib/portage/util/futures/extendedfutures.py` & `portage-3.0.64/lib/portage/util/futures/extendedfutures.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/futures/futures.py` & `portage-3.0.64/lib/portage/util/futures/futures.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/futures/iter_completed.py` & `portage-3.0.64/lib/portage/util/futures/iter_completed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/futures/unix_events.py` & `portage-3.0.64/lib/portage/util/futures/unix_events.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/hooks.py` & `portage-3.0.64/lib/portage/util/hooks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/install_mask.py` & `portage-3.0.64/lib/portage/util/install_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/iterators/MultiIterGroupBy.py` & `portage-3.0.64/lib/portage/util/iterators/MultiIterGroupBy.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/lafilefixer.py` & `portage-3.0.64/lib/portage/util/lafilefixer.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/listdir.py` & `portage-3.0.64/lib/portage/util/listdir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/locale.py` & `portage-3.0.64/lib/portage/util/locale.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import multiprocessing
 import sys
 import textwrap
 import traceback
 
 import portage
 from portage.util import _unicode_decode, writemsg_level
-from portage.util._ctypes import find_library, LoadLibrary
+from portage.util._ctypes import load_libc
 from portage.util.futures import asyncio
 
 
 locale_categories = (
     "LC_COLLATE",
     "LC_CTYPE",
     "LC_MONETARY",
@@ -39,23 +39,17 @@
 _check_locale_cache = {}
 
 
 def _check_locale(silent):
     """
     The inner locale check function.
     """
-    try:
-        from portage.util import libc
-    except ImportError:
-        libc_fn = find_library("c")
-        if libc_fn is None:
-            return None
-        libc = LoadLibrary(libc_fn)
-        if libc is None:
-            return None
+    (libc, _) = load_libc()
+    if libc is None:
+        return None
 
     lc = list(range(ord("a"), ord("z") + 1))
     uc = list(range(ord("A"), ord("Z") + 1))
     rlc = [libc.tolower(c) for c in uc]
     ruc = [libc.toupper(c) for c in lc]
 
     if lc != rlc or uc != ruc:
```

### Comparing `portage-3.0.63/lib/portage/util/meson.build` & `portage-3.0.64/lib/portage/util/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         'bin_entry_point.py',
         'changelog.py',
         'compression_probe.py',
         'configparser.py',
         'cpuinfo.py',
         'digraph.py',
         'env_update.py',
+        'file_copy.py',
         'formatter.py',
         'hooks.py',
         'install_mask.py',
         'lafilefixer.py',
         'listdir.py',
         'locale.py',
         'movefile.py',
@@ -37,13 +38,12 @@
     ],
     subdir : 'portage/util',
     pure : not native_extensions
 )
 
 subdir('elf')
 subdir('endian')
-subdir('file_copy')
 subdir('futures')
 subdir('iterators')
 subdir('_async')
 subdir('_dyn_libs')
 subdir('_eventloop')
```

### Comparing `portage-3.0.63/lib/portage/util/movefile.py` & `portage-3.0.64/lib/portage/util/movefile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/mtimedb.py` & `portage-3.0.64/lib/portage/util/mtimedb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/netlink.py` & `portage-3.0.64/lib/portage/util/netlink.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/path.py` & `portage-3.0.64/lib/portage/util/path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/shelve.py` & `portage-3.0.64/lib/portage/util/shelve.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/whirlpool.py` & `portage-3.0.64/lib/portage/util/whirlpool.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/util/writeable_check.py` & `portage-3.0.64/lib/portage/util/writeable_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,39 +43,40 @@
     invalids = []
 
     try:
         with open(
             "/proc/self/mountinfo",
             encoding=_encodings["content"],
             errors="replace",
+            newline="\n",
         ) as f:
             for line in f:
                 # we're interested in dir and both attr fields which always
                 # start with either 'ro' or 'rw'
                 # example line:
                 # 14 1 8:3 / / rw,noatime - ext3 /dev/root rw,errors=continue,commit=5,barrier=1,data=writeback
                 #       _dir ^ ^ attr1                     ^ attr2
                 # there can be a variable number of fields
                 # to the left of the ' - ', after the attr's, so split it there
                 mount = line.split(" - ", 1)
                 try:
-                    _dir, attr1 = mount[0].split()[4:6]
+                    _dir, attr1 = mount[0].split(" ")[4:6]
                 except ValueError:
                     # If it raises ValueError we can simply ignore the line.
                     invalids.append(line)
                     continue
                 # check for situation with invalid entries for /home and /root in /proc/self/mountinfo
                 # root path is missing sometimes on WSL
                 # for example: 16 1 0:16 / /root rw,noatime - lxfs  rw
                 if len(mount) > 1:
                     try:
-                        attr2 = mount[1].split()[2]
+                        attr2 = mount[1].split(" ")[2]
                     except IndexError:
                         try:
-                            attr2 = mount[1].split()[1]
+                            attr2 = mount[1].split(" ")[1]
                         except IndexError:
                             invalids.append(line)
                             continue
                 else:
                     invalids.append(line)
                     continue
                 if attr1.startswith("ro") or attr2.startswith("ro"):
```

### Comparing `portage-3.0.63/lib/portage/versions.py` & `portage-3.0.64/lib/portage/versions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/xml/metadata.py` & `portage-3.0.64/lib/portage/xml/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/lib/portage/xpak.py` & `portage-3.0.64/lib/portage/xpak.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/make.conf.example-repatch.sh` & `portage-3.0.64/make.conf.example-repatch.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/color.map.5` & `portage-3.0.64/man/color.map.5`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/dispatch-conf.1` & `portage-3.0.64/man/dispatch-conf.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/ebuild.1` & `portage-3.0.64/man/ebuild.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/ebuild.5` & `portage-3.0.64/man/ebuild.5`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/egencache.1` & `portage-3.0.64/man/egencache.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/emaint.1` & `portage-3.0.64/man/emaint.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/emerge.1` & `portage-3.0.64/man/emerge.1`

 * *Files 0% similar despite different names*

```diff
@@ -443,23 +443,25 @@
 unsatisfied dependency (default: \'20\').
 .TP
 .BR "\-\-binpkg\-changed\-deps [ y | n ]"
 Tells emerge to ignore binary packages for which the corresponding
 ebuild dependencies have changed since the packages were built.
 In order to help avoid issues with resolving inconsistent dependencies,
 this option is automatically enabled unless the \fB\-\-usepkgonly\fR
-option is enabled. Behavior with respect to changed build\-time
+(or \fB\-\-getbinpkgonly\fR) option is enabled.
+Behavior with respect to changed build\-time
 dependencies is controlled by the \fB\-\-with\-bdeps\fR option.
 .TP
 .BR "\-\-binpkg\-respect\-use [ y | n ]"
 Tells emerge to ignore binary packages if their USE flags
 don't match the current configuration. In order to help avoid issues
 with resolving inconsistent USE flag settings, this option is
-automatically enabled unless the \fB\-\-usepkgonly\fR option
-is enabled. If \fB\-\-binpkg\-respect\-use\fR is given explicitly,
+automatically enabled unless the \fB\-\-usepkgonly\fR
+(or \fB\-\-getbinpkgonly\fR) option is enabled.
+If \fB\-\-binpkg\-respect\-use\fR is given explicitly,
 then it implies \fB\-\-autounmask\-use=n\fR, because these options
 naturally oppose each other.
 .TP
 .BR "\-\-buildpkg [ y | n ]" ", " \-b
 Tells emerge to build binary packages for all ebuilds processed in
 addition to actually merging the packages.  Useful for maintainers
 or if you administrate multiple Gentoo Linux systems (build once,
```

### Comparing `portage-3.0.63/man/emirrordist.1` & `portage-3.0.64/man/emirrordist.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/env-update.1` & `portage-3.0.64/man/env-update.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/etc-update.1` & `portage-3.0.64/man/etc-update.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/glsa-check.1` & `portage-3.0.64/man/glsa-check.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/make.conf.5` & `portage-3.0.64/man/make.conf.5`

 * *Files 1% similar despite different names*

```diff
@@ -648,17 +648,20 @@
 .B parallel\-fetch
 Fetch in the background while compiling. Run
 `tail \-f /var/log/emerge\-fetch.log` in a
 terminal to view parallel-fetch progress.
 .TP
 .B parallel\-install
 Use finer\-grained locks when installing packages, allowing for greater
-parallelism. Note that \fIparallel\-install\fR currently has no effect
-unless \fImerge\-wait\fR is disabled. For additional parallelism,
-disable \fIebuild\-locks\fR.
+parallelism. For additional parallelism disable \fIebuild\-locks\fR.
+Also disable \fImerge\-wait\fR for additional parallelism if desired,
+but that increases the possibility of random build failures. When
+\fIparallel\-install\fR is used together with \fImerge\-wait\fR,
+parallel installation occurs in batches when there are no builds
+running.
 .TP
 .B pid\-sandbox
 Isolate the process space for the ebuild processes. This makes it
 possible to cleanly kill all processes spawned by the ebuild.
 Supported only on Linux. Requires PID and mount namespace support
 in kernel. /proc is remounted inside the mount namespace to account
 for new PID namespace.
```

### Comparing `portage-3.0.63/man/meson.build` & `portage-3.0.64/man/meson.build`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/portage.5` & `portage-3.0.64/man/portage.5`

 * *Files 0% similar despite different names*

```diff
@@ -1136,15 +1136,15 @@
 sync\-rcu\-spare\-snapshots configures the number of previous snapshots
 that are exempt). If the ttl is set too low, then a snapshot could
 expire while it is in use by a running process.
 .TP
 .B sync\-type
 Specifies type of synchronization performed by `emerge \-\-sync`.
 .br
-Valid non\-empty values: cvs, git, mercurial, rsync, svn, webrsync
+Valid non\-empty values: cvs, git, mercurial, rsync, zipfile, svn, webrsync
 (emerge\-webrsync)
 .br
 This attribute can be set to empty value to disable synchronization of given
 repository. Empty value is default.
 .TP
 .B sync\-umask
 Specifies umask used to synchronize the repository.
@@ -1161,14 +1161,16 @@
 .TP
 Syntax:
 cvs: [cvs://]:access_method:[username@]hostname[:port]:/path
 .br
 git: (git|git+ssh|http|https)://[username@]hostname[:port]/path
 .br
 rsync: (rsync|ssh)://[username@]hostname[:port]/(module|path)
+.br
+zipfile: (http|https)://hostname[:port]/path/to/zipfile.zip
 .TP
 Examples:
 .RS
 rsync://private\-mirror.com/portage\-module
 .br
 rsync://rsync\-user@private\-mirror.com:873/gentoo\-portage
 .br
@@ -1323,14 +1325,21 @@
 
 # Overlay 'voip' synchronized with layman's plug-in sync module
 [voip]
 location = /var/lib/layman/voip
 sync\-type = laymanator
 sync\-uri = git://anongit.gentoo.org/proj/voip.git
 auto\-sync = yes
+
+# Overlay with latest ebuild repository snapshot.
+[snapshot]
+location = /var/db/repos/snapshot
+sync\-type = zipfile
+sync\-uri = https://github.com/gentoo/gentoo/archive/refs/heads/master.zip
+auto\-sync = yes
 .fi
 .RE
 .TP
 .BR sets.conf
 A package set configuration file. Settings here override settings from
 \fB/var/db/repos/gentoo/sets.conf\fR and \fB/usr/share/portage/config/sets\fR.
 The format is described extensively in the
```

### Comparing `portage-3.0.63/man/quickpkg.1` & `portage-3.0.64/man/quickpkg.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/ru/color.map.5` & `portage-3.0.64/man/ru/color.map.5`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/ru/dispatch-conf.1` & `portage-3.0.64/man/ru/dispatch-conf.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/ru/ebuild.1` & `portage-3.0.64/man/ru/ebuild.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/ru/env-update.1` & `portage-3.0.64/man/ru/env-update.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/ru/etc-update.1` & `portage-3.0.64/man/ru/etc-update.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/ru/fixpackages.1` & `portage-3.0.64/man/ru/fixpackages.1`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/man/xpak.5` & `portage-3.0.64/man/xpak.5`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/meson.build` & `portage-3.0.64/meson.build`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 project(
     'portage',
     'c',
-    version : '3.0.63',
+    version : '3.0.64',
     license : 'GPL-2.0-or-later',
     meson_version : '>=0.58.0'
 )
 
 py_mod = import('python')
 # TODO: Add "pure : not native_extensions" here instead of py.install_sources()
 # when requiring Meson >=0.64.0.
@@ -93,14 +93,28 @@
 subdir('bin')
 subdir('lib')
 
 if native_extensions
     subdir('src')
 endif
 
+if system_wide
+	METADATA = configure_file(
+		input : 'cnf/METADATA',
+		output : 'METADATA',
+		configuration : conf_data
+	)
+	install_data(
+		[
+			METADATA
+		],
+		install_dir : py.get_install_dir() / 'portage-@0@.dist-info'.format(conf_data.get('VERSION'))
+	)
+endif
+
 test(
     'pytest',
     py,
     args : ['-m', 'pytest', '--rootdir', meson.current_source_dir(), meson.current_source_dir()],
     timeout : 0
 )
```

### Comparing `portage-3.0.63/meson_options.txt` & `portage-3.0.64/meson_options.txt`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/misc/emerge-delta-webrsync` & `portage-3.0.64/misc/emerge-delta-webrsync`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/pylintrc` & `portage-3.0.64/pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -478,8 +478,8 @@
 preferred-modules=
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "BaseException, Exception".
-overgeneral-exceptions=BaseException
+overgeneral-exceptions=builtins.BaseException
```

### Comparing `portage-3.0.63/pyproject.toml` & `portage-3.0.64/pyproject.toml`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/src/portage_util__whirlpool.c` & `portage-3.0.64/src/portage_util__whirlpool.c`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/testpath` & `portage-3.0.64/testpath`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/tox.ini` & `portage-3.0.64/tox.ini`

 * *Files identical despite different names*

### Comparing `portage-3.0.63/PKG-INFO` & `portage-3.0.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portage
-Version: 3.0.63
+Version: 3.0.64
 Summary: Portage is the package management and distribution system for Gentoo
 Author-Email: Gentoo Portage Development Team <dev-portage@gentoo.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

