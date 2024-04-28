# Comparing `tmp/frenetix-0.2.0rc5.tar.gz` & `tmp/frenetix-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frenetix-0.2.0rc5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "frenetix-0.3.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `frenetix-0.2.0rc5.tar` & `frenetix-0.3.0.tar`

### file list

```diff
@@ -1,144 +1,145 @@
--rw-r--r--   0        0        0     2354 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/.gitignore
--rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/.gitlab-ci.yml
--rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/.gitmodules
--rw-r--r--   0        0        0     9426 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/CMakeLists.txt
--rw-r--r--   0        0        0     7632 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/LICENSE
--rw-r--r--   0        0        0      606 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/README.md
--rw-r--r--   0        0        0     1007 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/cmake/AppleOpenMP.cmake
--rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/cmake/external/ExternalBoost.cmake
--rw-r--r--   0        0        0      909 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/cmake/external/ExternalDrivabilityChecker.cmake
--rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/cmake/external/ExternalEigen.cmake
--rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/cmake/external/ExternalTaskflow.cmake
--rw-r--r--   0        0        0     1446 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/pyproject.toml
--rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/requirements.txt
--rw-r--r--   0        0        0     2832 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/CMakeLists.txt
--rw-r--r--   0        0        0     3641 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/CoordinateSystemWrapper.cpp
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/CoordinateSystemWrapper.hpp
--rw-r--r--   0        0        0     5779 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/TrajectoryHandler.cpp
--rw-r--r--   0        0        0     3454 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/TrajectoryHandler.hpp
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/geometryMsgs.cpp
--rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/geometryMsgs.hpp
--rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/math/covariance.hpp
--rw-r--r--   0        0        0     1410 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/math/mvn.cpp
--rw-r--r--   0        0        0     1579 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/math/mvn.hpp
--rw-r--r--   0        0        0    46387 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/math/mvndst.f
--rw-r--r--   0        0        0      448 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/math/mvndst.hpp
--rw-r--r--   0        0        0     4489 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/cartesianSampleBinding.cpp
--rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/cartesianSampleBinding.hpp
--rw-r--r--   0        0        0     3249 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/coordinateSystemWrapperBinding.cpp
--rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/coordinateSystemWrapperBinding.hpp
--rw-r--r--   0        0        0      570 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/costStrategyBinding.cpp
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/costStrategyBinding.hpp
--rw-r--r--   0        0        0     4590 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/curviLinearSampleBinding.cpp
--rw-r--r--   0        0        0      315 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/curviLinearSampleBinding.hpp
--rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/feasabilityStrategyBinding.cpp
--rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/feasabilityStrategyBinding.hpp
--rw-r--r--   0        0        0     1751 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/geometryMsgsBinding.cpp
--rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/geometryMsgsBinding.hpp
--rw-r--r--   0        0        0     4352 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/handlerBinding.cpp
--rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/handlerBinding.hpp
--rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/mainBindings.cpp
--rw-r--r--   0        0        0     2773 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/polynomialTrajectoryBinding.cpp
--rw-r--r--   0        0        0      300 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/polynomialTrajectoryBinding.hpp
--rw-r--r--   0        0        0     9162 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/costFunctionsBinding.cpp
--rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/costFunctionsBinding.hpp
--rw-r--r--   0        0        0     3011 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/feasabilityFunctionsBinding.cpp
--rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/feasabilityFunctionsBinding.hpp
--rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/otherFunctionsBinding.cpp
--rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/otherFunctionsBinding.hpp
--rw-r--r--   0        0        0     6135 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectorySampleBinding.cpp
--rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectorySampleBinding.hpp
--rw-r--r--   0        0        0      981 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryStrategyBinding.cpp
--rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryStrategyBinding.hpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/.gitkeep
--rw-r--r--   0        0        0      519 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/__init__.py
--rw-r--r--   0        0        0     1052 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/__init__.pyi
--rw-r--r--   0        0        0    12803 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/_frenetix/__init__.pyi
--rw-r--r--   0        0        0     1202 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/_frenetix/trajectory_functions/__init__.pyi
--rw-r--r--   0        0        0     5639 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/_frenetix/trajectory_functions/cost_functions/__init__.pyi
--rw-r--r--   0        0        0     2002 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/_frenetix/trajectory_functions/feasability_functions/__init__.pyi
--rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/_version.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/py.typed
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/trajectory_functions/__init__.py
--rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/trajectory_functions/__init__.pyi
--rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/trajectory_functions/cost_functions/__init__.py
--rw-r--r--   0        0        0     5704 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/trajectory_functions/cost_functions/__init__.pyi
--rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/trajectory_functions/feasability_functions/__init__.py
--rw-r--r--   0        0        0     2002 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/python/frenetix/trajectory_functions/feasability_functions/__init__.pyi
--rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateAccelerationCost.cpp
--rw-r--r--   0        0        0     1111 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateAccelerationCost.hpp
--rw-r--r--   0        0        0     5716 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateCollisionProbabilityFast.cpp
--rw-r--r--   0        0        0     4497 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateCollisionProbabilityFast.hpp
--rw-r--r--   0        0        0     1999 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateCollisionProbabilityMahalanobis.cpp
--rw-r--r--   0        0        0     1842 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateCollisionProbabilityMahalanobis.hpp
--rw-r--r--   0        0        0     2188 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateDistanceToObstacleCost.cpp
--rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateDistanceToObstacleCost.hpp
--rw-r--r--   0        0        0      687 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateDistanceToReferencePathCost.cpp
--rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateDistanceToReferencePathCost.hpp
--rw-r--r--   0        0        0      923 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateJerkCost.cpp
--rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateJerkCost.hpp
--rw-r--r--   0        0        0      554 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLaneCenterOffsetCost.cpp
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLaneCenterOffsetCost.hpp
--rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLateralJerkCost.cpp
--rw-r--r--   0        0        0      399 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLateralJerkCost.hpp
--rw-r--r--   0        0        0      553 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLongitudinalJerkCost.cpp
--rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLongitudinalJerkCost.hpp
--rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLongitudinalVelocityCost.cpp
--rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLongitudinalVelocityCost.hpp
--rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateOrientationOffsetCost.cpp
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateOrientationOffsetCost.hpp
--rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateSteeringAngleCost.cpp
--rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateSteeringAngleCost.hpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateSteeringRateCost.cpp
--rw-r--r--   0        0        0      387 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateSteeringRateCost.hpp
--rw-r--r--   0        0        0      749 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateVelocityOffsetCost.cpp
--rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateVelocityOffsetCost.hpp
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateYawCost.cpp
--rw-r--r--   0        0        0      342 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateYawCost.hpp
--rw-r--r--   0        0        0      608 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/CostStrategy.hpp
--rw-r--r--   0        0        0     1236 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckAccelerationConstraint.cpp
--rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckAccelerationConstraint.hpp
--rw-r--r--   0        0        0     1064 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckCurvatureConstraints.cpp
--rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckCurvatureConstraints.hpp
--rw-r--r--   0        0        0     1306 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckCurvatureRateConstrains.cpp
--rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckCurvatureRateConstrains.hpp
--rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckVelocityConstraints.cpp
--rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckVelocityConstraints.hpp
--rw-r--r--   0        0        0     1158 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckYawRateConstraint.cpp
--rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckYawRateConstraint.hpp
--rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/FeasabilityStrategy.hpp
--rw-r--r--   0        0        0     4949 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/Functions/ComputeInitalState.cpp
--rw-r--r--   0        0        0      708 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/Functions/ComputeInitalState.hpp
--rw-r--r--   0        0        0     8066 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/Functions/FillCoordinates.cpp
--rw-r--r--   0        0        0      700 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/Functions/FillCoordinates.hpp
--rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/strategies/TrajectoryStrategy.hpp
--rw-r--r--   0        0        0     1752 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/trajectory/CartesianSample.cpp
--rw-r--r--   0        0        0     1892 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/trajectory/CartesianSample.hpp
--rw-r--r--   0        0        0     1724 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/trajectory/CurvilinearSample.cpp
--rw-r--r--   0        0        0     1620 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/trajectory/CurvilinearSample.hpp
--rw-r--r--   0        0        0     3087 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/trajectory/TrajectorySample.cpp
--rw-r--r--   0        0        0     2992 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/trajectory/TrajectorySample.hpp
--rw-r--r--   0        0        0     8502 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/trajectory/polynomial.hpp
--rw-r--r--   0        0        0     2958 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/util.cpp
--rw-r--r--   0        0        0     3460 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/src/util.hpp
--rw-r--r--   0        0        0     1540 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/CMakeLists.txt
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/application_settings.h
--rw-r--r--   0        0        0    27845 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/curvilinear_coordinate_system.h
--rw-r--r--   0        0        0     7909 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/segment.h
--rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/basic_types.h
--rw-r--r--   0        0        0      989 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/curvilinear_coordinate_system_export.h
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/export_structs/curvilinear_coordinate_system_export_struct.h
--rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/icurvilinear_coordinate_system_export.h
--rw-r--r--   0        0        0      537 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/public/serialize_public.h
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/serialize.h
--rw-r--r--   0        0        0      490 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/serialize_reg_impl.h
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/vector2d_export.h
--rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/vector2d_export_streams.h
--rw-r--r--   0        0        0     7359 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/include/geometry/util.h
--rw-r--r--   0        0        0    61825 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/src/curvilinear_coordinate_system.cc
--rw-r--r--   0        0        0     7263 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/src/segment.cc
--rw-r--r--   0        0        0     2915 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/src/serialize/public/serialize_public.cc
--rw-r--r--   0        0        0     2910 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/src/serialize/serialize_curvil_cs.cc
--rw-r--r--   0        0        0     3618 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/third_party/crdc/src/util.cc
--rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 frenetix-0.2.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     2354 2022-11-09 12:37:21.000000 frenetix-0.3.0/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 frenetix-0.3.0/.gitignore
+-rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 frenetix-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 frenetix-0.3.0/.gitmodules
+-rw-r--r--   0        0        0     9426 2022-11-09 12:37:21.000000 frenetix-0.3.0/CMakeLists.txt
+-rw-r--r--   0        0        0     7632 2022-11-09 12:37:21.000000 frenetix-0.3.0/LICENSE
+-rw-r--r--   0        0        0      606 2022-11-09 12:37:21.000000 frenetix-0.3.0/README.md
+-rw-r--r--   0        0        0     1007 2022-11-09 12:37:21.000000 frenetix-0.3.0/cmake/AppleOpenMP.cmake
+-rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 frenetix-0.3.0/cmake/external/ExternalBoost.cmake
+-rw-r--r--   0        0        0      909 2022-11-09 12:37:21.000000 frenetix-0.3.0/cmake/external/ExternalDrivabilityChecker.cmake
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 frenetix-0.3.0/cmake/external/ExternalEigen.cmake
+-rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 frenetix-0.3.0/cmake/external/ExternalTaskflow.cmake
+-rw-r--r--   0        0        0     1446 2022-11-09 12:37:21.000000 frenetix-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 frenetix-0.3.0/requirements.txt
+-rw-r--r--   0        0        0     2832 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/CMakeLists.txt
+-rw-r--r--   0        0        0     3641 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/CoordinateSystemWrapper.cpp
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/CoordinateSystemWrapper.hpp
+-rw-r--r--   0        0        0     6628 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/TrajectoryHandler.cpp
+-rw-r--r--   0        0        0     3682 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/TrajectoryHandler.hpp
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/geometryMsgs.cpp
+-rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/geometryMsgs.hpp
+-rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/math/covariance.hpp
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/math/mvn.cpp
+-rw-r--r--   0        0        0     1579 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/math/mvn.hpp
+-rw-r--r--   0        0        0    46387 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/math/mvndst.f
+-rw-r--r--   0        0        0      448 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/math/mvndst.hpp
+-rw-r--r--   0        0        0     4489 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/cartesianSampleBinding.cpp
+-rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/cartesianSampleBinding.hpp
+-rw-r--r--   0        0        0     3298 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/coordinateSystemWrapperBinding.cpp
+-rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/coordinateSystemWrapperBinding.hpp
+-rw-r--r--   0        0        0      570 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/costStrategyBinding.cpp
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/costStrategyBinding.hpp
+-rw-r--r--   0        0        0     4590 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/curviLinearSampleBinding.cpp
+-rw-r--r--   0        0        0      315 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/curviLinearSampleBinding.hpp
+-rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/feasabilityStrategyBinding.cpp
+-rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/feasabilityStrategyBinding.hpp
+-rw-r--r--   0        0        0     1851 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/geometryMsgsBinding.cpp
+-rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/geometryMsgsBinding.hpp
+-rw-r--r--   0        0        0     4628 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/handlerBinding.cpp
+-rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/handlerBinding.hpp
+-rw-r--r--   0        0        0     1032 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/mainBindings.cpp
+-rw-r--r--   0        0        0     2959 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/polynomialTrajectoryBinding.cpp
+-rw-r--r--   0        0        0      300 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/polynomialTrajectoryBinding.hpp
+-rw-r--r--   0        0        0     9162 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/costFunctionsBinding.cpp
+-rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/costFunctionsBinding.hpp
+-rw-r--r--   0        0        0     3011 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/feasabilityFunctionsBinding.cpp
+-rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/feasabilityFunctionsBinding.hpp
+-rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/otherFunctionsBinding.cpp
+-rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/otherFunctionsBinding.hpp
+-rw-r--r--   0        0        0     8229 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectorySampleBinding.cpp
+-rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectorySampleBinding.hpp
+-rw-r--r--   0        0        0      981 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectoryStrategyBinding.cpp
+-rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/pybind11Bindings/trajectoryStrategyBinding.hpp
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/.gitkeep
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/__init__.py
+-rw-r--r--   0        0        0      787 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/__init__.pyi
+-rw-r--r--   0        0        0    16399 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/_frenetix/__init__.pyi
+-rw-r--r--   0        0        0     1210 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/_frenetix/trajectory_functions/__init__.pyi
+-rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/_frenetix/trajectory_functions/cost_functions.pyi
+-rw-r--r--   0        0        0     1750 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/_frenetix/trajectory_functions/feasability_functions.pyi
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/_version.py
+-rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/_version.pyi
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/py.typed
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/trajectory_functions/__init__.py
+-rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/trajectory_functions/__init__.pyi
+-rw-r--r--   0        0        0      354 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/trajectory_functions/cost_functions/__init__.py
+-rw-r--r--   0        0        0     2199 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/trajectory_functions/cost_functions/__init__.pyi
+-rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/trajectory_functions/feasability_functions/__init__.py
+-rw-r--r--   0        0        0      868 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/python/frenetix/trajectory_functions/feasability_functions/__init__.pyi
+-rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateAccelerationCost.cpp
+-rw-r--r--   0        0        0     1111 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateAccelerationCost.hpp
+-rw-r--r--   0        0        0     5716 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateCollisionProbabilityFast.cpp
+-rw-r--r--   0        0        0     4497 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateCollisionProbabilityFast.hpp
+-rw-r--r--   0        0        0     1999 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateCollisionProbabilityMahalanobis.cpp
+-rw-r--r--   0        0        0     1842 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateCollisionProbabilityMahalanobis.hpp
+-rw-r--r--   0        0        0     2188 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateDistanceToObstacleCost.cpp
+-rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateDistanceToObstacleCost.hpp
+-rw-r--r--   0        0        0      687 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateDistanceToReferencePathCost.cpp
+-rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateDistanceToReferencePathCost.hpp
+-rw-r--r--   0        0        0      923 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateJerkCost.cpp
+-rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateJerkCost.hpp
+-rw-r--r--   0        0        0      554 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateLaneCenterOffsetCost.cpp
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateLaneCenterOffsetCost.hpp
+-rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateLateralJerkCost.cpp
+-rw-r--r--   0        0        0      399 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateLateralJerkCost.hpp
+-rw-r--r--   0        0        0      553 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateLongitudinalJerkCost.cpp
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateLongitudinalJerkCost.hpp
+-rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateLongitudinalVelocityCost.cpp
+-rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateLongitudinalVelocityCost.hpp
+-rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateOrientationOffsetCost.cpp
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateOrientationOffsetCost.hpp
+-rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateSteeringAngleCost.cpp
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateSteeringAngleCost.hpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateSteeringRateCost.cpp
+-rw-r--r--   0        0        0      387 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateSteeringRateCost.hpp
+-rw-r--r--   0        0        0      749 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateVelocityOffsetCost.cpp
+-rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateVelocityOffsetCost.hpp
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateYawCost.cpp
+-rw-r--r--   0        0        0      342 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostFunctions/CalculateYawCost.hpp
+-rw-r--r--   0        0        0      608 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/CostStrategy.hpp
+-rw-r--r--   0        0        0     1236 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckAccelerationConstraint.cpp
+-rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckAccelerationConstraint.hpp
+-rw-r--r--   0        0        0     1064 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckCurvatureConstraints.cpp
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckCurvatureConstraints.hpp
+-rw-r--r--   0        0        0     1306 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckCurvatureRateConstrains.cpp
+-rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckCurvatureRateConstrains.hpp
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckVelocityConstraints.cpp
+-rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckVelocityConstraints.hpp
+-rw-r--r--   0        0        0     1158 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckYawRateConstraint.cpp
+-rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckYawRateConstraint.hpp
+-rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/FeasabilityStrategy.hpp
+-rw-r--r--   0        0        0     4949 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/Functions/ComputeInitalState.cpp
+-rw-r--r--   0        0        0      708 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/Functions/ComputeInitalState.hpp
+-rw-r--r--   0        0        0     8066 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/Functions/FillCoordinates.cpp
+-rw-r--r--   0        0        0      700 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/Functions/FillCoordinates.hpp
+-rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/strategies/TrajectoryStrategy.hpp
+-rw-r--r--   0        0        0     1752 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/trajectory/CartesianSample.cpp
+-rw-r--r--   0        0        0     1892 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/trajectory/CartesianSample.hpp
+-rw-r--r--   0        0        0     1724 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/trajectory/CurvilinearSample.cpp
+-rw-r--r--   0        0        0     1620 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/trajectory/CurvilinearSample.hpp
+-rw-r--r--   0        0        0     8634 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/trajectory/TrajectorySample.cpp
+-rw-r--r--   0        0        0     3840 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/trajectory/TrajectorySample.hpp
+-rw-r--r--   0        0        0     9430 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/trajectory/polynomial.hpp
+-rw-r--r--   0        0        0     2958 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/util.cpp
+-rw-r--r--   0        0        0     3460 2022-11-09 12:37:21.000000 frenetix-0.3.0/src/util.hpp
+-rw-r--r--   0        0        0     1540 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/CMakeLists.txt
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/application_settings.h
+-rw-r--r--   0        0        0    27845 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/curvilinear_coordinate_system.h
+-rw-r--r--   0        0        0     7909 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/segment.h
+-rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/basic_types.h
+-rw-r--r--   0        0        0      989 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/curvilinear_coordinate_system_export.h
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/export_structs/curvilinear_coordinate_system_export_struct.h
+-rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/icurvilinear_coordinate_system_export.h
+-rw-r--r--   0        0        0      537 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/public/serialize_public.h
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/serialize.h
+-rw-r--r--   0        0        0      490 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/serialize_reg_impl.h
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/vector2d_export.h
+-rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/serialize/vector2d_export_streams.h
+-rw-r--r--   0        0        0     7359 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/include/geometry/util.h
+-rw-r--r--   0        0        0    61825 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/src/curvilinear_coordinate_system.cc
+-rw-r--r--   0        0        0     7263 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/src/segment.cc
+-rw-r--r--   0        0        0     2915 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/src/serialize/public/serialize_public.cc
+-rw-r--r--   0        0        0     2910 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/src/serialize/serialize_curvil_cs.cc
+-rw-r--r--   0        0        0     3618 2022-11-09 12:37:21.000000 frenetix-0.3.0/third_party/crdc/src/util.cc
+-rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 frenetix-0.3.0/PKG-INFO
```

