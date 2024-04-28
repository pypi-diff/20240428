# Comparing `tmp/tubeulator-0.0.6.tar.gz` & `tmp/tubeulator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubeulator-0.0.6.tar", last modified: Wed Mar 27 07:49:30 2024, max compression
+gzip compressed data, was "tubeulator-0.0.7.tar", last modified: Sun Apr 28 15:21:43 2024, max compression
```

## Comparing `tubeulator-0.0.6.tar` & `tubeulator-0.0.7.tar`

### file list

```diff
@@ -1,887 +1,897 @@
--rw-r--r--   0        0        0    12107 2024-03-25 09:22:31.141989 tubeulator-0.0.6/README.md
--rw-r--r--   0        0        0     1614 2024-03-27 07:49:30.266607 tubeulator-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      130 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/__init__.py
--rw-r--r--   0        0        0      169 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/api/__init__.py
--rw-r--r--   0        0        0       76 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/api/endpoint/__init__.py
--rw-r--r--   0        0        0      541 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/api/endpoint/names.py
--rw-r--r--   0        0        0     1225 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/__init__.py
--rw-r--r--   0        0        0      189 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/accident.py
--rw-r--r--   0        0        0      138 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/air.py
--rw-r--r--   0        0        0      877 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/bike.py
--rw-r--r--   0        0        0      357 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/crowding.py
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/disruption_lifts.py
--rw-r--r--   0        0        0      395 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/journey.py
--rw-r--r--   0        0        0     3015 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/line.py
--rw-r--r--   0        0        0      313 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/mode.py
--rw-r--r--   0        0        0      588 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/occupancy.py
--rw-r--r--   0        0        0     1331 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/place.py
--rw-r--r--   0        0        0      987 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/road.py
--rw-r--r--   0        0        0      674 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/search.py
--rw-r--r--   0        0        0     2941 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/stop.py
--rw-r--r--   0        0        0      415 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/types.py
--rw-r--r--   0        0        0      390 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/vehicle.py
--rw-r--r--   0        0        0      784 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/api/interface.py
--rw-r--r--   0        0        0    18434 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/api/request.py
--rw-r--r--   0        0        0     1920 2024-03-27 07:47:40.886912 tubeulator-0.0.6/src/tubeulator/cli.py
--rw-r--r--   0        0        0        0 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/codegen/__init__.py
--rw-r--r--   0        0        0      119 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/codegen/gen/__init__.py
--rw-r--r--   0        0        0    13343 2024-03-27 07:47:40.886912 tubeulator-0.0.6/src/tubeulator/codegen/gen/dto.py
--rw-r--r--   0        0        0     2851 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/codegen/gen/emit.py
--rw-r--r--   0        0        0      566 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/codegen/gen/helpers.py
--rw-r--r--   0        0        0      735 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/codegen/gen/jsonschema.py
--rw-r--r--   0        0        0     2203 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/codegen/gen/resolution.py
--rw-r--r--   0        0        0      538 2024-03-25 01:25:47.183790 tubeulator-0.0.6/src/tubeulator/codegen/load_test.py
--rw-r--r--   0        0        0      658 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/codegen/populate.py
--rw-r--r--   0        0        0    10306 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/AccidentStats.json
--rw-r--r--   0        0        0      812 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/accidentdetail.json
--rw-r--r--   0        0        0      683 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/all.json
--rw-r--r--   0        0        0      344 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/casualty.json
--rw-r--r--   0        0        0      164 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-1.json
--rw-r--r--   0        0        0      164 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-2.json
--rw-r--r--   0        0        0      164 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-3.json
--rw-r--r--   0        0        0      164 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray.json
--rw-r--r--   0        0        0      135 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/vehicle.json
--rw-r--r--   0        0        0     2473 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AirQuality/AirQuality.json
--rw-r--r--   0        0        0       67 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AirQuality/schemas/all.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/AirQuality/schemas/object.json
--rw-r--r--   0        0        0    12586 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/BikePoint.json
--rw-r--r--   0        0        0      359 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/additionalproperties.json
--rw-r--r--   0        0        0      788 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/all.json
--rw-r--r--   0        0        0     1491 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/place.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-1.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-2.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-3.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-4.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-5.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-6.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-7.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.187790 tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray.json
--rw-r--r--   0        0        0     3569 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Disruptions-Lifts-v2/Disruptions-Lifts-v2.json
--rw-r--r--   0        0        0      132 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/all.json
--rw-r--r--   0        0        0      120 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      828 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/liftdisruption.json
--rw-r--r--   0        0        0    64106 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/Journey.json
--rw-r--r--   0        0        0     1988 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/all.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/metamodesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/metamodesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/metamodesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/metamodesget200textxmlresponse.json
--rw-r--r--   0        0        0      873 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-10.json
--rw-r--r--   0        0        0      620 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-11.json
--rw-r--r--   0        0        0      350 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-12.json
--rw-r--r--   0        0        0      424 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-13.json
--rw-r--r--   0        0        0      307 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-14.json
--rw-r--r--   0        0        0      243 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-15.json
--rw-r--r--   0        0        0      359 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-16.json
--rw-r--r--   0        0        0     1418 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-17.json
--rw-r--r--   0        0        0     2645 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-18.json
--rw-r--r--   0        0        0      218 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-19.json
--rw-r--r--   0        0        0      180 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-2.json
--rw-r--r--   0        0        0     1362 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-20.json
--rw-r--r--   0        0        0     1892 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-21.json
--rw-r--r--   0        0        0      355 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-22.json
--rw-r--r--   0        0        0     1294 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-23.json
--rw-r--r--   0        0        0      464 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-24.json
--rw-r--r--   0        0        0      194 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-25.json
--rw-r--r--   0        0        0      711 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-26.json
--rw-r--r--   0        0        0      179 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-27.json
--rw-r--r--   0        0        0      368 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-28.json
--rw-r--r--   0        0        0      561 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-29.json
--rw-r--r--   0        0        0     1324 2024-03-25 01:25:47.191790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-3.json
--rw-r--r--   0        0        0      550 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-30.json
--rw-r--r--   0        0        0      714 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-31.json
--rw-r--r--   0        0        0     1335 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-32.json
--rw-r--r--   0        0        0      178 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-33.json
--rw-r--r--   0        0        0      858 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-34.json
--rw-r--r--   0        0        0      552 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-35.json
--rw-r--r--   0        0        0      268 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-36.json
--rw-r--r--   0        0        0      297 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-37.json
--rw-r--r--   0        0        0      345 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-38.json
--rw-r--r--   0        0        0      263 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-39.json
--rw-r--r--   0        0        0      285 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-4.json
--rw-r--r--   0        0        0      743 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-40.json
--rw-r--r--   0        0        0      302 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-5.json
--rw-r--r--   0        0        0      453 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-6.json
--rw-r--r--   0        0        0      378 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-7.json
--rw-r--r--   0        0        0     1062 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-8.json
--rw-r--r--   0        0        0      511 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-9.json
--rw-r--r--   0        0        0      304 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl.json
--rw-r--r--   0        0        0   232588 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/Line.json
--rw-r--r--   0        0        0     7137 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/all.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.195790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-routeget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-routeget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-routeget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-routeget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-statusget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-statusget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-statusget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/ids-statusget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metamodesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metamodesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metamodesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metamodesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.199790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metaseverityget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metaseverityget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metaseverityget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/metaseverityget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/routeget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/routeget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/routeget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/routeget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/status-severity-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/status-severity-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/status-severity-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/status-severity-get200textxmlresponse.json
--rw-r--r--   0        0        0     1417 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-10.json
--rw-r--r--   0        0        0     2641 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-11.json
--rw-r--r--   0        0        0      218 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-12.json
--rw-r--r--   0        0        0     1362 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-13.json
--rw-r--r--   0        0        0     1892 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-14.json
--rw-r--r--   0        0        0      550 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-15.json
--rw-r--r--   0        0        0      714 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-16.json
--rw-r--r--   0        0        0     1335 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-17.json
--rw-r--r--   0        0        0      178 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-18.json
--rw-r--r--   0        0        0      858 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-19.json
--rw-r--r--   0        0        0      269 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-2.json
--rw-r--r--   0        0        0     1221 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-20.json
--rw-r--r--   0        0        0     1232 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-21.json
--rw-r--r--   0        0        0      285 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-22.json
--rw-r--r--   0        0        0      762 2024-03-25 01:25:47.203790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-23.json
--rw-r--r--   0        0        0      477 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-24.json
--rw-r--r--   0        0        0      159 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-25.json
--rw-r--r--   0        0        0      829 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-26.json
--rw-r--r--   0        0        0      244 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-27.json
--rw-r--r--   0        0        0      216 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-28.json
--rw-r--r--   0        0        0      237 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-29.json
--rw-r--r--   0        0        0      378 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-3.json
--rw-r--r--   0        0        0      257 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-30.json
--rw-r--r--   0        0        0      181 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-31.json
--rw-r--r--   0        0        0      254 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-32.json
--rw-r--r--   0        0        0      408 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-33.json
--rw-r--r--   0        0        0      458 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-34.json
--rw-r--r--   0        0        0      306 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-35.json
--rw-r--r--   0        0        0      247 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-36.json
--rw-r--r--   0        0        0      185 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-37.json
--rw-r--r--   0        0        0      207 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-38.json
--rw-r--r--   0        0        0      654 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-39.json
--rw-r--r--   0        0        0     1062 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-4.json
--rw-r--r--   0        0        0      529 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-40.json
--rw-r--r--   0        0        0     2708 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-41.json
--rw-r--r--   0        0        0      511 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-5.json
--rw-r--r--   0        0        0      873 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-6.json
--rw-r--r--   0        0        0      307 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-7.json
--rw-r--r--   0        0        0      243 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-8.json
--rw-r--r--   0        0        0      359 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-9.json
--rw-r--r--   0        0        0      304 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl.json
--rw-r--r--   0        0        0    19274 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/Mode.json
--rw-r--r--   0        0        0      186 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/activeservicetype.json
--rw-r--r--   0        0        0      939 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/all.json
--rw-r--r--   0        0        0     2748 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/prediction.json
--rw-r--r--   0        0        0      529 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/predictiontiming.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-1.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-2.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-3.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-4.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-5.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-6.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.207790 tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-7.json
--rw-r--r--   0        0        0    42059 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/Place.json
--rw-r--r--   0        0        0     2157 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/all.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/get200applicationjsonresponse-1.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/get200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/id-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/id-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/id-get200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/id-get200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/searchget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/searchget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/searchget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/searchget200textxmlresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/system.json
--rw-r--r--   0        0        0     2640 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-10.json
--rw-r--r--   0        0        0      359 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-2.json
--rw-r--r--   0        0        0     1416 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-3.json
--rw-r--r--   0        0        0      378 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-4.json
--rw-r--r--   0        0        0     1062 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-5.json
--rw-r--r--   0        0        0      511 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-6.json
--rw-r--r--   0        0        0      873 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-7.json
--rw-r--r--   0        0        0      307 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-8.json
--rw-r--r--   0        0        0      243 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-9.json
--rw-r--r--   0        0        0      242 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/type-types-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/type-types-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/type-types-get200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/type-types-get200textxmlresponse.json
--rw-r--r--   0        0        0      822 2024-03-25 01:25:47.211790 tubeulator-0.0.6/src/tubeulator/data/openapi/README.md
--rw-r--r--   0        0        0   112822 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/Road.json
--rw-r--r--   0        0        0     2250 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/all.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/get200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/get200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/get200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationgeo-jsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-statusget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-statusget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-statusget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/ids-statusget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200textxmlresponse.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/system-2.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/system-3.json
--rw-r--r--   0        0        0      307 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/system.json
--rw-r--r--   0        0        0      813 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-2.json
--rw-r--r--   0        0        0     1501 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-3.json
--rw-r--r--   0        0        0     1358 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-4.json
--rw-r--r--   0        0        0      579 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-5.json
--rw-r--r--   0        0        0      519 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-6.json
--rw-r--r--   0        0        0      245 2024-03-25 01:25:47.215790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-7.json
--rw-r--r--   0        0        0     5927 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-8.json
--rw-r--r--   0        0        0      269 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-9.json
--rw-r--r--   0        0        0     1958 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl.json
--rw-r--r--   0        0        0    20177 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/Search.json
--rw-r--r--   0        0        0      985 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/all.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metasortsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metasortsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metasortsget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/metasortsget200textxmlresponse.json
--rw-r--r--   0        0        0      642 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/tfl-2.json
--rw-r--r--   0        0        0      358 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/tfl.json
--rw-r--r--   0        0        0   137945 2024-03-27 07:47:40.886912 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/StopPoint.json
--rw-r--r--   0        0        0     6467 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/all.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.219790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200textxmlresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200applicationjsonresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200applicationxmlresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200textjsonresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.223790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200textxmlresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/system.json
--rw-r--r--   0        0        0     1417 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-10.json
--rw-r--r--   0        0        0     2641 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-11.json
--rw-r--r--   0        0        0      178 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-12.json
--rw-r--r--   0        0        0      209 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-13.json
--rw-r--r--   0        0        0      258 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-14.json
--rw-r--r--   0        0        0      529 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-15.json
--rw-r--r--   0        0        0     2708 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-16.json
--rw-r--r--   0        0        0     1869 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-17.json
--rw-r--r--   0        0        0      755 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-18.json
--rw-r--r--   0        0        0      646 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-19.json
--rw-r--r--   0        0        0      304 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-2.json
--rw-r--r--   0        0        0      967 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-20.json
--rw-r--r--   0        0        0      358 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-21.json
--rw-r--r--   0        0        0      645 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-22.json
--rw-r--r--   0        0        0      378 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-3.json
--rw-r--r--   0        0        0     1062 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-4.json
--rw-r--r--   0        0        0      511 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-5.json
--rw-r--r--   0        0        0      873 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-6.json
--rw-r--r--   0        0        0      307 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-7.json
--rw-r--r--   0        0        0      243 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-8.json
--rw-r--r--   0        0        0      359 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-9.json
--rw-r--r--   0        0        0      242 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200textxmlresponse.json
--rw-r--r--   0        0        0    15378 2024-03-27 07:47:40.886912 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/Vehicle.json
--rw-r--r--   0        0        0      425 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/all.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.227790 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200textxmlresponse.json
--rw-r--r--   0        0        0     2705 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/tfl-2.json
--rw-r--r--   0        0        0      495 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/tfl-3.json
--rw-r--r--   0        0        0      529 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/tfl.json
--rw-r--r--   0        0        0     3579 2024-03-27 07:47:40.886912 tubeulator-0.0.6/src/tubeulator/data/openapi/crowding/crowding.json
--rw-r--r--   0        0        0     5361 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/error_inventory.md
--rw-r--r--   0        0        0    11496 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/namespace.json
--rw-r--r--   0        0        0     7685 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/naming.md
--rw-r--r--   0        0        0    24650 2024-03-27 07:47:40.886912 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/occupancy.json
--rw-r--r--   0        0        0     1365 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/all.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/carparkget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/carparkget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/carparkget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/carparkget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200textxmlresponse.json
--rw-r--r--   0        0        0      330 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/tfl-2.json
--rw-r--r--   0        0        0      360 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/tfl-3.json
--rw-r--r--   0        0        0      697 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/tfl-4.json
--rw-r--r--   0        0        0      356 2024-03-25 01:25:47.231790 tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/tfl.json
--rw-r--r--   0        0        0     1503 2024-03-27 07:47:40.886912 tubeulator-0.0.6/src/tubeulator/data/openapi/stationdata/stationdata.json
--rw-r--r--   0        0        0   676093 2024-03-25 01:25:47.235790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/ReleasedUnifiedAPIProd.json
--rw-r--r--   0        0        0      812 2024-03-25 01:25:47.235790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentdetail.json
--rw-r--r--   0        0        0      283 2024-03-25 01:25:47.235790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentstatsorderedsummary.json
--rw-r--r--   0        0        0      186 2024-03-25 01:25:47.235790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/activeservicetype.json
--rw-r--r--   0        0        0      359 2024-03-25 01:25:47.235790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/additionalproperties.json
--rw-r--r--   0        0        0    29934 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/all.json
--rw-r--r--   0        0        0      361 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/apiversioninfo.json
--rw-r--r--   0        0        0     1909 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/arrivaldeparture.json
--rw-r--r--   0        0        0      356 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bay.json
--rw-r--r--   0        0        0      697 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bikepointoccupancy.json
--rw-r--r--   0        0        0      360 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/carparkoccupancy.json
--rw-r--r--   0        0        0      344 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/casualty.json
--rw-r--r--   0        0        0      360 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/chargeconnectoroccupancy.json
--rw-r--r--   0        0        0      531 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/coordinate.json
--rw-r--r--   0        0        0      586 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/crowding.json
--rw-r--r--   0        0        0     1378 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/cyclesuperhighway.json
--rw-r--r--   0        0        0      245 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/daterange.json
--rw-r--r--   0        0        0      245 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/daterangenullable.json
--rw-r--r--   0        0        0      184 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/dbgeography.json
--rw-r--r--   0        0        0      307 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/dbgeographywellknownvalue.json
--rw-r--r--   0        0        0      262 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disambiguation.json
--rw-r--r--   0        0        0      185 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disambiguationoption.json
--rw-r--r--   0        0        0      646 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruptedpoint.json
--rw-r--r--   0        0        0     1961 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruption.json
--rw-r--r--   0        0        0      757 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/fare.json
--rw-r--r--   0        0        0      860 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farebounds.json
--rw-r--r--   0        0        0      179 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farecaveat.json
--rw-r--r--   0        0        0     1483 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faredetails.json
--rw-r--r--   0        0        0      254 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faresmode.json
--rw-r--r--   0        0        0      443 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faresperiod.json
--rw-r--r--   0        0        0      571 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faressection.json
--rw-r--r--   0        0        0      364 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farestation.json
--rw-r--r--   0        0        0      247 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faretap.json
--rw-r--r--   0        0        0      464 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faretapdetails.json
--rw-r--r--   0        0        0      695 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geocodesearchmatch.json
--rw-r--r--   0        0        0      271 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geopoint.json
--rw-r--r--   0        0        0      877 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/identifier.json
--rw-r--r--   0        0        0      325 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instruction.json
--rw-r--r--   0        0        0     1362 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instructionstep.json
--rw-r--r--   0        0        0      216 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/interval.json
--rw-r--r--   0        0        0     1002 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/itineraryresult.json
--rw-r--r--   0        0        0      653 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journey.json
--rw-r--r--   0        0        0      460 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyfare.json
--rw-r--r--   0        0        0      552 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyplannercyclehiredockingstationdata.json
--rw-r--r--   0        0        0      263 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyvector.json
--rw-r--r--   0        0        0      620 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/jpelevation.json
--rw-r--r--   0        0        0      257 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/knownjourney.json
--rw-r--r--   0        0        0     1649 2024-03-25 01:25:47.239790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/leg.json
--rw-r--r--   0        0        0     1038 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/line.json
--rw-r--r--   0        0        0      307 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linegroup.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      243 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemodegroup.json
--rw-r--r--   0        0        0      477 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineroutesection.json
--rw-r--r--   0        0        0      305 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineservicetype.json
--rw-r--r--   0        0        0      178 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineservicetypeinfo.json
--rw-r--r--   0        0        0      252 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linespecificservicetype.json
--rw-r--r--   0        0        0      786 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linestatus.json
--rw-r--r--   0        0        0     1335 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroute.json
--rw-r--r--   0        0        0      159 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroutesections.json
--rw-r--r--   0        0        0     1256 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedstop.json
--rw-r--r--   0        0        0      357 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/message.json
--rw-r--r--   0        0        0      304 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/mode.json
--rw-r--r--   0        0        0      361 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/networkstatus.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/object.json
--rw-r--r--   0        0        0      302 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/obstacle.json
--rw-r--r--   0        0        0      285 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/orderedroute.json
--rw-r--r--   0        0        0      378 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/passengerflow.json
--rw-r--r--   0        0        0      315 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/passengertype.json
--rw-r--r--   0        0        0      419 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/path.json
--rw-r--r--   0        0        0      180 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/pathattribute.json
--rw-r--r--   0        0        0      542 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/period.json
--rw-r--r--   0        0        0     1491 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/place.json
--rw-r--r--   0        0        0      242 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placecategory.json
--rw-r--r--   0        0        0      513 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placegeo.json
--rw-r--r--   0        0        0      262 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placepolygon.json
--rw-r--r--   0        0        0      355 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/plannedwork.json
--rw-r--r--   0        0        0      453 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/point.json
--rw-r--r--   0        0        0      403 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/postcodeinput.json
--rw-r--r--   0        0        0     2748 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/prediction.json
--rw-r--r--   0        0        0      529 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/predictiontiming.json
--rw-r--r--   0        0        0     1340 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendation.json
--rw-r--r--   0        0        0      245 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendationresponse.json
--rw-r--r--   0        0        0      233 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/redirect.json
--rw-r--r--   0        0        0     1958 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadcorridor.json
--rw-r--r--   0        0        0     6179 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruption.json
--rw-r--r--   0        0        0      542 2024-03-25 01:25:47.243790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionimpactarea.json
--rw-r--r--   0        0        0      602 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionline.json
--rw-r--r--   0        0        0      245 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionschedule.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0     1358 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadproject.json
--rw-r--r--   0        0        0      458 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routeoption.json
--rw-r--r--   0        0        0      948 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchmatch.json
--rw-r--r--   0        0        0      284 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchresponse.json
--rw-r--r--   0        0        0     1417 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesection.json
--rw-r--r--   0        0        0      251 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesectionnaptanentrysequence.json
--rw-r--r--   0        0        0      874 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesequence.json
--rw-r--r--   0        0        0      596 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/schedule.json
--rw-r--r--   0        0        0      399 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchcriteria.json
--rw-r--r--   0        0        0      358 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmatch.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200textxmlresponse.json
--rw-r--r--   0        0        0      680 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchresponse.json
--rw-r--r--   0        0        0      254 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/servicefrequency.json
--rw-r--r--   0        0        0      269 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stationinterval.json
--rw-r--r--   0        0        0      269 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/statusseverity.json
--rw-r--r--   0        0        0     2822 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppoint.json
--rw-r--r--   0        0        0      242 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointcategory.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200applicationjsonresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200applicationxmlresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200textjsonresponse.json
--rw-r--r--   0        0        0       69 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200textxmlresponse.json
--rw-r--r--   0        0        0      755 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointroutesection.json
--rw-r--r--   0        0        0     1267 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsequence.json
--rw-r--r--   0        0        0     1000 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsresponse.json
--rw-r--r--   0        0        0     1539 2024-03-25 01:25:47.247790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/street.json
--rw-r--r--   0        0        0      813 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/streetsegment.json
--rw-r--r--   0        0        0      164 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-1.json
--rw-r--r--   0        0        0      164 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-2.json
--rw-r--r--   0        0        0      164 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-3.json
--rw-r--r--   0        0        0      164 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-1.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-2.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-3.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray.json
--rw-r--r--   0        0        0      152 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-1.json
--rw-r--r--   0        0        0      152 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-2.json
--rw-r--r--   0        0        0      152 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-3.json
--rw-r--r--   0        0        0      152 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray.json
--rw-r--r--   0        0        0      154 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-1.json
--rw-r--r--   0        0        0      154 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-2.json
--rw-r--r--   0        0        0      154 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-3.json
--rw-r--r--   0        0        0      154 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray.json
--rw-r--r--   0        0        0      152 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-1.json
--rw-r--r--   0        0        0      152 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-2.json
--rw-r--r--   0        0        0      152 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-3.json
--rw-r--r--   0        0        0      152 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray.json
--rw-r--r--   0        0        0      160 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-1.json
--rw-r--r--   0        0        0      160 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-2.json
--rw-r--r--   0        0        0      160 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-3.json
--rw-r--r--   0        0        0      160 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-4.json
--rw-r--r--   0        0        0      160 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-5.json
--rw-r--r--   0        0        0      160 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-6.json
--rw-r--r--   0        0        0      160 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-7.json
--rw-r--r--   0        0        0      160 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-1.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-2.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-3.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-4.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-5.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-6.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-7.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-1.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-2.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-3.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-4.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-5.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-6.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-7.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.251790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-1.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-10.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-11.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-12.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-13.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-14.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-15.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-16.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-17.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-18.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-19.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-2.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-20.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-21.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-22.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-23.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-24.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-25.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-26.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-27.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-28.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-29.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-3.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-30.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-31.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-32.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-33.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-34.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-35.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-4.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-5.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-6.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-7.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-8.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-9.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray.json
--rw-r--r--   0        0        0      151 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-1.json
--rw-r--r--   0        0        0      151 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-2.json
--rw-r--r--   0        0        0      151 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-3.json
--rw-r--r--   0        0        0      151 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-1.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-10.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-11.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-2.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-3.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-4.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.255790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-5.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-6.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-7.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-8.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-9.json
--rw-r--r--   0        0        0      140 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-1.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-10.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-11.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-12.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-13.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-14.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-15.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-16.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-17.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-18.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-19.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-2.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-20.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-21.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-22.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-23.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-24.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-25.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-26.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-27.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-28.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-29.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-3.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-30.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-31.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-4.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-5.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-6.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-7.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-8.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-9.json
--rw-r--r--   0        0        0      141 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray.json
--rw-r--r--   0        0        0      149 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-1.json
--rw-r--r--   0        0        0      149 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-2.json
--rw-r--r--   0        0        0      149 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-3.json
--rw-r--r--   0        0        0      149 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-4.json
--rw-r--r--   0        0        0      149 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-5.json
--rw-r--r--   0        0        0      149 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-6.json
--rw-r--r--   0        0        0      149 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-7.json
--rw-r--r--   0        0        0      149 2024-03-25 01:25:47.259790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-1.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-10.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-11.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-12.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-13.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-14.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-15.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-2.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-3.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-4.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-5.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-6.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-7.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-8.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-9.json
--rw-r--r--   0        0        0      146 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-1.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-10.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-11.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-2.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-3.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-4.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-5.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-6.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-7.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-8.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-9.json
--rw-r--r--   0        0        0      148 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-1.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-2.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-3.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-4.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-1.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-2.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-3.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-4.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-5.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-6.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-7.json
--rw-r--r--   0        0        0      150 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-1.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-10.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-11.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-12.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.263790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-13.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-14.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-15.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-16.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-17.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-18.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-19.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-2.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-20.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-21.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-22.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-23.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-24.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-25.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-26.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-27.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-3.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-4.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-5.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-6.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-7.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-8.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-9.json
--rw-r--r--   0        0        0      145 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-1.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-2.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-3.json
--rw-r--r--   0        0        0      153 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray.json
--rw-r--r--   0        0        0      157 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-1.json
--rw-r--r--   0        0        0      157 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-2.json
--rw-r--r--   0        0        0      157 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-3.json
--rw-r--r--   0        0        0      157 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray.json
--rw-r--r--   0        0        0      685 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/ticket.json
--rw-r--r--   0        0        0      186 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tickettime.json
--rw-r--r--   0        0        0      186 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tickettype.json
--rw-r--r--   0        0        0      268 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timeadjustment.json
--rw-r--r--   0        0        0      509 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timeadjustments.json
--rw-r--r--   0        0        0      285 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetable.json
--rw-r--r--   0        0        0      806 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableresponse.json
--rw-r--r--   0        0        0      377 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableroute.json
--rw-r--r--   0        0        0     1062 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/trainloading.json
--rw-r--r--   0        0        0      181 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/twentyfourhourclocktime.json
--rw-r--r--   0        0        0      550 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/validityperiod.json
--rw-r--r--   0        0        0      135 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/vehicle.json
--rw-r--r--   0        0        0      495 2024-03-25 01:25:47.267790 tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/vehiclematch.json
--rw-r--r--   0        0        0      126 2024-03-27 07:47:40.886912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/FeedInfo.csv
--rw-r--r--   0        0        0    54508 2024-03-27 07:47:40.890912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/Lifts.csv
--rw-r--r--   0        0        0      347 2024-03-27 07:47:40.890912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/ModesAndLines.csv
--rw-r--r--   0        0        0   168607 2024-03-27 07:47:40.890912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/PlatformServices.csv
--rw-r--r--   0        0        0   145838 2024-03-27 07:47:40.890912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/Platforms.csv
--rw-r--r--   0        0        0    20909 2024-03-27 07:47:40.894912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/RampRoutes.csv
--rw-r--r--   0        0        0   389058 2024-03-27 07:47:40.894912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/SameLevelPaths.csv
--rw-r--r--   0        0        0   273465 2024-03-27 07:47:40.898912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/StationPoints.csv
--rw-r--r--   0        0        0    37832 2024-03-27 07:47:40.898912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/Stations.csv
--rw-r--r--   0        0        0     8344 2024-03-27 07:47:40.898912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/StepFreeIntechangeInfo.csv
--rw-r--r--   0        0        0    28533 2024-03-27 07:47:40.898912 tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/Toilets.csv
--rw-r--r--   0        0        0      119 2024-03-27 07:47:40.898912 tubeulator-0.0.6/src/tubeulator/data/stationdata/gtfs/feed_info.csv
--rw-r--r--   0        0        0      135 2024-03-27 07:47:40.898912 tubeulator-0.0.6/src/tubeulator/data/stationdata/gtfs/levels.csv
--rw-r--r--   0        0        0   548638 2024-03-27 07:47:40.902912 tubeulator-0.0.6/src/tubeulator/data/stationdata/gtfs/pathways.csv
--rw-r--r--   0        0        0   430539 2024-03-27 07:47:40.906912 tubeulator-0.0.6/src/tubeulator/data/stationdata/gtfs/stops.csv
--rw-r--r--   0        0        0        0 2024-03-25 01:25:47.271790 tubeulator-0.0.6/src/tubeulator/db/__init__.py
--rw-r--r--   0        0        0     2290 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/db/mongod.py
--rw-r--r--   0        0        0     1332 2024-03-25 01:25:47.271790 tubeulator-0.0.6/src/tubeulator/db/store_creds.py
--rw-r--r--   0        0        0      722 2024-03-25 09:22:31.145989 tubeulator-0.0.6/src/tubeulator/exc.py
--rw-r--r--   0        0        0     2937 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/AccidentStats.py
--rw-r--r--   0        0        0      699 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/AirQuality.py
--rw-r--r--   0        0        0     2217 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/BikePoint.py
--rw-r--r--   0        0        0     1469 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/DisruptionsLiftsv2.py
--rw-r--r--   0        0        0    25751 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/Journey.py
--rw-r--r--   0        0        0    36477 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/Line.py
--rw-r--r--   0        0        0     3711 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/Mode.py
--rw-r--r--   0        0        0    10641 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/Place.py
--rw-r--r--   0        0        0    11678 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/Road.py
--rw-r--r--   0        0        0     2960 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/Search.py
--rw-r--r--   0        0        0    16550 2024-03-27 07:47:40.906912 tubeulator-0.0.6/src/tubeulator/generated/StopPoint.py
--rw-r--r--   0        0        0     3067 2024-03-25 09:22:34.125990 tubeulator-0.0.6/src/tubeulator/generated/Vehicle.py
--rw-r--r--   0        0        0        0 2024-03-25 01:25:47.271790 tubeulator-0.0.6/src/tubeulator/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 01:25:47.271790 tubeulator-0.0.6/src/tubeulator/generated/crowding.py
--rw-r--r--   0        0        0     2803 2024-03-27 07:47:40.906912 tubeulator-0.0.6/src/tubeulator/generated/occupancy.py
--rw-r--r--   0        0        0      431 2024-03-25 09:22:31.149989 tubeulator-0.0.6/src/tubeulator/journey.py
--rw-r--r--   0        0        0        0 2024-03-25 01:25:47.271790 tubeulator-0.0.6/src/tubeulator/openapi/__init__.py
--rw-r--r--   0        0        0     1116 2024-03-25 09:22:31.149989 tubeulator-0.0.6/src/tubeulator/openapi/_types.py
--rw-r--r--   0        0        0     3063 2024-03-25 01:25:47.271790 tubeulator-0.0.6/src/tubeulator/openapi/dataclass_generator.py
--rw-r--r--   0        0        0     1642 2024-03-27 07:47:40.906912 tubeulator-0.0.6/src/tubeulator/openapi/fetch.py
--rw-r--r--   0        0        0     2028 2024-03-25 09:22:31.149989 tubeulator-0.0.6/src/tubeulator/openapi/reference.py
--rw-r--r--   0        0        0     1944 2024-03-25 09:22:31.149989 tubeulator-0.0.6/src/tubeulator/openapi/scan.py
--rw-r--r--   0        0        0        0 2024-03-25 01:25:47.271790 tubeulator-0.0.6/src/tubeulator/openapi/schema/__init__.py
--rw-r--r--   0        0        0    13251 2024-03-25 09:22:31.149989 tubeulator-0.0.6/src/tubeulator/openapi/schema/aliased.py
--rw-r--r--   0        0        0     1201 2024-03-25 09:22:31.149989 tubeulator-0.0.6/src/tubeulator/openapi/schema/base.py
--rw-r--r--   0        0        0      519 2024-03-25 09:22:31.153989 tubeulator-0.0.6/src/tubeulator/openapi/schema/unified.py
--rw-r--r--   0        0        0        0 2024-03-25 01:25:47.271790 tubeulator-0.0.6/src/tubeulator/py.typed
--rw-r--r--   0        0        0        0 2024-03-25 01:25:47.275790 tubeulator-0.0.6/src/tubeulator/utils/__init__.py
--rw-r--r--   0        0        0     4520 2024-03-25 09:22:31.153989 tubeulator-0.0.6/src/tubeulator/utils/lcp_trie.py
--rw-r--r--   0        0        0      670 2024-03-25 09:22:31.153989 tubeulator-0.0.6/src/tubeulator/utils/logs.py
--rw-r--r--   0        0        0     2696 2024-03-25 09:22:31.153989 tubeulator-0.0.6/src/tubeulator/utils/paths.py
--rw-r--r--   0        0        0     1680 2024-03-25 09:22:31.153989 tubeulator-0.0.6/src/tubeulator/utils/string_conv.py
--rw-r--r--   0        0        0       65 2024-03-25 01:25:47.275790 tubeulator-0.0.6/tests/core_test.py
--rw-r--r--   0        0        0      281 2024-03-27 07:47:40.906912 tubeulator-0.0.6/tests/dto_test.py
--rw-r--r--   0        0        0      212 2024-03-25 01:25:47.275790 tubeulator-0.0.6/tests/fetch_test.py
--rw-r--r--   0        0        0    12825 1970-01-01 00:00:00.000000 tubeulator-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-28 15:13:09.506000 tubeulator-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0    12107 2024-04-28 15:13:09.506000 tubeulator-0.0.7/README.md
+-rw-r--r--   0        0        0     1850 2024-04-28 15:21:43.715927 tubeulator-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      565 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/__init__.py
+-rw-r--r--   0        0        0       76 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/__init__.py
+-rw-r--r--   0        0        0      541 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/names.py
+-rw-r--r--   0        0        0     1225 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/__init__.py
+-rw-r--r--   0        0        0      189 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/accident.py
+-rw-r--r--   0        0        0      138 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/air.py
+-rw-r--r--   0        0        0      877 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/bike.py
+-rw-r--r--   0        0        0      357 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/crowding.py
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/disruption_lifts.py
+-rw-r--r--   0        0        0      395 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/journey.py
+-rw-r--r--   0        0        0     3015 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/line.py
+-rw-r--r--   0        0        0      313 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/mode.py
+-rw-r--r--   0        0        0      588 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/occupancy.py
+-rw-r--r--   0        0        0     1331 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/place.py
+-rw-r--r--   0        0        0      987 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/road.py
+-rw-r--r--   0        0        0      674 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/search.py
+-rw-r--r--   0        0        0     2941 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/stop.py
+-rw-r--r--   0        0        0      415 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/types.py
+-rw-r--r--   0        0        0      390 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/vehicle.py
+-rw-r--r--   0        0        0      784 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/interface.py
+-rw-r--r--   0        0        0    18440 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/api/request.py
+-rw-r--r--   0        0        0     1920 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/cli.py
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/__init__.py
+-rw-r--r--   0        0        0      120 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/gen/__init__.py
+-rw-r--r--   0        0        0    13792 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/gen/dto.py
+-rw-r--r--   0        0        0     2880 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/gen/emit.py
+-rw-r--r--   0        0        0      566 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/gen/helpers.py
+-rw-r--r--   0        0        0      735 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/gen/jsonschema.py
+-rw-r--r--   0        0        0     2204 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/gen/resolution.py
+-rw-r--r--   0        0        0      538 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/load_test.py
+-rw-r--r--   0        0        0      658 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/codegen/populate.py
+-rw-r--r--   0        0        0    10306 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/AccidentStats.json
+-rw-r--r--   0        0        0      812 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/accidentdetail.json
+-rw-r--r--   0        0        0      683 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/all.json
+-rw-r--r--   0        0        0      344 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/casualty.json
+-rw-r--r--   0        0        0      164 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-1.json
+-rw-r--r--   0        0        0      164 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-2.json
+-rw-r--r--   0        0        0      164 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-3.json
+-rw-r--r--   0        0        0      164 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray.json
+-rw-r--r--   0        0        0      135 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/vehicle.json
+-rw-r--r--   0        0        0     2473 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AirQuality/AirQuality.json
+-rw-r--r--   0        0        0       67 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AirQuality/schemas/all.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/AirQuality/schemas/object.json
+-rw-r--r--   0        0        0    12586 2024-04-28 15:13:09.506000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/BikePoint.json
+-rw-r--r--   0        0        0      359 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/additionalproperties.json
+-rw-r--r--   0        0        0      788 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/all.json
+-rw-r--r--   0        0        0     1491 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/place.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-1.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-2.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-3.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-4.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-5.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-6.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-7.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray.json
+-rw-r--r--   0        0        0     3569 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Disruptions-Lifts-v2/Disruptions-Lifts-v2.json
+-rw-r--r--   0        0        0      132 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/all.json
+-rw-r--r--   0        0        0      120 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      828 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/liftdisruption.json
+-rw-r--r--   0        0        0    64106 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/Journey.json
+-rw-r--r--   0        0        0     1988 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/all.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/metamodesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/metamodesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/metamodesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/metamodesget200textxmlresponse.json
+-rw-r--r--   0        0        0      873 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-10.json
+-rw-r--r--   0        0        0      620 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-11.json
+-rw-r--r--   0        0        0      350 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-12.json
+-rw-r--r--   0        0        0      424 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-13.json
+-rw-r--r--   0        0        0      307 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-14.json
+-rw-r--r--   0        0        0      243 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-15.json
+-rw-r--r--   0        0        0      359 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-16.json
+-rw-r--r--   0        0        0     1418 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-17.json
+-rw-r--r--   0        0        0     2645 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-18.json
+-rw-r--r--   0        0        0      218 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-19.json
+-rw-r--r--   0        0        0      180 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-2.json
+-rw-r--r--   0        0        0     1362 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-20.json
+-rw-r--r--   0        0        0     1892 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-21.json
+-rw-r--r--   0        0        0      355 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-22.json
+-rw-r--r--   0        0        0     1294 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-23.json
+-rw-r--r--   0        0        0      464 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-24.json
+-rw-r--r--   0        0        0      194 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-25.json
+-rw-r--r--   0        0        0      711 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-26.json
+-rw-r--r--   0        0        0      179 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-27.json
+-rw-r--r--   0        0        0      368 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-28.json
+-rw-r--r--   0        0        0      561 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-29.json
+-rw-r--r--   0        0        0     1324 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-3.json
+-rw-r--r--   0        0        0      550 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-30.json
+-rw-r--r--   0        0        0      714 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-31.json
+-rw-r--r--   0        0        0     1335 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-32.json
+-rw-r--r--   0        0        0      178 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-33.json
+-rw-r--r--   0        0        0      858 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-34.json
+-rw-r--r--   0        0        0      552 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-35.json
+-rw-r--r--   0        0        0      268 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-36.json
+-rw-r--r--   0        0        0      297 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-37.json
+-rw-r--r--   0        0        0      345 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-38.json
+-rw-r--r--   0        0        0      263 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-39.json
+-rw-r--r--   0        0        0      285 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-4.json
+-rw-r--r--   0        0        0      743 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-40.json
+-rw-r--r--   0        0        0      302 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-5.json
+-rw-r--r--   0        0        0      453 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-6.json
+-rw-r--r--   0        0        0      378 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-7.json
+-rw-r--r--   0        0        0     1062 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-8.json
+-rw-r--r--   0        0        0      511 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-9.json
+-rw-r--r--   0        0        0      304 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl.json
+-rw-r--r--   0        0        0   232588 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/Line.json
+-rw-r--r--   0        0        0     7137 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/all.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-routeget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-routeget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-routeget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-routeget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.510000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-statusget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-statusget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-statusget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/ids-statusget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metamodesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metamodesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metamodesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metamodesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metaseverityget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metaseverityget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metaseverityget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/metaseverityget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/routeget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/routeget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/routeget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/routeget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/status-severity-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/status-severity-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/status-severity-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/status-severity-get200textxmlresponse.json
+-rw-r--r--   0        0        0     1417 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-10.json
+-rw-r--r--   0        0        0     2641 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-11.json
+-rw-r--r--   0        0        0      218 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-12.json
+-rw-r--r--   0        0        0     1362 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-13.json
+-rw-r--r--   0        0        0     1892 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-14.json
+-rw-r--r--   0        0        0      550 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-15.json
+-rw-r--r--   0        0        0      714 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-16.json
+-rw-r--r--   0        0        0     1335 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-17.json
+-rw-r--r--   0        0        0      178 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-18.json
+-rw-r--r--   0        0        0      858 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-19.json
+-rw-r--r--   0        0        0      269 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-2.json
+-rw-r--r--   0        0        0     1221 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-20.json
+-rw-r--r--   0        0        0     1232 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-21.json
+-rw-r--r--   0        0        0      285 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-22.json
+-rw-r--r--   0        0        0      762 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-23.json
+-rw-r--r--   0        0        0      477 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-24.json
+-rw-r--r--   0        0        0      159 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-25.json
+-rw-r--r--   0        0        0      829 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-26.json
+-rw-r--r--   0        0        0      244 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-27.json
+-rw-r--r--   0        0        0      216 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-28.json
+-rw-r--r--   0        0        0      237 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-29.json
+-rw-r--r--   0        0        0      378 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-3.json
+-rw-r--r--   0        0        0      257 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-30.json
+-rw-r--r--   0        0        0      181 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-31.json
+-rw-r--r--   0        0        0      254 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-32.json
+-rw-r--r--   0        0        0      408 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-33.json
+-rw-r--r--   0        0        0      458 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-34.json
+-rw-r--r--   0        0        0      306 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-35.json
+-rw-r--r--   0        0        0      247 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-36.json
+-rw-r--r--   0        0        0      185 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-37.json
+-rw-r--r--   0        0        0      207 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-38.json
+-rw-r--r--   0        0        0      654 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-39.json
+-rw-r--r--   0        0        0     1062 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-4.json
+-rw-r--r--   0        0        0      529 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-40.json
+-rw-r--r--   0        0        0     2708 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-41.json
+-rw-r--r--   0        0        0      511 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-5.json
+-rw-r--r--   0        0        0      873 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-6.json
+-rw-r--r--   0        0        0      307 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-7.json
+-rw-r--r--   0        0        0      243 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-8.json
+-rw-r--r--   0        0        0      359 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-9.json
+-rw-r--r--   0        0        0      304 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl.json
+-rw-r--r--   0        0        0    19274 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/Mode.json
+-rw-r--r--   0        0        0      186 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/activeservicetype.json
+-rw-r--r--   0        0        0      939 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/all.json
+-rw-r--r--   0        0        0     2748 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/prediction.json
+-rw-r--r--   0        0        0      529 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/predictiontiming.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-1.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-2.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-3.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-4.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-5.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-6.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-7.json
+-rw-r--r--   0        0        0    42059 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/Place.json
+-rw-r--r--   0        0        0     2157 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/all.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/get200applicationjsonresponse-1.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/get200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/id-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/id-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/id-get200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/id-get200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.514000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/searchget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/searchget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/searchget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/searchget200textxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/system.json
+-rw-r--r--   0        0        0     2640 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-10.json
+-rw-r--r--   0        0        0      359 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-2.json
+-rw-r--r--   0        0        0     1416 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-3.json
+-rw-r--r--   0        0        0      378 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-4.json
+-rw-r--r--   0        0        0     1062 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-5.json
+-rw-r--r--   0        0        0      511 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-6.json
+-rw-r--r--   0        0        0      873 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-7.json
+-rw-r--r--   0        0        0      307 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-8.json
+-rw-r--r--   0        0        0      243 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-9.json
+-rw-r--r--   0        0        0      242 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/type-types-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/type-types-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/type-types-get200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/type-types-get200textxmlresponse.json
+-rw-r--r--   0        0        0      822 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/README.md
+-rw-r--r--   0        0        0   112822 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/Road.json
+-rw-r--r--   0        0        0     2250 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/all.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/get200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/get200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationgeo-jsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-statusget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-statusget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-statusget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/ids-statusget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200textxmlresponse.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/system-2.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/system-3.json
+-rw-r--r--   0        0        0      307 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/system.json
+-rw-r--r--   0        0        0      813 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-2.json
+-rw-r--r--   0        0        0     1501 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-3.json
+-rw-r--r--   0        0        0     1358 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-4.json
+-rw-r--r--   0        0        0      579 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-5.json
+-rw-r--r--   0        0        0      519 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-6.json
+-rw-r--r--   0        0        0      245 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-7.json
+-rw-r--r--   0        0        0     5927 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-8.json
+-rw-r--r--   0        0        0      269 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-9.json
+-rw-r--r--   0        0        0     1958 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl.json
+-rw-r--r--   0        0        0    20177 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/Search.json
+-rw-r--r--   0        0        0      985 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/all.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metasortsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metasortsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metasortsget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/metasortsget200textxmlresponse.json
+-rw-r--r--   0        0        0      642 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/tfl-2.json
+-rw-r--r--   0        0        0      358 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/tfl.json
+-rw-r--r--   0        0        0   137945 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/StopPoint.json
+-rw-r--r--   0        0        0     6467 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/all.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.518000 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200textxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200textjsonresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200textxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/system.json
+-rw-r--r--   0        0        0     1417 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-10.json
+-rw-r--r--   0        0        0     2641 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-11.json
+-rw-r--r--   0        0        0      178 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-12.json
+-rw-r--r--   0        0        0      209 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-13.json
+-rw-r--r--   0        0        0      258 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-14.json
+-rw-r--r--   0        0        0      529 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-15.json
+-rw-r--r--   0        0        0     2708 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-16.json
+-rw-r--r--   0        0        0     1869 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-17.json
+-rw-r--r--   0        0        0      755 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-18.json
+-rw-r--r--   0        0        0      646 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-19.json
+-rw-r--r--   0        0        0      304 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-2.json
+-rw-r--r--   0        0        0      967 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-20.json
+-rw-r--r--   0        0        0      358 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-21.json
+-rw-r--r--   0        0        0      645 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-22.json
+-rw-r--r--   0        0        0      378 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-3.json
+-rw-r--r--   0        0        0     1062 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-4.json
+-rw-r--r--   0        0        0      511 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-5.json
+-rw-r--r--   0        0        0      873 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-6.json
+-rw-r--r--   0        0        0      307 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-7.json
+-rw-r--r--   0        0        0      243 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-8.json
+-rw-r--r--   0        0        0      359 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-9.json
+-rw-r--r--   0        0        0      242 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200textxmlresponse.json
+-rw-r--r--   0        0        0    15378 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/Vehicle.json
+-rw-r--r--   0        0        0      425 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/all.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200textxmlresponse.json
+-rw-r--r--   0        0        0     2705 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/tfl-2.json
+-rw-r--r--   0        0        0      495 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/tfl-3.json
+-rw-r--r--   0        0        0      529 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/tfl.json
+-rw-r--r--   0        0        0     3579 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/crowding/crowding.json
+-rw-r--r--   0        0        0     5361 2024-04-28 15:13:09.521999 tubeulator-0.0.7/src/tubeulator/data/openapi/error_inventory.md
+-rw-r--r--   0        0        0    11496 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/namespace.json
+-rw-r--r--   0        0        0     7685 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/naming.md
+-rw-r--r--   0        0        0    24650 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/occupancy.json
+-rw-r--r--   0        0        0     1365 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/all.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/carparkget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/carparkget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/carparkget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/carparkget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200textxmlresponse.json
+-rw-r--r--   0        0        0      330 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/tfl-2.json
+-rw-r--r--   0        0        0      360 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/tfl-3.json
+-rw-r--r--   0        0        0      697 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/tfl-4.json
+-rw-r--r--   0        0        0      356 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/tfl.json
+-rw-r--r--   0        0        0     1503 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi/stationdata/stationdata.json
+-rw-r--r--   0        0        0   676093 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/ReleasedUnifiedAPIProd.json
+-rw-r--r--   0        0        0      812 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentdetail.json
+-rw-r--r--   0        0        0      283 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentstatsorderedsummary.json
+-rw-r--r--   0        0        0      186 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/activeservicetype.json
+-rw-r--r--   0        0        0      359 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/additionalproperties.json
+-rw-r--r--   0        0        0    29934 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/all.json
+-rw-r--r--   0        0        0      361 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/apiversioninfo.json
+-rw-r--r--   0        0        0     1909 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/arrivaldeparture.json
+-rw-r--r--   0        0        0      356 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bay.json
+-rw-r--r--   0        0        0      697 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bikepointoccupancy.json
+-rw-r--r--   0        0        0      360 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/carparkoccupancy.json
+-rw-r--r--   0        0        0      344 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/casualty.json
+-rw-r--r--   0        0        0      360 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/chargeconnectoroccupancy.json
+-rw-r--r--   0        0        0      531 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/coordinate.json
+-rw-r--r--   0        0        0      586 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/crowding.json
+-rw-r--r--   0        0        0     1378 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/cyclesuperhighway.json
+-rw-r--r--   0        0        0      245 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/daterange.json
+-rw-r--r--   0        0        0      245 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/daterangenullable.json
+-rw-r--r--   0        0        0      184 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/dbgeography.json
+-rw-r--r--   0        0        0      307 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/dbgeographywellknownvalue.json
+-rw-r--r--   0        0        0      262 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disambiguation.json
+-rw-r--r--   0        0        0      185 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disambiguationoption.json
+-rw-r--r--   0        0        0      646 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruptedpoint.json
+-rw-r--r--   0        0        0     1961 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruption.json
+-rw-r--r--   0        0        0      757 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/fare.json
+-rw-r--r--   0        0        0      860 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farebounds.json
+-rw-r--r--   0        0        0      179 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farecaveat.json
+-rw-r--r--   0        0        0     1483 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faredetails.json
+-rw-r--r--   0        0        0      254 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faresmode.json
+-rw-r--r--   0        0        0      443 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faresperiod.json
+-rw-r--r--   0        0        0      571 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faressection.json
+-rw-r--r--   0        0        0      364 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farestation.json
+-rw-r--r--   0        0        0      247 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faretap.json
+-rw-r--r--   0        0        0      464 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faretapdetails.json
+-rw-r--r--   0        0        0      695 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geocodesearchmatch.json
+-rw-r--r--   0        0        0      271 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geopoint.json
+-rw-r--r--   0        0        0      877 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/identifier.json
+-rw-r--r--   0        0        0      325 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instruction.json
+-rw-r--r--   0        0        0     1362 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instructionstep.json
+-rw-r--r--   0        0        0      216 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/interval.json
+-rw-r--r--   0        0        0     1002 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/itineraryresult.json
+-rw-r--r--   0        0        0      653 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journey.json
+-rw-r--r--   0        0        0      460 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyfare.json
+-rw-r--r--   0        0        0      552 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyplannercyclehiredockingstationdata.json
+-rw-r--r--   0        0        0      263 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyvector.json
+-rw-r--r--   0        0        0      620 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/jpelevation.json
+-rw-r--r--   0        0        0      257 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/knownjourney.json
+-rw-r--r--   0        0        0     1649 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/leg.json
+-rw-r--r--   0        0        0     1038 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/line.json
+-rw-r--r--   0        0        0      307 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linegroup.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.525999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      243 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemodegroup.json
+-rw-r--r--   0        0        0      477 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineroutesection.json
+-rw-r--r--   0        0        0      305 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineservicetype.json
+-rw-r--r--   0        0        0      178 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineservicetypeinfo.json
+-rw-r--r--   0        0        0      252 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linespecificservicetype.json
+-rw-r--r--   0        0        0      786 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linestatus.json
+-rw-r--r--   0        0        0     1335 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroute.json
+-rw-r--r--   0        0        0      159 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroutesections.json
+-rw-r--r--   0        0        0     1256 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedstop.json
+-rw-r--r--   0        0        0      357 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/message.json
+-rw-r--r--   0        0        0      304 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/mode.json
+-rw-r--r--   0        0        0      361 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/networkstatus.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/object.json
+-rw-r--r--   0        0        0      302 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/obstacle.json
+-rw-r--r--   0        0        0      285 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/orderedroute.json
+-rw-r--r--   0        0        0      378 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/passengerflow.json
+-rw-r--r--   0        0        0      315 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/passengertype.json
+-rw-r--r--   0        0        0      419 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/path.json
+-rw-r--r--   0        0        0      180 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/pathattribute.json
+-rw-r--r--   0        0        0      542 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/period.json
+-rw-r--r--   0        0        0     1491 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/place.json
+-rw-r--r--   0        0        0      242 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placecategory.json
+-rw-r--r--   0        0        0      513 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placegeo.json
+-rw-r--r--   0        0        0      262 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placepolygon.json
+-rw-r--r--   0        0        0      355 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/plannedwork.json
+-rw-r--r--   0        0        0      453 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/point.json
+-rw-r--r--   0        0        0      403 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/postcodeinput.json
+-rw-r--r--   0        0        0     2748 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/prediction.json
+-rw-r--r--   0        0        0      529 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/predictiontiming.json
+-rw-r--r--   0        0        0     1340 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendation.json
+-rw-r--r--   0        0        0      245 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendationresponse.json
+-rw-r--r--   0        0        0      233 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/redirect.json
+-rw-r--r--   0        0        0     1958 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadcorridor.json
+-rw-r--r--   0        0        0     6179 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruption.json
+-rw-r--r--   0        0        0      542 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionimpactarea.json
+-rw-r--r--   0        0        0      602 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionline.json
+-rw-r--r--   0        0        0      245 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionschedule.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0     1358 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadproject.json
+-rw-r--r--   0        0        0      458 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routeoption.json
+-rw-r--r--   0        0        0      948 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchmatch.json
+-rw-r--r--   0        0        0      284 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchresponse.json
+-rw-r--r--   0        0        0     1417 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesection.json
+-rw-r--r--   0        0        0      251 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesectionnaptanentrysequence.json
+-rw-r--r--   0        0        0      874 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesequence.json
+-rw-r--r--   0        0        0      596 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/schedule.json
+-rw-r--r--   0        0        0      399 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchcriteria.json
+-rw-r--r--   0        0        0      358 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmatch.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200textxmlresponse.json
+-rw-r--r--   0        0        0      680 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchresponse.json
+-rw-r--r--   0        0        0      254 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/servicefrequency.json
+-rw-r--r--   0        0        0      269 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stationinterval.json
+-rw-r--r--   0        0        0      269 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/statusseverity.json
+-rw-r--r--   0        0        0     2822 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppoint.json
+-rw-r--r--   0        0        0      242 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointcategory.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200applicationjsonresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200applicationxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200textjsonresponse.json
+-rw-r--r--   0        0        0       69 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      755 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointroutesection.json
+-rw-r--r--   0        0        0     1267 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsequence.json
+-rw-r--r--   0        0        0     1000 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsresponse.json
+-rw-r--r--   0        0        0     1539 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/street.json
+-rw-r--r--   0        0        0      813 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/streetsegment.json
+-rw-r--r--   0        0        0      164 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-1.json
+-rw-r--r--   0        0        0      164 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-2.json
+-rw-r--r--   0        0        0      164 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-3.json
+-rw-r--r--   0        0        0      164 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-1.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-2.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-3.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray.json
+-rw-r--r--   0        0        0      152 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-1.json
+-rw-r--r--   0        0        0      152 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-2.json
+-rw-r--r--   0        0        0      152 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-3.json
+-rw-r--r--   0        0        0      152 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray.json
+-rw-r--r--   0        0        0      154 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-1.json
+-rw-r--r--   0        0        0      154 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-2.json
+-rw-r--r--   0        0        0      154 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-3.json
+-rw-r--r--   0        0        0      154 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray.json
+-rw-r--r--   0        0        0      152 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-1.json
+-rw-r--r--   0        0        0      152 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-2.json
+-rw-r--r--   0        0        0      152 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-3.json
+-rw-r--r--   0        0        0      152 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray.json
+-rw-r--r--   0        0        0      160 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-1.json
+-rw-r--r--   0        0        0      160 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-2.json
+-rw-r--r--   0        0        0      160 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-3.json
+-rw-r--r--   0        0        0      160 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-4.json
+-rw-r--r--   0        0        0      160 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-5.json
+-rw-r--r--   0        0        0      160 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-6.json
+-rw-r--r--   0        0        0      160 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-7.json
+-rw-r--r--   0        0        0      160 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-1.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-2.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-3.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-4.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-5.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-6.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-7.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-1.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.529999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-2.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-3.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-4.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-5.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-6.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-7.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-1.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-10.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-11.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-12.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-13.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-14.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-15.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-16.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-17.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-18.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-19.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-2.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-20.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-21.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-22.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-23.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-24.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-25.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-26.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-27.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-28.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-29.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-3.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-30.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-31.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-32.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-33.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-34.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-35.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-4.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-5.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-6.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-7.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-8.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-9.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray.json
+-rw-r--r--   0        0        0      151 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-1.json
+-rw-r--r--   0        0        0      151 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-2.json
+-rw-r--r--   0        0        0      151 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-3.json
+-rw-r--r--   0        0        0      151 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-1.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-10.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-11.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-2.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-3.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-4.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-5.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-6.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-7.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-8.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-9.json
+-rw-r--r--   0        0        0      140 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-1.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-10.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-11.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-12.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-13.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-14.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-15.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-16.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-17.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-18.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-19.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-2.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-20.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-21.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-22.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-23.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-24.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-25.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-26.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-27.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-28.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-29.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-3.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-30.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-31.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-4.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-5.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-6.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-7.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-8.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-9.json
+-rw-r--r--   0        0        0      141 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray.json
+-rw-r--r--   0        0        0      149 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-1.json
+-rw-r--r--   0        0        0      149 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-2.json
+-rw-r--r--   0        0        0      149 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-3.json
+-rw-r--r--   0        0        0      149 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-4.json
+-rw-r--r--   0        0        0      149 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-5.json
+-rw-r--r--   0        0        0      149 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-6.json
+-rw-r--r--   0        0        0      149 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-7.json
+-rw-r--r--   0        0        0      149 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-1.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-10.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-11.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-12.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-13.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-14.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-15.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-2.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-3.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-4.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-5.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-6.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-7.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-8.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-9.json
+-rw-r--r--   0        0        0      146 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-1.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-10.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-11.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-2.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-3.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-4.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-5.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.533999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-6.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-7.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-8.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-9.json
+-rw-r--r--   0        0        0      148 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-1.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-2.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-3.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-4.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-1.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-2.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-3.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-4.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-5.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-6.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-7.json
+-rw-r--r--   0        0        0      150 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-1.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-10.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-11.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-12.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-13.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-14.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-15.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-16.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-17.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-18.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-19.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-2.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-20.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-21.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-22.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-23.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-24.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-25.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-26.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-27.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-3.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-4.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-5.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-6.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-7.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-8.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-9.json
+-rw-r--r--   0        0        0      145 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-1.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-2.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-3.json
+-rw-r--r--   0        0        0      153 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray.json
+-rw-r--r--   0        0        0      157 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-1.json
+-rw-r--r--   0        0        0      157 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-2.json
+-rw-r--r--   0        0        0      157 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-3.json
+-rw-r--r--   0        0        0      157 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray.json
+-rw-r--r--   0        0        0      685 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/ticket.json
+-rw-r--r--   0        0        0      186 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tickettime.json
+-rw-r--r--   0        0        0      186 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tickettype.json
+-rw-r--r--   0        0        0      268 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timeadjustment.json
+-rw-r--r--   0        0        0      509 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timeadjustments.json
+-rw-r--r--   0        0        0      285 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetable.json
+-rw-r--r--   0        0        0      806 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableresponse.json
+-rw-r--r--   0        0        0      377 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableroute.json
+-rw-r--r--   0        0        0     1062 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/trainloading.json
+-rw-r--r--   0        0        0      181 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/twentyfourhourclocktime.json
+-rw-r--r--   0        0        0      550 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/validityperiod.json
+-rw-r--r--   0        0        0      135 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/vehicle.json
+-rw-r--r--   0        0        0      495 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/vehiclematch.json
+-rw-r--r--   0        0        0      126 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/FeedInfo.csv
+-rw-r--r--   0        0        0    54508 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/Lifts.csv
+-rw-r--r--   0        0        0      347 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/ModesAndLines.csv
+-rw-r--r--   0        0        0   168607 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/PlatformServices.csv
+-rw-r--r--   0        0        0   145838 2024-04-28 15:13:09.537999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/Platforms.csv
+-rw-r--r--   0        0        0    20909 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/RampRoutes.csv
+-rw-r--r--   0        0        0   389058 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/SameLevelPaths.csv
+-rw-r--r--   0        0        0   273465 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/StationPoints.csv
+-rw-r--r--   0        0        0    37832 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/Stations.csv
+-rw-r--r--   0        0        0     8344 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/StepFreeIntechangeInfo.csv
+-rw-r--r--   0        0        0    28533 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/Toilets.csv
+-rw-r--r--   0        0        0      119 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/gtfs/feed_info.txt
+-rw-r--r--   0        0        0      135 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/gtfs/levels.txt
+-rw-r--r--   0        0        0   548638 2024-04-28 15:13:09.541999 tubeulator-0.0.7/src/tubeulator/data/stationdata/gtfs/pathways.txt
+-rw-r--r--   0        0        0   430539 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/data/stationdata/gtfs/stops.txt
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/db/__init__.py
+-rw-r--r--   0        0        0     2290 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/db/mongod.py
+-rw-r--r--   0        0        0     1332 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/db/store_creds.py
+-rw-r--r--   0        0        0      722 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/exc.py
+-rw-r--r--   0        0        0     2937 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/AccidentStats.py
+-rw-r--r--   0        0        0      699 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/AirQuality.py
+-rw-r--r--   0        0        0     2217 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/BikePoint.py
+-rw-r--r--   0        0        0     1469 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/DisruptionsLiftsv2.py
+-rw-r--r--   0        0        0    25751 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/Journey.py
+-rw-r--r--   0        0        0    36477 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/Line.py
+-rw-r--r--   0        0        0     3711 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/Mode.py
+-rw-r--r--   0        0        0    10641 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/Place.py
+-rw-r--r--   0        0        0    11678 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/Road.py
+-rw-r--r--   0        0        0     2960 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/Search.py
+-rw-r--r--   0        0        0    16550 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/StopPoint.py
+-rw-r--r--   0        0        0     3067 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/Vehicle.py
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/crowding.py
+-rw-r--r--   0        0        0     2803 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/occupancy.py
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/generated/stationdata.py
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/__init__.py
+-rw-r--r--   0        0        0     1116 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/_types.py
+-rw-r--r--   0        0        0     3063 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/dataclass_generator.py
+-rw-r--r--   0        0        0     1643 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/fetch.py
+-rw-r--r--   0        0        0     2028 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/reference.py
+-rw-r--r--   0        0        0     1971 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/scan.py
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/schema/__init__.py
+-rw-r--r--   0        0        0    13251 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/schema/aliased.py
+-rw-r--r--   0        0        0     1201 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/schema/base.py
+-rw-r--r--   0        0        0      489 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/openapi/schema/unified.py
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/py.typed
+-rw-r--r--   0        0        0      583 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/topology/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/topology/combine.py
+-rw-r--r--   0        0        0     1934 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/topology/data_model.py
+-rw-r--r--   0        0        0      592 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/topology/gtfs_data_model.py
+-rw-r--r--   0        0        0     1095 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/topology/load.py
+-rw-r--r--   0        0        0     1206 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/topology/load_gtfs.py
+-rw-r--r--   0        0        0        0 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/utils/__init__.py
+-rw-r--r--   0        0        0     4521 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/utils/lcp_trie.py
+-rw-r--r--   0        0        0      670 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/utils/logs.py
+-rw-r--r--   0        0        0     1508 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/utils/paths.py
+-rw-r--r--   0        0        0     1874 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/utils/schemas.py
+-rw-r--r--   0        0        0     2297 2024-04-28 15:13:09.545999 tubeulator-0.0.7/src/tubeulator/utils/string_conv.py
+-rw-r--r--   0        0        0       65 2024-04-28 15:13:09.545999 tubeulator-0.0.7/tests/core_test.py
+-rw-r--r--   0        0        0      281 2024-04-28 15:13:09.545999 tubeulator-0.0.7/tests/dto_test.py
+-rw-r--r--   0        0        0      212 2024-04-28 15:13:09.545999 tubeulator-0.0.7/tests/fetch_test.py
+-rw-r--r--   0        0        0      732 2024-04-28 15:13:09.545999 tubeulator-0.0.7/tests/topo_combine_test.py
+-rw-r--r--   0        0        0      563 2024-04-28 15:13:09.545999 tubeulator-0.0.7/tests/topo_load_test.py
+-rw-r--r--   0        0        0    13098 1970-01-01 00:00:00.000000 tubeulator-0.0.7/PKG-INFO
```

### Comparing `tubeulator-0.0.6/README.md` & `tubeulator-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/pyproject.toml` & `tubeulator-0.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -22,20 +22,30 @@
     "pydantic>=2.6.4",
     "pymongo",
     "urllib3<2",
 ]
 description = "TfL open data interface library."
 name = "tubeulator"
 readme = "README.md"
