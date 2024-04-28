# Comparing `tmp/cmap-0.1.3.tar.gz` & `tmp/cmap-0.2.0.tar.gz`

## Comparing `cmap-0.1.3.tar` & `cmap-0.2.0.tar`

### file list

```diff
@@ -1,197 +1,200 @@
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 cmap-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/__init__.py
--rw-r--r--   0        0        0    14615 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/_catalog.py
--rw-r--r--   0        0        0    20370 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/_color.py
--rw-r--r--   0        0        0    45787 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/_colormap.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/_external.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/_png.py
--rw-r--r--   0        0        0    16225 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/__init__.py
--rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/bids/__init__.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/bids/record.json
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/chrisluts/record.json
--rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cividis/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cividis/record.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmap/record.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/__init__.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/algae.py
--rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/amp.py
--rw-r--r--   0        0        0    22339 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/balance.py
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/curl.py
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/deep.py
--rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/delta.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/dense.py
--rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/diff.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/haline.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/ice.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/matter.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/oxy.py
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/phase.py
--rw-r--r--   0        0        0    17189 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/rain.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/record.json
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/solar.py
--rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/speed.py
--rw-r--r--   0        0        0    21589 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/tarn.py
--rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/tempo.py
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/thermal.py
--rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/topo.py
--rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cmocean/turbid.py
--rw-r--r--   0        0        0    39760 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorbrewer/__init__.py
--rw-r--r--   0        0        0    45183 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorbrewer/record.json
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C1.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C10.py
--rw-r--r--   0        0        0     9105 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C11.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C2.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C3.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C4.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C5.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C6.py
--rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C7.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C8.py
--rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_C9.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBC1.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBC2.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBD1.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBD2.py
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBL1.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBL2.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBL3.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBL4.py
--rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBTC1.py
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBTC2.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBTD1.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBTL1.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBTL2.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBTL3.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_CBTL4.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D1.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D10.py
--rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D11.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D12.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D13.py
--rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D1A.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D2.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D3.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D4.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D5.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D6.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D7.py
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D8.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_D9.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_I1.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_I2.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_I3.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L1.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L10.py
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L11.py
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L12.py
--rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L13.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L14.py
--rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L15.py
--rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L16.py
--rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L17.py
--rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L18.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L19.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L2.py
--rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L20.py
--rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L3.py
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L4.py
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L5.py
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L6.py
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L7.py
--rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L8.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_L9.py
--rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_R1.py
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_R2.py
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_R3.py
--rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/CET_R4.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/__init__.py
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/colorcet/record.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/__init__.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/acton.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/bam.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/bamO.py
--rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/bamako.py
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/batlow.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/batlowK.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/batlowW.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/berlin.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/bilbao.py
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/broc.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/brocO.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/buda.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/bukavu.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/cork.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/corkO.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/davos.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/devon.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/fes.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/grayC.py
--rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/hawaii.py
--rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/imola.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/lajolla.py
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/lapaz.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/lisbon.py
--rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/nuuk.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/oleron.py
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/oslo.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/record.json
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/roma.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/romaO.py
--rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/tofino.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/tokyo.py
--rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/turku.py
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/vanimo.py
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/vik.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/crameri/vikO.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cubehelix/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/cubehelix/record.json
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/glasbey/__init__.py
--rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/glasbey/_glasbey.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/glasbey/_grids.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/glasbey/_internals.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/glasbey/prebuilt.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/glasbey/record.json
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/gnuplot/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/gnuplot/record.json
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/google/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/google/record.json
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/imagej/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/imagej/record.json
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/matlab/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/matlab/record.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/matplotlib/_CMRmap.py
--rw-r--r--   0        0        0    45911 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/matplotlib/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/matplotlib/_coolwarm.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/matplotlib/_wistia.py
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/matplotlib/record.json
--rw-r--r--   0        0        0    64086 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/seaborn/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/seaborn/record.json
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/tableau/__init__.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/tableau/record.json
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/vispy/__init__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/vispy/record.json
--rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/yorick/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmap-0.1.3/src/cmap/data/yorick/record.json
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 cmap-0.1.3/tests/test_catalog.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 cmap-0.1.3/tests/test_color.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 cmap-0.1.3/tests/test_colormap.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cmap-0.1.3/tests/test_data.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 cmap-0.1.3/tests/test_glasbey.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 cmap-0.1.3/tests/test_model_fields.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 cmap-0.1.3/tests/test_third_party.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 cmap-0.1.3/tests/test_utils.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 cmap-0.1.3/.gitignore
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 cmap-0.1.3/README.md
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 cmap-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE_CMOCEAN
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE_COLORBREWER
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE_COLORCET
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE_CRAMERI
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE_CVIDIS
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE_GLASBEY
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE_WISTIA
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 cmap-0.1.3/LICENSE/LICENSE_YORICK
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 cmap-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/__init__.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_catalog.py
+-rw-r--r--   0        0        0    21048 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_color.py
+-rw-r--r--   0        0        0    54457 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_colormap.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_external.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_png.py
+-rw-r--r--   0        0        0    16225 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/__init__.py
+-rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/bids/__init__.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/bids/record.json
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/chrisluts/record.json
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cividis/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cividis/record.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmap/record.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/__init__.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/algae.py
+-rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/amp.py
+-rw-r--r--   0        0        0    22339 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/balance.py
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/curl.py
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/deep.py
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/delta.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/dense.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/diff.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/haline.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/ice.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/matter.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/oxy.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/phase.py
+-rw-r--r--   0        0        0    17189 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/rain.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/record.json
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/solar.py
+-rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/speed.py
+-rw-r--r--   0        0        0    21589 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/tarn.py
+-rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/tempo.py
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/thermal.py
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/topo.py
+-rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/turbid.py
+-rw-r--r--   0        0        0    39760 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorbrewer/__init__.py
+-rw-r--r--   0        0        0    45183 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorbrewer/record.json
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C1.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C10.py
+-rw-r--r--   0        0        0     9105 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C11.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C2.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C3.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C4.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C5.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C6.py
+-rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C7.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C8.py
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C9.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBC1.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBC2.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBD1.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBD2.py
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBL1.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBL2.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBL3.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBL4.py
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTC1.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTC2.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTD1.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL1.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL2.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL3.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL4.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D1.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D10.py
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D11.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D12.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D13.py
+-rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D1A.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D2.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D3.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D4.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D5.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D6.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D7.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D8.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D9.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_I1.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_I2.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_I3.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L1.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L10.py
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L11.py
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L12.py
+-rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L13.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L14.py
+-rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L15.py
+-rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L16.py
+-rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L17.py
+-rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L18.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L19.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L2.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L20.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L3.py
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L4.py
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L5.py
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L6.py
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L7.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L8.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L9.py
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_R1.py
+-rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_R2.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_R3.py
+-rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_R4.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/__init__.py
+-rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/record.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/__init__.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/acton.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bam.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bamO.py
+-rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bamako.py
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/batlow.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/batlowK.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/batlowW.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/berlin.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bilbao.py
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/broc.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/brocO.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/buda.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bukavu.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/cork.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/corkO.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/davos.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/devon.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/fes.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/grayC.py
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/hawaii.py
+-rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/imola.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/lajolla.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/lapaz.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/lisbon.py
+-rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/nuuk.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/oleron.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/oslo.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/record.json
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/roma.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/romaO.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/tofino.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/tokyo.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/turku.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/vanimo.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/vik.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/vikO.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cubehelix/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cubehelix/record.json
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/__init__.py
+-rw-r--r--   0        0        0     8584 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/_glasbey.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/_grids.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/_internals.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/prebuilt.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/record.json
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/gnuplot/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/gnuplot/record.json
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/google/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/google/record.json
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/imagej/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/imagej/record.json
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matlab/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matlab/record.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/_CMRmap.py
+-rw-r--r--   0        0        0    45911 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/_coolwarm.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/_wistia.py
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/record.json
+-rw-r--r--   0        0        0    64086 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/seaborn/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/seaborn/record.json
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/tableau/__init__.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/tableau/record.json
+-rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/tol/__init__.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/tol/record.json
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/vispy/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/vispy/record.json
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/yorick/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/yorick/record.json
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_catalog.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_color.py
+-rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_colormap.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_data.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_glasbey.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_model_fields.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_third_party.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 cmap-0.2.0/.gitignore
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 cmap-0.2.0/README.md
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 cmap-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_CMOCEAN
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_COLORBREWER
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_COLORCET
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_CRAMERI
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_CVIDIS
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_GLASBEY
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_TOL
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_WISTIA
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_YORICK
+-rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 cmap-0.2.0/PKG-INFO
```

### Comparing `cmap-0.1.3/CHANGELOG.md` & `cmap-0.2.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,52 @@
 # Changelog
 