### Comparing `frenetix-0.2.0rc5/.github/workflows/build_wheels.yml` & `frenetix-0.3.0/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/.gitlab-ci.yml` & `frenetix-0.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/CMakeLists.txt` & `frenetix-0.3.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/LICENSE` & `frenetix-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/README.md` & `frenetix-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/cmake/AppleOpenMP.cmake` & `frenetix-0.3.0/cmake/AppleOpenMP.cmake`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/cmake/external/ExternalBoost.cmake` & `frenetix-0.3.0/cmake/external/ExternalBoost.cmake`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/cmake/external/ExternalDrivabilityChecker.cmake` & `frenetix-0.3.0/cmake/external/ExternalDrivabilityChecker.cmake`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/cmake/external/ExternalEigen.cmake` & `frenetix-0.3.0/cmake/external/ExternalEigen.cmake`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/cmake/external/ExternalTaskflow.cmake` & `frenetix-0.3.0/cmake/external/ExternalTaskflow.cmake`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/pyproject.toml` & `frenetix-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/CMakeLists.txt` & `frenetix-0.3.0/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/CoordinateSystemWrapper.cpp` & `frenetix-0.3.0/src/CoordinateSystemWrapper.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/CoordinateSystemWrapper.hpp` & `frenetix-0.3.0/src/CoordinateSystemWrapper.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/TrajectoryHandler.cpp` & `frenetix-0.3.0/src/TrajectoryHandler.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,16 @@
             //All costFunctions
             for(auto& [funName, function] : m_costFunctions)
             {
                 function->evaluateTrajectory(trajectory);
             }
         }
     }