-requires-python = ">=3.10,<=3.12"
-version = "0.0.6"
+requires-python = ">=3.10,<3.13"
+version = "0.0.7"
 
 [project.license]
 text = "MIT"
 
+[project.optional-dependencies]
+polars = [
+    "patito>=0.6.1",
+    "polars>=0.20.17",
+]
+polars-lts-cpu = [
+    "patito>=0.6.1",
+    "polars-lts-cpu>=0.20.17",
+]
+
 [project.scripts]
 tubeulator = "tubeulator.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/lmmx/tubeulator"
 Repository = "https://github.com/lmmx/tubeulator.git"
 
@@ -52,14 +62,20 @@
 test = [
     "pytest>=7.4.0",
 ]
 vercel = [
     "urllib3<2",
 ]
 
+[tool.pdm.resolution]
+excludes = [
+    "polars",
+    "polars-lts-cpu",
+]
+
 [tool.ruff.lint]
 ignore = [
     "C408",
     "C901",
     "E501",
     "E741",
 ]
```

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/names.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/names.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/__init__.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/bike.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/bike.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/line.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/line.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/occupancy.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/occupancy.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/place.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/place.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/road.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/road.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/search.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/search.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/endpoint/routes/stop.py` & `tubeulator-0.0.7/src/tubeulator/api/endpoint/routes/stop.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/interface.py` & `tubeulator-0.0.7/src/tubeulator/api/interface.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/api/request.py` & `tubeulator-0.0.7/src/tubeulator/api/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,16 @@
 
 import httpx
 from pydantic import BaseModel, TypeAdapter
 
 from ..codegen import load_test
 from ..db.store_creds import check_creds
 from ..exc import RequestError
-from ..utils.paths import (
-    RefPath,
-    SchemaPath,
-    load_endpoint_component_schemas,
-    load_endpoint_schema,
-)
+from ..utils.paths import RefPath, SchemaPath
+from ..utils.schemas import load_endpoint_component_schemas, load_endpoint_schema
 from .endpoint.names import EndpointNames
 from .endpoint.routes.types import AnyEndpointRouteEnum
 
 __all__ = ["TflApiPath", "Path", "Request", "GET"]
 
 
 class TflApiPath:
```