+## [v0.2.0](https://github.com/tlambert03/cmap/tree/v0.2.0) (2024-04-28)
+
+[Full Changelog](https://github.com/tlambert03/cmap/compare/v0.2.0...v0.2.0)
+
+**Implemented enhancements:**
+
+- feat: add shifted method [\#52](https://github.com/tlambert03/cmap/pull/52) ([tlambert03](https://github.com/tlambert03))
+- feat: add over/under/bad colors [\#50](https://github.com/tlambert03/cmap/pull/50) ([tlambert03](https://github.com/tlambert03))
+- feat: add Paul Tol's colormaps [\#48](https://github.com/tlambert03/cmap/pull/48) ([Jhsmit](https://github.com/Jhsmit))
+
+**Fixed bugs:**
+
+- fix: fix interpolation argument preservation in custom colormaps [\#47](https://github.com/tlambert03/cmap/pull/47) ([tlambert03](https://github.com/tlambert03))
+
+**Documentation:**
+
+- docs: use natsort for docs [\#51](https://github.com/tlambert03/cmap/pull/51) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- ci\(dependabot\): bump softprops/action-gh-release from 1 to 2 [\#42](https://github.com/tlambert03/cmap/pull/42) ([dependabot[bot]](https://github.com/apps/dependabot))
+- chore: use ruff instead of black [\#41](https://github.com/tlambert03/cmap/pull/41) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.2.0](https://github.com/tlambert03/cmap/tree/v0.2.0) (2024-03-09)
+
+[Full Changelog](https://github.com/tlambert03/cmap/compare/v0.1.3...v0.2.0)
+
+**Implemented enhancements:**
+
+- feat: add support for pyqtgraph [\#32](https://github.com/tlambert03/cmap/pull/32) ([tlambert03](https://github.com/tlambert03))
+
+**Fixed bugs:**
+
+- fix: misc fixes for pydantic deprecations and other breakages [\#38](https://github.com/tlambert03/cmap/pull/38) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- test: Add test\_min extra and make sure tests run with bare minimum [\#40](https://github.com/tlambert03/cmap/pull/40) ([tlambert03](https://github.com/tlambert03))
+- ci\(dependabot\): bump aganders3/headless-gui from 2.1 to 2.2 [\#37](https://github.com/tlambert03/cmap/pull/37) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(dependabot\): bump codecov/codecov-action from 3 to 4 [\#36](https://github.com/tlambert03/cmap/pull/36) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(dependabot\): bump actions/setup-python from 4 to 5 [\#34](https://github.com/tlambert03/cmap/pull/34) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(dependabot\): bump aganders3/headless-gui from 1.2 to 2.1 [\#33](https://github.com/tlambert03/cmap/pull/33) ([dependabot[bot]](https://github.com/apps/dependabot))
+
 ## [v0.1.3](https://github.com/tlambert03/cmap/tree/v0.1.3) (2023-12-04)
 
 [Full Changelog](https://github.com/tlambert03/cmap/compare/v0.1.2...v0.1.3)
 
 **Fixed bugs:**
 
 - update to\_pygfx [\#31](https://github.com/tlambert03/cmap/pull/31) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `cmap-0.1.3/src/cmap/__init__.py` & `cmap-0.2.0/src/cmap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Scientific colormaps for python, without dependencies."""
+
 from importlib.metadata import PackageNotFoundError, version
 from typing import TYPE_CHECKING, Iterator, Mapping
 
 try:
     __version__ = version("cmap")
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "uninstalled"
```

### Comparing `cmap-0.1.3/src/cmap/_catalog.py` & `cmap-0.2.0/src/cmap/_catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Catalog of available colormaps.
 
 This module contains the logic that indexes all of the "record.json" files found
 in the data directory.
 
 TODO: this needs to be cleaned up, and documented better.
 """
+
 from __future__ import annotations
 
 import json
 import logging
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import (
@@ -37,14 +38,17 @@
     class UnloadedCatalogItem(TypedDict):
         data: str
         category: Category
         tags: NotRequired[list[str]]
         interpolation: NotRequired[bool]
         info: NotRequired[str]
         aliases: NotRequired[list[str]]
+        over: NotRequired[str]
+        under: NotRequired[str]
+        bad: NotRequired[str]
 
     class UnloadedCatalogAlias(TypedDict):
         alias: str
         conflicts: NotRequired[list[str]]
 
     CatalogDict: TypeAlias = dict[str, UnloadedCatalogItem | UnloadedCatalogAlias]
 
@@ -100,27 +104,36 @@
         A list of tags for the colormap. These are displayed in the documentation.
     aliases: list[str]
         A list of aliases for the colormap. These are alternative names that can be
         used to access the colormap. Currently, they must be accessed using the
         fully qualified name (`namespace:alias`).
     qualified_name: str
         The fully qualified name of the colormap, e.g. "matplotlib:viridis".
+    under: str | None
+        The color to use for under-range values.
+    over: str | None
+        The color to use for over-range values.
+    bad: str | None
+        The color to use for bad values.
     """
 
     data: ColorStopsLike
     name: str
     category: Category
     license: str = "UNKNOWN"
     source: str = ""
     info: str = ""
     namespace: str = ""
     authors: list[str] = field(default_factory=list)
     interpolation: bool | Interpolation = "linear"
     tags: list[str] = field(default_factory=list)
     aliases: list[str] = field(default_factory=list)
+    under: str | None = None
+    over: str | None = None
+    bad: str | None = None
 
     @property
     def qualified_name(self) -> str:
         return f"{self.namespace}{NAMESPACE_DELIMITER}{self.name}"
 
 
 def _build_catalog(records: Iterable[FileDescriptorOrPath]) -> CatalogDict:
```

### Comparing `cmap-0.1.3/src/cmap/_color.py` & `cmap-0.2.0/src/cmap/_color.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,28 @@
     SupportsFloat,
     cast,
     overload,
 )
 
 import numpy as np
 
+try:
+    from pydantic import model_serializer
+except ImportError:
+    model_serializer = lambda x: x  # noqa: E731
+
 from . import _external
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
     from typing import Union
 
     import numpy.typing as npt
+    from pydantic import GetCoreSchemaHandler
+    from pydantic_core import CoreSchema
     from typing_extensions import TypeAlias
 
     # not used internally... but available for typing
     RGBTuple: TypeAlias = "tuple[int, int, int] | tuple[float, float, float]"
     RGBATuple: TypeAlias = (
         "tuple[int, int, int, float] | tuple[float, float, float, float]"
     )
@@ -333,18 +340,20 @@
         # convert 24-bit integer to RGBA8 with bit shifting
         r = (value >> 16) & 0xFF
         g = (value >> 8) & 0xFF
         b = value & 0xFF
         return RGBA8(r, g, b).to_float()
 
     # support for pydantic.color.Color
-    pydantic_color = sys.modules.get("pydantic.color")
-    if pydantic_color and isinstance(value, pydantic_color.Color):
-        r, g, b, *alpha = value.as_rgb_tuple()
-        return RGBA(r / 255, g / 255, b / 255, alpha[0] if alpha else 1)
+    for mod in ("pydantic", "pydantic_extra_types"):
+        if (pydantic_color := sys.modules.get(f"{mod}.color")) and isinstance(
+            value, pydantic_color.Color
+        ):
+            r, g, b, *alpha = value.as_rgb_tuple()
+            return RGBA(r / 255, g / 255, b / 255, alpha[0] if alpha else 1)
 
     # support for colour.Color
     colour_color = sys.modules.get("colour")
     if colour_color and isinstance(value, colour_color.Color):
         return RGBA(*_bound_0_1(value.get_rgb()))
 
     raise TypeError(f"Cannot convert type {type(value)!r} to Color")
@@ -473,14 +482,28 @@
         return f"{self.__class__.__name__}({arg!r})"
 
     def __rich_repr__(self) -> Any:
         """Provide a rich representation of the color, with color swatch."""
         return _external.rich_print_color(self)
 
     @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        from pydantic_core import core_schema
+
+        schema = handler(Any)
+
+        return core_schema.no_info_after_validator_function(
+            cls,
+            schema,
+            serialization=core_schema.plain_serializer_function_ser_schema(str),
+        )
+
+    @classmethod
     def __get_validators__(cls) -> Iterator[Callable]:
         yield cls  # pydantic validator
 
     def _json_encode(self) -> str:
         # psygnal.EventedModel support
         return str(self)
```

### Comparing `cmap-0.1.3/src/cmap/_colormap.py` & `cmap-0.2.0/src/cmap/_colormap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from __future__ import annotations
 
 import base64
 import warnings
 from functools import partial
 from numbers import Number
-from typing import TYPE_CHECKING, NamedTuple, Sequence, cast, overload
+from typing import TYPE_CHECKING, Any, NamedTuple, Sequence, cast, overload
 
 import numpy as np
 import numpy.typing as npt
 
 from . import _external
 from ._catalog import Catalog
 from ._color import Color
 
 if TYPE_CHECKING:
-    from typing import Any, Callable, Iterable, Iterator, Literal, Union
+    from typing import Callable, Iterable, Iterator, Literal, Union
 
     import bokeh.models
     import matplotlib.colors
     import matplotlib.figure
     import napari.utils.colormaps
     import pygfx
+    import pyqtgraph
     import vispy.color
     from numpy.typing import ArrayLike, NDArray
+    from pydantic import GetCoreSchemaHandler
+    from pydantic_core import CoreSchema
     from typing_extensions import TypeAlias, TypedDict, TypeGuard
 
     from ._catalog import CatalogItem
     from ._color import ColorLike
 
+    LutCacheKey = tuple[int, float, bool]
     Interpolation = Literal["linear", "nearest"]
     LutCallable: TypeAlias = Callable[[NDArray], NDArray]
     ColorStopLike: TypeAlias = Union[tuple[float, ColorLike], np.ndarray]
     # All of the things that we can pass to the constructor of Colormap
     ColorStopsLike: TypeAlias = Union[
         str,  # colormap name, w/ optional "_r" suffix
         Iterable[ColorLike | ColorStopLike],
@@ -51,14 +55,17 @@
     class ColormapDict(TypedDict):
         name: str
         identifier: str
         category: str | None
         value: list[tuple[float, list[float]]]
 
 
+BAD_COLOR = (0.0, 0.0, 0.0, 0.0)
+
+
 class Colormap:
     """A colormap is a mapping from scalar values to RGB(A) colors.
 
     Parameters
     ----------
     value : Color | ColorStop | Iterable[Color | ColorStop] | dict[float, Color]
         The color data to use for the colormap. Can be a single color, a single
@@ -92,36 +99,43 @@
         `"custom colormap"`.
     identifier : str | None
         The identifier of the colormap. If None, will be set to the name, converted
         to lowercase and with spaces and dashes replaced by underscores.
     category : str | None
         An optional category of the colormap (e.g. `"diverging"`, `"sequential"`).
         Not used internally.
+    interpolation : str | bool | None
+        The interpolation mode to use when mapping scalar values to colors. Can be
+        `"linear"` (default) or `"nearest"`. If `True`, will use `"linear"`, if `False`,
+        will use `"nearest"`.  Providing this value will override any interpolation
+        from a catalog entry.
+    under : ColorLike | None
+        The color to use for values below the colormap's range.
+    over : ColorLike | None
+        The color to use for values above the colormap's range.
+    bad : ColorLike | None
+        The color to use for bad (NaN, inf) values.
     """
 
     __slots__ = (
+        "bad_color",
+        "category",
         "color_stops",
-        "name",
         "identifier",
-        "category",
         "info",
-        "_lut_cache",
         "interpolation",
+        "name",
+        "over_color",
+        "under_color",
         "_initialized",
+        "_lut_cache",
         "__weakref__",
     )
 
     #: ColorStops dett
-    color_stops: ColorStops
-
-    name: str
-    identifier: str
-    category: str | None
-    interpolation: Interpolation
-    info: CatalogItem | None
 
     _catalog_instance: Catalog | None = None
 
     @classmethod
     def catalog(cls) -> Catalog:
         """Return the global colormaps catalog."""
         if cls._catalog_instance is None:
@@ -132,86 +146,96 @@
         self,
         value: ColorStopsLike,
         *,
         name: str | None = None,
         identifier: str | None = None,
         category: str | None = None,
         interpolation: Interpolation | bool | None = None,
+        under: ColorLike | None = None,
+        over: ColorLike | None = None,
+        bad: ColorLike | None = None,
     ) -> None:
+        self.info: CatalogItem | None = None
+
         if isinstance(value, str):
             rev = value.endswith("_r")
             info = self.catalog()[value[:-2] if rev else value]
             name = name or f"{info.namespace}:{info.name}"
             category = category or info.category
+            over = info.over if over is None else over
+            under = info.under if under is None else under
+            bad = info.bad if bad is None else bad
             self.info = info
             if isinstance(info.data, list):
                 ld = len(info.data[0])
                 if ld == 2:
                     # if it's a list of tuples, it's a list of color stops
                     stops = ColorStops._from_uniform_stops(info.data)
                 elif ld == 3:
                     stops = ColorStops._from_colorarray_like(info.data)
                 else:  # pragma: no cover
                     raise ValueError(
                         f"Invalid catalog colormap data for {info.name!r}: {info.data}"
                     )
             else:
                 stops = _parse_colorstops(info.data)
-            stops._interpolation = _norm_interp(interpolation or info.interpolation)
-            interpolation = stops._interpolation
+            if interpolation is None:
+                interpolation = info.interpolation
             if rev:
                 stops = stops.reversed()
         elif isinstance(value, Colormap):
             name = name or value.name
             identifier = identifier or value.identifier
             self.info = value.info
             category = category or value.category
-            interpolation = interpolation or value.interpolation
+            if interpolation is None:
+                interpolation = value.interpolation
             stops = value.color_stops
-            self.info = None
         else:
             stops = _parse_colorstops(value)
-            self.info = None
 
         name = name or identifier
         if not name:
             name = value if isinstance(value, str) else "custom colormap"
 
-        self.color_stops = stops
-        self.name = name
-        self.identifier = _make_identifier(identifier or name)
-        self.category = category
-        # TODO: this just clobbers the interpolation from the user...
-        # need to unify with the catalog
-        self.interpolation = _norm_interp(interpolation)
+        self.interpolation: Interpolation = _norm_interp(interpolation)
+        stops._interpolation = self.interpolation
+        self.color_stops: ColorStops = stops
+        self.name: str = name
+        self.identifier: str = _make_identifier(identifier or name)
+        self.category: str | None = category
+
+        self.under_color = None if under is None else Color(under)
+        self.over_color = None if over is None else Color(over)
+        self.bad_color = None if bad is None else Color(bad)
 
-        self._lut_cache: dict[tuple[int, float], np.ndarray] = {}
+        self._lut_cache: dict[LutCacheKey, np.ndarray] = {}
         self._initialized = True
 
     @overload
     def __call__(
-        # would prefer to make this Arraylike, but that overlaps with float
         self,
-        x: NDArray | Sequence[float],
+        x: NDArray | Iterable[float],
         *,
         N: int = 256,
         gamma: float = 1,
         bytes: bool = False,
-    ) -> NDArray[np.float64]:
-        ...
-
+    ) -> NDArray[np.float64]: ...
     @overload
     def __call__(
-        self, x: float, *, N: int = 256, gamma: float = 1, bytes: bool = False
-    ) -> Color:
-        ...
-
+        self,
+        x: float,
+        *,
+        N: int = 256,
+        gamma: float = 1,
+        bytes: bool = False,
+    ) -> Color: ...
     def __call__(
         self,
-        x: float | NDArray | Sequence[float],
+        x: float | NDArray | Iterable[float],
         *,
         N: int = 256,
         gamma: float = 1,
         bytes: bool = False,
     ) -> Color | NDArray[np.float64]:
         r"""Map scalar values in X to an RGBA array.
 
@@ -246,83 +270,130 @@
         Returns
         -------
         color : Color | NDArray
             If X is a float, a single RGBA color will be returned. If x is an
             array-like, an array of RGBA colors will be returned with shape
             `x.shape + (4,)`
 
-
         Examples
         --------
         >>> from cmap import Colormap
         >>> from tifffile import imread
         >>> cmap = Colormap("viridis")
         >>> data = imread('some_path.tif')
         >>> data = data - data.min()  # normalize to 0-1
         >>> data = data / data.max()  # normalize to 0-1
         >>> colored_img = cmap(data)
         """
-        lut = self.lut(N=N, gamma=gamma)
+        lut = self.lut(N=N, gamma=gamma, with_over_under=True)
         if bytes:
             lut = (lut * 255).astype(np.uint8)
+        # the lut wil have three additional colors at the end for under, over, and bad
+        N = len(lut) - 3
 
         xa = np.array(x, copy=True)
         if not xa.dtype.isnative:
             xa = xa.byteswap().newbyteorder()  # Native byteorder is faster.
         if xa.dtype.kind == "f":
-            N = len(lut)
-            with np.errstate(invalid="ignore"):
-                xa *= N
-                # Negative values are out of range, but astype(int) would
-                # truncate them towards zero.
-                xa[xa < 0] = -1
-                # xa == 1 (== N after multiplication) is not out of range.
-                xa[xa == N] = N - 1
-                # Avoid converting large positive values to negative integers.
-                np.clip(xa, -1, N, out=xa)
-                xa = xa.astype(int)
+            xa *= N
+            # xa == 1 (== N after multiplication) is not out of range.
+            xa[xa == N] = N - 1
+
+        mask_under = xa < 0
+        mask_over = xa >= N
+        # If input was masked, get the bad mask from it; else mask out nans.
+        mask_bad = x.mask if np.ma.is_masked(x) else np.isnan(xa)  # type: ignore
+
+        with np.errstate(invalid="ignore"):
+            # We need this cast for unsigned ints as well as floats
+            xa = xa.astype(int)
+
+        xa[mask_under] = N
+        xa[mask_over] = N + 1
+        xa[mask_bad] = N + 2
 
-        result = lut.take(xa, axis=0, mode="clip")
-        return result if np.iterable(x) else Color(result)
+        rgba = lut.take(xa, axis=0, mode="clip")
+        return rgba if np.iterable(x) else Color(rgba)
+
+    def with_extremes(
+        self,
+        *,
+        bad: ColorLike | None = None,
+        under: ColorLike | None = None,
+        over: ColorLike | None = None,
+    ) -> Colormap:
+        """Return a copy of the colormap with new extreme values."""
+        return type(self)(
+            self.color_stops,
+            name=self.name,
+            category=self.category,
+            bad=bad,
+            under=under,
+            over=over,
+        )
 
     def as_dict(self) -> ColormapDict:
         """Return a dictionary representation of the colormap.
 
         The returned dictionary is suitable for serialization, or for passing to the
         Colormap constructor.
         """
         return {
             "name": self.name,
             "identifier": self.identifier,
             "category": self.category,
             "value": [(p, list(c)) for p, c in self.color_stops],
         }
 
-    def lut(self, N: int = 256, gamma: float = 1) -> np.ndarray:
+    def lut(
+        self, N: int = 256, gamma: float = 1, *, with_over_under: bool = False
+    ) -> np.ndarray:
         """Return a lookup table (LUT) for the colormap.
 
         The returned LUT is a numpy array of RGBA values, with shape (N, 4), where N is
-        the number of requested colors in the LUT. The LUT can be used to map scalar
-        values (that have been normalized to 0-1) to colors.
+        the number of requested colors in the LUT. If `with_over_under`
+        is `True` the returned shape will be (N + 3, 4), where index N is the under
+        color, index N + 1 is the over color, and index N + 2 is the bad (NaN) color.
+
+        The LUT can be used to map scalar values (that have been normalized to 0-1) to
+        colors, using fancy indexing or `np.take`.
 
         The output of this function is used by the `__call__` method, but may also
         be used directly by users.
 
         LUTs of a particular size and gamma value are cached.
 
         Parameters
         ----------
         N : int
             The number of colors in the LUT.
         gamma : float
             The gamma value to use for the LUT.
+        with_over_under : bool
+            If True, the LUT will include the under, over, and bad colors as the
+            last three colors in the LUT.  If False, the LUT will only include the
+            colors defined by the color_stops.
         """
-        if (N, gamma) not in self._lut_cache:
-            self._lut_cache[(N, gamma)] = self.color_stops.to_lut(N, gamma)
-        return self._lut_cache[(N, gamma)]
+        key = (N, gamma, with_over_under)
+        if key not in self._lut_cache:
+            lut = self.color_stops.to_lut(N, gamma)
+
+            if with_over_under:
+                under = lut[0] if self.under_color is None else self.under_color.rgba
+                over = lut[-1] if self.over_color is None else self.over_color.rgba
+                bad = BAD_COLOR if self.bad_color is None else self.bad_color.rgba
+                # expand (N, 4) lut to (N+3, 4) to include under, over, and bad colors
+                lut = np.vstack((lut, np.zeros((3, 4))))
+                lut[-3] = under
+                lut[-2] = over
+                lut[-1] = bad
+
+            self._lut_cache[key] = lut
+
+        return self._lut_cache[key]
 
     def iter_colors(self, N: Iterable[float] | int | None = None) -> Iterator[Color]:
         """Return a list of N color objects sampled evenly over the range of the LUT.
 
         If N is an integer, it will return a list of N colors spanning the full range
         of the colormap. If N is an iterable, it will return a list of colors at the
         positions specified by the iterable.
@@ -359,14 +430,57 @@
         if name is None:
             name = self.name[:-2] if self.name.endswith("_r") else f"{self.name}_r"
 
         return type(self)(
             self.color_stops.reversed(), name=name, category=self.category
         )
 
+    def shifted(
+        self,
+        shift: float = 0.5,
+        name: str | None = None,
+        mode: Literal["wrap", "clip"] = "wrap",
+    ) -> Colormap:
+        """Return a new Colormap, with colors shifted by a scalar value.
+
+        This method shifts the stops in the colormap by a scalar value.
+        It makes most sense for cyclic colormaps, but can be used with any colormap.
+
+        Parameters
+        ----------
+        shift : float
+            The amount to shift the colormap.  Positive values shift the colormap
+            towards the end, negative values shift the colormap towards the beginning.
+        name : str
+            A new name for the colormap.  If not provided, the name of the new colormap
+            will be the name of the original colormap with "_shifted{shift}" appended.
+        mode : {'wrap', 'clip'}, optional
+            The mode to use when shifting the colormap.  Must be one of 'wrap' or
+            'clip'. If 'wrap', the colormap will be shifted and wrapped around the ends.
+            If 'clip', the colormap will be shifted and the colors at the ends will be
+            clipped and/or repeated as necessary.
+
+        Returns
+        -------
+        Colormap
+            A new colormap with the colors shifted.
+        """
+        if name is None:
+            name = f"{self.name}_shifted{shift}"
+
+        return type(self)(
+            self.color_stops.shifted(shift=shift, mode=mode),
+            name=name,
+            category=self.category,
+            interpolation=self.interpolation,
+            under=self.under_color,
+            over=self.over_color,
+            bad=self.bad_color,
+        )
+
     def to_css(
         self,
         max_stops: int | None = None,
         angle: int = 90,
         radial: bool = False,
         as_hex: bool = False,
     ) -> str:
@@ -407,15 +521,24 @@
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Colormap):
             try:
                 other = Colormap(other)  # type: ignore
             except Exception:
                 return NotImplemented
-        return self.color_stops == other.color_stops
+
+        return (
+            self.color_stops == other.color_stops
+            and self.under_color == other.under_color
+            and self.over_color == other.over_color
+            and self.bad_color == other.bad_color
+            and self.interpolation == other.interpolation
+        )
+
+    # -------------------------- reprs ----------------------------------
 
     def __repr__(self) -> str:
         return f"Colormap(name={self.name!r}, <{len(self.color_stops)} colors>)"
 
     def _repr_png_(
         self, *, width: int = 512, height: int = 48, img: np.ndarray | None = None
     ) -> bytes:
@@ -425,30 +548,62 @@
         X = img if img is not None else np.tile(np.linspace(0, 1, width), (height, 1))
         return encode_png(self(X, bytes=True))
 
     def _repr_html_(self) -> str:
         """Generate an HTML representation of the Colormap."""
         png_base64 = base64.b64encode(self._repr_png_()).decode("ascii")
 
-        return (
-            f'<div style="vertical-align: middle;"><strong>{self.name}</strong></div>'
-            "<div>"
-            f'<img alt="{self.name} colormap" title="{self.name}" '
-            f'style="border: 1px solid #555;" src="data:image/png;base64,{png_base64}">'
+        html = (
+            '<div style="vertical-align: middle;">'
+            f"<strong>{self.name}</strong> "
             "</div>"
+            '<div class="cmap"><img '
+            f'alt="{self.name} colormap" '
+            f'title="{self.name}" '
+            'style="border: 1px solid #555;" '
+            f'src="data:image/png;base64,{png_base64}"></div>'
         )
+        if any(
+            x is not None for x in (self.under_color, self.over_color, self.bad_color)
+        ):
+            html += (
+                '<div style="vertical-align: middle; '
+                "max-width: 514px; "
+                'display: flex; justify-content: space-between;">'
+                '<div style="float: left;">'
+                f"{_html_color_patch(self.under_color)} under"
+                "</div>"
+                '<div style="margin: 0 auto; display: inline-block;">'
+                f"bad {_html_color_patch(self.bad_color or Color(BAD_COLOR))}"
+                "</div>"
+                '<div style="float: right;">'
+                f"over {_html_color_patch(self.over_color)}"
+                "</div>"
+            )
 
-    # -------------------------- RICH REPR SUPPORT ----------------------------------
+        return html
 
     def __rich_repr__(self) -> Any:
         return _external.rich_print_colormap(self)  # side effect
 
     # -------------------------- PYDANTIC SUPPORT -----------------------------------
 
     @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        from pydantic_core import core_schema
+
+        schema = handler(Any)
+        ser = core_schema.plain_serializer_function_ser_schema(lambda x: x.as_dict())
+        return core_schema.no_info_after_validator_function(
+            cls._validate, schema, serialization=ser
+        )
+
+    @classmethod
     def __get_validators__(cls) -> Iterator[Callable]:
         yield cls._validate  # pydantic validator
 
     @classmethod
     def _validate(cls, v: Any) -> Colormap:
         if isinstance(v, cls):
             return v  # pragma: no cover
@@ -530,26 +685,30 @@
         Returns
         -------
         fig : matplotlib.figure.Figure
             The figure object containing the plot.
         """
         return _external.viscm_plot(self, dpi, dest)
 
+    def to_pyqtgraph(self) -> pyqtgraph.ColorMap:
+        """Return a `pyqtgraph.ColorMap`."""
+        return _external.to_pyqtgraph(self)
+
 
 class ColorStop(NamedTuple):
     """A color stop in a color gradient."""
 
     position: float
     color: Color
 
 
 def _norm_interp(interp: Interpolation | bool | str | None) -> Interpolation:
     if isinstance(interp, bool):
         return "linear" if interp else "nearest"
-    elif not interp:
+    if interp is None:
         return "linear"
     if interp not in {"linear", "nearest"}:
         raise ValueError(
             f"Invalid interpolation mode: {interp!r}. "
             "Must be one of 'linear' or 'nearest'"
         )
     return cast("Interpolation", interp)
@@ -689,25 +848,19 @@
         """Return an (N, 4) array of RGBA values."""
         return self._stops[:, 1:]
 
     def __len__(self) -> int:
         return len(self._stops)
 
     @overload
-    def __getitem__(self, key: int) -> ColorStop:
-        ...
-
+    def __getitem__(self, key: int) -> ColorStop: ...
     @overload
-    def __getitem__(self, key: slice) -> ColorStops:
-        ...
-
+    def __getitem__(self, key: slice) -> ColorStops: ...
     @overload
-    def __getitem__(self, key: tuple) -> np.ndarray:
-        ...
-
+    def __getitem__(self, key: tuple) -> np.ndarray: ...
     def __getitem__(
         self, key: int | slice | tuple
     ) -> ColorStop | ColorStops | np.ndarray:
         """Get an item or slice of the color stops.
 
         If key is an integer, return a single `ColorStop` tuple.
         If key is a slice, return a new `ColorStops` object.
@@ -855,15 +1008,57 @@
             else:
                 # partial to maintain picklability
                 rev_lutfunc = partial(self._reverser, lut_func)
             return type(self)(lut_func=rev_lutfunc)
         # invert the positions in the stops
         rev_stops = self._stops[::-1]
         rev_stops[:, 0] = 1 - rev_stops[:, 0]
-        return type(self)(rev_stops)
+        return type(self)(rev_stops, interpolation=self._interpolation)
+
+    def shifted(
+        self, shift: float, mode: Literal["wrap", "clip"] = "wrap"
+    ) -> ColorStops:
+        """Return a new ColorStops object with all positions shifted by `shift`.
+
+        Parameters
+        ----------
+        shift : float
+            The amount to shift the colormap.  Positive values shift the colormap
+            towards the end, negative values shift the colormap towards the beginning.
+        mode : {'wrap', 'clip'}, optional
+            The mode to use when shifting the colormap.  Must be one of 'wrap' or
+            'clip'. If 'wrap', the colormap will be shifted and wrapped around the ends.
+            If 'clip', the colormap will be shifted and the colors at the ends will be
+            clipped and/or repeated as necessary.
+        """
+        if mode not in {"wrap", "clip"}:  # pragma: no cover
+            raise ValueError("mode must be 'wrap' or 'clip'")
+
+        if mode == "wrap":
+            stops = _wrap_shift_color_stops(self._stops, shift)
+        else:
+            stops = self._stops.copy()
+            stops[:, 0] += shift
+            # throw away stops that are out of bounds
+            stops = stops[(stops[:, 0] >= 0) & (stops[:, 0] <= 1)]
+        return type(self)(stops, interpolation=self._interpolation)
+
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        from pydantic_core import core_schema
+
+        schema = handler(Any)
+        ser = core_schema.plain_serializer_function_ser_schema(
+            lambda x: [(p, list(c)) for p, c in x]
+        )
+        return core_schema.no_info_after_validator_function(
+            cls.parse, schema, serialization=ser
+        )
 
     @classmethod
     def __get_validators__(cls) -> Iterator[Callable]:
         yield cls.parse  # pydantic validator
 
     def _json_encode(self) -> list:
         return cast(list, self._stops.tolist())
@@ -1175,7 +1370,34 @@
         _colors.append(Color(item))  # type: ignore  # this will raise if invalid
 
     if (np.diff([x for x in _positions if x is not None]) < 0).any():
         raise ValueError("Color stops must be in ascending position order")
 
     _stops = _fill_stops(_positions, "neighboring")  # TODO: expose fill_mode?
     return cls(zip(_stops, _colors))
+
+
+def _html_color_patch(color: Color | None) -> str:
+    if color is None:
+        return ""
+    return (
+        f'<div title="{color.hex}" '
+        'style="display: inline-block; '
+        "width: 1em; height: 1em; "
+        "margin: 0; "
+        "vertical-align: middle; "
+        "border: 1px solid #555; "
+        f'background-color: {color.hex};"></div>'
+    )
+
+
+def _wrap_shift_color_stops(data: np.ndarray, shift_amount: float) -> np.ndarray:
+    """Shift (N, 5) array of color stops by `shift_amount` and wrap around."""
+    out = np.array(data, copy=True)
+    # ensure that 0 <= data < 1
+    # this is important for dealing with wraparound when shifting
+    out[:, 0][out[:, 0] == 1] = 1 - np.finfo(float).eps
+    out[:, 0] += shift_amount
+    out[:, 0] %= 1
+    # sort the array by the first column
+    out = out[out[:, 0].argsort()]
+    return out
```

### Comparing `cmap-0.1.3/src/cmap/_external.py` & `cmap-0.2.0/src/cmap/_external.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 """Functions for interacting with external libraries."""
+
 from __future__ import annotations
 
 import contextlib
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 if TYPE_CHECKING:
     import pygfx
     from bokeh.models import LinearColorMapper as BokehLinearColorMapper
     from matplotlib.colors import Colormap as MplColormap
     from matplotlib.colors import LinearSegmentedColormap as MplLinearSegmentedColormap
+    from matplotlib.colors import ListedColormap as MplListedColormap
     from matplotlib.figure import Figure as MplFigure
     from napari.utils.colormaps import Colormap as NapariColormap
+    from pyqtgraph import ColorMap as PyqtgraphColorMap
     from vispy.color import Colormap as VispyColormap
 
     from ._color import Color
     from ._colormap import Colormap
 
 
 def to_mpl(
     cm: Colormap, N: int = 256, gamma: float = 1.0
-) -> MplLinearSegmentedColormap:
+) -> MplLinearSegmentedColormap | MplListedColormap:
     """Return a matplotlib colormap."""
     import matplotlib.colors as mplc
 
+    mpl_cm: mplc.Colormap
     if cm.interpolation == "nearest":
-        return mplc.ListedColormap(colors=cm.color_stops.color_array, name=cm.name)
-
-    try:
-        return mplc.LinearSegmentedColormap.from_list(
-            cm.name, cm.color_stops, N=N, gamma=gamma
-        )
-    except ValueError as e:
-        from matplotlib import __version__
-
-        # broken in matplotlib 3.8.0, fixed by
-        # https://github.com/matplotlib/matplotlib/pull/26952
-        if len(cm.color_stops) == 2 and __version__ == "3.8.0":
-            raise ValueError(
-                "matplotlib 3.8.0 has a bug that prevents creating a colormap "
-                "from only two colors.  Please upgrade or downgrade matplotlib."
-            ) from e
-        raise
+        mpl_cm = mplc.ListedColormap(colors=cm.color_stops.color_array, name=cm.name)
+    else:
+        try:
+            mpl_cm = mplc.LinearSegmentedColormap.from_list(
+                cm.name, cm.color_stops, N=N, gamma=gamma
+            )
+        except ValueError as e:  # pragma: no cover
+            from matplotlib import __version__
+
+            # broken in matplotlib 3.8.0, fixed by
+            # https://github.com/matplotlib/matplotlib/pull/26952
+            if len(cm.color_stops) == 2 and __version__ == "3.8.0":
+                raise ValueError(
+                    "matplotlib 3.8.0 has a bug that prevents creating a colormap "
+                    "from only two colors.  Please upgrade or downgrade matplotlib."
+                ) from e
+            raise
+
+    return mpl_cm.with_extremes(
+        bad=cm.bad_color,  # type: ignore
+        over=cm.over_color,  # type: ignore
+        under=cm.under_color,  # type: ignore
+    )
 
 
 def to_vispy(cm: Colormap) -> VispyColormap:
     """Return a vispy colormap."""
     from vispy.color import Colormap
 
     return Colormap(colors=cm.color_stops.color_array, controls=cm.color_stops.stops)
@@ -92,14 +102,25 @@
     """Return an altair colorscale with N color samples from the colormap.
 
     Suitable for passing to the range parameter of altair.Scale.
     """
     return [color.hex for color in cm.iter_colors(N)]
 
 
+def to_pyqtgraph(cm: Colormap) -> PyqtgraphColorMap:
+    """Return a `pyqtgraph.Colormap`."""
+    from pyqtgraph import ColorMap
+
+    colors = (cm.color_stops.color_array * 255).astype(np.uint8)
+    return ColorMap(cm.color_stops.stops, colors, name=cm.name)
+
+
+# ==========================================
+
+
 def viscm_plot(
     cmap: Colormap | MplColormap, dpi: int = 100, dest: str | None = None
 ) -> MplFigure:
     """Evaluate goodness of colormap using perceptual deltas.
 
     Parameters
     ----------
```

### Comparing `cmap-0.1.3/src/cmap/_png.py` & `cmap-0.2.0/src/cmap/_png.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/_util.py` & `cmap-0.2.0/src/cmap/_util.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/bids/__init__.py` & `cmap-0.2.0/src/cmap/data/bids/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/bids/record.json` & `cmap-0.2.0/src/cmap/data/bids/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/chrisluts/record.json` & `cmap-0.2.0/src/cmap/data/chrisluts/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cividis/__init__.py` & `cmap-0.2.0/src/cmap/data/cividis/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cividis/record.json` & `cmap-0.2.0/src/cmap/data/cividis/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmap/record.json` & `cmap-0.2.0/src/cmap/data/cmap/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/algae.py` & `cmap-0.2.0/src/cmap/data/cmocean/algae.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/amp.py` & `cmap-0.2.0/src/cmap/data/cmocean/amp.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/balance.py` & `cmap-0.2.0/src/cmap/data/cmocean/balance.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/curl.py` & `cmap-0.2.0/src/cmap/data/cmocean/curl.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/deep.py` & `cmap-0.2.0/src/cmap/data/cmocean/deep.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/delta.py` & `cmap-0.2.0/src/cmap/data/cmocean/delta.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/dense.py` & `cmap-0.2.0/src/cmap/data/cmocean/dense.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/diff.py` & `cmap-0.2.0/src/cmap/data/cmocean/diff.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/haline.py` & `cmap-0.2.0/src/cmap/data/cmocean/haline.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/ice.py` & `cmap-0.2.0/src/cmap/data/cmocean/ice.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/matter.py` & `cmap-0.2.0/src/cmap/data/cmocean/matter.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/oxy.py` & `cmap-0.2.0/src/cmap/data/cmocean/oxy.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/phase.py` & `cmap-0.2.0/src/cmap/data/cmocean/phase.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/rain.py` & `cmap-0.2.0/src/cmap/data/cmocean/rain.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/record.json` & `cmap-0.2.0/src/cmap/data/cmocean/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/solar.py` & `cmap-0.2.0/src/cmap/data/cmocean/solar.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/speed.py` & `cmap-0.2.0/src/cmap/data/cmocean/speed.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/tarn.py` & `cmap-0.2.0/src/cmap/data/cmocean/tarn.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/tempo.py` & `cmap-0.2.0/src/cmap/data/cmocean/tempo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/thermal.py` & `cmap-0.2.0/src/cmap/data/cmocean/thermal.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/topo.py` & `cmap-0.2.0/src/cmap/data/cmocean/topo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cmocean/turbid.py` & `cmap-0.2.0/src/cmap/data/cmocean/turbid.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorbrewer/__init__.py` & `cmap-0.2.0/src/cmap/data/colorbrewer/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorbrewer/record.json` & `cmap-0.2.0/src/cmap/data/colorbrewer/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C10.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C11.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C3.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C4.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C5.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C6.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C7.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C8.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_C9.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_C9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBC1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBC1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBC2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBC2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBD1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBD1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBD2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBD2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBL1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBL1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBL2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBL2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBL3.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBL3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBL4.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBL4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBTC1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTC1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBTC2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTC2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBTD1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTD1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBTL1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBTL2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBTL3.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_CBTL4.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D10.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D11.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D12.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D12.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D13.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D13.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D1A.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D1A.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D3.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D4.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D5.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D6.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D7.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D8.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_D9.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_D9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_I1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_I1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_I2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_I2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_I3.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_I3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L10.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L11.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L12.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L12.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L13.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L13.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L14.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L14.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L15.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L15.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L16.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L16.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L17.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L17.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L18.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L18.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L19.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L19.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L20.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L20.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L3.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L4.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L5.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L6.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L7.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L8.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_L9.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_L9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_R1.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_R1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_R2.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_R2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_R3.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_R3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/CET_R4.py` & `cmap-0.2.0/src/cmap/data/colorcet/CET_R4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/__init__.py` & `cmap-0.2.0/src/cmap/data/colorcet/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/colorcet/record.json` & `cmap-0.2.0/src/cmap/data/colorcet/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/acton.py` & `cmap-0.2.0/src/cmap/data/crameri/acton.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/bam.py` & `cmap-0.2.0/src/cmap/data/crameri/bam.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/bamO.py` & `cmap-0.2.0/src/cmap/data/crameri/bamO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/bamako.py` & `cmap-0.2.0/src/cmap/data/crameri/bamako.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/batlow.py` & `cmap-0.2.0/src/cmap/data/crameri/batlow.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/batlowK.py` & `cmap-0.2.0/src/cmap/data/crameri/batlowK.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/batlowW.py` & `cmap-0.2.0/src/cmap/data/crameri/batlowW.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/berlin.py` & `cmap-0.2.0/src/cmap/data/crameri/berlin.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/bilbao.py` & `cmap-0.2.0/src/cmap/data/crameri/bilbao.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/broc.py` & `cmap-0.2.0/src/cmap/data/crameri/broc.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/brocO.py` & `cmap-0.2.0/src/cmap/data/crameri/brocO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/buda.py` & `cmap-0.2.0/src/cmap/data/crameri/buda.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/bukavu.py` & `cmap-0.2.0/src/cmap/data/crameri/bukavu.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/cork.py` & `cmap-0.2.0/src/cmap/data/crameri/cork.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/corkO.py` & `cmap-0.2.0/src/cmap/data/crameri/corkO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/davos.py` & `cmap-0.2.0/src/cmap/data/crameri/davos.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/devon.py` & `cmap-0.2.0/src/cmap/data/crameri/devon.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/fes.py` & `cmap-0.2.0/src/cmap/data/crameri/fes.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/grayC.py` & `cmap-0.2.0/src/cmap/data/crameri/grayC.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/hawaii.py` & `cmap-0.2.0/src/cmap/data/crameri/hawaii.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/imola.py` & `cmap-0.2.0/src/cmap/data/crameri/imola.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/lajolla.py` & `cmap-0.2.0/src/cmap/data/crameri/lajolla.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/lapaz.py` & `cmap-0.2.0/src/cmap/data/crameri/lapaz.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/lisbon.py` & `cmap-0.2.0/src/cmap/data/crameri/lisbon.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/nuuk.py` & `cmap-0.2.0/src/cmap/data/crameri/nuuk.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/oleron.py` & `cmap-0.2.0/src/cmap/data/crameri/oleron.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/oslo.py` & `cmap-0.2.0/src/cmap/data/crameri/oslo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/record.json` & `cmap-0.2.0/src/cmap/data/crameri/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/roma.py` & `cmap-0.2.0/src/cmap/data/crameri/roma.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/romaO.py` & `cmap-0.2.0/src/cmap/data/crameri/romaO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/tofino.py` & `cmap-0.2.0/src/cmap/data/crameri/tofino.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/tokyo.py` & `cmap-0.2.0/src/cmap/data/crameri/tokyo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/turku.py` & `cmap-0.2.0/src/cmap/data/crameri/turku.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/vanimo.py` & `cmap-0.2.0/src/cmap/data/crameri/vanimo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/vik.py` & `cmap-0.2.0/src/cmap/data/crameri/vik.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/crameri/vikO.py` & `cmap-0.2.0/src/cmap/data/crameri/vikO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/cubehelix/__init__.py` & `cmap-0.2.0/src/cmap/data/cubehelix/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/glasbey/__init__.py` & `cmap-0.2.0/src/cmap/data/glasbey/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/glasbey/_glasbey.py` & `cmap-0.2.0/src/cmap/data/glasbey/_glasbey.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,21 @@
 
     Returns
     -------
     palette: List of hex-code string or array of shape (palette_size, 3)
         The palette created, either as hex colors, or an array of floats of RGB values
         -- consumable by most plotting libraries.
     """
+    try:
+        import colorspacious  # noqa: F401
+    except ImportError as e:  # pragma: no cover
+        raise ImportError(
+            "The colorspacious package is required to run glasbey.create_palette"
+        ) from e
+
     if grid_space.lower() == "jch":
         colors = jch_grid(
             grid_size=grid_size,
             lightness_bounds=lightness_bounds,
             chroma_bounds=chroma_bounds,
             hue_bounds=hue_bounds,
             output_colorspace="CAM02-UCS",
```

### Comparing `cmap-0.1.3/src/cmap/data/glasbey/_grids.py` & `cmap-0.2.0/src/cmap/data/glasbey/_grids.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/glasbey/_internals.py` & `cmap-0.2.0/src/cmap/data/glasbey/_internals.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/glasbey/prebuilt.py` & `cmap-0.2.0/src/cmap/data/glasbey/prebuilt.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/gnuplot/__init__.py` & `cmap-0.2.0/src/cmap/data/gnuplot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 #   21: 3x             22: 3x-1           23: 3x-2
 #   24: |3x-1|         25: |3x-2|         26: (3x-1)/2
 #   27: (3x-2)/2       28: |(3x-1)/2|     29: |(3x-2)/2|
 #   30: x/0.32-0.78125 31: 2*x-0.84       32: 4x;1;-2x+1.84;x/0.08-11.5
 #   33: |2*x - 0.5|    34: 2*x            35: 2*x - 0.5
 #   36: 2*x - 1
 """
+
 from functools import partial
 from typing import TYPE_CHECKING, Sequence
 
 import numpy as np
 
 if TYPE_CHECKING:
     from typing import Callable
```

### Comparing `cmap-0.1.3/src/cmap/data/gnuplot/record.json` & `cmap-0.2.0/src/cmap/data/gnuplot/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/google/__init__.py` & `cmap-0.2.0/src/cmap/data/google/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/google/record.json` & `cmap-0.2.0/src/cmap/data/google/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/imagej/__init__.py` & `cmap-0.2.0/src/cmap/data/imagej/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/imagej/record.json` & `cmap-0.2.0/src/cmap/data/imagej/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/matlab/__init__.py` & `cmap-0.2.0/src/cmap/data/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/matlab/record.json` & `cmap-0.2.0/src/cmap/data/matlab/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/matplotlib/_CMRmap.py` & `cmap-0.2.0/src/cmap/data/matplotlib/_CMRmap.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/matplotlib/__init__.py` & `cmap-0.2.0/src/cmap/data/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/matplotlib/_coolwarm.py` & `cmap-0.2.0/src/cmap/data/matplotlib/_coolwarm.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/matplotlib/_wistia.py` & `cmap-0.2.0/src/cmap/data/matplotlib/_wistia.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 __license__ = "MIT"
 __source__ = "https://github.com/wistia/heatmap-palette"
 
 # Wistia = [
 #     (228, 255, 122),  # #e4ff7a
 #     (255, 232, 26),  # #ffe81a
 #     (255, 189, 0),  # ffbd00
```

### Comparing `cmap-0.1.3/src/cmap/data/matplotlib/record.json` & `cmap-0.2.0/src/cmap/data/matplotlib/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/seaborn/__init__.py` & `cmap-0.2.0/src/cmap/data/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/seaborn/record.json` & `cmap-0.2.0/src/cmap/data/seaborn/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/tableau/__init__.py` & `cmap-0.2.0/src/cmap/data/tableau/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/tableau/record.json` & `cmap-0.2.0/src/cmap/data/tableau/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/vispy/__init__.py` & `cmap-0.2.0/src/cmap/data/vispy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Colormaps in vispy/vispy/color/colormap.py.
 
 https://github.com/vispy/vispy/blob/356800a784f0dcb7428aa2ade3c9025a8bc2d5cc/vispy/color/colormap.py
 """
+
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike
```

### Comparing `cmap-0.1.3/src/cmap/data/vispy/record.json` & `cmap-0.2.0/src/cmap/data/vispy/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/src/cmap/data/yorick/__init__.py` & `cmap-0.2.0/src/cmap/data/yorick/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 Yorick's random number generator and several special functions in
 Yorick/include were taken from Numerical Recipes by Press, et. al.,
 although the Yorick implementations are unrelated to those in
 Numerical Recipes.  A small amount of code in Gist was adapted from
 the X11R4 release, copyright M.I.T. -- the complete copyright notice
 may be found in the (unused) file Gist/host.c.
 """
+
 import numpy as np
 
 # https://github.com/LLNL/yorick/blob/fda4a1ed1e2441e30de88e01b251b822f3604b1f/g/earth.gp
 earth = [
     (0.0, (0.0, 0.0, 0.0, 1.0)),
     (0.0039, (0.0025990793201133146, 0.0, 0.1684, 1.0)),
     (0.0078, (0.005198158640226629, 0.0, 0.2212, 1.0)),
```

### Comparing `cmap-0.1.3/src/cmap/data/yorick/record.json` & `cmap-0.2.0/src/cmap/data/yorick/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/tests/test_catalog.py` & `cmap-0.2.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/tests/test_color.py` & `cmap-0.2.0/tests/test_color.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,24 @@
     import colour
 
     colourRed = colour.Color("red")
 except ImportError:
     colourRed = "red"
 
 try:
-    import pydantic.color
+    import pydantic_extra_types.color
 
-    pydanticRed = pydantic.color.Color("red")
+    pydanticRed = pydantic_extra_types.color.Color("red")
 except ImportError:
-    pydanticRed = "red"
+    try:
+        import pydantic.color
+
+        pydanticRed = pydantic.color.Color("red")
+    except ImportError:
+        pydanticRed = "red"
 
 
 @pytest.mark.parametrize(
     "color, expected",
     [
         ("royalblue", (65, 105, 225)),
         (Color("royalblue"), (65, 105, 225)),
```

### Comparing `cmap-0.1.3/tests/test_colormap.py` & `cmap-0.2.0/tests/test_colormap.py`

 * *Files 16% similar despite different names*

```diff
@@ -192,7 +192,45 @@
     assert isinstance(cm._repr_png_(), bytes)
 
 
 def test_cmap_from_cmap() -> None:
     cm = Colormap(("red", "blue"), name="mymap")
     cm2 = Colormap(cm)
     assert cm2.name == "mymap"
+
+
+def test_interp_arg_passed_to_stops() -> None:
+    cm = Colormap(["#364B9A", "#4A7BB7", "#6EA6CD", "#98CAE1"], interpolation=False)
+    assert cm.color_stops._interpolation == "nearest"
+
+    cm = Colormap(["#364B9A", "#4A7BB7", "#6EA6CD", "#98CAE1"])
+    assert cm.color_stops._interpolation == "linear"
+
+
+def test_with_extremes() -> None:
+    cm = Colormap(["red", "blue"], under="green", over="yellow", bad="black")
+    cm2 = Colormap(["red", "blue"]).with_extremes(
+        under="green", over="yellow", bad="black"
+    )
+    assert cm == cm2
+
+    assert cm2.under_color == cm.under_color == Color("green")
+    assert "under" in cm2._repr_html_()
+
+
+def test_shifted() -> None:
+    cm = Colormap(["red", "blue", "yellow"])
+    assert cm.shifted(1) == cm
+    assert "shifted0.3" in cm.shifted(0.3).name
+    # two shifts of 0.5 should give the original array
+    assert cm.shifted().shifted() == cm
+
+    wrapped = cm.shifted(0.2, mode="wrap")
+    assert wrapped == Colormap([(0.2, "yellow"), (0.2, "red"), (0.7, "blue")])
+    clipped = cm.shifted(0.5, mode="clip")
+    assert clipped == Colormap([(0.5, "red"), (1, "blue")])
+
+    cm = Colormap("viridis")
+    # forward and backward shifts should cancel out
+    assert cm.shifted(0.5).shifted(-0.5) == cm
+    # two shifts of 0.5 should give the original array
+    assert cm.shifted().shifted() == cm
```

### Comparing `cmap-0.1.3/tests/test_data.py` & `cmap-0.2.0/tests/test_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 if TYPE_CHECKING:
     from matplotlib.colors import Colormap as MPLColormap
 
 catalog = Colormap.catalog()
 
 
+@pytest.mark.skipif(not MPL_CMAPS, reason="matplotlib not installed")
 def test_matplotlib_name_parity() -> None:
-    if not MPL_CMAPS:
-        pytest.skip("matplotlib not installed")
     if missing := (MPL_CMAPS - set(catalog._original_names)):
         raise AssertionError(f"missing cmap keys from matplotlib: {missing}")
 
 
 def test_napari_name_parity() -> None:
     # might need to importorskip later
+    pytest.importorskip("napari")
     import napari.utils.colormaps.colormap_utils as ncm
 
     napari_cmaps: Set[str] = set(ncm.AVAILABLE_COLORMAPS)
     napari_cmaps.update(ncm._VISPY_COLORMAPS_ORIGINAL)
     napari_cmaps.update(ncm._MATPLOTLIB_COLORMAP_NAMES)
     # TODO: later it would be good to make sure we can accept all strings
     # without having to do any extra work
```

### Comparing `cmap-0.1.3/tests/test_glasbey.py` & `cmap-0.2.0/tests/test_glasbey.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 @pytest.mark.parametrize("cvd_severity", [None, 0.5], ids=("no_cvd", "cvd"))
 def test_glasbey_create_palette(
     use_numba: bool,
     grid_space: Literal["RGB", "JCh"],
     grid_size: int | tuple[int, int, int],
     cvd_severity: float | None,
 ) -> None:
+    pytest.importorskip("colorspacious")
     with nullcontext() if use_numba else pytest.warns(UserWarning):
         from cmap.data.glasbey import create_palette
 
         create_palette(
             palette_size=256 if use_numba else 4,
             grid_space=grid_space,
             grid_size=grid_size,
```

### Comparing `cmap-0.1.3/tests/test_model_fields.py` & `cmap-0.2.0/tests/test_model_fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,82 @@
 import os
 from typing import ClassVar
 
 import numpy as np
 import pytest
 
+from cmap import Color, Colormap
+from cmap._colormap import ColorStops
+
 try:
     import pydantic
-    import pydantic.color
+    from pydantic_compat import BaseModel
+
+    V2 = int(pydantic.__version__.split(".")[0]) >= 2
 except ImportError:
     pytest.skip("pydantic not installed", allow_module_level=True)
 
-from cmap import Color, Colormap
-from cmap._colormap import ColorStops
+try:
+    import pydantic_extra_types.color as pydantic_color
+except ImportError:
+    import pydantic.color as pydantic_color
 
 
 def test_pydantic_casting() -> None:
-    assert Color(pydantic.color.Color("red")) is Color("red")
+    assert Color(pydantic_color.Color("red")) is Color("red")
 
 
 # we're interested in testing serializeability...
 # Color can serialized with `str`, and Colormap can be serialized with `as_dict`
+@pytest.mark.filterwarnings("ignore:`json_encoders` is deprecated")
 def test_pydantic_validate() -> None:
-    class MyModel(pydantic.BaseModel):
+    class MyModel(BaseModel):
         color: Color
         colormap: Colormap
 
-        class Config:
-            # since json.dump is not extendable, this just needs to be documented.
-            json_encoders: ClassVar[dict] = {Color: str, Colormap: Colormap.as_dict}
+        if V2:
+
+            class Config:
+                # since json.dump is not extendable, this just needs to be documented.
+                json_encoders: ClassVar[dict] = {Color: str, Colormap: Colormap.as_dict}
 
     obj = MyModel(color=np.array([1.0, 0, 0]), colormap=["r", (0.7, "b"), "w"])
     assert obj.color is Color("red")
     assert obj.colormap == Colormap(["r", (0.7, "b"), "w"])
     serialized = obj.json()
     if os.getenv("CI"):
-        # FIXME: why is this different on CI?
+        # not sure why this is different in CI
         assert serialized == (
-            '{"color": "red", '
-            '"colormap": {"name": "custom colormap", "identifier": "custom_colormap", '
-            '"category": null, '
-            '"value": ['
-            "[0.0, [1.0, 0.0, 0.0, 1]], "
-            "[0.7, [0.0, 0.0, 1.0, 1]], "
-            "[1.0, [1.0, 1.0, 1.0, 1]]]}"
+            '{"color":"red",'
+            '"colormap":{"name":"custom colormap","identifier":"custom_colormap",'
+            '"category":null,'
+            '"value":['
+            "[0.0,[1.0,0.0,0.0,1]],"
+            "[0.7,[0.0,0.0,1.0,1]],"
+            "[1.0,[1.0,1.0,1.0,1]]]}"
             "}"
         )
-    assert MyModel.parse_raw(serialized) == obj
+    if hasattr(MyModel, "model_validate_json"):
+        assert MyModel.model_validate_json(serialized) == obj
+    else:
+        assert MyModel.parse_raw(serialized) == obj
 
 
 def test_psygnal_serialization() -> None:
     # support for _json_encode_ is built into psygnal, ... don't need json_encoders
     psygnal = pytest.importorskip("psygnal")
 
     class MyModel(psygnal.EventedModel):  # type: ignore
         color: Color
         colormap: Colormap
         stops: ColorStops
 
     obj = MyModel(
         color=np.array([1, 0, 0]), colormap=["r", (0.7, "b"), "w"], stops="green_r"
     )
-    assert MyModel.parse_raw(obj.json()) == obj
+
+    data = obj.model_dump_json() if V2 else obj.json()
+
+    if hasattr(MyModel, "model_validate_json"):
+        assert MyModel.model_validate_json(data) == obj
+    else:
+        assert MyModel.parse_raw(data) == obj
```

### Comparing `cmap-0.1.3/tests/test_third_party.py` & `cmap-0.2.0/tests/test_third_party.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,30 @@
 from unittest.mock import MagicMock, patch
 
 import numpy as np
 import pytest
 
 from cmap import Color, Colormap
 
+try:
+    import pytestqt  # noqa F401
+except ImportError:
+    pytest.skip("pytest-qt not installed", allow_module_level=True)
+
 if TYPE_CHECKING:
     from qtpy.QtWidgets import QApplication
 
 # This module is slow, so we skip it unless running on CI
 # or if the THIRD environment variable is set.
 if not (os.getenv("CI") or os.getenv("THIRD")):
     pytest.skip("Skipping third party tests", allow_module_level=True)
 
-CMAP = Colormap(["black", (0, 1, 0), "00FFFF33", "w"])
+OVER = "red"
+UNDER = "blue"
+CMAP = Colormap(["black", (0, 1, 0), "00FFFF33", "w"], over=OVER, under=UNDER)
 IMG = np.random.rand(10, 10).astype("float32")
 CI = bool(os.getenv("CI"))
 LINUX = sys.platform.startswith("linux")
 
 
 def test_colour_support() -> None:
     colour = pytest.importorskip("colour")
@@ -45,18 +52,22 @@
         cm.__rich_repr__()
         rich_print_colormap(cm, 100)  # for coverage... could be fixed with PropertyMock
     mock.print.assert_called()
 
 
 def test_matplotlib() -> None:
     plt = pytest.importorskip("matplotlib.pyplot")
-    plt.imshow(IMG, cmap=CMAP.to_mpl())
+    mpl_cmap = CMAP.to_mpl()
+    plt.imshow(IMG, cmap=mpl_cmap)
+    assert tuple(mpl_cmap.get_bad()) == (0, 0, 0, 0)
+    assert tuple(mpl_cmap.get_over()) == Color(OVER).rgba
+    assert tuple(mpl_cmap.get_under()) == Color(UNDER).rgba
 
 
-@pytest.mark.skipif(sys.version_info >= (3, 12), reason="napari not working on py3.12")
+@pytest.mark.filterwarnings("ignore")
 def test_napari(qapp: "QApplication") -> None:
     napari = pytest.importorskip("napari")
 
     v = napari.view_image(IMG, colormap=CMAP.to_napari())
     v.close()
 
 
@@ -111,14 +122,15 @@
     canvas.request_draw(animate)
     QWidget.close(canvas)  # pygfx overrides close with a broken method :)
     canvas.deleteLater()
 
 
 @pytest.mark.skipif(os.name == "nt" and sys.version_info >= (3, 11), reason="segfaults")
 def test_bokeh() -> None:
+    pytest.importorskip("bokeh")
     from bokeh.plotting import figure
 
     p = figure()
     h, w = IMG.shape
     p.image(image=[np.flipud(IMG)], x=0, y=0, dw=w, dh=h, color_mapper=CMAP.to_bokeh())
 
 
@@ -128,20 +140,31 @@
     alt = cmap1.to_altair()
     assert isinstance(alt, list) and all(isinstance(c, str) for c in alt)
     assert alt[0] == "#FF0000"
     assert alt[-1] == "#0000FF"
 
 
 def test_viscm(tmp_path: Path) -> None:
+    pytest.importorskip("viscm")
     # NOT using importorskip here because there IS an error import viscm
     # in the current release
     cmap1 = Colormap(["red", "green", "blue"])
     out = tmp_path / "test.png"
     cmap1.to_viscm(dest=str(out))  # use dest to avoid show
     assert out.is_file()
 
 
+def test_pyqtgraph() -> None:
+    pytest.importorskip("pyqtgraph")
+    cmap1 = Colormap(["red", "green", "blue"])
+    cm = cmap1.to_pyqtgraph()
+
+    cm.getGradient()
+    cm.linearize()
+    cm.reverse()
+
+
 # def microvis_imshow(img_data: np.ndarray, cmap: cmap.Colormap) -> None:
 #     from microvis import _util, imshow
 
 #     with _util.exec_if_new_qt_app():
 #         imshow(img_data, cmap=cmap)
```

### Comparing `cmap-0.1.3/tests/test_utils.py` & `cmap-0.2.0/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 import numpy as np
 import pytest
-from matplotlib.figure import Figure as MplFigure
+
+try:
+    from matplotlib.figure import Figure as MplFigure
+except ImportError:
+    MplFigure = None
 
 from cmap import Colormap, _util
 
 CMAP_NAME = "viridis"
 CMAP_INSTANCE = Colormap(CMAP_NAME)
 
 
 def test_ensure_cmap() -> None:
     cm = _util._ensure_cmap(CMAP_NAME)
     assert isinstance(cm, Colormap)
     cm2 = _util._ensure_cmap(cm)
     assert cm is cm2
 
 
+@pytest.mark.skipif(MplFigure is None, reason="matplotlib not installed")
 def test_plot() -> None:
     fig = _util.plot_color_gradients([CMAP_NAME], compare=True)
     assert isinstance(fig, MplFigure)
 
 
+@pytest.mark.skipif(MplFigure is None, reason="matplotlib not installed")
 def test_plot_rgb() -> None:
     fig = _util.plot_rgb(CMAP_NAME)
     assert isinstance(fig, MplFigure)
 
 
 def test_calc_lightness() -> None:
+    pytest.importorskip("colorspacious")
     lightness = _util.calc_lightness(CMAP_NAME)
     assert isinstance(lightness, np.ndarray)
 
 
+@pytest.mark.skipif(MplFigure is None, reason="matplotlib not installed")
 def test_plot_lightness() -> None:
+    pytest.importorskip("colorspacious")
     fig = _util.plot_lightness(CMAP_NAME)
     assert isinstance(fig, MplFigure)
 
 
 def test_hsv_to_rgb() -> None:
     rgb = _util.hsv_to_rgb([0.5, 0.5, 0.5])
     assert isinstance(rgb, np.ndarray)
@@ -59,12 +68,13 @@
     assert isinstance(ramp, np.ndarray)
 
     ramp = _util.circlesineramp(128)
     assert isinstance(ramp, np.ndarray)
 
 
 def test_report() -> None:
+    pytest.importorskip("colorspacious")
     report = _util.report(CMAP_INSTANCE)
     assert isinstance(report, dict)
 
     report2 = _util.report(Colormap("red"))
     assert isinstance(report2, dict)
```

### Comparing `cmap-0.1.3/.gitignore` & `cmap-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/README.md` & `cmap-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -88,27 +88,35 @@
 
 Note that the input array must be normalized from 0-1, so if you're applying a colormap
 to an integer array (like an image) you must apply any contrast limits and rescale to
 0-1 before passing it to a `Colormap`.
 
 ## Third Party Library Support
 
-The `cmap.Colormap` object has convenience methods that allow it to be used with a number of third-party colormap objects (like
-`matplotlib`, `vispy`, `napari`, `plotly`, etc...).
+The `cmap.Colormap` object has convenience methods that export it to a number of known
+third-party colormap objects, including:
+
+- [matplotlib](https://matplotlib.org/)
+- [napari](https://napari.org/)
+- [vispy](https://vispy.org/)
+- [pygfx](https://pygfx.readthedocs.io/en/latest/) (& [fastplotlib](https://github.com/fastplotlib/fastplotlib))
+- [plotly](https://plotly.com/python/)
+- [bokeh](https://docs.bokeh.org/en/latest/)
+- [altair](https://altair-viz.github.io/)
+- [pyqtgraph](https://www.pyqtgraph.org/)
 
 See [documentation](https://cmap-docs.readthedocs.io/en/latest/colormaps/#usage-with-external-visualization-libraries)
 for details.
 
 If you would like to see support added for a particular library, please open an issue or PR.
 
 ## Alternatives
 
 Other libraries providing colormaps:
 
-
 - [matplotlib](https://matplotlib.org/stable/tutorials/colors/colormaps.html)
 - [seaborn](https://seaborn.pydata.org/tutorial/color_palettes.html)  (subclasses matplotlib)
 - [proplot](https://proplot.readthedocs.io/en/latest/colormaps.html)  (subclasses matplotlib)
 - [palettable](https://jiffyclub.github.io/palettable/) (mostly data, import doesn't depend on matplotlib, but usage largely does)
 - [cmocean](https://matplotlib.org/cmocean/) (mostly data, outputs matplotlib colormaps)
 - [colorcet](https://colorcet.holoviz.org/) (mostly data, usage requires either matplotlib or bokeh)
 - [cmasher](https://cmasher.readthedocs.io/) (requires matplotlib)
@@ -124,8 +132,8 @@
 - [A Better Default Colormap for Matplotlib | SciPy 2015 | Nathaniel Smith and Stéfan van der Walt](https://www.youtube.com/watch?v=xAoljeRJ3lU)
 - blog post for above video: <https://bids.github.io/colormap/>
 - [Origins of Colormaps, Cleve Moler, February 2, 2015](https://blogs.mathworks.com/cleve/2015/02/02/origins-of-colormaps/)
 - [Documenting the matplotlib colormaps, @endolith](https://gist.github.com/endolith/2719900)
 - [Color Map Advice for Scientific Visualization](https://www.kennethmoreland.com/color-advice/)
 - <https://colorcet.com/>, Peter Kovesi
 - [Kovesi: Good Colour Maps: How to Design Them.](https://arxiv.org/abs/1509.03700)
-- https://www.fabiocrameri.ch/colourmaps/
+- <https://www.fabiocrameri.ch/colourmaps/>
```

### Comparing `cmap-0.1.3/pyproject.toml` & `cmap-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,49 +27,51 @@
 [project.license-files]
 globs = ["LICENSE/*"]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 docs = [
-    'mkdocs',
-    'mkdocs-material',
-    'mkdocstrings-python',
-    'mkdocs-minify-plugin',
-    'mkdocs-literate-nav',
-    'mkdocs-gen-files',
+    'colorcet',
     'colorspacious',
     'imageio',
-    'colorcet',
+    'mkdocs-gen-files',
+    'mkdocs-literate-nav',
+    'mkdocs-material',
+    'mkdocs-minify-plugin',
+    'mkdocs',
+    'mkdocstrings-python',
+    'natsort',
 ]
-test = [
-    "pytest>=6.0",
-    "pytest-cov",
-    "numba; python_version<'3.11'",
+test_min = ["pytest>=6.0"]
+test = ["cmap[test_min]", "pytest-cov"]
+test_thirdparty = [
+    "cmap[test]",
+    "numba; python_version<'3.13'",
     "matplotlib",
-]
-thirdparty = [
+    "colorspacious",
     "bokeh",
     "colour",
     "napari",
     "plotly",
     "pydantic",
+    "pydantic-extra-types",
     "pygfx",
     "pytest-qt",
     "rich",
     "viscm",
     "vispy",
+    "pyqtgraph",
 ]
 dev = [
-    "black",
+    "cmap[test_thirdparty]",
     "ipython",
     "mypy",
     "pdbpp",
     "pre-commit",
-    "pytest-cov",
     "pytest",
     "rich",
     "ruff",
 ]
 
 [project.urls]
 Homepage = "https://github.com/tlambert03/cmap"
@@ -86,43 +88,42 @@
 include = ["/src", "/tests", "CHANGELOG.md"]
 
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
 target-version = "py38"
-fix = true
 src = ["src"]
-select = [
-    "E",   # style errors
-    "F",   # flakes
-    "D",   # pydocstyle
-    "I",   # isort
-    "UP",  # pyupgrade
-    "S",   # bandit
-    "C4",  # flake8-comprehensions
-    "B",   # flake8-bugbear
-    "ISC", # implicit-str-concat
-    "TID", # tidy-imports
-    "RUF", # ruff-specific rules
-    "TCH",  # flake8-type-checking
-    "TID",  # flake8-tidy-imports
-]
+
 [tool.ruff.lint]
 pydocstyle = { convention = "numpy" }
-extend-select = [
+select = [
+    "E",    # style errors
+    "F",    # flakes
+    "D",    # pydocstyle
     "D417", # Missing argument descriptions in Docstrings
+    "I",    # isort
+    "UP",   # pyupgrade
+    "S",    # bandit
+    "C4",   # flake8-comprehensions
+    "B",    # flake8-bugbear
+    "ISC",  # implicit-str-concat
+    "TID",  # tidy-imports
+    "RUF",  # ruff-specific rules
+    "TCH",  # flake8-type-checking
+    "TID",  # flake8-tidy-imports
 ]
-extend-ignore = [
+ignore = [
     "D100", # Missing docstring in public module
     "D104", # Missing docstring in public module
     "D401", # First line should be in imperative mood (remove to opt in)
+    "ISC001", # conflicts with formatter
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*.py" = ["D", "S101"]
 "src/cmap/data/**/*.py" = ["E501"]
 "docs/*.py" = ["E501"]
 
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
@@ -131,14 +132,15 @@
 testpaths = ["tests"]
 filterwarnings = [
     "error",
     "ignore:distutils Version classes are deprecated",
     "ignore:`np.bool8` is a deprecated:DeprecationWarning",
     "ignore:datetime.datetime.utcfromtimestamp:DeprecationWarning",
     "ignore::DeprecationWarning:docstring_parser",
+    "ignore:Pyarrow will become a required dependency of pandas",
 ]
 
 # https://mypy.readthedocs.io/en/stable/config_file.html
 [tool.mypy]
 files = "src/**/"
 strict = true
 disallow_any_generics = false
```

### Comparing `cmap-0.1.3/LICENSE/LICENSE` & `cmap-0.2.0/LICENSE/LICENSE`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/LICENSE/LICENSE_CMOCEAN` & `cmap-0.2.0/LICENSE/LICENSE_CMOCEAN`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/LICENSE/LICENSE_COLORBREWER` & `cmap-0.2.0/LICENSE/LICENSE_COLORBREWER`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/LICENSE/LICENSE_CRAMERI` & `cmap-0.2.0/LICENSE/LICENSE_CRAMERI`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/LICENSE/LICENSE_CVIDIS` & `cmap-0.2.0/LICENSE/LICENSE_CVIDIS`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/LICENSE/LICENSE_GLASBEY` & `cmap-0.2.0/LICENSE/LICENSE_GLASBEY`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/LICENSE/LICENSE_WISTIA` & `cmap-0.2.0/LICENSE/LICENSE_WISTIA`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/LICENSE/LICENSE_YORICK` & `cmap-0.2.0/LICENSE/LICENSE_YORICK`

 * *Files identical despite different names*

### Comparing `cmap-0.1.3/PKG-INFO` & `cmap-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,95 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cmap
-Version: 0.1.3
+Version: 0.2.0
 Summary: Scientific colormaps for python, without dependencies
 Project-URL: Homepage, https://github.com/tlambert03/cmap
 Project-URL: Repository, https://github.com/tlambert03/cmap
 Project-URL: Bug Tracker, https://github.com/tlambert03/cmap/issues
 Project-URL: Documentation, https://cmap-docs.rtfd.io/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE/LICENSE
 License-File: LICENSE/LICENSE_CMOCEAN
 License-File: LICENSE/LICENSE_COLORBREWER
 License-File: LICENSE/LICENSE_COLORCET
 License-File: LICENSE/LICENSE_CRAMERI
 License-File: LICENSE/LICENSE_CVIDIS
 License-File: LICENSE/LICENSE_GLASBEY
+License-File: LICENSE/LICENSE_TOL
 License-File: LICENSE/LICENSE_WISTIA
 License-File: LICENSE/LICENSE_YORICK
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: numpy
 Provides-Extra: dev
-Requires-Dist: black; extra == 'dev'
+Requires-Dist: bokeh; extra == 'dev'
+Requires-Dist: colorspacious; extra == 'dev'
+Requires-Dist: colour; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
+Requires-Dist: matplotlib; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: napari; extra == 'dev'
+Requires-Dist: numba; (python_version < '3.13') and extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
+Requires-Dist: plotly; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pydantic; extra == 'dev'
+Requires-Dist: pydantic-extra-types; extra == 'dev'
+Requires-Dist: pygfx; extra == 'dev'
+Requires-Dist: pyqtgraph; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-qt; extra == 'dev'
+Requires-Dist: pytest>=6.0; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: viscm; extra == 'dev'
+Requires-Dist: vispy; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: colorcet; extra == 'docs'
 Requires-Dist: colorspacious; extra == 'docs'
 Requires-Dist: imageio; extra == 'docs'
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-gen-files; extra == 'docs'
 Requires-Dist: mkdocs-literate-nav; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocs-minify-plugin; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
+Requires-Dist: natsort; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: matplotlib; extra == 'test'
-Requires-Dist: numba; python_version < '3.11' and extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
-Provides-Extra: thirdparty
-Requires-Dist: bokeh; extra == 'thirdparty'
-Requires-Dist: colour; extra == 'thirdparty'
-Requires-Dist: napari; extra == 'thirdparty'
-Requires-Dist: plotly; extra == 'thirdparty'
-Requires-Dist: pydantic; extra == 'thirdparty'
-Requires-Dist: pygfx; extra == 'thirdparty'
-Requires-Dist: pytest-qt; extra == 'thirdparty'
-Requires-Dist: rich; extra == 'thirdparty'
-Requires-Dist: viscm; extra == 'thirdparty'
-Requires-Dist: vispy; extra == 'thirdparty'
+Provides-Extra: test-min
+Requires-Dist: pytest>=6.0; extra == 'test-min'
+Provides-Extra: test-thirdparty
+Requires-Dist: bokeh; extra == 'test-thirdparty'
+Requires-Dist: colorspacious; extra == 'test-thirdparty'
+Requires-Dist: colour; extra == 'test-thirdparty'
+Requires-Dist: matplotlib; extra == 'test-thirdparty'
+Requires-Dist: napari; extra == 'test-thirdparty'
+Requires-Dist: numba; (python_version < '3.13') and extra == 'test-thirdparty'
+Requires-Dist: plotly; extra == 'test-thirdparty'
+Requires-Dist: pydantic; extra == 'test-thirdparty'
+Requires-Dist: pydantic-extra-types; extra == 'test-thirdparty'
+Requires-Dist: pygfx; extra == 'test-thirdparty'
+Requires-Dist: pyqtgraph; extra == 'test-thirdparty'
+Requires-Dist: pytest-cov; extra == 'test-thirdparty'
+Requires-Dist: pytest-qt; extra == 'test-thirdparty'
+Requires-Dist: pytest>=6.0; extra == 'test-thirdparty'
+Requires-Dist: rich; extra == 'test-thirdparty'
+Requires-Dist: viscm; extra == 'test-thirdparty'
+Requires-Dist: vispy; extra == 'test-thirdparty'
 Description-Content-Type: text/markdown
 
 # cmap
 
 [![License](https://img.shields.io/pypi/l/cmap.svg?color=green)](https://github.com/tlambert03/cmap/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/cmap.svg?color=green)](https://pypi.org/project/cmap)
 ![Conda](https://img.shields.io/conda/v/conda-forge/cmap)
@@ -155,27 +178,35 @@
 
 Note that the input array must be normalized from 0-1, so if you're applying a colormap
 to an integer array (like an image) you must apply any contrast limits and rescale to
 0-1 before passing it to a `Colormap`.
 
 ## Third Party Library Support
 
-The `cmap.Colormap` object has convenience methods that allow it to be used with a number of third-party colormap objects (like
-`matplotlib`, `vispy`, `napari`, `plotly`, etc...).
+The `cmap.Colormap` object has convenience methods that export it to a number of known
+third-party colormap objects, including:
+
+- [matplotlib](https://matplotlib.org/)
+- [napari](https://napari.org/)
+- [vispy](https://vispy.org/)
+- [pygfx](https://pygfx.readthedocs.io/en/latest/) (& [fastplotlib](https://github.com/fastplotlib/fastplotlib))
+- [plotly](https://plotly.com/python/)
+- [bokeh](https://docs.bokeh.org/en/latest/)
+- [altair](https://altair-viz.github.io/)
+- [pyqtgraph](https://www.pyqtgraph.org/)
 
 See [documentation](https://cmap-docs.readthedocs.io/en/latest/colormaps/#usage-with-external-visualization-libraries)
 for details.
 
 If you would like to see support added for a particular library, please open an issue or PR.
 
 ## Alternatives
 
 Other libraries providing colormaps:
 
-
 - [matplotlib](https://matplotlib.org/stable/tutorials/colors/colormaps.html)
 - [seaborn](https://seaborn.pydata.org/tutorial/color_palettes.html)  (subclasses matplotlib)
 - [proplot](https://proplot.readthedocs.io/en/latest/colormaps.html)  (subclasses matplotlib)
 - [palettable](https://jiffyclub.github.io/palettable/) (mostly data, import doesn't depend on matplotlib, but usage largely does)
 - [cmocean](https://matplotlib.org/cmocean/) (mostly data, outputs matplotlib colormaps)
 - [colorcet](https://colorcet.holoviz.org/) (mostly data, usage requires either matplotlib or bokeh)
 - [cmasher](https://cmasher.readthedocs.io/) (requires matplotlib)
@@ -191,8 +222,8 @@
 - [A Better Default Colormap for Matplotlib | SciPy 2015 | Nathaniel Smith and Stéfan van der Walt](https://www.youtube.com/watch?v=xAoljeRJ3lU)
 - blog post for above video: <https://bids.github.io/colormap/>
 - [Origins of Colormaps, Cleve Moler, February 2, 2015](https://blogs.mathworks.com/cleve/2015/02/02/origins-of-colormaps/)
 - [Documenting the matplotlib colormaps, @endolith](https://gist.github.com/endolith/2719900)
 - [Color Map Advice for Scientific Visualization](https://www.kennethmoreland.com/color-advice/)
 - <https://colorcet.com/>, Peter Kovesi
 - [Kovesi: Good Colour Maps: How to Design Them.](https://arxiv.org/abs/1509.03700)
-- https://www.fabiocrameri.ch/colourmaps/
+- <https://www.fabiocrameri.ch/colourmaps/>
```