+
+    removeInvalid();
 }
 
 void TrajectoryHandler::evaluateAllCurrentFunctionsConcurrent(bool calculateAllCosts)
 {
     //Iterate over all trajectories
     for(auto& trajectory: m_trajectories)
     {
@@ -128,14 +130,46 @@
         A.precede(B);
         B.precede(C);
     }
     m_executor.run(m_taskflow).wait();
 
     m_taskflow.clear();
 
+    removeInvalid();
+}
+
+void TrajectoryHandler::removeInvalid() {
+    auto new_end = std::remove_if(
+        m_trajectories.begin(),
+        m_trajectories.end(),
+        [](const TrajectorySample& traj) {
+            return !traj.m_valid;
+        }
+    );
+    m_trajectories.erase(new_end, m_trajectories.end());
+}
+
+size_t TrajectoryHandler::getFeasibleCount() const {
+    return std::count_if(
+        m_trajectories.cbegin(),
+        m_trajectories.cend(),
+        [](const TrajectorySample& traj) {
+            return traj.m_valid && traj.m_feasible;
+        }
+    );
+}
+
+size_t TrajectoryHandler::getInfeasibleCount() const {
+    return std::count_if(
+        m_trajectories.cbegin(),
+        m_trajectories.cend(),
+        [](const TrajectorySample& traj) {
+            return traj.m_valid && !traj.m_feasible;
+        }
+    );
 }
 
 void TrajectoryHandler::sort()
 {
     std::sort(
         m_trajectories.begin(),
         m_trajectories.end(),
@@ -147,32 +181,30 @@
             return a.m_cost < b.m_cost;
         }
     );
 }
 
 void TrajectoryHandler::generateTrajectories(const SamplingMatrixXd& samplingMatrix, bool lowVelocityMode)
 {
-    Eigen::Vector3d x0_lonOrder {0,1,2};
-    Eigen::Vector2d x1_lonOrder {1,2};
-
+    m_trajectories.clear();
     m_trajectories.reserve(samplingMatrix.rows());
 
     for(Eigen::Index iii = 0; iii < samplingMatrix.rows(); iii++)
     {
         Eigen::Vector3d x0_lon {samplingMatrix.row(iii)[2], samplingMatrix.row(iii)[3], samplingMatrix.row(iii)[4]};
         Eigen::Vector2d x1_lon {samplingMatrix.row(iii)[5], samplingMatrix.row(iii)[6]};
 
         TrajectorySample::LongitudinalTrajectory longitudinalTrajectory (
             samplingMatrix.row(iii)[0],
             samplingMatrix.row(iii)[1],
             x0_lon,
             x1_lon,
-            x0_lonOrder,
-            x1_lonOrder
-            );
+            TrajectorySample::LongitudinalX0Order,
+            TrajectorySample::LongitudinalXDOrder
+        );
 
         double t1 = 0.0;
         if (lowVelocityMode) {
             t1 = longitudinalTrajectory(samplingMatrix.row(iii)[1]) - x0_lon[0];
             if (t1 <= 0.0) {
                 t1 = samplingMatrix.row(iii)[1];
             }
@@ -196,12 +228,11 @@
             lateralTrajectory,
             iii,
             samplingMatrix.row(iii)
             );
     }
 }
 
-
 void TrajectoryHandler::resetTrajectories()
 {
     m_trajectories.clear();
 }
```

### Comparing `frenetix-0.2.0rc5/src/TrajectoryHandler.hpp` & `frenetix-0.3.0/src/TrajectoryHandler.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,25 @@
     void generateTrajectories(const SamplingMatrixXd& samplingMatrix, bool lowVelocityMode);
     void sort();
     void addFeasabilityFunction(std::shared_ptr<FeasabilityStrategy> function);
     void addFunction(std::shared_ptr<TrajectoryStrategy> function);
     void addCostFunction(std::shared_ptr<CostStrategy> function);
     void clearCostFunctions();
     void setAllCostWeightsToZero();