### Comparing `tubeulator-0.0.6/src/tubeulator/cli.py` & `tubeulator-0.0.7/src/tubeulator/cli.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/codegen/gen/dto.py` & `tubeulator-0.0.7/src/tubeulator/codegen/gen/dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ast
 import textwrap
 from itertools import starmap
 from typing import Literal
 
 from ...openapi.scan import scan_namespace
-from ...utils.paths import SchemaPath, load_endpoint_component_schemas
+from ...utils.paths import SchemaPath
+from ...utils.schemas import load_endpoint_component_schemas
 from ...utils.string_conv import to_pascal_case
 from .jsonschema import python_type
 from .resolution import (
     find_array_literals,
     find_arrays,
     find_backrefs,
     find_chased,
@@ -19,14 +20,16 @@
     "import_node",
     "generate_dataclass_name",
     "generate_dataclass",
     "hidden_field",
     "generate_source",
 ]
 
+GenModes = Literal["patito", "pydantic", "jsonw"]
+
 
 def import_node(module: str, names: list[str]) -> ast.Import:
     if names:
         return ast.ImportFrom(module=module, names=[*map(ast.alias, names)], level=0)
     else:
         return ast.Import(names=[ast.alias(name=module)])
 
@@ -171,44 +174,47 @@
             indent_level=indent_level,
             idx=idx,
             schema_mapping=schema_mapping,
         )
     return preproc_class_name, output
 
 