+
+    /**
+     * Get number of feasible trajectories.
+     */
+    size_t getFeasibleCount() const;
+
+    /**
+     * Get number of infeasible trajectories.
+     */
+    size_t getInfeasibleCount() const;
+
     /**
      * @brief Evaluates all current functions for each trajectory in the container.
      * 
      * This function iterates over all trajectories in the container, and for each trajectory,
      * evaluates the m_otherFunctions, m_feasabilityFunctions, and m_costFunctions. This function is 
      * used to update the trajectories' properties based on the given functions.
      * 
@@ -83,10 +94,12 @@
     std::map<std::string, std::shared_ptr<CostStrategy>> m_costFunctions;
     std::map<std::string, std::shared_ptr<FeasabilityStrategy>> m_feasabilityFunctions;
     std::map<std::string, std::shared_ptr<TrajectoryStrategy>> m_otherFunctions;
 private:
     double m_dt;
     tf::Taskflow m_taskflow;
     tf::Executor m_executor;
+
+    void removeInvalid();
 };
 
 #endif
```

### Comparing `frenetix-0.2.0rc5/src/geometryMsgs.cpp` & `frenetix-0.3.0/src/geometryMsgs.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/geometryMsgs.hpp` & `frenetix-0.3.0/src/geometryMsgs.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/math/covariance.hpp` & `frenetix-0.3.0/src/math/covariance.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/math/mvn.cpp` & `frenetix-0.3.0/src/math/mvn.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 }
 
 double bvn_prob(
     const Eigen::AlignedBox<double, 2>& box,
     const Eigen::Matrix<double, 2, 1>& means,
     const Eigen::Matrix<double, 2, 2>& covar
 ) {
-    check_covariance_matrix(covar);
+    // check_covariance_matrix(covar);
 
     Eigen::Vector2d stddev = covar.diagonal().array().sqrt();
 
     Eigen::Vector2d norm_lower = (box.min() - means).array() / stddev.array();
     Eigen::Vector2d norm_upper = (box.max() - means).array() / stddev.array();
 
     Eigen::AlignedBox2d norm_box { norm_lower, norm_upper };
```

### Comparing `frenetix-0.2.0rc5/src/math/mvn.hpp` & `frenetix-0.3.0/src/math/mvn.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/math/mvndst.f` & `frenetix-0.3.0/src/math/mvndst.f`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/cartesianSampleBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/cartesianSampleBinding.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/coordinateSystemWrapperBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/coordinateSystemWrapperBinding.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
         // TODO: Registering the CCS class is required for correct type signatures,
         // but we can't register the class here since it is also exported by commonroad_dc.
         // Registering it multiple times would result in pybind11 errors.
         // py::class_<geometry::CurvilinearCoordinateSystem, std::shared_ptr<geometry::CurvilinearCoordinateSystem>>(m, "_CurvilinearCoordinateSystem", py::module_local());
 
         py::class_<CoordinateSystemWrapper, std::shared_ptr<CoordinateSystemWrapper>>(m, "CoordinateSystemWrapper")
             .def(py::init<Eigen::Ref<RowMatrixXd>>(), py::arg("ref_path"))
-            .def_property("system", &CoordinateSystemWrapper::getSystem, &CoordinateSystemWrapper::setSystem)
+            // CCS property is problematic...
+            // .def_property("system", &CoordinateSystemWrapper::getSystem, &CoordinateSystemWrapper::setSystem)
             .def_property("ref_pos",
                           [](CoordinateSystemWrapper &self) -> Eigen::Ref<Eigen::VectorXd> { return self.m_refPos;},
                           [](CoordinateSystemWrapper &self, const Eigen::Ref<const Eigen::VectorXd> arr) {self.m_refPos = arr;})
             .def_property("ref_curv",
                           [](CoordinateSystemWrapper &self) -> Eigen::Ref<Eigen::VectorXd> { return self.m_refCurv;},
                           [](CoordinateSystemWrapper &self, const Eigen::Ref<const Eigen::VectorXd> arr) {self.m_refCurv = arr;})
             .def_property("ref_theta",
```

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/costStrategyBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/costStrategyBinding.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/curviLinearSampleBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/curviLinearSampleBinding.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/feasabilityStrategyBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/feasabilityStrategyBinding.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/geometryMsgsBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/geometryMsgsBinding.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,16 @@
             }))
             .def("__repr__", [](const PoseWithCovariance &p) {
                 std::ostringstream oss;
                 oss << p;
                 return oss.str();
             })
             .def_readonly("position", &PoseWithCovariance::position)
-            .def_readonly("orientation", &PoseWithCovariance::orientation)
+            .def_property_readonly("orientation",
+                          [](PoseWithCovariance &self) -> Eigen::Ref<Eigen::Vector4d> { return self.orientation.coeffs(); })
             .def_readonly("covariance", &PoseWithCovariance::covariance);
 
         py::class_<PredictedObject>(m, "PredictedObject")
             //.def(py::init<size_t>())
             .def(py::init<int, const std::vector<PoseWithCovariance>&, double, double>())
             .def("__repr__", [](const PredictedObject &p) {
                 std::ostringstream oss;
```

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/handlerBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/handlerBinding.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,24 @@
             (
                 "evaluate_all_current_functions_concurrent", 
                 &TrajectoryHandler::evaluateAllCurrentFunctionsConcurrent, 
                 py::arg("calculateAllCosts") = false
             )
             .def
             (
+                "get_feasible_count",
+                &TrajectoryHandler::getFeasibleCount
+            )
+            .def
+            (
+                "get_infeasible_count",
+                &TrajectoryHandler::getInfeasibleCount
+            )
+            .def
+            (
                 "get_sorted_trajectories", 
                 [](TrajectoryHandler &self) 
                 {
                     self.sort();
                     return py::make_iterator(self.m_trajectories.begin(), self.m_trajectories.end());
                 }
                 , py::keep_alive<0, 1>() // Keep object alive while iterator is used
```

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/mainBindings.cpp` & `frenetix-0.3.0/src/pybind11Bindings/mainBindings.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 #include "trajectoryStrategyBinding.hpp"
 
 namespace py = pybind11;
 namespace plannerCPP
 {
     PYBIND11_MODULE(_frenetix, m)
     {
-        initBindHandler(m);
+        // NOTE: Order of these bindings is critical to ensure proper stubs generation
         initBindCoordinateSystemWrapper(m);
+
         initBindCartesianSample(m);
         initBindCurviLinearSample(m);
+
         initBindPolynomialTrajectory(m);
-        initBindTrajectoryStrategy(m);
         initBindTrajectorySample(m);
         initBindGeometryMsg(m);
 
+        initBindTrajectoryStrategy(m);
+
+        initBindHandler(m);
+
         py::register_exception<invalid_covariance_matrix_error>(m, "InvalidCovarianceMatrixError", PyExc_ValueError);
     }
 } //plannerCPP
```

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/polynomialTrajectoryBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/polynomialTrajectoryBinding.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 //pybind includes
 #include <pybind11/eigen.h> // IWYU pragma: keep
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
 #include <Eigen/Core>
 #include <string>
+#include <type_traits>
 
 #include "polynomial.hpp"
+#include "TrajectorySample.hpp"
 
 #include "polynomialTrajectoryBinding.hpp"
 
 namespace py = pybind11;
 
 namespace plannerCPP
 {
@@ -17,58 +19,62 @@
     /**
      * @brief Function to create polynomial Trajectories of different degrees and giving it a suffix
      * 
      * @tparam Degree 
      * @param m 
      * @param pre Pre Suffix for the class
      */
-    template <int Degree>
+    template <int Degree, int X0, int XD, typename RefType>
     void bindPolynomialtrajectory(py::module &m, const std::string &pre) 
     {
-        py::class_<PolynomialTrajectory<Degree>>(m, (pre + "Trajectory").c_str())
+        using Traj = PolynomialTrajectory<Degree, X0, XD>;
+
+        static_assert(std::is_same<RefType, Traj>::value, "RefType mismatch");
+
+        py::class_<Traj>(m, (pre + "Trajectory").c_str())
             .def(py::init([](double t0, 
                             double t1, 
-                            Eigen::VectorXd x_0, 
-                            Eigen::VectorXd x_d, 
-                            Eigen::VectorXd x_0_order, 
-                            Eigen::VectorXd x_d_order) 
-                            {return new PolynomialTrajectory<Degree>(t0, t1, x_0, x_d, x_0_order, x_d_order);}), 
+                            typename Traj::VectorX0 x_0, 
+                            typename Traj::VectorXD x_d, 
+                            typename Traj::OrderVectorX0 x_0_order, 
+                            typename Traj::OrderVectorXD x_d_order) 
+                            {return new Traj(t0, t1, x_0, x_d, x_0_order, x_d_order);}), 
                             py::arg("tau_0"), 
                             py::arg("delta_tau"), 
                             py::arg("x_0"), 
                             py::arg("x_d"),
-                            py::arg("x_0_order") = Eigen::VectorXd(), 
-                            py::arg("x_d_order") = Eigen::VectorXd())
-            .def_property_readonly("coeffs", &PolynomialTrajectory<Degree>::getCoeffs)
-            .def("__call__", py::vectorize(&PolynomialTrajectory<Degree>::operator()))
-            .def("squared_jerk_integral", &PolynomialTrajectory<Degree>::squaredJerkIntegral)
-            .def_property_readonly("delta_tau", &PolynomialTrajectory<Degree>::get_t1)
+                            py::arg("x_0_order") = typename Traj::VectorX0(), 
+                            py::arg("x_d_order") = typename Traj::VectorXD())
+            .def_property_readonly("coeffs", &Traj::getCoeffs)
+            .def("__call__", py::vectorize(&Traj::operator()))
+            .def("squared_jerk_integral", &Traj::squaredJerkIntegral)
+            .def_property_readonly("delta_tau", &Traj::get_t1)
             .def(py::pickle(
-                [](const PolynomialTrajectory<Degree> &traj) { // __getstate__
+                [](const Traj &traj) { // __getstate__
                     using namespace pybind11::literals; // to bring in the `_a` literal
                     const auto coeffs = traj.getCoeffs();
 
                     py::dict d(
                         "coeffs"_a=coeffs
                     );
 
                     return d;
                 },
                 [](py::dict d) { // __setstate__
                     py::object obj = d["coeffs"];
                     typename Eigen::Vector<double, Degree + 1> coeffs = obj.cast<Eigen::Vector<double, Degree + 1>>();
-                    PolynomialTrajectory<Degree> traj { coeffs };
+                    Traj traj { coeffs };
 
                     return traj;
                 }
             ));
     }
 
     void initBindPolynomialTrajectory(pybind11::module &m) 
     {
         // Bind the PolynomialTrajectory class
-        bindPolynomialtrajectory<4>(m, "Quartic");
-        bindPolynomialtrajectory<5>(m, "Quintic");
+        bindPolynomialtrajectory<4, 3, 2, TrajectorySample::LongitudinalTrajectory>(m, "Quartic");
+        bindPolynomialtrajectory<5, 3, 3, TrajectorySample::LateralTrajectory>(m, "Quintic");
     }
 
 } //plannerCPP
```

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/costFunctionsBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/costFunctionsBinding.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/feasabilityFunctionsBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/feasabilityFunctionsBinding.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryFunctionsBinding/otherFunctionsBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/trajectoryFunctionsBinding/otherFunctionsBinding.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/trajectorySampleBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/trajectorySampleBinding.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,54 @@
 namespace py = pybind11;
 
 namespace plannerCPP
 {
 
     void initBindTrajectorySample(pybind11::module &m) 
     {
+        py::class_<PlannerState::Cartesian>(m, "CartesianPlannerState")
+            .def(py::init<Eigen::Vector2d, double, double, double, double>(),
+                 py::arg("pos"),
+                 py::arg("orientation"), 
+                 py::arg("velocity"),
+                 py::arg("acceleration"),
+                 py::arg("steering_angle")
+            )
+            .def_readwrite("pos", &PlannerState::Cartesian::pos)
+            .def_readwrite("orientation", &PlannerState::Cartesian::orientation)
+            .def_readwrite("velocity", &PlannerState::Cartesian::velocity)
+            .def_readwrite("acceleration", &PlannerState::Cartesian::acceleration)
+            .def_readwrite("steering_angle", &PlannerState::Cartesian::steering_angle);
+
+        py::class_<PlannerState::Curvilinear>(m, "CurvilinearPlannerState")
+            .def(py::init<Eigen::Vector3d, Eigen::Vector3d>(),
+                 py::arg("x0_lon"),
+                 py::arg("x0_lat")
+            )
+            .def_readwrite("x0_lon", &PlannerState::Curvilinear::x0_lon)
+            .def_readwrite("x0_lat", &PlannerState::Curvilinear::x0_lat);
+
+        py::class_<PlannerState>(m, "PlannerState")
+            .def(py::init<PlannerState::Cartesian, PlannerState::Curvilinear, double>(),
+                 py::arg("x_0"),
+                 py::arg("x_cl"),
+                 py::arg("wheelbase")
+            )
+            .def_readwrite("x_0", &PlannerState::x_0)
+            .def_readwrite("x_cl", &PlannerState::x_cl)
+            .def_readwrite("wheelbase", &PlannerState::wheelbase);
+
+        m.def("compute_initial_state",
+                &computeInitialState,
+                py::arg("coordinate_system"),
+                py::arg("x_0"),
+                py::arg("wheelbase"),
+                py::arg("low_velocity_mode")
+            );
+
         py::class_<TrajectorySample>(m, "TrajectorySample")
             .def(py::init<double, TrajectorySample::LongitudinalTrajectory, TrajectorySample::LateralTrajectory, int>(),
                  py::arg("dt"),
                  py::arg("trajectoryLongitudinal"), 
                  py::arg("trajectoryLateral"), 
                  py::arg("uniqueId"))
             .def(py::init<double, double, double, double, double>(),
@@ -51,15 +91,23 @@
             .def_readwrite("costMap", &TrajectorySample::m_costMap)
             .def_readwrite("feasible", &TrajectorySample::m_feasible)
             .def_readwrite("valid", &TrajectorySample::m_valid)
             .def_property("sampling_parameters",
                 [](TrajectorySample &self) -> Eigen::Ref<Eigen::VectorXd> { return self.m_samplingParameters;},
                 [](TrajectorySample &self, const Eigen::Ref<const Eigen::VectorXd> arr) {self.m_samplingParameters = arr;})
 
-        
+            .def_static("compute_standstill_trajectory",
+                &TrajectorySample::standstillTrajectory,
+                py::arg("coordinate_system"),
+                py::arg("planner_state"),
+                py::arg("dt"),
+                py::arg("horizon")
+            )
+
+
             .def(py::pickle(
                 [](const TrajectorySample &traj) { // __getstate__
                     using namespace pybind11::literals; // to bring in the `_a` literal
                     py::dict d(
                         "dt"_a=traj.m_dT,
 
                         "cost"_a=traj.m_cost,
```

### Comparing `frenetix-0.2.0rc5/src/pybind11Bindings/trajectoryStrategyBinding.cpp` & `frenetix-0.3.0/src/pybind11Bindings/trajectoryStrategyBinding.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/python/frenetix/__init__.py` & `frenetix-0.3.0/src/python/frenetix/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from ._frenetix import (
     CartesianSample,
     CoordinateSystemWrapper, CurviLinearSample,
     QuarticTrajectory, QuinticTrajectory,
     PoseWithCovariance, PredictedObject,
     TrajectoryHandler,
     TrajectorySample,
+    PlannerState,
+    CartesianPlannerState,
+    CurvilinearPlannerState,
     trajectory_functions
 )
 
 __all__ = (
     "CartesianSample",
     "CoordinateSystemWrapper",
     "CurviLinearSample",
     "PoseWithCovariance",
     "PredictedObject",
     "QuarticTrajectory",
     "QuinticTrajectory",
     "TrajectoryHandler",
     "TrajectorySample",
+    "PlannerState",
+    "CartesianPlannerState",
+    "CurvilinearPlannerState",
     "trajectory_functions"
 )
```

### Comparing `frenetix-0.2.0rc5/src/python/frenetix/_frenetix/trajectory_functions/__init__.pyi` & `frenetix-0.3.0/src/python/frenetix/_frenetix/trajectory_functions/feasability_functions.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 from __future__ import annotations
-import frenetix._frenetix.trajectory_functions
-import typing
 import frenetix._frenetix