-def hidden_field(default_value: str, style: Literal["pydantic", "jsonw"]) -> str:
+def hidden_field(default_value: str, style: GenModes) -> str:
     if style == "jsonw":
         value = f"field(default={default_value!r}, repr=False)"
-    elif style == "pydantic":
+    elif style in ["patito", "pydantic"]:
         value = f"PrivateAttr(default={default_value!r})"
     return value
 
 
-def make_class_header(class_name: str, style: Literal["pydantic", "jsonw"]) -> str:
+def make_class_header(class_name: str, style: GenModes) -> str:
     if style == "jsonw":
         hed = f"@dataclass\nclass {class_name}(JSONWizard):\n"
     elif style == "pydantic":
         hed = f"class {class_name}(BaseModel):\n"
+    elif style == "patito":
+        hed = f"class {class_name}(Model):\n"
     return hed
 
 
 def generate_source(
     class_name: str,
     component_name: str,
     schema_name: str,
     gen_source: str,
     schema: dict,
     parent_schema: dict,
     indent_level: int,
     idx: int,
     schema_mapping: dict[str, str] | None,
-    style: Literal["pydantic", "jsonw"] = "pydantic",
+    style: GenModes = "pydantic",
 ) -> str:
     is_jsonw = style == "jsonw"
-    is_pydantic = style == "pydantic"
+    is_patito = style == "patito"
+    is_pydantic = style in ["patito", "pydantic"]  # Careful: patito subclasses Pydantic
     properties = schema.get("properties", {})
     required = schema.get("required", [])
     contains_list = False
     dc_source = make_class_header(class_name=class_name, style=style)
     docstring = f"Autogenerated from {schema_name}::{gen_source}"
     dc_source += textwrap.indent(f'"""\n{docstring}\n"""\n', " " * indent_level * 4)
     if is_pydantic:
@@ -296,15 +302,21 @@
         "dataclass_wizard.loaders": ["fromdict"],
         "jsonschema": [],
     }
     pydantic_imports = {
         "tubeulator.utils.string_conv": ["to_camel_case"],
         "pydantic": ["AliasGenerator", "BaseModel", "ConfigDict", "PrivateAttr"],
     }
+    patito_imports = {
+        "tubeulator.utils.string_conv": ["to_camel_case"],
+        "patito": ["Model"],
+        "pydantic": ["AliasGenerator", "ConfigDict", "PrivateAttr"],
+    }
     jsonw_utils = ["load_endpoint_component_schemas"]
+    pydantic_imports = patito_imports if is_patito else pydantic_imports
     import_list = {
         "__future__": ["annotations"],
         "json": [],
         "datetime": ["datetime"],
         "dataclasses": ["dataclass"],
         # "pathlib": ["Path"], # I think this was a mistake
         **(jsonw_imports if is_jsonw else {}),
```

### Comparing `tubeulator-0.0.6/src/tubeulator/codegen/gen/emit.py` & `tubeulator-0.0.7/src/tubeulator/codegen/gen/emit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Emit DTO code generated for TfL APIs (detected from their loaded Swagger schemas)."""
+
 from ...openapi.scan import scan_namespace
-from ...utils.paths import load_endpoint_component_schemas, to_enum_friendly_str
+from ...utils.paths import to_enum_friendly_str
+from ...utils.schemas import load_endpoint_component_schemas
 from .dto import generate_dataclass, generate_dataclass_name
 from .helpers import logger
 
 __all__ = ["emit_deserialisers"]
 
 
 def emit_deserialisers(schema_name: str) -> str:
```

### Comparing `tubeulator-0.0.6/src/tubeulator/codegen/gen/helpers.py` & `tubeulator-0.0.7/src/tubeulator/codegen/gen/helpers.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/codegen/gen/jsonschema.py` & `tubeulator-0.0.7/src/tubeulator/codegen/gen/jsonschema.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/codegen/gen/resolution.py` & `tubeulator-0.0.7/src/tubeulator/codegen/gen/resolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functions for the unique resolution of schema identifiers."""
+
 from ...utils.lcp_trie import Trie
 from ...utils.paths import SchemaPath
 
 __all__ = [
     "find_backrefs",
     "find_string_literals",
     "find_array_literals",
```

### Comparing `tubeulator-0.0.6/src/tubeulator/codegen/load_test.py` & `tubeulator-0.0.7/src/tubeulator/codegen/load_test.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/codegen/populate.py` & `tubeulator-0.0.7/src/tubeulator/codegen/populate.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/AccidentStats.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/AccidentStats.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/accidentdetail.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/accidentdetail.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/AccidentStats/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/AccidentStats/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/AirQuality/AirQuality.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/AirQuality/AirQuality.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/BikePoint.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/BikePoint.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/BikePoint/schemas/place.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/BikePoint/schemas/place.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Disruptions-Lifts-v2/Disruptions-Lifts-v2.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Disruptions-Lifts-v2/Disruptions-Lifts-v2.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/liftdisruption.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/liftdisruption.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/Journey.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/Journey.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-10.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-10.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-11.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-11.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-17.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-17.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-18.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-18.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-20.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-20.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-21.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-21.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-23.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-23.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-26.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-26.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-29.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-29.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-3.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-3.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-30.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-30.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-31.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-31.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-32.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-32.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-34.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-34.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-35.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-35.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-40.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-40.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Journey/schemas/tfl-8.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Journey/schemas/tfl-8.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/Line.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/Line.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-10.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-10.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-11.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-11.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-13.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-13.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-14.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-14.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-15.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-15.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-16.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-16.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-17.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-17.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-19.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-19.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-20.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-20.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-21.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-21.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-23.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-23.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-26.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-26.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-39.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-39.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-4.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-4.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-40.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-40.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-41.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-41.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Line/schemas/tfl-6.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Line/schemas/tfl-6.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/Mode.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/Mode.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/prediction.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/prediction.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Mode/schemas/predictiontiming.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Mode/schemas/predictiontiming.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Place/Place.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Place/Place.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-10.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-10.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-3.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-3.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-5.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-5.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Place/schemas/tfl-7.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Place/schemas/tfl-7.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/README.md` & `tubeulator-0.0.7/src/tubeulator/data/openapi/README.md`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/Road.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/Road.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-2.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-2.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-3.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-3.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-4.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-4.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-5.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-5.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-6.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-6.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl-8.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl-8.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Road/schemas/tfl.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Road/schemas/tfl.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Search/Search.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Search/Search.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Search/schemas/tfl-2.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Search/schemas/tfl-2.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/StopPoint.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/StopPoint.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-10.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-10.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-11.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-11.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-15.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-15.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-16.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-16.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-17.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-17.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-18.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-18.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-19.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-19.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-20.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-20.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-22.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-22.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-4.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-4.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/StopPoint/schemas/tfl-6.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/StopPoint/schemas/tfl-6.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/Vehicle.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/Vehicle.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/tfl-2.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/tfl-2.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/Vehicle/schemas/tfl.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/Vehicle/schemas/tfl.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/crowding/crowding.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/crowding/crowding.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/error_inventory.md` & `tubeulator-0.0.7/src/tubeulator/data/openapi/error_inventory.md`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/namespace.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/namespace.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/naming.md` & `tubeulator-0.0.7/src/tubeulator/data/openapi/naming.md`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/occupancy.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/occupancy.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/occupancy/schemas/tfl-4.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/occupancy/schemas/tfl-4.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi/stationdata/stationdata.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi/stationdata/stationdata.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/ReleasedUnifiedAPIProd.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/ReleasedUnifiedAPIProd.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentdetail.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentdetail.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/all.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/arrivaldeparture.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/arrivaldeparture.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bikepointoccupancy.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bikepointoccupancy.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/coordinate.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/coordinate.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/crowding.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/crowding.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/cyclesuperhighway.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/cyclesuperhighway.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruptedpoint.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruptedpoint.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruption.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruption.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/fare.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/fare.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farebounds.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farebounds.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faredetails.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faredetails.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faressection.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faressection.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geocodesearchmatch.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geocodesearchmatch.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/identifier.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/identifier.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instructionstep.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instructionstep.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/itineraryresult.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/itineraryresult.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journey.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journey.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyplannercyclehiredockingstationdata.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyplannercyclehiredockingstationdata.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/jpelevation.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/jpelevation.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/leg.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/leg.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/line.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/line.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linestatus.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linestatus.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroute.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroute.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedstop.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedstop.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/period.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/period.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/place.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/place.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placegeo.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placegeo.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/prediction.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/prediction.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/predictiontiming.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/predictiontiming.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendation.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendation.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadcorridor.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadcorridor.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruption.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruption.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionimpactarea.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionimpactarea.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionline.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionline.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadproject.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadproject.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchmatch.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchmatch.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesection.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesection.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesequence.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesequence.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/schedule.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/schedule.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchresponse.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchresponse.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppoint.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppoint.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointroutesection.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointroutesection.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsequence.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsequence.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsresponse.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsresponse.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/street.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/street.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/streetsegment.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/streetsegment.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/ticket.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/ticket.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableresponse.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableresponse.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/trainloading.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/trainloading.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/validityperiod.json` & `tubeulator-0.0.7/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/validityperiod.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/Lifts.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/Lifts.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/PlatformServices.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/PlatformServices.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/Platforms.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/Platforms.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/RampRoutes.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/RampRoutes.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/SameLevelPaths.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/SameLevelPaths.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/StationPoints.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/StationPoints.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/Stations.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/Stations.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/StepFreeIntechangeInfo.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/StepFreeIntechangeInfo.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/detailed/Toilets.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/detailed/Toilets.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/gtfs/pathways.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/gtfs/pathways.txt`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/data/stationdata/gtfs/stops.csv` & `tubeulator-0.0.7/src/tubeulator/data/stationdata/gtfs/stops.txt`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/db/mongod.py` & `tubeulator-0.0.7/src/tubeulator/db/mongod.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/db/store_creds.py` & `tubeulator-0.0.7/src/tubeulator/db/store_creds.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/exc.py` & `tubeulator-0.0.7/src/tubeulator/exc.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/AccidentStats.py` & `tubeulator-0.0.7/src/tubeulator/generated/AccidentStats.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/AirQuality.py` & `tubeulator-0.0.7/src/tubeulator/generated/AirQuality.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/BikePoint.py` & `tubeulator-0.0.7/src/tubeulator/generated/BikePoint.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/DisruptionsLiftsv2.py` & `tubeulator-0.0.7/src/tubeulator/generated/DisruptionsLiftsv2.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/Journey.py` & `tubeulator-0.0.7/src/tubeulator/generated/Journey.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/Line.py` & `tubeulator-0.0.7/src/tubeulator/generated/Line.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/Mode.py` & `tubeulator-0.0.7/src/tubeulator/generated/Mode.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/Place.py` & `tubeulator-0.0.7/src/tubeulator/generated/Place.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/Road.py` & `tubeulator-0.0.7/src/tubeulator/generated/Road.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/Search.py` & `tubeulator-0.0.7/src/tubeulator/generated/Search.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/StopPoint.py` & `tubeulator-0.0.7/src/tubeulator/generated/StopPoint.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/Vehicle.py` & `tubeulator-0.0.7/src/tubeulator/generated/Vehicle.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/generated/occupancy.py` & `tubeulator-0.0.7/src/tubeulator/generated/occupancy.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/openapi/_types.py` & `tubeulator-0.0.7/src/tubeulator/openapi/_types.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/openapi/dataclass_generator.py` & `tubeulator-0.0.7/src/tubeulator/openapi/dataclass_generator.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/openapi/fetch.py` & `tubeulator-0.0.7/src/tubeulator/openapi/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Download and store (overwrite) the OpenAPI JSON schemas for TfL APIs."""
+
 import json
 
 import httpx
 
 from ..utils.paths import openapi_schemas_path
 
 __all__ = ["fetch_schema"]
```

### Comparing `tubeulator-0.0.6/src/tubeulator/openapi/reference.py` & `tubeulator-0.0.7/src/tubeulator/openapi/reference.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/openapi/scan.py` & `tubeulator-0.0.7/src/tubeulator/openapi/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from pathlib import Path
 
-from ..utils.paths import find_schema, openapi_schemas_path
+from ..utils.paths import openapi_schemas_path
+from ..utils.schemas import find_schema
 from ._types import ApiAliasToUnifiedEntities, NamespaceInventory
 from .schema.aliased import AliasedApiSchema
 
 __all__ = ["api_schema_inventory", "scan_namespace"]
 
 
 # TODO: duplication here suggests need for an API schema class (from JSON to entities)
```

### Comparing `tubeulator-0.0.6/src/tubeulator/openapi/schema/aliased.py` & `tubeulator-0.0.7/src/tubeulator/openapi/schema/aliased.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/openapi/schema/base.py` & `tubeulator-0.0.7/src/tubeulator/openapi/schema/base.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/utils/lcp_trie.py` & `tubeulator-0.0.7/src/tubeulator/utils/lcp_trie.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """LCP trie adapted from dict (char) trie at:
 https://ychai.uk/notes/2019/03/03/Programming/Tricks-of-Python/
 """
+
 from __future__ import annotations
 
 __all__ = ["TrieNode", "Trie"]
 
 
 class TrieNode:
     def __init__(self):
```

### Comparing `tubeulator-0.0.6/src/tubeulator/utils/logs.py` & `tubeulator-0.0.7/src/tubeulator/utils/logs.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.6/src/tubeulator/utils/string_conv.py` & `tubeulator-0.0.7/src/tubeulator/utils/string_conv.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 Object (DTO) JSON keys.
 
 Pydantic uses 'alias generators' for this, the same as DCW just in the opposite
 direction (DCW consider conversions going from JSON key to model field). Unfortunately
 Pydantic's string conversion helpers do not actually do the job required here,
 so I copied over these helper functions rather than enforce a dependency for them.
 """
+
 import re
 
-__all__ = ["to_camel_case", "to_pascal_case"]
+__all__ = ["to_camel_case", "to_pascal_case", "to_snake_case"]
 
 
 def replace_multi_with_single(string: str, char="_") -> str:
     """
     Replace multiple consecutive occurrences of `char` with a single one.
     """
     rep = char + char
@@ -58,7 +59,32 @@
     string = replace_multi_with_single(string.replace("-", "_").replace(" ", "_"))
 
     return string[0].upper() + re.sub(
         r"(?:_)(.)",
         lambda m: m.group(1).upper(),
         string[1:],
     )
+
+
+def to_snake_case(string: str) -> str:
+    """
+    Make an underscored, lowercase form from the expression in the string.
+
+
+    Example::
+
+
+        >>> to_snake_case("DeviceType")
+        'device_type'
+
+
+    """
+    string = string.replace("-", "_").replace(" ", "_")
+    # Short path: the field is already
+    # lower-cased, so we don't need to handle
+    # for camel or title case.
+    if string.islower():
+        return replace_multi_with_single(string)
+
+    result = re.sub(r"((?!^)(?<!_)[A-Z][a-z]+|(?<=[a-z0-9])[A-Z])", r"_\1", string)
+
+    return replace_multi_with_single(result.lower())
```

### Comparing `tubeulator-0.0.6/PKG-INFO` & `tubeulator-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: tubeulator
-Version: 0.0.6
+Version: 0.0.7
 Summary: TfL open data interface library.
 Author-Email: Louis Maddox <louismmx@gmail.com>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/lmmx/tubeulator
 Project-URL: Repository, https://github.com/lmmx/tubeulator.git
-Requires-Python: <=3.12,>=3.10
+Requires-Python: <3.13,>=3.10
 Requires-Dist: defopt
 Requires-Dist: httpx
 Requires-Dist: jsonschema
 Requires-Dist: orjson
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: pymongo
 Requires-Dist: urllib3<2
+Requires-Dist: patito>=0.6.1; extra == "polars"
+Requires-Dist: polars>=0.20.17; extra == "polars"
+Requires-Dist: patito>=0.6.1; extra == "polars-lts-cpu"
+Requires-Dist: polars-lts-cpu>=0.20.17; extra == "polars-lts-cpu"
+Provides-Extra: polars
+Provides-Extra: polars-lts-cpu
 Description-Content-Type: text/markdown
 
 # tubeulator
 
 > It's time for the tubeulator
 
 TfL open data interface library
```