-
-__all__ = [
-    "ComputeInitialState",
-    "CostStrategy",
-    "FeasabilityStrategy",
-    "FillCoordinates",
-    "TrajectoryStrategy",
-    "cost_functions",
-    "feasability_functions"
-]
-
-
-class TrajectoryStrategy():
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    @property
-    def name(self) -> str:
-        """
-        :type: str
-        """
-    pass
-class CostStrategy(TrajectoryStrategy):
-    pass
-class FeasabilityStrategy(TrajectoryStrategy):
-    pass
-class FillCoordinates(TrajectoryStrategy):
-    def __init__(self, lowVelocityMode: bool, initialOrientation: float, coordinateSystem: frenetix._frenetix.CoordinateSystemWrapper, horizon: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class ComputeInitialState(TrajectoryStrategy):
-    def __init__(self, coordinateSystem: frenetix._frenetix.CoordinateSystemWrapper, wheelBase: float, steeringAngle: float, lowVelocityMode: bool) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
+import frenetix._frenetix.trajectory_functions
+__all__ = ['CheckAccelerationConstraint', 'CheckCurvatureConstraint', 'CheckCurvatureRateConstraint', 'CheckVelocityConstraint', 'CheckYawRateConstraint']
+class CheckAccelerationConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy):
+    def __init__(self, switchingVelocity: float, maxAcceleration: float, wholeTrajectory: bool) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CheckCurvatureConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy):
+    def __init__(self, deltaMax: float, wheelbase: float, wholeTrajectory: bool) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CheckCurvatureRateConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy):
+    def __init__(self, wheelbase: float, velocityDeltaMax: float, wholeTrajectory: bool) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CheckVelocityConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy):
+    def __init__(self, wholeTrajectory: bool) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CheckYawRateConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy):
+    def __init__(self, deltaMax: float, wheelbase: float, wholeTrajectory: bool) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
```

### Comparing `frenetix-0.2.0rc5/src/python/frenetix/_frenetix/trajectory_functions/feasability_functions/__init__.pyi` & `frenetix-0.3.0/src/python/frenetix/_frenetix/trajectory_functions/__init__.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 from __future__ import annotations
-import frenetix._frenetix.trajectory_functions.feasability_functions
-import typing
-import frenetix._frenetix.trajectory_functions
-
-__all__ = [
-    "CheckAccelerationConstraint",
-    "CheckCurvatureConstraint",
-    "CheckCurvatureRateConstraint",
-    "CheckVelocityConstraint",
-    "CheckYawRateConstraint"
-]
-
-
-class CheckAccelerationConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, switchingVelocity: float, maxAcceleration: float, wholeTrajectory: bool) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
+import frenetix._frenetix
+from . import cost_functions
+from . import feasability_functions
+__all__ = ['ComputeInitialState', 'CostStrategy', 'FeasabilityStrategy', 'FillCoordinates', 'TrajectoryStrategy', 'cost_functions', 'feasability_functions']
+class ComputeInitialState(TrajectoryStrategy):
+    def __init__(self, coordinateSystem: frenetix._frenetix.CoordinateSystemWrapper, wheelBase: float, steeringAngle: float, lowVelocityMode: bool) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CostStrategy(TrajectoryStrategy):
     pass
-class CheckCurvatureConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, deltaMax: float, wheelbase: float, wholeTrajectory: bool) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CheckCurvatureRateConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, wheelbase: float, velocityDeltaMax: float, wholeTrajectory: bool) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CheckVelocityConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, wholeTrajectory: bool) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CheckYawRateConstraint(frenetix._frenetix.trajectory_functions.FeasabilityStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, deltaMax: float, wheelbase: float, wholeTrajectory: bool) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
+class FeasabilityStrategy(TrajectoryStrategy):
     pass
+class FillCoordinates(TrajectoryStrategy):
+    def __init__(self, lowVelocityMode: bool, initialOrientation: float, coordinateSystem: frenetix._frenetix.CoordinateSystemWrapper, horizon: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class TrajectoryStrategy:
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+    @property
+    def name(self) -> str:
+        ...
```

### Comparing `frenetix-0.2.0rc5/src/python/frenetix/trajectory_functions/cost_functions/__init__.pyi` & `frenetix-0.3.0/src/python/frenetix/_frenetix/trajectory_functions/cost_functions.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 from __future__ import annotations
-import frenetix._frenetix.trajectory_functions.cost_functions
-import typing
+import frenetix._frenetix
 import frenetix._frenetix.trajectory_functions
 import numpy
-from frenetix._frenetix import TrajectorySample, PredictedObject
-
-__all__ = [
-    "CalculateAccelerationCost",
-    "CalculateCollisionProbabilityFast",
-    "CalculateCollisionProbabilityMahalanobis",
-    "CalculateDistanceToObstacleCost",
-    "CalculateDistanceToReferencePathCost",
-    "CalculateJerkCost",
-    "CalculateLaneCenterOffsetCost",
-    "CalculateLateralJerkCost",
-    "CalculateLongitudinalJerkCost",
-    "CalculateLongitudinalVelocityCost",
-    "CalculateOrientationOffsetCost",
-    "CalculateSteeringAngleCost",
-    "CalculateSteeringRateCost",
-    "CalculateVelocityOffsetCost",
-    "CalculateYawCost"
-]
-
-
-class CalculateAccelerationCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateCollisionProbabilityFast(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float, predictions: typing.Dict[int, PredictedObject], vehicleLength: float, vehicleWidth: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    def printPredictions(self) -> None: ...
-    pass
-class CalculateCollisionProbabilityMahalanobis(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float, predictions: typing.Dict[int, PredictedObject]) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateDistanceToObstacleCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float, obstacles: numpy.ndarray) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateDistanceToReferencePathCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateJerkCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateLaneCenterOffsetCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateLateralJerkCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateLongitudinalJerkCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateLongitudinalVelocityCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateOrientationOffsetCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateSteeringAngleCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateSteeringRateCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateVelocityOffsetCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float, desiredSpeed: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
-class CalculateYawCost(frenetix._frenetix.trajectory_functions.CostStrategy, frenetix._frenetix.trajectory_functions.TrajectoryStrategy):
-    def __init__(self, function_name: str, cost_weight: float) -> None: ...
-    def evaluate_trajectory(self, trajectory: TrajectorySample) -> None: ...
-    pass
+import pybind11_stubgen.typing_ext
+import typing
+__all__ = ['CalculateAccelerationCost', 'CalculateCollisionProbabilityFast', 'CalculateCollisionProbabilityMahalanobis', 'CalculateDistanceToObstacleCost', 'CalculateDistanceToReferencePathCost', 'CalculateJerkCost', 'CalculateLaneCenterOffsetCost', 'CalculateLateralJerkCost', 'CalculateLongitudinalJerkCost', 'CalculateLongitudinalVelocityCost', 'CalculateOrientationOffsetCost', 'CalculateSteeringAngleCost', 'CalculateSteeringRateCost', 'CalculateVelocityOffsetCost', 'CalculateYawCost']
+class CalculateAccelerationCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateCollisionProbabilityFast(frenetix._frenetix.trajectory_functions.CostStrategy):
+    @typing.overload
+    def __init__(self, function_name: str, cost_weight: float, predictions: dict[int, frenetix._frenetix.PredictedObject], vehicleLength: float, vehicleWidth: float) -> None:
+        ...
+    @typing.overload
+    def __init__(self, function_name: str, cost_weight: float, predictions: dict[int, frenetix._frenetix.PredictedObject], vehicle_length: float, vehicle_width: float, wheelbase_rear: float, off_center_weight: float = 0.5) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+    def printPredictions(self) -> None:
+        ...
+class CalculateCollisionProbabilityMahalanobis(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float, predictions: dict[int, frenetix._frenetix.PredictedObject]) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateDistanceToObstacleCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float, obstacles: typing.Annotated[numpy.ndarray, numpy.float64, pybind11_stubgen.typing_ext.DynamicSize('m', 'n'), numpy.ndarray.flags.writeable, numpy.ndarray.flags.c_contiguous]) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateDistanceToReferencePathCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateJerkCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateLaneCenterOffsetCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateLateralJerkCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateLongitudinalJerkCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateLongitudinalVelocityCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateOrientationOffsetCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateSteeringAngleCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateSteeringRateCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateVelocityOffsetCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float, desiredSpeed: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
+class CalculateYawCost(frenetix._frenetix.trajectory_functions.CostStrategy):
+    def __init__(self, function_name: str, cost_weight: float) -> None:
+        ...
+    def evaluate_trajectory(self, trajectory: frenetix._frenetix.TrajectorySample) -> None:
+        ...
```

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateAccelerationCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateAccelerationCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateAccelerationCost.hpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateAccelerationCost.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateCollisionProbabilityFast.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateCollisionProbabilityFast.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateCollisionProbabilityFast.hpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateCollisionProbabilityFast.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateCollisionProbabilityMahalanobis.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateCollisionProbabilityMahalanobis.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateCollisionProbabilityMahalanobis.hpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateCollisionProbabilityMahalanobis.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateDistanceToObstacleCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateDistanceToObstacleCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateDistanceToObstacleCost.hpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateDistanceToObstacleCost.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateDistanceToReferencePathCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateDistanceToReferencePathCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateJerkCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateJerkCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLaneCenterOffsetCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateLaneCenterOffsetCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLateralJerkCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateLateralJerkCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLongitudinalJerkCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateLongitudinalJerkCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateLongitudinalVelocityCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateLongitudinalVelocityCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateSteeringAngleCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateSteeringAngleCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateSteeringRateCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateSteeringRateCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostFunctions/CalculateVelocityOffsetCost.cpp` & `frenetix-0.3.0/src/strategies/CostFunctions/CalculateVelocityOffsetCost.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/CostStrategy.hpp` & `frenetix-0.3.0/src/strategies/CostStrategy.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckAccelerationConstraint.cpp` & `frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckAccelerationConstraint.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckAccelerationConstraint.hpp` & `frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckAccelerationConstraint.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckCurvatureConstraints.cpp` & `frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckCurvatureConstraints.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckCurvatureConstraints.hpp` & `frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckCurvatureConstraints.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckCurvatureRateConstrains.cpp` & `frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckCurvatureRateConstrains.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckCurvatureRateConstrains.hpp` & `frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckCurvatureRateConstrains.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckYawRateConstraint.cpp` & `frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckYawRateConstraint.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityFunctions/CheckYawRateConstraint.hpp` & `frenetix-0.3.0/src/strategies/FeasabilityFunctions/CheckYawRateConstraint.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/FeasabilityStrategy.hpp` & `frenetix-0.3.0/src/strategies/FeasabilityStrategy.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/Functions/ComputeInitalState.cpp` & `frenetix-0.3.0/src/strategies/Functions/ComputeInitalState.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/Functions/ComputeInitalState.hpp` & `frenetix-0.3.0/src/strategies/Functions/ComputeInitalState.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/Functions/FillCoordinates.cpp` & `frenetix-0.3.0/src/strategies/Functions/FillCoordinates.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/Functions/FillCoordinates.hpp` & `frenetix-0.3.0/src/strategies/Functions/FillCoordinates.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/strategies/TrajectoryStrategy.hpp` & `frenetix-0.3.0/src/strategies/TrajectoryStrategy.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/trajectory/CartesianSample.cpp` & `frenetix-0.3.0/src/trajectory/CartesianSample.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/trajectory/CartesianSample.hpp` & `frenetix-0.3.0/src/trajectory/CartesianSample.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/trajectory/CurvilinearSample.cpp` & `frenetix-0.3.0/src/trajectory/CurvilinearSample.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/trajectory/CurvilinearSample.hpp` & `frenetix-0.3.0/src/trajectory/CurvilinearSample.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/trajectory/TrajectorySample.hpp` & `frenetix-0.3.0/src/trajectory/TrajectorySample.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,42 @@
-#ifndef TRAJECTORYSAMPLE_HPP
-#define TRAJECTORYSAMPLE_HPP
+#pragma once
 
 #include <stddef.h>
 #include <Eigen/Core>
 #include <map>
 #include <optional>
 #include <string>
 #include <utility>
 
 #include "CartesianSample.hpp"
 #include "CurvilinearSample.hpp"
 #include "polynomial.hpp"
+#include "CoordinateSystemWrapper.hpp"
 
+struct PlannerState {
+    struct Cartesian {
+        Eigen::Vector2d pos;
+        double orientation;
+        double velocity;
+        double acceleration;
+        double steering_angle;
+    } x_0;
+    struct Curvilinear {
+        Eigen::Vector3d x0_lon;
+        Eigen::Vector3d x0_lat;
+    } x_cl;
+    double wheelbase;
+};
+
+PlannerState::Curvilinear computeInitialState(
+        std::shared_ptr<CoordinateSystemWrapper> coordinateSystem,
+        PlannerState::Cartesian cps,
+        double wheelbase, 
+        bool lowVelocityMode
+);
 
 class TrajectorySample
 {
 public:
     size_t m_size;
     size_t m_acutualSize;
     double m_dT;
@@ -36,31 +57,42 @@
     Eigen::VectorXd m_samplingParameters;
 
     std::map<std::string, std::pair<double,double>> m_costMap;
     std::map<std::string, double> m_feasabilityMap;
 
     using LongitudinalTrajectory = PolynomialTrajectory<4, 3, 2>;
     using LateralTrajectory = PolynomialTrajectory<5, 3, 3>;
+    static const LongitudinalTrajectory::OrderVectorX0 LongitudinalX0Order;
+    static const LongitudinalTrajectory::OrderVectorXD LongitudinalXDOrder;
     LongitudinalTrajectory m_trajectoryLongitudinal;
     LateralTrajectory m_trajectoryLateral;
+
     CartesianSample m_cartesianSample;
     CurviLinearSample m_curvilinearSample;
+
     bool m_valid = true;
 
     TrajectorySample(double dt,
                      LongitudinalTrajectory trajectoryLongitudinal,
                      LateralTrajectory trajectoryLateral,
                      int uniqueId);
 
     TrajectorySample(double dt,
                      LongitudinalTrajectory trajectoryLongitudinal,
                      LateralTrajectory trajectoryLateral,
                      int uniqueId,
                      Eigen::VectorXd samplingParameters);
 
+    static TrajectorySample standstillTrajectory(
+        std::shared_ptr<CoordinateSystemWrapper> coordinateSystem,
+        PlannerState state,
+        double dt,
+        double horizon
+    );
+
     /**
      * @brief Construct a new Trajectory Sample object just with the initial position.
      *
      * @param x0
      * @param y0
      * @param orientation0
      */
@@ -97,8 +129,7 @@
 
     void addFeasabilityValueToList(std::string costFunctionName, double value);
 
 
     size_t size();
 };
 
-#endif //TRAJECTORYSAMPLE_HPP
```

### Comparing `frenetix-0.2.0rc5/src/trajectory/polynomial.hpp` & `frenetix-0.3.0/src/trajectory/polynomial.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,125 @@
 #pragma once
 
-#include <Eigen/Core>
-#include <Eigen/QR>
-#include <cassert>
 #include <cmath>
 #include <stdexcept>
 
-#include <iostream>
+#include <numeric>
+
+#include <Eigen/Core>
+#include <Eigen/QR>
 
 /**
  * @brief A class representing a polynomial trajectory of a given degree.
  *
  * The PolynomialTrajectory class is a template class, with the Degree template parameter
  * representing the degree of the polynomial trajectory. It is designed to create
  * a polynomial trajectory that satisfies a set of initial and final point conditions.
  *
- * The number of initial condions must euqal to the Degree + 1.
+ * The number of initial condions must equal to the Degree + 1.
  *
  * The class solves a system of linear equations to determine the coefficients of the monom
  * basis of the polynomial trajectory. The trajectory can be evaluated at a given time
  * using the overloaded call operator with an optional derivative parameter.
  *
  * @tparam Degree Degree of the polynomial trajectory.
+ * @tparam X0 Static dimension of first point conditions.
+ * @tparam XD Static dimension of second point conditions.
  */
 template <int Degree, int X0 = Eigen::Dynamic, int XD = Eigen::Dynamic>
 class PolynomialTrajectory
 {
     static_assert(X0 == Eigen::Dynamic || XD == Eigen::Dynamic || X0 + XD == Degree + 1, "dimensions error");
+    static_assert((X0 >= 1 || X0 == Eigen::Dynamic) && (XD >= 1 || XD == Eigen::Dynamic), "dimensions need to be positive");
+    static_assert(Degree >= 0, "degree needs to be positive");
 
 public:
     using VectorX0 = Eigen::Vector<double, X0>;
     using VectorXD = Eigen::Vector<double, XD>;
+    using OrderVectorX0 = Eigen::Vector<int, X0>;
+    using OrderVectorXD = Eigen::Vector<int, XD>;
+    using Coeffs = Eigen::Vector<double, Degree + 1>;
 
-    explicit PolynomialTrajectory(const Eigen::Vector<double, Degree + 1>& coeffs) 
+    explicit PolynomialTrajectory(const Coeffs& coeffs) 
         : coeffs{coeffs} { }
 
     /**
      * @brief Constructs a new polynomial trajectory.
      *
      * @param t0 The first time.
      * @param t1 The second time.
      * @param x_0 The first point conditions.
      * @param x_d The second point conditions.
      */
     PolynomialTrajectory(double t0, double t1,
                          const VectorX0& x_0,
                          const VectorXD& x_d,
-                         const VectorX0& x_0_order,
-                         const VectorXD& x_d_order)
+                         const OrderVectorX0& x_0_order,
+                         const OrderVectorXD& x_d_order)
         : m_t0(t0)
         , m_t1(t1)
     {
-        assert(((x_0.size()+x_d.size()-1)==Degree) && "To many or to less equations for the choosen degree");
+        if (X0 == Eigen::Dynamic || XD == Eigen::Dynamic) {
+            if (x_0.size() + x_d.size() != Degree + 1) {
+                throw std::invalid_argument { "Too many or too few equations for the chosen degree" };
+            }
 
-        assert((x_0.size() == x_0_order.size()) && "Order size not correct");
-        assert((x_d.size() == x_d_order.size()) && "Order size not correct");
+            if (x_0.size() != x_0_order.size() || x_d.size() != x_d_order.size()) {
+                throw std::invalid_argument { "Order size not correct" };
+            }
+        }
 
-        calc_coeffs(t0, t1, x_0, x_d, x_0_order, x_d_order);
+        coeffs = calc_coeffs(t0, t1, x_0, x_d, x_0_order, x_d_order);
     }
 
     /**
      * @brief Constructs a new polynomial trajectory.
      *
      * @param t0 The first time.
      * @param t1 The second time.
      * @param x_0 The first point conditions.
      * @param x_d The second point conditions.
      */
     PolynomialTrajectory(double t0, double t1,
                          const VectorX0& x_0,
                          const VectorXD& x_d)
-        : m_t0(t0)
-        , m_t1(t1)
+        : PolynomialTrajectory(t0, t1, x_0, x_d, defaultX0Order(), defaultXDOrder())
+    {
+    }
+
+    constexpr OrderVectorX0 defaultX0Order()
     {
-        VectorX0 x_0_order = VectorX0::LinSpaced(x_0.size(), 0, x_0.size() - 1);
-        VectorXD x_d_order = VectorXD::LinSpaced(x_d.size(), 0, x_d.size() - 1);
+        OrderVectorX0 x_0_order;
+        std::iota(x_0_order.begin(), x_0_order.end(), 0);
+        return x_0_order;
+    }
 
-        calc_coeffs(t0, t1, x_0, x_d, x_0_order, x_d_order);
+    constexpr OrderVectorXD defaultXDOrder()
+    {
+        OrderVectorXD x_d_order;
+        std::iota(x_d_order.begin(), x_d_order.end(), 0);
+        return x_d_order;
     }
 
     PolynomialTrajectory() = default;
 
     /**
      * @brief Calculates the polynomial coefficients.
      */
-    void calc_coeffs(double t0, double t1,
+    static Coeffs calc_coeffs(double t0, double t1,
         VectorX0 x_0, VectorXD x_d,
-        VectorX0 x_0_order, VectorXD x_d_order);
+        OrderVectorX0 x_0_order, OrderVectorXD x_d_order);
 
 
     /**
      * @brief Gets the polynomial coefficients.
      *
      * @return The coefficients as an Eigen::Vector of size Degree + 1.
      */
-    Eigen::Vector<double,Degree+1> getCoeffs() const;
+    Coeffs getCoeffs() const;
 
     /**
      * @brief Evaluates the polynomial trajectory at a given time and derivative.
      *
      * @param t The time at which to evaluate the polynomial.
      * @param derivative The order of the derivative to evaluate, defaults to 0.
      * @return The value of the polynomial at the given time and derivative.
@@ -132,22 +153,22 @@
     * @return The value of the integral of the squared jerk from 0 to \p t.
     *
     * @throw std::invalid_argument If the Degree is not 4 or 5.
     */
     constexpr double squaredJerkIntegral(double t) const;
 
 private:
-    Eigen::Vector<double, Degree+1> coeffs;
+    Coeffs coeffs;
     double m_t0, m_t1;
 };
 
 template<int Degree, int X0, int XD>
-void PolynomialTrajectory<Degree, X0, XD>::calc_coeffs(double t0, double t1,
+typename PolynomialTrajectory<Degree, X0, XD>::Coeffs PolynomialTrajectory<Degree, X0, XD>::calc_coeffs(double t0, double t1,
     VectorX0 x_0, VectorXD x_d,
-    VectorX0 x_0_order, VectorXD x_d_order)
+    OrderVectorX0 x_0_order, OrderVectorXD x_d_order)
 {
     constexpr int n = Degree + 1;
 
     ////cache a if it stays the same
     //static double lastT0 = 0;
     //static double lastT1 = 0;
 
@@ -177,29 +198,29 @@
             else
             {
                 a(iii, jjj) = 0;
             }
         }
         b(iii) = isFirstPoint ? x_0[iii] : x_d[iii - x_0.size()];
     }
-    coeffs = a.colPivHouseholderQr().solve(b);
+    return a.colPivHouseholderQr().solve(b);
 }
 
 template<int Degree, int X0, int XD>
-Eigen::Vector<double,Degree+1> PolynomialTrajectory<Degree, X0, XD>::getCoeffs() const
+typename PolynomialTrajectory<Degree, X0, XD>::Coeffs PolynomialTrajectory<Degree, X0, XD>::getCoeffs() const
 {
     return coeffs;
 }
 
 template<int Degree, int X0, int XD>
 inline constexpr
 typename PolynomialTrajectory<Degree, X0, XD>::VVV
 PolynomialTrajectory<Degree, X0, XD>::horner_eval(double t) const
 {
-    static_assert(Degree > 2, "invalid Degree: must greater than 2");
+    static_assert(Degree > 2, "invalid Degree: must greater than 2 for horner_eval");
 
     double f = coeffs[Degree];
     double fp = f;
     double fpp = fp;
 
     for (int i = Degree - 1; i >= 2; i--) {
         f = std::fma(t, f, coeffs[i]);
@@ -261,7 +282,10 @@
         double integral_squared_jerk = (36 * coeffs[3] * coeffs[3] * t +
                                         144 * coeffs[3] * coeffs[4] * t2 +
                                         192 * coeffs[4] * coeffs[4] * t3);
         return integral_squared_jerk;
     }
 }
 
+extern template class PolynomialTrajectory<4, 3, 2>;
+extern template class PolynomialTrajectory<5, 3, 3>;
+
```

### Comparing `frenetix-0.2.0rc5/src/util.cpp` & `frenetix-0.3.0/src/util.cpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/src/util.hpp` & `frenetix-0.3.0/src/util.hpp`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/CMakeLists.txt` & `frenetix-0.3.0/third_party/crdc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/include/geometry/curvilinear_coordinate_system.h` & `frenetix-0.3.0/third_party/crdc/include/geometry/curvilinear_coordinate_system.h`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/include/geometry/segment.h` & `frenetix-0.3.0/third_party/crdc/include/geometry/segment.h`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/curvilinear_coordinate_system_export.h` & `frenetix-0.3.0/third_party/crdc/include/geometry/serialize/curvilinear_coordinate_system_export.h`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/public/serialize_public.h` & `frenetix-0.3.0/third_party/crdc/include/geometry/serialize/public/serialize_public.h`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/include/geometry/serialize/vector2d_export_streams.h` & `frenetix-0.3.0/third_party/crdc/include/geometry/serialize/vector2d_export_streams.h`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/include/geometry/util.h` & `frenetix-0.3.0/third_party/crdc/include/geometry/util.h`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/src/curvilinear_coordinate_system.cc` & `frenetix-0.3.0/third_party/crdc/src/curvilinear_coordinate_system.cc`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/src/segment.cc` & `frenetix-0.3.0/third_party/crdc/src/segment.cc`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/src/serialize/public/serialize_public.cc` & `frenetix-0.3.0/third_party/crdc/src/serialize/public/serialize_public.cc`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/src/serialize/serialize_curvil_cs.cc` & `frenetix-0.3.0/third_party/crdc/src/serialize/serialize_curvil_cs.cc`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/third_party/crdc/src/util.cc` & `frenetix-0.3.0/third_party/crdc/src/util.cc`

 * *Files identical despite different names*

### Comparing `frenetix-0.2.0rc5/PKG-INFO` & `frenetix-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frenetix
-Version: 0.2.0rc5
+Version: 0.3.0
 Summary: C++-accelerated Frenet Trajectory Planning Handler
 Author-Email: Georg Schmalhofer <georg.schmalhofer@tum.de>, Tobias Markus <tobias.markus@tum.de>, Rainer Trauth <rainer.trauth@tum.de>
 Maintainer-Email: Rainer Trauth <rainer.trauth@tum.de>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/TUM-AVS/Frenetix
 Project-URL: Bug tracker, https://github.com/TUM-AVS/Frenetix/issues
 Requires-Python: <3.13,>=3.8
```

