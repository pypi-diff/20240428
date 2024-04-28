# Comparing `tmp/keras_nightly-3.3.2.dev2024042503.tar.gz` & `tmp/keras_nightly-3.3.3.dev2024042703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.2.dev2024042503.tar", last modified: Thu Apr 25 03:21:25 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.3.dev2024042703.tar", last modified: Sat Apr 27 03:20:46 2024, max compression
```

## Comparing `keras_nightly-3.3.2.dev2024042503.tar` & `keras_nightly-3.3.3.dev2024042703.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.399355 keras_nightly-3.3.2.dev2024042503/
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-25 03:21:25.399355 keras_nightly-3.3.2.dev2024042503/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.311355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.315355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.319355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.323355 keras_nightly-3.3.2.dev2024042503/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.327355 keras_nightly-3.3.2.dev2024042503/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.331355 keras_nightly-3.3.2.dev2024042503/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.335355 keras_nightly-3.3.2.dev2024042503/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.335355 keras_nightly-3.3.2.dev2024042503/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.335355 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.339355 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26214 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30920 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.343355 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18006 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28155 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.343355 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26595 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    77857 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.347355 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    47523 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.347355 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.351355 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.351355 keras_nightly-3.3.2.dev2024042503/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.351355 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.351355 keras_nightly-3.3.2.dev2024042503/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.351355 keras_nightly-3.3.2.dev2024042503/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.355355 keras_nightly-3.3.2.dev2024042503/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.355355 keras_nightly-3.3.2.dev2024042503/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.355355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.355355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.355355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.359355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.359355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25225 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    42009 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    63910 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.363355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.363355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.367355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.371355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.371355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.371355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.375355 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.375355 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.375355 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.379355 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.379355 keras_nightly-3.3.2.dev2024042503/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.379355 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.383355 keras_nightly-3.3.2.dev2024042503/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    32507 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.383355 keras_nightly-3.3.2.dev2024042503/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    64046 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   195656 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.387355 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.387355 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.387355 keras_nightly-3.3.2.dev2024042503/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.387355 keras_nightly-3.3.2.dev2024042503/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.387355 keras_nightly-3.3.2.dev2024042503/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.387355 keras_nightly-3.3.2.dev2024042503/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/saving/keras_saveable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.391355 keras_nightly-3.3.2.dev2024042503/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.391355 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25940 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.391355 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.391355 keras_nightly-3.3.2.dev2024042503/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/tree/tree_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.399355 keras_nightly-3.3.2.dev2024042503/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-04-25 03:20:10.000000 keras_nightly-3.3.2.dev2024042503/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:25.399355 keras_nightly-3.3.2.dev2024042503/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-25 03:21:25.000000 keras_nightly-3.3.2.dev2024042503/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-04-25 03:21:25.000000 keras_nightly-3.3.2.dev2024042503/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:21:25.000000 keras_nightly-3.3.2.dev2024042503/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 03:21:25.000000 keras_nightly-3.3.2.dev2024042503/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 03:21:25.000000 keras_nightly-3.3.2.dev2024042503/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:21:25.399355 keras_nightly-3.3.2.dev2024042503/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-25 03:21:23.000000 keras_nightly-3.3.2.dev2024042503/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.813469 keras_nightly-3.3.3.dev2024042703/
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-27 03:20:46.813469 keras_nightly-3.3.3.dev2024042703/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.725469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.729469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.733469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-27 03:20:42.000000 keras_nightly-3.3.3.dev2024042703/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.737469 keras_nightly-3.3.3.dev2024042703/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.741469 keras_nightly-3.3.3.dev2024042703/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.745469 keras_nightly-3.3.3.dev2024042703/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.749469 keras_nightly-3.3.3.dev2024042703/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.749469 keras_nightly-3.3.3.dev2024042703/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.749469 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.753469 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30920 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.753469 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30646 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28155 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.757469 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77857 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.761469 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27095 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47523 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.761469 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.765469 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.765469 keras_nightly-3.3.3.dev2024042703/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.765469 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.765469 keras_nightly-3.3.3.dev2024042703/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.765469 keras_nightly-3.3.3.dev2024042703/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.769469 keras_nightly-3.3.3.dev2024042703/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.769469 keras_nightly-3.3.3.dev2024042703/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.769469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.769469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.769469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.773469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.773469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25225 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42009 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63910 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.777469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.777469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.781469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.785469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.785469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.785469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.789469 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.789469 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.789469 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.793469 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.793469 keras_nightly-3.3.3.dev2024042703/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69104 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.793469 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.793469 keras_nightly-3.3.3.dev2024042703/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32507 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.797469 keras_nightly-3.3.3.dev2024042703/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37275 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67520 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195656 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.801469 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.801469 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.801469 keras_nightly-3.3.3.dev2024042703/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.801469 keras_nightly-3.3.3.dev2024042703/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.801469 keras_nightly-3.3.3.dev2024042703/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.801469 keras_nightly-3.3.3.dev2024042703/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/saving/keras_saveable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.801469 keras_nightly-3.3.3.dev2024042703/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.805469 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.805469 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.805469 keras_nightly-3.3.3.dev2024042703/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/tree/tree_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.809469 keras_nightly-3.3.3.dev2024042703/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-04-27 03:19:29.000000 keras_nightly-3.3.3.dev2024042703/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-27 03:20:44.000000 keras_nightly-3.3.3.dev2024042703/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:20:46.813469 keras_nightly-3.3.3.dev2024042703/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-27 03:20:46.000000 keras_nightly-3.3.3.dev2024042703/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-04-27 03:20:46.000000 keras_nightly-3.3.3.dev2024042703/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:20:46.000000 keras_nightly-3.3.3.dev2024042703/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 03:20:46.000000 keras_nightly-3.3.3.dev2024042703/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 03:20:46.000000 keras_nightly-3.3.3.dev2024042703/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 03:20:46.813469 keras_nightly-3.3.3.dev2024042703/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-27 03:20:44.000000 keras_nightly-3.3.3.dev2024042703/setup.py
```

### Comparing `keras_nightly-3.3.2.dev2024042503/PKG-INFO` & `keras_nightly-3.3.3.dev2024042703/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.2.dev2024042503
+Version: 3.3.3.dev2024042703
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.2.dev2024042503/README.md` & `keras_nightly-3.3.3.dev2024042703/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from keras.src.ops.nn import log_sigmoid
 from keras.src.ops.nn import log_softmax
 from keras.src.ops.nn import max_pool
 from keras.src.ops.nn import moments
 from keras.src.ops.nn import multi_hot
 from keras.src.ops.nn import normalize
 from keras.src.ops.nn import one_hot
+from keras.src.ops.nn import psnr
 from keras.src.ops.nn import relu
 from keras.src.ops.nn import relu6
 from keras.src.ops.nn import selu
 from keras.src.ops.nn import separable_conv
 from keras.src.ops.nn import sigmoid
 from keras.src.ops.nn import silu
 from keras.src.ops.nn import silu as swish
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from keras.src.ops.nn import log_sigmoid
 from keras.src.ops.nn import log_softmax
 from keras.src.ops.nn import max_pool
 from keras.src.ops.nn import moments
 from keras.src.ops.nn import multi_hot
 from keras.src.ops.nn import normalize
 from keras.src.ops.nn import one_hot
+from keras.src.ops.nn import psnr
 from keras.src.ops.nn import relu
 from keras.src.ops.nn import relu6
 from keras.src.ops.nn import selu
 from keras.src.ops.nn import separable_conv
 from keras.src.ops.nn import sigmoid
 from keras.src.ops.nn import silu
 from keras.src.ops.nn import silu as swish
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/activations/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/applications/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/backend/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/config/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/layers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/losses/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/ops/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from keras.src.ops.nn import log_sigmoid
 from keras.src.ops.nn import log_softmax
 from keras.src.ops.nn import max_pool
 from keras.src.ops.nn import moments
 from keras.src.ops.nn import multi_hot
 from keras.src.ops.nn import normalize
 from keras.src.ops.nn import one_hot
+from keras.src.ops.nn import psnr
 from keras.src.ops.nn import relu
 from keras.src.ops.nn import relu6
 from keras.src.ops.nn import selu
 from keras.src.ops.nn import separable_conv
 from keras.src.ops.nn import sigmoid
 from keras.src.ops.nn import silu
 from keras.src.ops.nn import silu as swish
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/ops/nn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from keras.src.ops.nn import log_sigmoid
 from keras.src.ops.nn import log_softmax
 from keras.src.ops.nn import max_pool
 from keras.src.ops.nn import moments
 from keras.src.ops.nn import multi_hot
 from keras.src.ops.nn import normalize
 from keras.src.ops.nn import one_hot
+from keras.src.ops.nn import psnr
 from keras.src.ops.nn import relu
 from keras.src.ops.nn import relu6
 from keras.src.ops.nn import selu
 from keras.src.ops.nn import separable_conv
 from keras.src.ops.nn import sigmoid
 from keras.src.ops.nn import silu
 from keras.src.ops.nn import silu as swish
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/random/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/saving/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/tree/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/api/utils/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/activations/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/activations/activations.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/api_export.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/convnext.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/densenet.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/nasnet.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/resnet.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/vgg16.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/vgg19.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/applications/xception.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/common/variables.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/config.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/exports.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/core.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/image.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/linalg.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,26 @@
 from keras.src.backend.common import dtypes
 from keras.src.backend.jax.core import cast
 from keras.src.backend.jax.core import convert_to_tensor
 
 
 def cholesky(a):
     out = jnp.linalg.cholesky(a)
-    if jnp.any(jnp.isnan(out)):
-        raise ValueError(
-            "Cholesky decomposition failed. "
-            "The input might not be a valid positive definite matrix."
-        )
+    try:
+        # In eager mode, raise for nan to
+        # achieve behavior consistency with numpy
+        if jnp.any(jnp.isnan(out)):
+            raise ValueError(
+                "Cholesky decomposition failed. "
+                "The input might not be a valid "
+                "positive definite matrix."
+            )
+    except jax.errors.TracerBoolConversionError:
+        # Cannot raise for nan in tracing mode
+        pass
     return out
 
 
 def det(a):
     return jnp.linalg.det(a)
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/math.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+import builtins
+import math
+
 import jax
 import jax.experimental.sparse as jax_sparse
 import jax.numpy as jnp
-import numpy as np
 from jax import lax
 from jax import nn as jnn
 
-from keras.src.backend import standardize_data_format
-from keras.src.backend import standardize_dtype
+from keras.src import backend
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_padding_args_for_jax,
 )
-from keras.src.backend.config import epsilon
 from keras.src.backend.jax.core import cast
 from keras.src.backend.jax.core import convert_to_tensor
 
 
 def relu(x):
     x = convert_to_tensor(x)
     return jnn.relu(x)
@@ -153,15 +153,15 @@
 def max_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     pool_size = _convert_to_spatial_operand(
         pool_size, num_spatial_dims, data_format
     )
     strides = pool_size if strides is None else strides
     strides = _convert_to_spatial_operand(
         strides, num_spatial_dims, data_format
@@ -172,28 +172,28 @@
 def average_pool(
     inputs,
     pool_size,
     strides,
     padding,
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     pool_size = _convert_to_spatial_operand(
         pool_size, num_spatial_dims, data_format
     )
     strides = pool_size if strides is None else strides
     strides = _convert_to_spatial_operand(
         strides, num_spatial_dims, data_format
     )
 
     pooled = _pool(inputs, 0.0, lax.add, pool_size, strides, padding)
     if padding == "valid":
         # Avoid the extra reduce_window.
-        return pooled / np.prod(pool_size)
+        return pooled / math.prod(pool_size)
     else:
         # Count the number of valid entries at each input point, then use that
         # for computing average. Assumes that any two arrays of same shape will
         # be padded the same. Avoid broadcasting on axis where pooling is
         # skipped.
         shape = [
             (a if b != 1 else 1) for (a, b) in zip(inputs.shape, pool_size)
@@ -238,15 +238,15 @@
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     dimension_numbers = _convert_to_lax_conv_dimension_numbers(
         num_spatial_dims,
         data_format,
         transpose=False,
     )
     strides = _convert_to_spatial_operand(
@@ -288,15 +288,15 @@
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     dimension_numbers = _convert_to_lax_conv_dimension_numbers(
         num_spatial_dims,
         data_format,
         transpose=False,
     )
     strides = _convert_to_spatial_operand(
@@ -334,15 +334,15 @@
     depthwise_kernel,
     pointwise_kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     depthwise_conv_output = depthwise_conv(
         inputs,
         depthwise_kernel,
         strides,
         padding,
         data_format,
         dilation_rate,
@@ -362,15 +362,15 @@
     kernel,
     strides=1,
     padding="valid",
     output_padding=None,
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     padding_values = compute_conv_transpose_padding_args_for_jax(
         input_shape=inputs.shape,
         kernel_shape=kernel.shape,
         strides=strides,
         padding=padding,
         output_padding=output_padding,
@@ -473,15 +473,15 @@
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
         log_prob = jax.nn.log_softmax(output, axis=axis)
     else:
         output = output / jnp.sum(output, axis, keepdims=True)
-        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+        output = jnp.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         log_prob = jnp.log(output)
     return -jnp.sum(target * log_prob, axis=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
     target = jnp.array(target, dtype="int32")
     output = jnp.array(output)
@@ -500,15 +500,15 @@
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
         log_prob = jax.nn.log_softmax(output, axis=axis)
     else:
         output = output / jnp.sum(output, axis, keepdims=True)
-        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+        output = jnp.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         log_prob = jnp.log(output)
     target = jnn.one_hot(target, output.shape[axis], axis=axis)
     return -jnp.sum(target * log_prob, axis=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
     target = jnp.array(target)
@@ -522,30 +522,30 @@
         )
 
     if from_logits:
         log_logits = jax.nn.log_sigmoid(output)
         log_neg_logits = jax.nn.log_sigmoid(-output)
         return -1.0 * target * log_logits - (1.0 - target) * log_neg_logits
 
-    output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+    output = jnp.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
     bce = target * jnp.log(output)
     bce += (1.0 - target) * jnp.log(1.0 - output)
     return -bce
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
             "Argument synchronized=True is not supported with JAX."
         )
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
-    ori_dtype = standardize_dtype(x.dtype)
+    ori_dtype = backend.standardize_dtype(x.dtype)
     if ori_dtype in ("float16", "bfloat16"):
         need_cast = True
         x = cast(x, "float32")
 
     mean = jnp.mean(x, axes, keepdims=True)
     variance = jnp.var(x, axis=axes, keepdims=True)
 
@@ -582,137 +582,167 @@
     if offset is not None:
         offset = jnp.reshape(offset, shape)
         res = res + offset
 
     return jnp.add(x * inv, res)
 
 
-def ctc_loss(
-    target,
-    output,
-    target_length,
-    output_length,
-    mask_index=0,
-):
-    batch_size, _, _ = output.shape
-    batch_size, max_target_length = target.shape
+def ctc_loss(target, output, target_length, output_length, mask_index=0):
+    # Ref: https://github.com/google-deepmind/optax
+    # optax.ctc_loss_with_forward_probs
+    target = convert_to_tensor(target, dtype="int32")
+    output = convert_to_tensor(output)
+    target_length = convert_to_tensor(target_length, "int32")
+    output_length = convert_to_tensor(output_length, "int32")
+    batch_size, _, num_classes = output.shape
+    batch_size, max_label_length = target.shape
+    log_epsilon = -1e5
 
-    output = output.transpose((1, 0, 2))
-    target = target.transpose((1, 0)).astype("int32")
+    # Ensure that the dtype promotion behavior matchs that of `tf.nn.ctc_loss`
+    dtype = backend.result_type(output.dtype, "float32")
+    output = cast(output, dtype)
 
-    logits = jnn.log_softmax(output)
-    mgrid_t, mgrid_b = jnp.meshgrid(
-        jnp.arange(max_target_length), jnp.arange(batch_size)
-    )
-    logprobs_emit = logits[mgrid_t, mgrid_b, target[:, :, None]]
-    logprobs_mask = logits[:, :, mask_index]
+    def _lengths_to_paddings(lengths, max_length):
+        indices = jnp.arange(max_length).reshape(
+            (1,) * lengths.ndim + (max_length,)
+        )
+        lengths = jnp.expand_dims(lengths, axis=-1)
+        elem_valid = indices < lengths
+        return jnp.logical_not(elem_valid)
+
+    target_paddings = _lengths_to_paddings(target_length, max_label_length)
+    output_paddings = _lengths_to_paddings(output_length, max_label_length)
+    target_paddings = target_paddings.astype(output.dtype)
+    output_paddings = output_paddings.astype(output.dtype)
 
-    logit_paddings = jnp.array(
-        jnp.arange(max_target_length) < output_length[:, None],
-        dtype=jnp.float32,
+    logprobs = jnn.log_softmax(output)
+    label_lengths = max_label_length - jnp.sum(target_paddings, axis=1).astype(
+        jnp.int32
     )
 
-    repeat = jnp.array(target[1:] == target[:-1])
-    repeat = jnp.pad(repeat, ((0, 1), (0, 0))).transpose((1, 0))
+    # repeat[b, n] == 1.0 when label[b, n] == label[b, n+1].
+    repeat = (target[:, :-1] == target[:, 1:]).astype(jnp.float32)
+    repeat = jnp.pad(repeat, ((0, 0), (0, 1)))
 
-    _logepsilon = -100000.0
+    logprobs_phi = logprobs[:, :, mask_index : mask_index + 1]  # [B, T, 1]
+    logprobs_phi = jnp.transpose(logprobs_phi, (1, 0, 2))  # [T, B, 1]
 
-    def _iterate(prev, x):
-        prev_mask, prev_emit = prev
-        logprob_mask, logprob_emit, pad = x
+    _one_hot = jax.nn.one_hot(target, num_classes=num_classes)  # [B, N, K]
+    logprobs_emit = jnp.einsum("btk,bnk->btn", logprobs, _one_hot)
+    logprobs_emit = jnp.transpose(logprobs_emit, (1, 0, 2))  # [T, B, N]
 
-        prev_mask_orig = prev_mask
-        prev_mask = prev_mask.at[:, 1:].set(
-            jnp.logaddexp(prev_mask[:, 1:], prev_emit + _logepsilon * repeat),
-        )
-        emit = jnp.logaddexp(
-            prev_mask[:, :-1] + logprob_emit, prev_emit + logprob_emit
-        )
+    # [B, N]
+    logalpha_phi_init = (
+        jnp.ones((batch_size, max_label_length + 1), dtype=output.dtype)
+        * log_epsilon
+    )
+    logalpha_phi_init = logalpha_phi_init.at[:, 0].set(0.0)
+    logalpha_emit_init = (
+        jnp.ones((batch_size, max_label_length), dtype=output.dtype)
+        * log_epsilon
+    )
 
-        mask = prev_mask + logprob_mask[:, None]
-        mask = mask.at[:, 1:].set(
-            jnp.logaddexp(
-                mask[:, 1:],
-                prev_emit + logprob_mask[:, None] + _logepsilon * (1 - repeat),
-            )
+    def update_phi_score(phi, added_score):
+        # Update `phi[:, 1:]`` with adding `added_score` in log space.
+        return jnp.concatenate(
+            [phi[:, :1], jnp.logaddexp(phi[:, 1:], added_score)], axis=-1
         )
 
-        pad = pad[:, None]
-        emit = emit * pad + prev_emit * (1 - pad)
-        mask = mask * pad + prev_mask_orig * (1 - pad)
+    def loop_body(prev, x):
+        prev_phi, prev_emit = prev
+        # emit-to-phi epsilon transition, except if the next label is repetition
+        prev_phi_orig = prev_phi
+        prev_phi = update_phi_score(prev_phi, prev_emit + log_epsilon * repeat)
 
-        return (mask, emit), (mask, emit)
+        logprob_emit, logprob_phi, pad = x
 
-    mask_init = jnp.full((batch_size, max_target_length + 1), _logepsilon)
-    mask_init = mask_init.at[:, 0].set(0.0)
-    emit_init = jnp.full((batch_size, max_target_length), _logepsilon)
+        # phi-to-emit transition
+        next_emit = jnp.logaddexp(
+            prev_phi[:, :-1] + logprob_emit, prev_emit + logprob_emit
+        )
+        # self-loop transition
+        next_phi = prev_phi + logprob_phi
+        # emit-to-phi blank transition only when the next label is repetition
+        next_phi = update_phi_score(
+            next_phi, prev_emit + logprob_phi + log_epsilon * (1.0 - repeat)
+        )
 
-    _, (alphas_mask, alphas_emit) = lax.scan(
-        _iterate,
-        (mask_init, emit_init),
-        (logprobs_mask, logprobs_emit, logit_paddings.transpose()),
-    )
+        pad = pad.reshape((batch_size, 1))
+        next_emit = pad * prev_emit + (1.0 - pad) * next_emit
+        next_phi = pad * prev_phi_orig + (1.0 - pad) * next_phi
+
+        return (next_phi, next_emit), (next_phi, next_emit)
 
-    last_alpha_mask = (
-        alphas_mask[-1]
-        .at[:, 1:]
-        .set(jnp.logaddexp(alphas_mask[-1, :, 1:], alphas_emit[-1]))
+    xs = (logprobs_emit, logprobs_phi, output_paddings.transpose((1, 0)))
+    _, (logalpha_phi, logalpha_emit) = jax.lax.scan(
+        loop_body, (logalpha_phi_init, logalpha_emit_init), xs
     )
 
-    return -last_alpha_mask[jnp.arange(batch_size), target_length]
+    # last row needs to be updated with the last epsilon transition
+    logalpha_phi_last = update_phi_score(logalpha_phi[-1], logalpha_emit[-1])
+    logalpha_phi = logalpha_phi.at[-1].set(logalpha_phi_last)
 
+    # extract per_seq_loss
+    # [B, N+1]
+    _one_hot = jax.nn.one_hot(label_lengths, num_classes=max_label_length + 1)
+    per_seq_loss = -jnp.einsum("bn,bn->b", logalpha_phi_last, _one_hot)
+    return per_seq_loss
 
-def ctc_greedy_decode(
+
+def _ctc_greedy_decode(
     inputs,
     sequence_length,
     merge_repeated=True,
     mask_index=None,
 ):
-    inputs = jnp.array(inputs)
-    sequence_length = jnp.array(sequence_length, dtype=jnp.int32)
+    inputs = convert_to_tensor(inputs)
+    sequence_length = convert_to_tensor(sequence_length, dtype="int32")
+    batch_size, max_length, num_classes = inputs.shape
 
     if mask_index is None:
-        mask_index = inputs.shape[-1] - 1
+        mask_index = num_classes - 1
 
     indices = jnp.argmax(inputs, axis=-1)
     scores = jnp.max(inputs, axis=-1)
 
-    seqlen_mask = jnp.arange(inputs.shape[1])[None, :]
+    seqlen_mask = jnp.arange(max_length)[None, :]
     seqlen_mask = seqlen_mask >= sequence_length[:, None]
 
-    if merge_repeated:
-        repeat = indices[:, 1:] == indices[:, :-1]
-        repeat = jnp.pad(repeat, ((0, 0), (1, 0)))
-
-        indices = jnp.where(repeat, mask_index, indices)
-    else:
-        repeat = jnp.zeros_like(indices, dtype=bool)
-
     indices = jnp.where(seqlen_mask, mask_index, indices)
-    indices = [batch[batch != mask_index] for batch in indices]
-    max_len = max(len(batch) for batch in indices)
-    indices = jnp.array(
-        [jnp.pad(batch, (0, max_len - len(batch))) for batch in indices]
-    )
-
     scores = jnp.where(seqlen_mask, 0.0, scores)
-    scores = -jnp.sum(scores, axis=1)[:, None]
 
-    return [indices], scores
+    if merge_repeated:
+        repeat_mask = indices[:, 1:] == indices[:, :-1]
+        repeat_mask = jnp.pad(repeat_mask, ((0, 0), (1, 0)))
+        indices = jnp.where(repeat_mask, mask_index, indices)
+
+    # We rearrange the indices by moving `mask_index` to the end of the array
+    invalid_mask = indices == mask_index
+    order = jnp.expand_dims(jnp.arange(max_length), axis=0)  # [1, N]
+    order = jnp.tile(order, (batch_size, 1))  # [B, N]
+    order = jnp.where(invalid_mask, max_length, order)
+    order = jnp.argsort(order, axis=-1)
+    indices = jnp.take_along_axis(indices, order, axis=-1)
+
+    # We set to -1 for blank labels
+    indices = jnp.where(invalid_mask, -1, indices)
+    scores = -jnp.sum(scores, axis=1)[:, None]
+    indices = jnp.expand_dims(indices, axis=0)
+    return indices, scores
 
 
-def ctc_beam_search_decode(
+def _ctc_beam_search_decode(
     inputs,
     sequence_length,
     beam_width=100,
     top_paths=1,
     mask_index=None,
 ):
-    inputs = jnp.array(inputs)
-    sequence_length = jnp.array(sequence_length)
+    inputs = convert_to_tensor(inputs)
+    sequence_length = convert_to_tensor(sequence_length)
 
     batch_size, max_seq_len, num_classes = inputs.shape
     inputs = jnn.log_softmax(inputs)
     seqlen_mask = jnp.arange(max_seq_len)[None, :] >= sequence_length[:, None]
 
     if mask_index is None:
         mask_index = num_classes - 1
@@ -726,21 +756,21 @@
 
     _pad = -1
 
     init_paths = jnp.full(
         (batch_size, 2 * beam_width, max_seq_len), _pad, dtype=jnp.int32
     )
 
-    num_init_paths = jnp.min(jnp.array([num_classes, beam_width]))
+    num_init_paths = builtins.min(num_classes, beam_width)
     max_classes = jnp.argsort(inputs[:, 0], axis=1)[:, -num_init_paths:]
     init_classes = jnp.where(max_classes == mask_index, _pad, max_classes)
     init_paths = init_paths.at[:, :num_init_paths, 0].set(init_classes)
 
     init_scores = (
-        jnp.full((batch_size, 2 * beam_width), -jnp.inf)
+        jnp.full((batch_size, 2 * beam_width), -jnp.inf, dtype=inputs.dtype)
         .at[:, :num_init_paths]
         .set(jnp.take_along_axis(inputs[:, 0], max_classes, axis=1))
     )
     init_masked = init_paths[:, :, 0] == _pad
 
     def _extend_paths(paths, scores, masked, x):
         paths = jnp.repeat(paths, num_classes, axis=0)
@@ -855,42 +885,57 @@
 
     paths, scores = jax.vmap(_decode_batch)(
         init_paths, init_scores, init_masked, inputs, seqlen_mask
     )
 
     # convert classes back to the correct indices
     paths = jnp.where(paths == _pad, _pad, num_classes - paths - 1)
-
-    lengths = jnp.argmax(paths == _pad, axis=2)
-    lengths = jnp.max(lengths, axis=0)
-    paths = jnp.where(paths == _pad, 0, paths)
-
-    paths = paths.transpose((1, 0, 2))
-    paths = [path[:, :length] for path, length in zip(paths, lengths)]
-
+    paths = jnp.transpose(paths, [1, 0, 2])
     return paths, scores
 
 
 def ctc_decode(
     inputs,
     sequence_length,
-    strategy,
+    strategy="greedy",
     beam_width=100,
     top_paths=1,
     merge_repeated=True,
     mask_index=None,
 ):
+    inputs = convert_to_tensor(inputs)
+    dtype = backend.result_type(inputs.dtype, "float32")
+    inputs = cast(inputs, dtype)
+
     if strategy == "greedy":
-        return ctc_greedy_decode(
+        return _ctc_greedy_decode(
             inputs,
             sequence_length,
             merge_repeated=merge_repeated,
             mask_index=mask_index,
         )
-    else:
-        return ctc_beam_search_decode(
+    elif strategy == "beam_search":
+        return _ctc_beam_search_decode(
             inputs,
             sequence_length,
             beam_width=beam_width,
             top_paths=top_paths,
             mask_index=mask_index,
         )
+    else:
+        raise ValueError(
+            f"Invalid strategy {strategy}. Supported values are "
+            "'greedy' and 'beam_search'."
+        )
+
+
+def psnr(x1, x2, max_val):
+    if x1.shape != x2.shape:
+        raise ValueError(
+            f"Input shapes {x1.shape} and {x2.shape} must "
+            "match for PSNR calculation. "
+        )
+
+    max_val = convert_to_tensor(max_val, dtype=x2.dtype)
+    mse = jnp.mean(jnp.square(x1 - x2))
+    psnr = 20 * jnp.log10(max_val) - 10 * jnp.log10(mse)
+    return psnr
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/random.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/linalg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,631 +1,638 @@
-import jax
-import numpy as np
-from jax import lax
-from jax import numpy as jnp
-
-from keras.src.backend import standardize_data_format
-from keras.src.backend import standardize_dtype
-from keras.src.backend.common.backend_utils import (
-    compute_conv_transpose_padding_args_for_jax,
-)
-from keras.src.backend.config import epsilon
-from keras.src.backend.numpy.core import cast
-from keras.src.backend.numpy.core import convert_to_tensor
-from keras.src.backend.numpy.core import is_tensor
-from keras.src.utils.module_utils import scipy
+from keras.src import backend
+from keras.src.api_export import keras_export
+from keras.src.backend import KerasTensor
+from keras.src.backend import any_symbolic_tensors
+from keras.src.ops.operation import Operation
+from keras.src.ops.operation_utils import reduce_shape
+
+
+class Cholesky(Operation):
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return _cholesky(x)
+
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        _assert_square(x)
+        return KerasTensor(x.shape, x.dtype)
+
+
+@keras_export(["keras.ops.cholesky", "keras.ops.linalg.cholesky"])
+def cholesky(x):
+    """Computes the Cholesky decomposition of a positive semi-definite matrix.
 
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
 
-def relu(x):
-    x = convert_to_tensor(x)
-    return np.maximum(x, np.array(0.0, x.dtype))
+    Returns:
+        A tensor of shape `(..., M, M)` representing the lower triangular
+        Cholesky factor of `x`.
 
+    """
+    if any_symbolic_tensors((x,)):
+        return Cholesky().symbolic_call(x)
+    return _cholesky(x)
 
-def relu6(x):
-    x = convert_to_tensor(x)
-    # np.clip incorrectly promote bfloat16 to float32, so we replace it with
-    # np.minimum and np.maximum here
-    return np.minimum(
-        np.maximum(x, np.array(0.0, x.dtype)), np.array(6.0, x.dtype)
-    )
 
+def _cholesky(x):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    _assert_square(x)
+    try:
+        return backend.linalg.cholesky(x)
+    except Exception as e:
+        raise ValueError(f"Cholesky decomposition failed: {e}")
 
-def sigmoid(x):
-    x = convert_to_tensor(x)
-    return np.array(1.0, x.dtype) / (np.array(1.0, x.dtype) + np.exp(-x))
 
+class Det(Operation):
 
-def tanh(x):
-    return np.tanh(x)
+    def __init__(self):
+        super().__init__()
 
+    def call(self, x):
+        return _det(x)
 
-def softplus(x):
-    x = convert_to_tensor(x)
-    return np.logaddexp(x, np.array(0.0, x.dtype))
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        _assert_square(x)
+        return KerasTensor(x.shape[:-2], x.dtype)
 
 
-def softsign(x):
-    x = convert_to_tensor(x)
-    return x / (np.array(1.0, x.dtype) + np.abs(x))
+@keras_export(["keras.ops.det", "keras.ops.linalg.det"])
+def det(x):
+    """Computes the determinant of a square tensor.
 
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
 
-def silu(x):
-    x = convert_to_tensor(x)
-    return x * sigmoid(x)
+    Returns:
+        A tensor of shape `(...,)` represeting the determinant of `x`.
 
+    """
+    if any_symbolic_tensors((x,)):
+        return Det().symbolic_call(x)
+    return _det(x)
 
-def log_sigmoid(x):
-    x = convert_to_tensor(x)
-    return -softplus(-x)
 
+def _det(x):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    _assert_square(x)
+    return backend.linalg.det(x)
 
-def leaky_relu(x, negative_slope=0.2):
-    x = convert_to_tensor(x)
-    return np.maximum(x, np.array(negative_slope, x.dtype) * x)
 
+class Eig(Operation):
 
-def hard_sigmoid(x):
-    # python numbers will be promoted to float64 by np, so it's necessary to
-    # first convert the python numbers to np scalars
-    x = x / np.array(6.0, x.dtype) + np.array(0.5, x.dtype)
-    return np.where(
-        x <= 0.0,
-        np.array(0.0, x.dtype),
-        np.where(x >= 1.0, np.array(1.0, x.dtype), x),
-    )
+    def __init__(self):
+        super().__init__()
 
+    def call(self, x):
+        return _eig(x)
 
-def hard_silu(x):
-    return x * hard_sigmoid(x)
+    def compute_output_spec(self, x):
+        _assert_square(x)
+        _assert_2d(x)
+        return (
+            KerasTensor(x.shape[:-1], x.dtype),
+            KerasTensor(x.shape, x.dtype),
+        )
 
 
-def elu(x, alpha=1.0):
-    x = convert_to_tensor(x)
-    return np.where(
-        x >= np.array(0.0, x.dtype), x, np.array(alpha, x.dtype) * np.expm1(x)
-    )
+@keras_export(["keras.ops.eig", "keras.ops.linalg.eig"])
+def eig(x):
+    """Computes the eigenvalues and eigenvectors of a square matrix.
 
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
 
-def selu(
-    x,
-    alpha=1.6732632423543772848170429916717,
-    scale=1.0507009873554804934193349852946,
-):
-    x = convert_to_tensor(x)
-    return np.array(scale, x.dtype) * elu(x, alpha)
+    Returns:
+        A tuple of two tensors: a tensor of shape `(..., M)` containing
+        eigenvalues and a tensor of shape `(..., M, M)` containing eigenvectors.
+    """
+    if any_symbolic_tensors((x,)):
+        return Eig().symbolic_call(x)
+    return _eig(x)
 
 
-def gelu(x, approximate=True):
-    x = convert_to_tensor(x)
-    # followed by JAX's implementation
-    if approximate:
-        sqrt_2_over_pi = np.sqrt(2 / np.pi).astype(x.dtype)
-        cdf = np.array(0.5, x.dtype) * (
-            np.array(1.0, x.dtype)
-            + np.tanh(
-                sqrt_2_over_pi
-                * (x + np.array(0.044715, x.dtype) * (x**3).astype(x.dtype))
-            )
-        )
-        return x * cdf
-    else:
-        sqrt_2 = np.sqrt(2).astype(x.dtype)
+def _eig(x):
+    x = backend.convert_to_tensor(x)
+    _assert_square(x)
+    _assert_2d(x)
+    return backend.linalg.eig(x)
+
+
+class Eigh(Operation):
+
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return _eigh(x)
+
+    def compute_output_spec(self, x):
+        _assert_square(x)
+        _assert_2d(x)
         return (
-            x
-            * (scipy.special.erf(x / sqrt_2) + 1).astype(x.dtype)
-            / np.array(2, x.dtype)
+            KerasTensor(x.shape[:-1], x.dtype),
+            KerasTensor(x.shape, x.dtype),
         )
 
 
-def softmax(x, axis=None):
-    exp_x = np.exp(x - np.max(x, axis=axis, keepdims=True))
-    return exp_x / np.sum(exp_x, axis=axis, keepdims=True)
-
-
-def log_softmax(x, axis=None):
-    max_x = np.max(x, axis=axis, keepdims=True)
-    logsumexp = np.log(np.exp(x - max_x).sum(axis=axis, keepdims=True))
-    return x - max_x - logsumexp
-
-
-def _convert_to_spatial_operand(
-    x,
-    num_spatial_dims,
-    data_format="channels_last",
-    include_batch_and_channels=True,
-):
-    # Helper function that converts an operand to a spatial operand.
-    x = (x,) * num_spatial_dims if isinstance(x, int) else x
-    if not include_batch_and_channels:
-        return x
-    if data_format == "channels_last":
-        x = (1,) + x + (1,)
-    else:
-        x = (1,) + (1,) + x
-    return x
-
-
-def _pool(
-    inputs,
-    initial_value,
-    reduce_fn,
-    pool_size,
-    strides=None,
-    padding="valid",
-):
-    """Helper function to define pooling functions.
-
-    Args:
-        inputs: input data of shape `N+2`.
-        initial_value: the initial value for the reduction.
-        reduce_fn: a reduce function of the form `(T, T) -> T`.
-        pool_size: a sequence of `N` integers, representing the window size to
-            reduce over.
-        strides: a sequence of `N` integers, representing the inter-window
-            strides (default: `(1, ..., 1)`).
-        padding: either the string `same` or `valid`.
-
-    Returns:
-        The output of the reduction for each window slice.
-    """
-    if padding not in ("same", "valid"):
-        raise ValueError(
-            f"Invalid padding '{padding}', must be 'same' or 'valid'."
-        )
-    padding = padding.upper()
-    return np.array(
-        lax.reduce_window(
-            inputs,
-            initial_value,
-            reduce_fn,
-            pool_size,
-            strides,
-            padding,
-        )
-    )
+@keras_export(["keras.ops.eigh", "keras.ops.linalg.eigh"])
+def eigh(x):
+    """Computes the eigenvalues and eigenvectors of a complex Hermitian.
 
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
 
-def max_pool(
-    inputs,
-    pool_size,
-    strides=None,
-    padding="valid",
-    data_format=None,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    pool_size = _convert_to_spatial_operand(
-        pool_size, num_spatial_dims, data_format
-    )
-    strides = pool_size if strides is None else strides
-    strides = _convert_to_spatial_operand(
-        strides, num_spatial_dims, data_format
-    )
-    return _pool(inputs, -jnp.inf, lax.max, pool_size, strides, padding)
-
-
-def average_pool(
-    inputs,
-    pool_size,
-    strides,
-    padding,
-    data_format=None,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    pool_size = _convert_to_spatial_operand(
-        pool_size, num_spatial_dims, data_format
-    )
-    strides = pool_size if strides is None else strides
-    strides = _convert_to_spatial_operand(
-        strides, num_spatial_dims, data_format
-    )
-
-    pooled = _pool(inputs, 0.0, lax.add, pool_size, strides, padding)
-    if padding == "valid":
-        # Avoid the extra reduce_window.
-        return pooled / np.prod(pool_size)
-    else:
-        # Count the number of valid entries at each input point, then use that
-        # for computing average. Assumes that any two arrays of same shape will
-        # be padded the same. Avoid broadcasting on axis where pooling is
-        # skipped.
-        shape = [
-            (a if b != 1 else 1) for (a, b) in zip(inputs.shape, pool_size)
-        ]
-        window_counts = _pool(
-            jnp.ones(shape, inputs.dtype),
-            0.0,
-            lax.add,
-            pool_size,
-            strides,
-            padding,
-        )
-        return pooled / window_counts
+    Returns:
+        A tuple of two tensors: a tensor of shape `(..., M)` containing
+        eigenvalues and a tensor of shape `(..., M, M)` containing eigenvectors.
 
+    """
+    if any_symbolic_tensors((x,)):
+        return Eigh().symbolic_call(x)
+    return _eigh(x)
 
-def _convert_to_lax_conv_dimension_numbers(
-    num_spatial_dims,
-    data_format="channels_last",
-    transpose=False,
-):
-    """Create a `lax.ConvDimensionNumbers` for the given inputs."""
-    num_dims = num_spatial_dims + 2
-
-    if data_format == "channels_last":
-        spatial_dims = tuple(range(1, num_dims - 1))
-        inputs_dn = (0, num_dims - 1) + spatial_dims
-    else:
-        spatial_dims = tuple(range(2, num_dims))
-        inputs_dn = (0, 1) + spatial_dims
-
-    if transpose:
-        kernel_dn = (num_dims - 2, num_dims - 1) + tuple(range(num_dims - 2))
-    else:
-        kernel_dn = (num_dims - 1, num_dims - 2) + tuple(range(num_dims - 2))
-
-    return lax.ConvDimensionNumbers(
-        lhs_spec=inputs_dn, rhs_spec=kernel_dn, out_spec=inputs_dn
-    )
-
-
-def conv(
-    inputs,
-    kernel,
-    strides=1,
-    padding="valid",
-    data_format=None,
-    dilation_rate=1,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    if data_format == "channels_last":
-        channels = inputs.shape[-1]
-    else:
-        channels = inputs.shape[1]
-    kernel_in_channels = kernel.shape[-2]
-    if channels % kernel_in_channels > 0:
-        raise ValueError(
-            "The number of input channels must be evenly divisible by "
-            f"kernel's in_channels. Received input channels {channels} and "
-            f"kernel in_channels {kernel_in_channels}. "
-        )
-    feature_group_count = channels // kernel_in_channels
-    return np.array(
-        jax.lax.conv_general_dilated(
-            inputs,
-            kernel if is_tensor(kernel) else kernel.numpy(),
-            strides,
-            padding,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            feature_group_count=feature_group_count,
-        )
-    )
 
+def _eigh(x):
+    x = backend.convert_to_tensor(x)
+    _assert_square(x)
+    _assert_2d(x)
+    return backend.linalg.eigh(x)
 
-def depthwise_conv(
-    inputs,
-    kernel,
-    strides=1,
-    padding="valid",
-    data_format=None,
-    dilation_rate=1,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    feature_group_count = (
-        inputs.shape[-1] if data_format == "channels_last" else inputs.shape[1]
-    )
-    kernel = jnp.reshape(
-        kernel if is_tensor(kernel) else kernel.numpy(),
-        kernel.shape[:-2] + (1, feature_group_count * kernel.shape[-1]),
-    )
-    return np.array(
-        jax.lax.conv_general_dilated(
-            inputs,
-            kernel,
-            strides,
-            padding,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            feature_group_count=feature_group_count,
-        )
-    )
 
+class Inv(Operation):
 
-def separable_conv(
-    inputs,
-    depthwise_kernel,
-    pointwise_kernel,
-    strides=1,
-    padding="valid",
-    data_format=None,
-    dilation_rate=1,
-):
-    data_format = standardize_data_format(data_format)
-    depthwise_conv_output = depthwise_conv(
-        inputs,
-        depthwise_kernel,
-        strides,
-        padding,
-        data_format,
-        dilation_rate,
-    )
-    return conv(
-        depthwise_conv_output,
-        pointwise_kernel,
-        strides=1,
-        padding="valid",
-        data_format=data_format,
-        dilation_rate=dilation_rate,
-    )
-
-
-def conv_transpose(
-    inputs,
-    kernel,
-    strides=1,
-    padding="valid",
-    output_padding=None,
-    data_format=None,
-    dilation_rate=1,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    padding_values = compute_conv_transpose_padding_args_for_jax(
-        input_shape=inputs.shape,
-        kernel_shape=kernel.shape,
-        strides=strides,
-        padding=padding,
-        output_padding=output_padding,
-        dilation_rate=dilation_rate,
-    )
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-
-    return np.array(
-        jax.lax.conv_transpose(
-            inputs,
-            kernel if is_tensor(kernel) else kernel.numpy(),
-            strides,
-            padding=padding_values,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            transpose_kernel=True,
-        )
-    )
+    def __init__(self):
+        super().__init__()
 
+    def call(self, x):
+        return _inv(x)
+
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        _assert_square(x)
+        return KerasTensor(x.shape, x.dtype)
 
-def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    if sparse:
-        raise ValueError("Unsupported value `sparse=True` with numpy backend")
-    x = convert_to_tensor(x)
-    input_shape = x.shape
-
-    # Shrink the last dimension if the shape is (..., 1).
-    if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
-        input_shape = tuple(input_shape[:-1])
-
-    x = x.reshape(-1)
-    if not num_classes:
-        num_classes = np.max(x) + 1
-
-    batch_size = x.shape[0]
-    categorical = np.zeros((batch_size, num_classes), dtype=dtype)
-    valid_indices = x >= 0
-    categorical[np.arange(batch_size)[valid_indices], x[valid_indices]] = 1
-
-    # First, reshape the array with the extra dimension at the end
-    output_shape = input_shape + (num_classes,)
-    categorical = np.reshape(categorical, output_shape)
-
-    # Then, move this new dimension to the right place (according to axis)
-    if axis != -1:
-        categorical = np.moveaxis(categorical, -1, axis)
-
-    return categorical
-
-
-def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    if sparse:
-        raise ValueError("Unsupported value `sparse=True` with numpy backend")
-    x = convert_to_tensor(x)
-    reduction_axis = 1 if len(x.shape) > 1 else 0
-    outputs = np.max(
-        one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
-        axis=reduction_axis,
-    )
-    return outputs
-
-
-def categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = np.array(target)
-    output = np.array(output)
-
-    if target.shape != output.shape:
-        raise ValueError(
-            "Arguments `target` and `output` must have the same shape. "
-            "Received: "
-            f"target.shape={target.shape}, output.shape={output.shape}"
-        )
-    if len(target.shape) < 1:
-        raise ValueError(
-            "Arguments `target` and `output` must be at least rank 1. "
-            "Received: "
-            f"target.shape={target.shape}, output.shape={output.shape}"
-        )
 
-    if from_logits:
-        log_prob = log_softmax(output, axis=axis)
-    else:
-        output = output / np.sum(output, axis, keepdims=True)
-        output = np.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = np.log(output)
-    return -np.sum(target * log_prob, axis=axis)
-
-
-def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = np.array(target, dtype="int32")
-    output = np.array(output)
-    if len(target.shape) == len(output.shape) and target.shape[-1] == 1:
-        target = np.squeeze(target, axis=-1)
-
-    if len(output.shape) < 1:
-        raise ValueError(
-            "Argument `output` must be at least rank 1. "
-            "Received: "
-            f"output.shape={output.shape}"
+@keras_export(["keras.ops.inv", "keras.ops.linalg.inv"])
+def inv(x):
+    """Computes the inverse of a square tensor.
+
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
+
+    Returns:
+        A tensor of shape `(..., M, M)` representing the inverse of `x`.
+
+    """
+    if any_symbolic_tensors((x,)):
+        return Inv().symbolic_call(x)
+    return _inv(x)
+
+
+def _inv(x):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    _assert_square(x)
+    return backend.linalg.inv(x)
+
+
+class LuFactor(Operation):
+
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return _lu_factor(x)
+
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        batch_shape = x.shape[:-2]
+        m, n = x.shape[-2:]
+        k = min(m, n)
+        return (
+            KerasTensor(batch_shape + (m, n), x.dtype),
+            KerasTensor(batch_shape + (k,), x.dtype),
         )
-    if target.shape != output.shape[:-1]:
-        raise ValueError(
-            "Arguments `target` and `output` must have the same shape "
-            "up until the last dimension: "
-            f"target.shape={target.shape}, output.shape={output.shape}"
+
+
+@keras_export(["keras.ops.lu_factor", "keras.ops.linalg.lu_factor"])
+def lu_factor(x):
+    """Computes the lower-upper decomposition of a square matrix.
+
+    Args:
+        x: A tensor of shape `(..., M, M)`.
+
+    Returns:
+        A tuple of two tensors: a tensor of shape `(..., M, M)` containing the
+        lower and upper triangular matrices and a tensor of shape `(..., M)`
+        containing the pivots.
+
+    """
+    if any_symbolic_tensors((x,)):
+        return LuFactor().symbolic_call(x)
+    return _lu_factor(x)
+
+
+def _lu_factor(x):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    if backend.backend() == "tensorflow":
+        try:
+            _assert_square(x)
+        except ValueError as e:
+            raise ValueError(
+                f"LU decomposition failed: {e}. LU decomposition is only "
+                "supported for square matrices in Tensorflow."
+            )
+    return backend.linalg.lu_factor(x)
+
+
+class Norm(Operation):
+    def __init__(self, ord=None, axis=None, keepdims=False):
+        super().__init__()
+        if isinstance(ord, str):
+            if ord not in ("fro", "nuc"):
+                raise ValueError(
+                    "Invalid `ord` argument. "
+                    "Expected one of {'fro', 'nuc'} when using string. "
+                    f"Received: ord={ord}"
+                )
+        if isinstance(axis, int):
+            axis = [axis]
+        self.ord = ord
+        self.axis = axis
+        self.keepdims = keepdims
+
+    def compute_output_spec(self, x):
+        output_dtype = backend.standardize_dtype(x.dtype)
+        if "int" in output_dtype or output_dtype == "bool":
+            output_dtype = backend.floatx()
+        if self.axis is None:
+            axis = tuple(range(len(x.shape)))
+        else:
+            axis = self.axis
+        num_axes = len(axis)
+        if num_axes == 1 and isinstance(self.ord, str):
+            raise ValueError(
+                "Invalid `ord` argument for vector norm. "
+                f"Received: ord={self.ord}"
+            )
+        elif num_axes == 2 and self.ord not in (
+            None,
+            "fro",
+            "nuc",
+            float("inf"),
+            float("-inf"),
+            1,
+            -1,
+            2,
+            -2,
+        ):
+            raise ValueError(
+                "Invalid `ord` argument for matrix norm. "
+                f"Received: ord={self.ord}"
+            )
+        return KerasTensor(
+            reduce_shape(x.shape, axis=self.axis, keepdims=self.keepdims),
+            dtype=output_dtype,
         )
-    if from_logits:
-        log_prob = log_softmax(output, axis=axis)
-    else:
-        output = output / np.sum(output, axis, keepdims=True)
-        output = np.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = np.log(output)
-    target = one_hot(target, output.shape[axis], axis=axis)
-    return -np.sum(target * log_prob, axis=axis)
-
-
-def binary_crossentropy(target, output, from_logits=False):
-    target = np.array(target)
-    output = np.array(output)
-
-    if target.shape != output.shape:
-        raise ValueError(
-            "Arguments `target` and `output` must have the same shape. "
-            "Received: "
-            f"target.shape={target.shape}, output.shape={output.shape}"
+
+    def call(self, x):
+        x = backend.convert_to_tensor(x)
+        return backend.linalg.norm(
+            x, ord=self.ord, axis=self.axis, keepdims=self.keepdims
         )
 
-    if from_logits:
-        output = sigmoid(output)
 
-    output = np.clip(output, epsilon(), 1.0 - epsilon())
-    bce = target * np.log(output)
-    bce += (1.0 - target) * np.log(1.0 - output)
-    return -bce
+@keras_export(["keras.ops.norm", "keras.ops.linalg.norm"])
+def norm(x, ord=None, axis=None, keepdims=False):
+    """Matrix or vector norm.
 
+    This function is able to return one of eight different matrix norms, or one
+    of an infinite number of vector norms (described below), depending on the
+    value of the `ord` parameter.
 
-def moments(x, axes, keepdims=False, synchronized=False):
-    if synchronized:
-        raise NotImplementedError(
-            "Argument synchronized=True is not supported with NumPy."
-        )
-    axes = tuple(axes) if isinstance(axes, list) else axes
-    # The dynamic range of float16 is too limited for statistics. As a
-    # workaround, we simply perform the operations on float32 and convert back
-    # to float16
-    need_cast = False
-    ori_dtype = standardize_dtype(x.dtype)
-    if ori_dtype == "float16":
-        need_cast = True
-        x = cast(x, "float32")
-
-    mean = np.mean(x, axes, keepdims=True)
-
-    # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
-    # but less numerically stable.
-    variance = np.mean(np.square(x), axis=axes, keepdims=True) - np.square(mean)
-
-    if not keepdims:
-        mean = np.squeeze(mean, axes)
-        variance = np.squeeze(variance, axes)
-    if need_cast:
-        # avoid overflow and underflow when casting from float16 to float32
-        mean = np.clip(mean, np.finfo(np.float16).min, np.finfo(np.float16).max)
-        variance = np.clip(
-            variance, np.finfo(np.float16).min, np.finfo(np.float16).max
+    Args:
+        x: Input tensor.
+        ord: Order of the norm (see table under Notes). The default is `None`.
+        axis: If `axis` is an integer, it specifies the axis of `x` along which
+            to compute the vector norms. If `axis` is a 2-tuple, it specifies
+            the axes that hold 2-D matrices, and the matrix norms of these
+            matrices are computed.
+        keepdims: If this is set to `True`, the axes which are reduced are left
+            in the result as dimensions with size one.
+
+    Note:
+        For values of `ord < 1`, the result is, strictly speaking, not a
+        mathematical 'norm', but it may still be useful for various numerical
+        purposes. The following norms can be calculated:
+        - For matrices:
+            - `ord=None`: Frobenius norm
+            - `ord="fro"`: Frobenius norm
+            - `ord="nuc"`: nuclear norm
+            - `ord=np.inf`: `max(sum(abs(x), axis=1))`
+            - `ord=-np.inf`: `min(sum(abs(x), axis=1))`
+            - `ord=0`: not supported
+            - `ord=1`: `max(sum(abs(x), axis=0))`
+            - `ord=-1`: `min(sum(abs(x), axis=0))`
+            - `ord=2`: 2-norm (largest sing. value)
+            - `ord=-2`: smallest singular value
+            - other: not supported
+        - For vectors:
+            - `ord=None`: 2-norm
+            - `ord="fro"`: not supported
+            - `ord="nuc"`: not supported
+            - `ord=np.inf`: `max(abs(x))`
+            - `ord=-np.inf`: `min(abs(x))`
+            - `ord=0`: `sum(x != 0)`
+            - `ord=1`: as below
+            - `ord=-1`: as below
+            - `ord=2`: as below
+            - `ord=-2`: as below
+            - other: `sum(abs(x)**ord)**(1./ord)`
+
+    Returns:
+        Norm of the matrix or vector(s).
+
+    Example:
+
+    >>> x = keras.ops.reshape(keras.ops.arange(9, dtype="float32") - 4, (3, 3))
+    >>> keras.ops.linalg.norm(x)
+    7.7459664
+    """
+    if any_symbolic_tensors((x,)):
+        return Norm(ord=ord, axis=axis, keepdims=keepdims).symbolic_call(x)
+    x = backend.convert_to_tensor(x)
+    return backend.linalg.norm(x, ord=ord, axis=axis, keepdims=keepdims)
+
+
+class Qr(Operation):
+    def __init__(self, mode="reduced"):
+        super().__init__()
+        if mode not in {"reduced", "complete"}:
+            raise ValueError(
+                "`mode` argument value not supported. "
+                "Expected one of {'reduced', 'complete'}. "
+                f"Received: mode={mode}"
+            )
+        self.mode = mode
+
+    def compute_output_spec(self, x):
+        if len(x.shape) < 2:
+            raise ValueError(
+                "Input should have rank >= 2. Received: "
+                f"input.shape = {x.shape}"
+            )
+        m = x.shape[-2]
+        n = x.shape[-1]
+        if m is None or n is None:
+            raise ValueError(
+                "Input should have its last 2 dimensions "
+                "fully-defined. Received: "
+                f"input.shape = {x.shape}"
+            )
+        k = min(m, n)
+        base = tuple(x.shape[:-2])
+        if self.mode == "reduced":
+            return (
+                KerasTensor(shape=base + (m, k), dtype=x.dtype),
+                KerasTensor(shape=base + (k, n), dtype=x.dtype),
+            )
+        # 'complete' mode.
+        return (
+            KerasTensor(shape=base + (m, m), dtype=x.dtype),
+            KerasTensor(shape=base + (m, n), dtype=x.dtype),
         )
-        mean = cast(mean, ori_dtype)
-        variance = cast(variance, ori_dtype)
-    return mean, variance
-
-
-def batch_normalization(
-    x, mean, variance, axis, offset=None, scale=None, epsilon=1e-3
-):
-    shape = [1] * len(x.shape)
-    shape[axis] = mean.shape[0]
-    mean = np.reshape(mean, shape)
-    variance = np.reshape(variance, shape)
-
-    inv = 1.0 / np.sqrt(variance + epsilon)
-    if scale is not None:
-        scale = np.reshape(scale, shape)
-        inv = inv * scale
-
-    res = -mean * inv
-    if offset is not None:
-        offset = np.reshape(offset, shape)
-        res = res + offset
-
-    return x * inv + res
-
-
-def ctc_decode(
-    inputs,
-    sequence_length,
-    strategy,
-    beam_width=100,
-    top_paths=1,
-    merge_repeated=True,
-    mask_index=None,
-):
-    raise NotImplementedError(
-        "NumPy backend does not yet support CTC decoding."
-    )
+
+    def call(self, x):
+        x = backend.convert_to_tensor(x)
+        return backend.linalg.qr(x, mode=self.mode)
+
+
+@keras_export(["keras.ops.qr", "keras.ops.linalg.qr"])
+def qr(x, mode="reduced"):
+    """Computes the QR decomposition of a tensor.
+
+    Args:
+        x: Input tensor of shape `(..., M, N)`.
+        mode: A string specifying the mode of the QR decomposition.
+            - 'reduced': Returns the reduced QR decomposition. (default)
+            - 'complete': Returns the complete QR decomposition.
+
+    Returns:
+        A tuple containing two tensors. The first tensor of shape `(..., M, K)`
+        is the orthogonal matrix `q` and the second tensor of shape
+        `(..., K, N)` is the upper triangular matrix `r`, where `K = min(M, N)`.
+
+    Example:
+
+    >>> x = keras.ops.convert_to_tensor([[1., 2.], [3., 4.], [5., 6.]])
+    >>> q, r = qr(x)
+    >>> print(q)
+    array([[-0.16903079  0.897085]
+           [-0.5070925   0.2760267 ]
+           [-0.8451542  -0.34503305]], shape=(3, 2), dtype=float32)
+    """
+    if any_symbolic_tensors((x,)):
+        return Qr(mode=mode).symbolic_call(x)
+    x = backend.convert_to_tensor(x)
+    return backend.linalg.qr(x, mode=mode)
+
+
+class Solve(Operation):
+
+    def __init__(self):
+        super().__init__()
+
+    def call(self, a, b):
+        return _solve(a, b)
+
+    def compute_output_spec(self, a, b):
+        _assert_2d(a)
+        _assert_square(a)
+        _assert_1d(b)
+        _assert_a_b_compat(a, b)
+        return KerasTensor(b.shape, b.dtype)
+
+
+@keras_export(["keras.ops.solve", "keras.ops.linalg.solve"])
+def solve(a, b):
+    """Solves a linear system of equations given by `a x = b`.
+
+    Args:
+        a: A tensor of shape `(..., M, M)` representing the coefficients matrix.
+        b: A tensor of shape `(..., M)` or `(..., M, N)` represeting the
+        right-hand side or "dependent variable" matrix.
+
+    Returns:
+        A tensor of shape `(..., M)` or `(..., M, N)` representing the solution
+        of the linear system. Returned shape is identical to `b`.
+
+    """
+    if any_symbolic_tensors((a, b)):
+        return Solve().symbolic_call(a, b)
+    return _solve(a, b)
+
+
+def _solve(a, b):
+    a = backend.convert_to_tensor(a)
+    b = backend.convert_to_tensor(b)
+    _assert_2d(a)
+    _assert_square(a)
+    _assert_1d(b)
+    _assert_a_b_compat(a, b)
+    return backend.linalg.solve(a, b)
+
+
+class SolveTriangular(Operation):
+
+    def __init__(self, lower=False):
+        super().__init__()
+        self.lower = lower
+
+    def call(self, a, b):
+        return _solve_triangular(a, b, self.lower)
+
+    def compute_output_spec(self, a, b):
+        _assert_2d(a)
+        _assert_square(a)
+        _assert_1d(b)
+        _assert_a_b_compat(a, b)
+        return KerasTensor(b.shape, b.dtype)
+
+
+@keras_export(
+    ["keras.ops.solve_triangular", "keras.ops.linalg.solve_triangular"]
+)
+def solve_triangular(a, b, lower=False):
+    """Solves a linear system of equations given by `a x = b`.
+
+    Args:
+        a: A tensor of shape `(..., M, M)` representing the coefficients matrix.
+        b: A tensor of shape `(..., M)` or `(..., M, N)` represeting the
+        right-hand side or "dependent variable" matrix.
+
+    Returns:
+        A tensor of shape `(..., M)` or `(..., M, N)` representing the solution
+        of the linear system. Returned shape is identical to `b`.
+
+    """
+    if any_symbolic_tensors((a, b)):
+        return SolveTriangular(lower).symbolic_call(a, b)
+    return _solve_triangular(a, b, lower)
+
+
+def _solve_triangular(a, b, lower=False):
+    a = backend.convert_to_tensor(a)
+    b = backend.convert_to_tensor(b)
+    _assert_2d(a)
+    _assert_square(a)
+    _assert_1d(b)
+    _assert_a_b_compat(a, b)
+    return backend.linalg.solve_triangular(a, b, lower)
+
+
+class SVD(Operation):
+
+    def __init__(self, full_matrices=True, compute_uv=True):
+        super().__init__()
+        self.full_matrices = full_matrices
+        self.compute_uv = compute_uv
+
+    def call(self, x):
+        return _svd(x, self.full_matrices, self.compute_uv)
+
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        rows, columns = x.shape[-2:]
+        batches = x.shape[:-2]
+        s_shape = batches + (min(rows, columns),)
+        if self.full_matrices:
+            u_shape = batches + (rows, rows)
+            v_shape = batches + (columns, columns)
+        else:
+            u_shape = batches + (rows, min(rows, columns))
+            v_shape = batches + (min(rows, columns), columns)
+
+        if self.compute_uv:
+            return (
+                KerasTensor(u_shape, x.dtype),
+                KerasTensor(s_shape, x.dtype),
+                KerasTensor(v_shape, x.dtype),
+            )
+        return KerasTensor(s_shape, x.dtype)
+
+
+@keras_export(["keras.ops.svd", "keras.ops.linalg.svd"])
+def svd(x, full_matrices=True, compute_uv=True):
+    """Computes the singular value decomposition of a matrix.
+
+    Args:
+        x: Input tensor of shape `(..., M, N)`.
+
+    Returns:
+        A tuple of three tensors: a tensor of shape `(..., M, M)` containing the
+        left singular vectors, a tensor of shape `(..., M, N)` containing the
+        singular values and a tensor of shape `(..., N, N)` containing the
+        right singular vectors.
+
+    """
+    if any_symbolic_tensors((x,)):
+        return SVD(full_matrices, compute_uv).symbolic_call(x)
+    return _svd(x, full_matrices, compute_uv)
+
+
+def _svd(x, full_matrices=True, compute_uv=True):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    return backend.linalg.svd(x, full_matrices, compute_uv)
+
+
+def _assert_1d(*arrays):
+    for a in arrays:
+        if a.ndim < 1:
+            raise ValueError(
+                "Expected input to have rank >= 1. "
+                "Received scalar input {a}."
+            )
+
+
+def _assert_2d(*arrays):
+    for a in arrays:
+        if a.ndim < 2:
+            raise ValueError(
+                "Expected input to have rank >= 2. "
+                "Received input with shape {a.shape}."
+            )
+
+
+def _assert_square(*arrays):
+    for a in arrays:
+        m, n = a.shape[-2:]
+        if m != n:
+            raise ValueError(
+                "Expected a square matrix. "
+                f"Received non-square input with shape {a.shape}"
+            )
+
+
+def _assert_a_b_compat(a, b):
+    if a.ndim == b.ndim:
+        if a.shape[-2] != b.shape[-2]:
+            raise ValueError(
+                "Incompatible shapes between `a` and `b`. "
+                "Expected `a.shape[-2] == b.shape[-2]`. "
+                f"Received: a.shape={a.shape}, b.shape={b.shape}"
+            )
+    elif a.ndim == b.ndim - 1:
+        if a.shape[-1] != b.shape[-1]:
+            raise ValueError(
+                "Incompatible shapes between `a` and `b`. "
+                "Expected `a.shape[-1] == b.shape[-1]`. "
+                f"Received: a.shape={a.shape}, b.shape={b.shape}"
+            )
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import math
 import warnings
 
 import tensorflow as tf
 
-from keras.src.backend import standardize_data_format
-from keras.src.backend import standardize_dtype
+from keras.src import backend
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_output_shape,
 )
-from keras.src.backend.config import epsilon
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
 
 
 def relu(x):
     return tf.nn.relu(x)
 
@@ -71,38 +69,15 @@
 
 def selu(x):
     return tf.nn.selu(x)
 
 
 def gelu(x, approximate=True):
     x = convert_to_tensor(x)
-    # we need to explicitly implement gelu because bfloat16 will trigger
-    # DTypePromotionError when using enable_numpy_behavior()
-    if approximate:
-        coeff = tf.constant(0.044715, x.dtype)
-        return (
-            tf.constant(0.5, x.dtype)
-            * x
-            * (
-                tf.constant(1.0, x.dtype)
-                + tf.math.tanh(
-                    tf.constant(0.7978845608028654, x.dtype)
-                    * (x + coeff * tf.pow(x, 3))
-                )
-            )
-        )
-    else:
-        return (
-            tf.constant(0.5, x.dtype)
-            * x
-            * (
-                tf.constant(1.0, x.dtype)
-                + tf.math.erf(x / tf.constant(1.4142135623730951, x.dtype))
-            )
-        )
+    return tf.nn.gelu(x, approximate=approximate)
 
 
 def softmax(x, axis=-1):
     logits = x
     if axis is None:
         # Unlike numpy, tf will handle axis=None as axis=-1.
         # We need this workaround for the reduction on every dim.
@@ -158,15 +133,15 @@
 def max_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     strides = pool_size if strides is None else strides
     padding = padding.upper()
     tf_data_format = _convert_data_format("channels_last", len(inputs.shape))
     if data_format == "channels_first":
         # Tensorflow pooling does not support `channels_first` format, so
         # we need to transpose to `channels_last` format.
         inputs = _transpose_spatial_inputs(inputs)
@@ -186,15 +161,15 @@
 def average_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     strides = pool_size if strides is None else strides
     padding = padding.upper()
     tf_data_format = _convert_data_format("channels_last", len(inputs.shape))
     if data_format == "channels_first":
         # Tensorflow pooling does not support `channels_first` format, so
         # we need to transpose to `channels_last` format.
         inputs = _transpose_spatial_inputs(inputs)
@@ -264,15 +239,15 @@
 
     # Reason for making this function is in Tensorflow, `groups > 1` does not
     # work on CPU for `tf.nn.convolution`, but wrapping it by XLA works.
     @tf.function(jit_compile=True)
     def _conv_xla():
         return _conv()
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
         channels = inputs.shape[-1]
     else:
         channels = inputs.shape[1]
     if channels != kernel.shape[-2]:
         # If kernel's in_channel does not match input's channels,  it indicates
         # convolution is broken down into groups.
@@ -284,15 +259,15 @@
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = len(inputs.shape) - 2
     if num_spatial_dims > 2:
         raise ValueError(
             "`inputs` rank must be 3 (1D conv) or 4 (2D conv). Received: "
             "{inputs.ndim}."
         )
     # Because we use `tf.nn.depthwise_conv2d` for both 1D and 2D convs, we set
@@ -347,15 +322,15 @@
     depthwise_kernel,
     pointwise_kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = len(inputs.shape) - 2
     if num_spatial_dims > 2:
         raise ValueError(
             "`num_spatial_dims` must be 1 or 2. Received: "
             f"num_spatial_dims={num_spatial_dims}."
         )
     # Because we use `tf.nn.separable_conv2d` for both 1D and 2D convs, we set
@@ -410,15 +385,15 @@
     kernel,
     strides=1,
     padding="valid",
     output_padding=None,
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     tf_data_format = _convert_data_format(data_format, len(inputs.shape))
     kernel_size = kernel.shape[:-2]
     filters = kernel.shape[-2]
     input_shape = list(inputs.shape)
     symbolic_shape = tf.shape(inputs)
     for i, e in enumerate(input_shape):
         if e is None:
@@ -593,15 +568,17 @@
     # Adjust the predictions so that the probability of
     # each class for every sample adds up to 1
     # This is needed to ensure that the cross entropy is
     # computed correctly.
     output = output / tf.reduce_sum(output, axis, keepdims=True)
 
     # Compute cross entropy from probabilities.
-    output = tf.clip_by_value(output, epsilon(), 1.0 - epsilon())
+    output = tf.clip_by_value(
+        output, backend.epsilon(), 1.0 - backend.epsilon()
+    )
     return -tf.reduce_sum(target * tf.math.log(output), axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
     """Categorical crossentropy with integer targets.
 
     Args:
@@ -649,15 +626,17 @@
             raise ValueError(
                 "Arguments `target` and `output` must have the same shape "
                 "up until the last dimension: "
                 f"target.shape={target.shape}, output.shape={output.shape}"
             )
 
     if not from_logits:
-        output = tf.clip_by_value(output, epsilon(), 1 - epsilon())
+        output = tf.clip_by_value(
+            output, backend.epsilon(), 1 - backend.epsilon()
+        )
         output = tf.math.log(output)
 
     result = tf.nn.sparse_softmax_cross_entropy_with_logits(
         labels=target, logits=output
     )
     return result
 
@@ -698,26 +677,28 @@
 
     if from_logits:
         return tf.nn.sigmoid_cross_entropy_with_logits(
             labels=target, logits=output
         )
 
     # Compute cross entropy from probabilities.
-    output = tf.clip_by_value(output, epsilon(), 1.0 - epsilon())
+    output = tf.clip_by_value(
+        output, backend.epsilon(), 1.0 - backend.epsilon()
+    )
     bce = target * tf.math.log(output)
     bce += (1 - target) * tf.math.log(1 - output)
     return -bce
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
-    ori_dtype = standardize_dtype(x.dtype)
+    ori_dtype = backend.standardize_dtype(x.dtype)
     if ori_dtype in ("float16", "bfloat16"):
         need_cast = True
         x = cast(x, "float32")
 
     if synchronized:
         mean, variance = _compute_moments_sync(x, axes, keepdims)
     else:
@@ -793,53 +774,90 @@
 def ctc_loss(
     target,
     output,
     target_length,
     output_length,
     mask_index=0,
 ):
-    target = tf.convert_to_tensor(target)
+    target = convert_to_tensor(target)
+    output = convert_to_tensor(output)
     target = tf.cast(target, dtype="int32")
-    output = tf.convert_to_tensor(output)
-    output = tf.cast(output, dtype="float32")
-    return tf.nn.ctc_loss(
+
+    # `tf.nn.ctc_loss` will internally cast to float32 when the input is float16
+    # or bfloat16. Additionally, it will raise an error when the input is
+    # float64. As a result, we perform the casting externally and add support
+    # for float64.
+    result_dtype = backend.result_type(output.dtype, "float32")
+    compute_dtype = "float32" if result_dtype == "float64" else result_dtype
+    output = tf.cast(output, compute_dtype)
+    loss = tf.nn.ctc_loss(
         labels=target,
         logits=output,
         label_length=target_length,
         logit_length=output_length,
         blank_index=mask_index,
         logits_time_major=False,
     )
+    return tf.cast(loss, result_dtype)
 
 
 def ctc_decode(
     inputs,
     sequence_length,
-    strategy,
+    strategy="greedy",
     beam_width=100,
     top_paths=1,
     merge_repeated=True,
     mask_index=None,
 ):
-    inputs = tf.convert_to_tensor(inputs)
+    inputs = convert_to_tensor(inputs)
+    input_shape = tf.shape(inputs)
+    num_samples, num_steps = input_shape[0], input_shape[1]
     inputs = tf.transpose(inputs, (1, 0, 2))
 
-    sequence_length = tf.convert_to_tensor(sequence_length, dtype="int32")
+    dtype = backend.result_type(inputs.dtype, "float32")
+    inputs = tf.cast(inputs, dtype)
+
+    sequence_length = convert_to_tensor(sequence_length, dtype="int32")
     if strategy == "greedy":
-        return tf.nn.ctc_greedy_decoder(
+        (decoded, scores) = tf.nn.ctc_greedy_decoder(
             inputs=inputs,
             sequence_length=sequence_length,
             merge_repeated=merge_repeated,
             blank_index=mask_index,
         )
     elif strategy == "beam_search":
-        return tf.nn.ctc_beam_search_decoder(
+        (decoded, scores) = tf.nn.ctc_beam_search_decoder(
             inputs=inputs,
             sequence_length=sequence_length,
             beam_width=beam_width,
             top_paths=top_paths,
         )
     else:
         raise ValueError(
             f"Invalid strategy {strategy}. Supported values are "
             "'greedy' and 'beam_search'."
         )
+
+    # Postprocess sparse tensor
+    decoded_dense = []
+    for st in decoded:
+        st = tf.SparseTensor(st.indices, st.values, (num_samples, num_steps))
+        decoded_dense.append(tf.sparse.to_dense(sp_input=st, default_value=-1))
+    decoded_dense = tf.stack(decoded_dense, axis=0)
+    decoded_dense = tf.cast(decoded_dense, "int32")
+    return decoded_dense, scores
+
+
+def psnr(x1, x2, max_val):
+    from keras.src.backend.tensorflow.numpy import log10
+
+    if x1.shape != x2.shape:
+        raise ValueError(
+            f"Input shapes {x1.shape} and {x2.shape} must "
+            "match for PSNR calculation. "
+        )
+
+    max_val = convert_to_tensor(max_val, dtype=x2.dtype)
+    mse = tf.reduce_mean(tf.square(x1 - x2))
+    psnr = 20 * log10(max_val) - 10 * log10(mse)
+    return psnr
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/core.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import contextlib
-import os
 
 import ml_dtypes
 import numpy as np
 import torch
 
 from keras.src import tree
 from keras.src.backend.common import KerasVariable
@@ -15,18 +14,15 @@
 from keras.src.backend.config import floatx
 
 SUPPORTS_SPARSE_TENSORS = False
 
 # Some operators such as 'aten::_foreach_mul_.Scalar'
 # are not currently implemented for the MPS device.
 # check https://github.com/pytorch/pytorch/issues/77764.
-if (
-    torch.backends.mps.is_available()
-    and os.getenv("PYTORCH_ENABLE_MPS_FALLBACK") == "1"
-):
+if torch.backends.mps.is_available():
     DEFAULT_DEVICE = "mps"
 elif torch.cuda.is_available():
     DEFAULT_DEVICE = "cuda"
 else:
     DEFAULT_DEVICE = "cpu"
 
 TORCH_DTYPES = {
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/image.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/math.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import torch
 import torch.nn.functional as tnn
 
+from keras.src import backend
 from keras.src import tree
-from keras.src.backend import standardize_data_format
-from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_padding_args_for_torch,
 )
-from keras.src.backend.config import epsilon
 from keras.src.backend.torch.core import cast
 from keras.src.backend.torch.core import convert_to_tensor
 from keras.src.backend.torch.core import get_device
 from keras.src.backend.torch.numpy import expand_dims
 from keras.src.backend.torch.numpy import maximum
 from keras.src.backend.torch.numpy import where
 from keras.src.utils.argument_validation import standardize_tuple
@@ -88,34 +86,40 @@
     if approximate:
         return tnn.gelu(x, approximate="tanh")
     return tnn.gelu(x)
 
 
 def softmax(x, axis=-1):
     x = convert_to_tensor(x)
-    dtype = standardize_dtype(x.dtype)
+    dtype = backend.standardize_dtype(x.dtype)
     # TODO: tnn.softmax doesn't support float16 using cpu
-    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
+    if (
+        get_device() == "cpu"
+        and backend.standardize_dtype(x.dtype) == "float16"
+    ):
         x = cast(x, "float32")
     if axis is None:
         # Unlike numpy, PyTorch will handle axis=None as axis=-1.
         # We need this workaround for the reduction on every dim.
         output = torch.reshape(x, [-1])
         output = tnn.softmax(output, dim=-1)
         output = torch.reshape(output, x.shape)
     else:
         output = tnn.softmax(x, dim=axis)
     return cast(output, dtype)
 
 
 def log_softmax(x, axis=-1):
     x = convert_to_tensor(x)
-    dtype = standardize_dtype(x.dtype)
+    dtype = backend.standardize_dtype(x.dtype)
     # TODO: tnn.log_softmax doesn't support float16 using cpu
-    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
+    if (
+        get_device() == "cpu"
+        and backend.standardize_dtype(x.dtype) == "float16"
+    ):
         x = cast(x, "float32")
     if axis is None:
         # Unlike numpy, PyTorch will handle axis=None as axis=-1.
         # We need this workaround for the reduction on every dim.
         output = torch.reshape(x, [-1])
         output = tnn.log_softmax(output, dim=-1)
         output = torch.reshape(output, x.shape)
@@ -236,15 +240,15 @@
     num_spatial_dims = inputs.ndim - 2
     pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
     if strides is None:
         strides = pool_size
     else:
         strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
         inputs = _transpose_spatial_inputs(inputs)
 
     if padding == "same":
         # Torch does not natively support `"same"` padding, we need to manually
         # apply the right amount of padding to `inputs`.
         inputs, padding = _apply_same_padding(
@@ -297,15 +301,15 @@
     num_spatial_dims = inputs.ndim - 2
     pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
     if strides is None:
         strides = pool_size
     else:
         strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
         inputs = _transpose_spatial_inputs(inputs)
     padding_value = 0
     if padding == "same":
         spatial_shape = inputs.shape[2:]
         num_spatial_dims = len(spatial_shape)
         padding_value = []
@@ -371,15 +375,15 @@
     dilation_rate=1,
 ):
     inputs = convert_to_tensor(inputs)
     kernel = convert_to_tensor(kernel)
     num_spatial_dims = inputs.ndim - 2
     strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
         inputs = _transpose_spatial_inputs(inputs)
     # Transpose kernel from keras format to torch format.
     kernel = _transpose_conv_kernel(kernel)
     if padding == "same" and any(d != 1 for d in tree.flatten(strides)):
         # Torch does not support this case in conv2d().
         # Manually pad the tensor.
@@ -490,15 +494,15 @@
     dilation_rate=1,
 ):
     inputs = convert_to_tensor(inputs)
     kernel = convert_to_tensor(kernel)
     num_spatial_dims = inputs.ndim - 2
     strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     (
         torch_padding,
         torch_output_padding,
     ) = compute_conv_transpose_padding_args_for_torch(
         input_shape=inputs.shape,
         kernel_shape=kernel.shape,
         strides=strides,
@@ -606,15 +610,15 @@
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
         log_prob = tnn.log_softmax(output, dim=axis)
     else:
         output = output / torch.sum(output, dim=axis, keepdim=True)
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        output = torch.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         log_prob = torch.log(output)
     return -torch.sum(target * log_prob, dim=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
     target = convert_to_tensor(target, dtype=torch.long)
     output = convert_to_tensor(output)
@@ -634,15 +638,15 @@
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
         log_prob = tnn.log_softmax(output, dim=axis)
     else:
         output = output / torch.sum(output, dim=axis, keepdim=True)
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        output = torch.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         log_prob = torch.log(output)
     target = one_hot(target, output.shape[axis], axis=axis)
     return -torch.sum(target * log_prob, dim=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
     target = convert_to_tensor(target)
@@ -657,29 +661,29 @@
     # By default, PyTorch, does reduction of `sum` over all rows,
     # change reduction to `none` to keep dim
     if from_logits:
         return tnn.binary_cross_entropy_with_logits(
             output, target, reduction="none"
         )
     else:
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        output = torch.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         return tnn.binary_cross_entropy(output, target, reduction="none")
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
             "Argument synchronized=True is not supported with PyTorch."
         )
     x = convert_to_tensor(x)
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
-    ori_dtype = standardize_dtype(x.dtype)
+    ori_dtype = backend.standardize_dtype(x.dtype)
     if ori_dtype == "float16":
         need_cast = True
         x = cast(x, "float32")
 
     mean = torch.mean(x, dim=axes, keepdim=True)
 
     # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
@@ -748,32 +752,116 @@
     mask_index=0,
 ):
     target = convert_to_tensor(target)
     output = convert_to_tensor(output)
     target_length = convert_to_tensor(target_length)
     output_length = convert_to_tensor(output_length)
 
+    # Ensure that the dtype promotion behavior matchs that of `tf.nn.ctc_loss`
+    dtype = backend.result_type(output.dtype, "float32")
+    output = cast(output, dtype)
+
     output = torch.transpose(output, 1, 0)
     logits = tnn.log_softmax(output, dim=-1)
-
-    return tnn.ctc_loss(
+    loss = tnn.ctc_loss(
         logits,
         target,
         output_length,
         target_length,
         blank=mask_index,
         reduction="none",
     )
+    return loss
+
+
+def _ctc_greedy_decode(
+    inputs,
+    sequence_length,
+    merge_repeated=True,
+    mask_index=None,
+):
+    inputs = convert_to_tensor(inputs)
+    sequence_length = convert_to_tensor(sequence_length, dtype="int32")
+    batch_size, max_length, num_classes = inputs.shape
+
+    if mask_index is None:
+        mask_index = num_classes - 1
+
+    indices = torch.argmax(inputs, axis=-1)
+    indices = cast(indices, "int32")
+    scores = torch.max(inputs, axis=-1)[0]
+
+    seqlen_mask = torch.arange(max_length, device=indices.device)[None, :]
+    seqlen_mask = seqlen_mask >= sequence_length[:, None]
+
+    indices = torch.where(seqlen_mask, mask_index, indices)
+    scores = torch.where(seqlen_mask, 0.0, scores)
+
+    if merge_repeated:
+        repeat = indices[:, 1:] == indices[:, :-1]
+        repeat = tnn.pad(repeat, (1, 0, 0, 0))
+        indices = torch.where(repeat, mask_index, indices)
+
+    # We rearrange the indices by moving `mask_index` to the end of the array
+    invalid_mask = indices == mask_index
+    order = torch.unsqueeze(
+        torch.arange(max_length, device=indices.device), dim=0
+    )  # [1, N]
+    order = torch.tile(order, (batch_size, 1))  # [B, N]
+    order = torch.where(invalid_mask, max_length, order)
+    order = torch.argsort(order, dim=-1)
+    indices = torch.take_along_dim(indices, order, dim=-1)
+
+    # We set to -1 for blank labels
+    indices = torch.where(invalid_mask, -1, indices)
+    scores = -torch.sum(scores, axis=1)[:, None]
+    indices = torch.unsqueeze(indices, dim=0)
+    return indices, scores
 
 
 def ctc_decode(
     inputs,
     sequence_length,
-    strategy,
+    strategy="greedy",
     beam_width=100,
     top_paths=1,
     merge_repeated=True,
     mask_index=None,
 ):
-    raise NotImplementedError(
-        "Torch backend does not yet support CTC decoding."
+    inputs = convert_to_tensor(inputs)
+    dtype = backend.result_type(inputs.dtype, "float32")
+    inputs = cast(inputs, dtype)
+
+    if strategy == "greedy":
+        return _ctc_greedy_decode(
+            inputs,
+            sequence_length,
+            merge_repeated=merge_repeated,
+            mask_index=mask_index,
+        )
+    elif strategy == "beam_search":
+        raise NotImplementedError(
+            "Torch backend doesn't yet support the beam search strategy for CTC"
+            "decoding."
+        )
+    else:
+        raise ValueError(
+            f"Invalid strategy {strategy}. Supported values are "
+            "'greedy' and 'beam_search'."
+        )
+
+
+def psnr(x1, x2, max_val):
+    if x1.shape != x2.shape:
+        raise ValueError(
+            f"Input shapes {x1.shape} and {x2.shape} must "
+            "match for PSNR calculation. "
+        )
+
+    x1, x2 = (
+        convert_to_tensor(x1),
+        convert_to_tensor(x2),
     )
+    max_val = convert_to_tensor(max_val, dtype=x1.dtype)
+    mse = torch.mean((x1 - x2) ** 2)
+    psnr = 20 * torch.log10(max_val) - 10 * torch.log10(mse)
+    return psnr
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/random.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/callback.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/early_stopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
             for `patience` epochs and restore weights from the best epoch in
             that set. Defaults to `False`.
         start_from_epoch: Number of epochs to wait before starting to monitor
             improvement. This allows for a warm-up period in which no
             improvement is expected and thus training will not be stopped.
             Defaults to `0`.
 
-
     Example:
 
     >>> callback = keras.callbacks.EarlyStopping(monitor='loss',
     ...                                               patience=3)
     >>> # This callback will stop the training when there is no improvement in
     >>> # the loss for three consecutive epochs.
     >>> model = keras.models.Sequential([keras.layers.Dense(10)])
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/history.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/constraints/constraints.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/cifar.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/imdb.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/mnist.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/datasets/reuters.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/export/export_lib.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/initializers/initializer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/dense.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/identity.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/masking.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/input_spec.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/layer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/add.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/average.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/bidirectional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import copy
 
 from keras.src import ops
 from keras.src import utils
 from keras.src.api_export import keras_export
-from keras.src.layers.core.wrapper import Wrapper
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
 
 
 @keras_export("keras.layers.Bidirectional")
-class Bidirectional(Wrapper):
+class Bidirectional(Layer):
     """Bidirectional wrapper for RNNs.
 
     Args:
         layer: `keras.layers.RNN` instance, such as
             `keras.layers.LSTM` or `keras.layers.GRU`.
             It could also be a `keras.layers.Layer` instance
             that meets the following criteria:
@@ -101,15 +100,15 @@
             )
         if merge_mode not in ["sum", "mul", "ave", "concat", None]:
             raise ValueError(
                 f"Invalid merge mode. Received: {merge_mode}. "
                 "Merge mode should be one of "
                 '{"sum", "mul", "ave", "concat", None}'
             )
-        super().__init__(layer, **kwargs)
+        super().__init__(**kwargs)
 
         # Recreate the forward layer from the original layer config, so that it
         # will not carry over any state from the layer.
         config = serialization_lib.serialize_keras_object(layer)
         config["config"]["name"] = "forward_" + utils.removeprefix(
             layer.name, "forward_"
         )
@@ -268,16 +267,18 @@
     @property
     def states(self):
         if self.forward_layer.states and self.backward_layer.states:
             return tuple(self.forward_layer.states + self.backward_layer.states)
         return None
 
     def build(self, sequences_shape, initial_state_shape=None):
-        self.forward_layer.build(sequences_shape)
-        self.backward_layer.build(sequences_shape)
+        if not self.forward_layer.built:
+            self.forward_layer.build(sequences_shape)
+        if not self.backward_layer.built:
+            self.backward_layer.build(sequences_shape)
         self.built = True
 
     def compute_mask(self, _, mask):
         if isinstance(mask, list):
             mask = mask[0]
         if self.return_sequences:
             if not self.merge_mode:
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/backend.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/layers.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/losses.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/losses/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/losses/loss.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/losses/losses.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/losses/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1889,15 +1889,15 @@
             containing logits (the output of your model).
             They should *not* be normalized via softmax.
     """
 
     def __init__(
         self,
         reduction="sum_over_batch_size",
-        name="sparse_categorical_crossentropy",
+        name="ctc",
     ):
         super().__init__(
             ctc,
             name=name,
             reduction=reduction,
         )
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/metric.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/models/cloning.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/models/cloning.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 from keras.src.models.functional import Functional
 from keras.src.models.functional import functional_like_constructor
 from keras.src.models.sequential import Sequential
 from keras.src.saving import serialization_lib
 
 
 @keras_export("keras.models.clone_model")
-def clone_model(model, input_tensors=None, clone_function=None):
+def clone_model(
+    model,
+    input_tensors=None,
+    clone_function=None,
+    call_function=None,
+    recursive=False,
+    **kwargs,
+):
     """Clone a Functional or Sequential `Model` instance.
 
     Model cloning is similar to calling a model on new inputs,
     except that it creates new layers (and thus new weights) instead
     of sharing the weights of the existing layers.
 
     Note that
@@ -25,32 +32,52 @@
 
     Args:
         model: Instance of `Model`
             (could be a Functional model or a Sequential model).
         input_tensors: optional list of input tensors or InputLayer objects
             to build the model upon. If not provided,
             new `Input` objects will be created.
-        clone_function: Callable to be used to clone each layer in the target
+        clone_function: Callable with signature `fn(layer)`
+            to be used to clone each layer in the target
             model (except `Input` instances). It takes as argument the
             layer instance to be cloned, and returns the corresponding layer
             instance to be used in the model copy. If unspecified, this callable
-            becomes the following serialization/deserialization function:
+            defaults to the following serialization/deserialization function:
             `lambda layer: layer.__class__.from_config(layer.get_config())`.
             By passing a custom callable, you can customize your copy of the
             model, e.g. by wrapping certain layers of interest (you might want
             to replace all `LSTM` instances with equivalent
             `Bidirectional(LSTM(...))` instances, for example).
             Defaults to `None`.
+        call_function: Callable with signature
+            `fn(layer, *args, **kwargs)` to be used to call each
+            cloned layer and a set of inputs. It takes the layer instance,
+            the call arguments and keyword arguments, and returns the
+            call outputs. If unspecified, this callable defaults to
+            the regular `__call__()` method:
+            `def fn(layer, *args, **kwargs): return layer(*args, **kwargs)`.
+            By passing a custom callable, you can insert new layers before or
+            after a given layer. Note: this argument can only be used with
+            Functional models.
+        recursive: Boolean. Whether to recursively clone any Sequential
+            or Functional models encountered in the original
+            Sequential/Functional model. If `False`,
+            then inner models are cloned by calling `clone_function()`.
+            If `True`, then inner models are cloned by calling `clone_model()`
+            with the same `clone_function`, `call_function`, and `recursive`
+            arguments. Note that in this case, `call_function`
+            will not be propagated to any Sequential model
+            (since it is not applicable to Sequential models).
 
     Returns:
         An instance of `Model` reproducing the behavior
         of the original model, on top of new inputs tensors,
         using newly instantiated weights. The cloned model may behave
         differently from the original model if a custom `clone_function`
-        modifies the layer.
+        or `call_function` modifies a layer or layer call.
 
     Example:
 
     ```python
     # Create a test Sequential model.
     model = keras.Sequential([
         keras.layers.Input(shape=(728,)),
@@ -70,65 +97,166 @@
         if "seed" in config:
             config["seed"] = 1337
         return layer.__class__.from_config(config)
 
     new_model = clone_model(model)
     ```
 
+    Using a `call_function` to add a `Dropout` layer after each `Dense` layer
+    (without recreating new layers):
+
+    ```python
+    def call_function(layer, *args, **kwargs):
+        out = layer(*args, **kwargs)
+        if isinstance(layer, keras.layers.Dense):
+            out = keras.layers.Dropout(0.5)(out)
+        return out
+
+    new_model = clone_model(
+        model,
+        clone_function=lambda x: x,  # Reuse the same layers.
+        call_function=call_function,
+    )
+    ```
+
     Note that subclassed models cannot be cloned by default,
     since their internal layer structure is not known.
     To achieve equivalent functionality
     as `clone_model` in the case of a subclassed model, simply make sure
     that the model class implements `get_config()`
     (and optionally `from_config()`), and call:
 
     ```python
     new_model = model.__class__.from_config(model.get_config())
     ```
 
     In the case of a subclassed model, you cannot using a custom
     `clone_function`.
     """
+    cache = kwargs.pop("cache", None)
+    if kwargs:
+        raise ValueError(
+            f"Unexpected keyword argument(s): {tuple(kwargs.keys())}"
+        )
+
     if isinstance(model, Sequential):
+        # Wrap clone_function to handle recursiveness and layer sharing.
+        clone_function = _wrap_clone_function(
+            clone_function,
+            call_function=call_function,
+            recursive=recursive,
+            cache=cache,
+        )
+        if call_function is not None:
+            raise ValueError(
+                "`call_function` argument is not supported with Sequential "
+                "models.  In a Sequential model, layers aren't called "
+                "at model-construction time (they're merely listed). "
+                "Use `call_function` with Functional models only. "
+                "Received model of "
+                f"type '{model.__class__.__name__}', with "
+                f"call_function={clone_function}"
+            )
         return _clone_sequential_model(
-            model, input_tensors=input_tensors, clone_function=clone_function
+            model,
+            clone_function=clone_function,
+            input_tensors=input_tensors,
         )
     if isinstance(model, Functional):
+        # Wrap clone_function to handle recursiveness and layer sharing.
+        clone_function = _wrap_clone_function(
+            clone_function,
+            call_function=call_function,
+            recursive=recursive,
+            cache=cache,
+        )
+
         # If the get_config() method is the same as a regular Functional
         # model, we're safe to use _clone_functional_model (which relies
         # on a Functional constructor). In the case where the get_config
         # is custom, this may not necessarily work, but if clone_function
         # or input_tensors are passed, we attempt it anyway
         # in order to preserve backwards compatibility.
         if utils.is_default(model.get_config) or (
             clone_function or input_tensors
         ):
             return _clone_functional_model(
                 model,
-                input_tensors=input_tensors,
                 clone_function=clone_function,
+                call_function=call_function,
+                input_tensors=input_tensors,
             )
 
     # Case of a custom model class
     if clone_function or input_tensors:
         raise ValueError(
-            "Arguments clone_function and input_tensors "
+            "Arguments `clone_function` and `input_tensors` "
             "are only supported for Sequential models "
             "or Functional models. Received model of "
             f"type '{model.__class__.__name__}', with "
             f"clone_function={clone_function} and "
             f"input_tensors={input_tensors}"
         )
+    if call_function is not None:
+        raise ValueError(
+            "Argument `call_function` is only supported "
+            "for Functional models. Received model of "
+            f"type '{model.__class__.__name__}', with "
+            f"call_function={clone_function}"
+        )
     config = serialization_lib.serialize_keras_object(model)
     return serialization_lib.deserialize_keras_object(
         config, custom_objects={model.__class__.__name__: model.__class__}
     )
 
 
-def _clone_sequential_model(model, input_tensors=None, clone_function=None):
+def _wrap_clone_function(
+    clone_function, call_function=None, recursive=False, cache=None
+):
+    """Wrapper to handle recursiveness and layer sharing."""
+    if clone_function is None:
+
+        def _clone_layer(layer):
+            return layer.__class__.from_config(layer.get_config())
+
+        clone_function = _clone_layer
+
+    if cache is None:
+        cache = {}
+
+    def wrapped_clone_function(layer):
+        if id(layer) in cache:
+            return cache[id(layer)]
+        if recursive:
+            if isinstance(layer, Sequential):
+                # Note: Sequential doens't support call_function.
+                clone = clone_model(
+                    layer,
+                    clone_function=clone_function,
+                    cache=cache,
+                )
+                cache[id(layer)] = clone
+                return clone
+            elif isinstance(layer, Functional):
+                clone = clone_model(
+                    layer,
+                    clone_function=clone_function,
+                    call_function=call_function,
+                    cache=cache,
+                )
+                cache[id(layer)] = clone
+                return clone
+        clone = clone_function(layer)
+        cache[id(layer)] = clone
+        return clone
+
+    return wrapped_clone_function
+
+
+def _clone_sequential_model(model, clone_function, input_tensors=None):
     """Clone a `Sequential` model instance.
 
     Model cloning is similar to calling a model on new inputs,
     except that it creates new layers (and thus new weights) instead
     of sharing the weights of the existing layers.
 
     Args:
@@ -140,20 +268,14 @@
             By default, it clones the layer (without copying the weights).
 
     Returns:
         An instance of `Sequential` reproducing the behavior
         of the original model, on top of new inputs tensors,
         using newly instantiated weights.
     """
-    if clone_function is None:
-
-        def _clone_layer(layer):
-            return layer.__class__.from_config(layer.get_config())
-
-        clone_function = _clone_layer
 
     if not isinstance(model, Sequential):
         raise ValueError(
             "Expected `model` argument "
             "to be a `Sequential` model instance. "
             f"Received: model={model}"
         )
@@ -198,15 +320,17 @@
                 dtype=input_dtype,
                 name=input_name,
             )
             new_layers = [inputs] + new_layers
     return Sequential(new_layers, name=model.name, trainable=model.trainable)
 
 
-def _clone_functional_model(model, input_tensors=None, clone_function=None):
+def _clone_functional_model(
+    model, clone_function, input_tensors=None, call_function=None
+):
     """Clone a `Functional` model instance.
 
     Model cloning is similar to calling a model on new inputs,
     except that it creates new layers (and thus new weights) instead
     of sharing the weights of the existing layers.
 
     Input layers are always cloned.
@@ -220,25 +344,14 @@
             By default, it clones the layer (without copying the weights).
 
     Returns:
         An instance of `Functional` reproducing the behavior
         of the original model, on top of new inputs tensors,
         using newly instantiated weights.
     """
-    if clone_function is None:
-        seen = {}
-
-        def _clone_layer(layer):
-            if layer in seen:
-                return seen[layer]
-            new_layer = layer.__class__.from_config(layer.get_config())
-            seen[layer] = new_layer
-            return new_layer
-
-        clone_function = _clone_layer
 
     if not callable(clone_function):
         raise ValueError(
             "Expected `clone_function` argument to be a callable. "
             f"Received: clone_function={clone_function}"
         )
 
@@ -272,15 +385,17 @@
         )
 
     def operation_fn(layer):
         new_layer = clone_function(layer)
         return new_layer
 
     output_tensors = model._run_through_graph(
-        input_tensors, operation_fn=operation_fn
+        input_tensors,
+        operation_fn=operation_fn,
+        call_fn=call_function,
     )
 
     if functional_like_constructor(model.__class__):
         new_model = model.__class__(
             input_tensors, output_tensors, name=model.name
         )
     else:
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/models/functional.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/models/model.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/models/sequential.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/core.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/function.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         )
 
     def call(self, inputs):
         """Computes output tensors for new inputs."""
         self._assert_input_compatibility(inputs)
         return self._run_through_graph(inputs, operation_fn=lambda op: op)
 
-    def _run_through_graph(self, inputs, operation_fn):
+    def _run_through_graph(self, inputs, operation_fn, call_fn=None):
         """Execute the graph.
 
         At each node we compute outputs via
         `operation_fn(node.operation)(*args, **kwargs)`.
         """
         inputs = tree.flatten(inputs)
 
@@ -144,15 +144,19 @@
                 if not node.operation or node.is_input:
                     continue  # Input tensors already exist.
 
                 if any(id(x) not in tensor_dict for x in node.input_tensors):
                     continue  # Node is not computable, try skipping.
 
                 args, kwargs = node.arguments.fill_in(tensor_dict)
-                outputs = operation_fn(node.operation)(*args, **kwargs)
+                op = operation_fn(node.operation)
+                if call_fn is not None:
+                    outputs = call_fn(op, *args, **kwargs)
+                else:
+                    outputs = op(*args, **kwargs)
 
                 # Update tensor_dict.
                 for x, y in zip(node.outputs, tree.flatten(outputs)):
                     tensor_dict[id(x)] = y
 
         output_tensors = []
         for x in self.outputs:
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/image.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
     if data_format == "channels_last":
         channels_in = image.shape[-1]
     elif data_format == "channels_first":
         channels_in = image.shape[-3]
     if not strides:
         strides = size
     out_dim = patch_h * patch_w * channels_in
-    kernel = backend.numpy.eye(out_dim)
+    kernel = backend.numpy.eye(out_dim, dtype=image.dtype)
     kernel = backend.numpy.reshape(
         kernel, (patch_h, patch_w, channels_in, out_dim)
     )
     _unbatched = False
     if len(image.shape) == 3:
         _unbatched = True
         image = backend.numpy.expand_dims(image, axis=0)
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/math.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/nn.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1806,16 +1806,16 @@
         )
 
     return backend.nn.batch_normalization(
         x, mean, variance, axis, offset, scale, epsilon
     )
 
 
-class CtcLoss(Operation):
-    def __init__(self, mask_index):
+class CTCLoss(Operation):
+    def __init__(self, mask_index=0):
         super().__init__()
         self.mask_index = mask_index
 
     def call(self, target, output, target_length, output_length):
         return backend.nn.ctc_loss(
             target, output, target_length, output_length, self.mask_index
         )
@@ -1834,16 +1834,16 @@
         )
         self._check_shape_first_dim(
             "target_length", target_length.shape, "target", target.shape
         )
         self._check_shape_first_dim(
             "output_length", output_length.shape, "output", output.shape
         )
-
-        return KerasTensor((target.shape[0],), dtype=target.dtype)
+        dtype = backend.result_type(output.dtype, "float32")
+        return KerasTensor((target.shape[0],), dtype=dtype)
 
 
 @keras_export(
     [
         "keras.ops.ctc_loss",
         "keras.ops.nn.ctc_loss",
     ]
@@ -1861,42 +1861,85 @@
         output_length: A tensor of shape `(batch_size,)` containing the
             output lengths.
         mask_index: The index of the mask character in the vocabulary.
             Defaults to `0`.
     """
 
     if any_symbolic_tensors((target, output, target_length, output_length)):
-        return CtcLoss(mask_index).symbolic_call(
+        return CTCLoss(mask_index).symbolic_call(
             target, output, target_length, output_length
         )
     return backend.nn.ctc_loss(
         target, output, target_length, output_length, mask_index
     )
 
 
+class CTCDecode(Operation):
+    def __init__(
+        self,
+        strategy="greedy",
+        beam_width=100,
+        top_paths=1,
+        merge_repeated=True,
+        mask_index=None,
+    ):
+        super().__init__()
+        self.strategy = strategy
+        self.beam_width = beam_width
+        self.top_paths = top_paths
+        self.merge_repeated = merge_repeated
+        self.mask_index = mask_index
+
+    def call(self, inputs, sequence_lengths):
+        return backend.nn.ctc_decode(
+            inputs,
+            sequence_lengths,
+            strategy=self.strategy,
+            beam_width=self.beam_width,
+            top_paths=self.top_paths,
+            merge_repeated=self.merge_repeated,
+            mask_index=self.mask_index,
+        )
+
+    def compute_output_spec(self, inputs, sequence_lengths):
+        inputs_shape = inputs.shape
+        if self.strategy == "greedy":
+            top_paths = 1
+        else:
+            top_paths = self.top_paths
+        dtype = backend.result_type(inputs.dtype, "float32")
+        return (
+            KerasTensor(
+                (top_paths, inputs_shape[0], inputs_shape[1]), dtype="int32"
+            ),
+            KerasTensor((inputs_shape[0], top_paths), dtype=dtype),
+        )
+
+
 @keras_export(
     [
         "keras.ops.ctc_decode",
         "keras.ops.nn.ctc_decode",
     ]
 )
 def ctc_decode(
     inputs,
     sequence_lengths,
-    strategy,
+    strategy="greedy",
     beam_width=100,
     top_paths=1,
     merge_repeated=True,
     mask_index=None,
 ):
     """Decodes the output of a CTC model.
 
     Args:
         inputs: A tensor of shape `(batch_size, max_length, num_classes)`
-            containing the logits (output of the model).
+            containing the logits (the output of the model).
+            They should *not* be normalized via softmax.
         sequence_lengths: A tensor of shape `(batch_size,)` containing the
             sequence lengths for the batch.
         strategy: A string for the decoding strategy. Supported values are
             `"greedy"` and `"beam_search"`.
         beam_width: An integer scalar beam width used in beam search.
             Defaults to 100.
         top_paths: An integer scalar, the number of top paths to return.
@@ -1904,28 +1947,34 @@
         merge_repeated: A boolean scalar, whether to merge repeated
             labels in the output. Defaults to `True`.
         mask_index: An integer scalar, the index of the mask character in
             the vocabulary. Defaults to `None`.
 
     Returns:
         A tuple containing:
-
-        - A list of decoded sequences.
-        - A list of the negative of the sum of the probability logits
-        (if strategy is `"greedy"`) or the log probability (if strategy is
-        `"beam_search"`) for each sequence.
+        - The tensor representing the list of decoded sequences. If
+            `strategy="greedy"`, the shape is `(1, batch_size, max_length)`. If
+            `strategy="beam_seatch"`, the shape is
+            `(top_paths, batch_size, max_length)`. Note that: `-1` indicates the
+            blank label.
+        - If `strategy="greedy"`, a tensor of shape `(batch_size, 1)`
+            representing the negative of the sum of the probability logits for
+            each sequence. If `strategy="beam_seatch"`, a tensor of shape
+            `(batch_size, top_paths)` representing the log probability for each
+            sequence.
     """
 
     if any_symbolic_tensors((inputs, sequence_lengths)):
-        raise NotImplementedError(
-            "CTC decoding is not supported with KerasTensors. Use it "
-            "inside the call() method of a Layer or the predict_step "
-            "method of a model."
-        )
-
+        return CTCDecode(
+            strategy=strategy,
+            beam_width=beam_width,
+            top_paths=top_paths,
+            merge_repeated=merge_repeated,
+            mask_index=mask_index,
+        ).symbolic_call(inputs, sequence_lengths)
     return backend.nn.ctc_decode(
         inputs=inputs,
         sequence_length=sequence_lengths,
         strategy=strategy,
         beam_width=beam_width,
         top_paths=top_paths,
         merge_repeated=merge_repeated,
@@ -1989,7 +2038,80 @@
     x = backend.convert_to_tensor(x)
     if len(x.shape) == 0:
         x = backend.numpy.expand_dims(x, axis=0)
     epsilon = backend.epsilon()
     norm = backend.linalg.norm(x, ord=order, axis=axis, keepdims=True)
     denom = backend.numpy.maximum(norm, epsilon)
     return backend.numpy.divide(x, denom)
+
+
+class PSNR(Operation):
+    def __init__(
+        self,
+        max_val,
+    ):
+        super().__init__()
+        self.max_val = max_val
+
+    def call(self, x1, x2):
+        return backend.nn.psnr(
+            x1=x1,
+            x2=x2,
+            max_val=self.max_val,
+        )
+
+    def compute_output_spec(self, x1, x2):
+        if len(x1.shape) != len(x2.shape):
+            raise ValueError("Inputs must have the same rank")
+
+        return KerasTensor(shape=())
+
+
+@keras_export(
+    [
+        "keras.ops.psnr",
+        "keras.ops.nn.psnr",
+    ]
+)
+def psnr(
+    x1,
+    x2,
+    max_val,
+):
+    """Peak Signal-to-Noise Ratio (PSNR) function.
+
+    This function computes the Peak Signal-to-Noise Ratio between two signals,
+    `x1` and `x2`. PSNR is a measure of the quality of a reconstructed signal.
+    The higher the PSNR, the closer the reconstructed signal is to the original
+    signal. Note that it can become negative when the signal power is
+    smaller that the noise power.
+
+    Args:
+        x1: The first input signal.
+        x2: The second input signal. Must have the same shape as `x1`.
+        max_val: The maximum possible value in the signals.
+
+    Returns:
+        float: The PSNR value between `x1` and `x2`.
+
+    Examples:
+
+    >>> x1 = keras.random.normal((2, 4, 4, 3))
+    >>> x2 = keras.random.normal((2, 4, 4, 3))
+    >>> max_val = 1.0
+    >>> keras.ops.nn.psnr(x1, x2, max_val)
+    -3.1697404
+    """
+    if any_symbolic_tensors(
+        (
+            x1,
+            x2,
+        )
+    ):
+        return PSNR(
+            max_val,
+        ).symbolic_call(x1, x2)
+    return backend.nn.psnr(
+        x1,
+        x2,
+        max_val,
+    )
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/node.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/numpy.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/operation.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adam.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/lion.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/random/random.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/random/seed_generator.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/saving/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/saving/keras_saveable.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/saving/keras_saveable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/saving/object_registration.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/saving/saving_api.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/testing/test_case.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/testing/test_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/compile_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     @property
     def variables(self):
         # Avoiding relying on implicit tracking since
         # CompileMetrics may be instantiated or built in a no tracking scope.
         if not self.built:
             return []
         vars = []
-        for m in self._flat_metrics + self._flat_weighted_metrics:
+        for m in self.metrics:
             if m is not None:
                 vars.extend(m.variables)
         return vars
 
     def build(self, y_true, y_pred):
         if self.output_names:
             output_names = self.output_names
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,21 @@
         if y is not None:
             raise_unsupported_arg("y", "the targets", "PyDataset")
         if sample_weight is not None:
             raise_unsupported_arg(
                 "sample_weights", "the sample weights", "PyDataset"
             )
         return PyDatasetAdapter(x, class_weight=class_weight, shuffle=shuffle)
+        # TODO: should we warn or not?
+        # if x.num_batches is None and shuffle:
+        #     warnings.warn(
+        #         "`shuffle=True` was passed, but will be ignored since the "
+        #         "data `x` was provided as a infinite PyDataset. The "
+        #         "PyDataset is expected to already be shuffled."
+        # )
     elif is_torch_dataloader(x):
         if y is not None:
             raise_unsupported_arg("y", "the targets", "torch DataLoader")
         if sample_weight is not None:
             raise_unsupported_arg(
                 "sample_weights", "the sample weights", "torch DataLoader"
             )
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import multiprocessing.dummy
 import queue
 import random
 import threading
 import time
 import warnings
 import weakref
@@ -149,31 +150,34 @@
             index: position of the batch in the PyDataset.
 
         Returns:
             A batch
         """
         raise NotImplementedError
 
-    def __len__(self):
-        """Number of batch in the PyDataset.
+    @property
+    def num_batches(self):
+        """Number of batches in the PyDataset.
 
         Returns:
-            The number of batches in the PyDataset.
+            The number of batches in the PyDataset or `None` to indicate that
+            the dataset is infinite.
         """
-        raise NotImplementedError
+        # For backwards compatibility, support `__len__`.
+        if hasattr(self, "__len__"):
+            return len(self)
+        raise NotImplementedError(
+            "You need to implement the `num_batches` property:\n\n"
+            "@property\ndef num_batches(self):\n  return ..."
+        )
 
     def on_epoch_end(self):
         """Method called at the end of every epoch."""
         pass
 
-    def __iter__(self):
-        """Create a generator that iterate over the PyDataset."""
-        for i in range(len(self)):
-            yield self[i]
-
 
 class PyDatasetAdapter(DataAdapter):
     """Adapter for `keras.utils.PyDataset` instances."""
 
     def __init__(
         self,
         x,
@@ -230,73 +234,83 @@
                     max_queue_size=self.py_dataset.max_queue_size,
                 )
                 return self.enqueuer.get()
 
         else:
 
             def generator_fn():
-                order = range(len(self.py_dataset))
-                if self.shuffle:
+                num_batches = self.py_dataset.num_batches
+                indices = (
+                    range(num_batches)
+                    if num_batches is not None
+                    else itertools.count()
+                )
+                if self.shuffle and num_batches is not None:
                     # Match the shuffle convention in OrderedEnqueuer.
-                    order = list(order)
-                    random.shuffle(order)
+                    indices = list(indices)
+                    random.shuffle(indices)
 
-                for i in order:
+                for i in indices:
                     yield self.py_dataset[i]
 
         return generator_fn
 
     def _get_iterator(self):
+        num_batches = self.py_dataset.num_batches
         gen_fn = self._make_multiprocessed_generator_fn()
         for i, batch in enumerate(gen_fn()):
             batch = self._standardize_batch(batch)
             yield batch
-            if i >= len(self.py_dataset) - 1 and self.enqueuer:
+            if (
+                self.enqueuer
+                and num_batches is not None
+                and i >= num_batches - 1
+            ):
                 self.enqueuer.stop()
 
     def get_numpy_iterator(self):
         return data_adapter_utils.get_numpy_iterator(self._get_iterator())
 
     def get_jax_iterator(self):
         return data_adapter_utils.get_jax_iterator(self._get_iterator())
 
     def get_tf_dataset(self):
         from keras.src.utils.module_utils import tensorflow as tf
 
+        num_batches = self.py_dataset.num_batches
         if self._output_signature is None:
-            num_samples = min(
-                data_adapter_utils.NUM_BATCHES_FOR_TENSOR_SPEC,
-                len(self.py_dataset),
-            )
+            num_samples = data_adapter_utils.NUM_BATCHES_FOR_TENSOR_SPEC
+            if num_batches is not None:
+                num_samples = min(num_samples, num_batches)
             batches = [
                 self._standardize_batch(self.py_dataset[i])
                 for i in range(num_samples)
             ]
             self._output_signature = data_adapter_utils.get_tensor_spec(batches)
 
         ds = tf.data.Dataset.from_generator(
             self._get_iterator,
             output_signature=self._output_signature,
         )
-        if self.shuffle:
+        if self.shuffle and num_batches is not None:
             ds = ds.shuffle(8)
         ds = ds.prefetch(tf.data.AUTOTUNE)
         return ds
 
     def get_torch_dataloader(self):
         return data_adapter_utils.get_torch_dataloader(self._get_iterator())
 
     def on_epoch_end(self):
         if self.enqueuer:
             self.enqueuer.stop()
         self.py_dataset.on_epoch_end()
 
     @property
     def num_batches(self):
-        return len(self.py_dataset)
+        return self.py_dataset.num_batches
 
     @property
     def batch_size(self):
         return None
 
 
 # Global variables to be shared across processes
@@ -324,19 +338,14 @@
     """Lazily create the queue to track worker ids."""
     global _WORKER_ID_QUEUE
     if _WORKER_ID_QUEUE is None:
         _WORKER_ID_QUEUE = multiprocessing.Queue()
     return _WORKER_ID_QUEUE
 
 
-def init_pool(seqs):
-    global _SHARED_SEQUENCES
-    _SHARED_SEQUENCES = seqs
-
-
 def get_index(uid, i):
     """Get the value from the PyDataset `uid` at index `i`.
 
     To allow multiple PyDatasets to be used at the same time, we use `uid` to
     get a specific one. A single PyDataset would cause the validation to
     overwrite the training PyDataset.
 
@@ -516,53 +525,65 @@
         while True:
             time.sleep(0.1)
             if self.queue.unfinished_tasks == 0 or self.stop_signal.is_set():
                 return
 
     def _run(self):
         """Submits request to the executor and queue the `Future` objects."""
-        indices = list(range(len(self.py_dataset)))
-        if self.shuffle:
-            random.shuffle(indices)
-        self._send_py_dataset()  # Share the initial py_dataset
-        while True:
-            with closing(self.executor_fn(_SHARED_SEQUENCES)) as executor:
-                for i in indices:
+        try:
+            num_batches = self.py_dataset.num_batches
+            indices = (
+                range(num_batches)
+                if num_batches is not None
+                else itertools.count()
+            )
+            if self.shuffle and num_batches is not None:
+                indices = list(indices)
+                random.shuffle(indices)
+            self._send_py_dataset()  # Share the initial py_dataset
+            while True:
+                with closing(self.executor_fn(_SHARED_SEQUENCES)) as executor:
+                    for i in indices:
+                        if self.stop_signal.is_set():
+                            return
+
+                        self.queue.put(
+                            executor.apply_async(get_index, (self.uid, i)),
+                            block=True,
+                        )
+
+                    # Done with the current epoch, waiting for the final batches
+                    self._wait_queue()
+
                     if self.stop_signal.is_set():
+                        # We're done
                         return
 
-                    self.queue.put(
-                        executor.apply_async(get_index, (self.uid, i)),
-                        block=True,
-                    )
-
-                # Done with the current epoch, waiting for the final batches
-                self._wait_queue()
-
-                if self.stop_signal.is_set():
-                    # We're done
-                    return
-
-            # Call the internal on epoch end.
-            self.py_dataset.on_epoch_end()
-            self._send_py_dataset()  # Update the pool
+                # Call the internal on epoch end.
+                self.py_dataset.on_epoch_end()
+                self._send_py_dataset()  # Update the pool
+        except Exception as e:
+            self.queue.put(e)  # Report exception
 
     def get(self):
         """Creates a generator to extract data from the queue.
 
         Skip the data if it is `None`.
 
         Yields:
             The next element in the queue, i.e. a tuple
             `(inputs, targets)` or
             `(inputs, targets, sample_weights)`.
         """
         while self.is_running():
             try:
-                inputs = self.queue.get(block=True, timeout=5).get()
+                value = self.queue.get(block=True, timeout=5)
+                if isinstance(value, Exception):
+                    raise value  # Propagate exception from other thread
+                inputs = value.get()
                 if self.is_running():
                     self.queue.task_done()
                 if inputs is not None:
                     yield inputs
             except queue.Empty:
                 pass
             except Exception as e:
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/trainers/trainer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/tree/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/tree/tree_api.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/__init__.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/audio_dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,31 +405,48 @@
     ragged,
     shuffle=False,
     shuffle_buffer_size=None,
     seed=None,
 ):
     """Constructs a fixed-size dataset of audio and labels."""
     path_ds = tf.data.Dataset.from_tensor_slices(file_paths)
-    if shuffle:
-        path_ds = path_ds.shuffle(
-            buffer_size=shuffle_buffer_size or 1024, seed=seed
+    if label_mode:
+        label_ds = dataset_utils.labels_to_dataset(
+            labels, label_mode, num_classes
         )
+        ds = tf.data.Dataset.zip((path_ds, label_ds))
+    else:
+        ds = path_ds
 
-    audio_ds = path_ds.map(
-        lambda x: read_and_decode_audio(
-            x, sampling_rate, output_sequence_length
-        ),
-        num_parallel_calls=tf.data.AUTOTUNE,
-    )
-
-    if ragged:
-        audio_ds = audio_ds.map(
-            lambda x: tf.RaggedTensor.from_tensor(x),
+    if shuffle:
+        ds = ds.shuffle(buffer_size=shuffle_buffer_size or 1024, seed=seed)
+
+    if label_mode:
+        ds = ds.map(
+            lambda x, y: (
+                read_and_decode_audio(x, sampling_rate, output_sequence_length),
+                y,
+            ),
             num_parallel_calls=tf.data.AUTOTUNE,
         )
 
-    if label_mode:
-        label_ds = dataset_utils.labels_to_dataset(
-            labels, label_mode, num_classes
+        if ragged:
+            ds = ds.map(
+                lambda x, y: (tf.RaggedTensor.from_tensor(x), y),
+                num_parallel_calls=tf.data.AUTOTUNE,
+            )
+
+    else:
+        ds = ds.map(
+            lambda x: read_and_decode_audio(
+                x, sampling_rate, output_sequence_length
+            ),
+            num_parallel_calls=tf.data.AUTOTUNE,
         )
-        audio_ds = tf.data.Dataset.zip((audio_ds, label_ds))
-    return audio_ds
+
+        if ragged:
+            ds = ds.map(
+                lambda x: tf.RaggedTensor.from_tensor(x),
+                num_parallel_calls=tf.data.AUTOTUNE,
+            )
+
+    return ds
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/code_stats.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/file_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/image_dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,38 +363,44 @@
     crop_to_aspect_ratio=False,
     pad_to_aspect_ratio=False,
     shuffle=False,
     shuffle_buffer_size=None,
     seed=None,
 ):
     """Constructs a dataset of images and labels."""
-    # TODO(fchollet): consider making num_parallel_calls settable
     path_ds = tf.data.Dataset.from_tensor_slices(image_paths)
-    if shuffle:
-        path_ds = path_ds.shuffle(
-            buffer_size=shuffle_buffer_size or 1024, seed=seed
+    if label_mode:
+        label_ds = dataset_utils.labels_to_dataset(
+            labels, label_mode, num_classes
         )
+        ds = tf.data.Dataset.zip((path_ds, label_ds))
+    else:
+        ds = path_ds
+
+    if shuffle:
+        ds = ds.shuffle(buffer_size=shuffle_buffer_size or 1024, seed=seed)
 
     args = (
         image_size,
         num_channels,
         interpolation,
         data_format,
         crop_to_aspect_ratio,
         pad_to_aspect_ratio,
     )
-    img_ds = path_ds.map(
-        lambda x: load_image(x, *args), num_parallel_calls=tf.data.AUTOTUNE
-    )
     if label_mode:
-        label_ds = dataset_utils.labels_to_dataset(
-            labels, label_mode, num_classes
+        ds = ds.map(
+            lambda x, y: (load_image(x, *args), y),
+            num_parallel_calls=tf.data.AUTOTUNE,
+        )
+    else:
+        ds = ds.map(
+            lambda x: load_image(x, *args), num_parallel_calls=tf.data.AUTOTUNE
         )
-        img_ds = tf.data.Dataset.zip((img_ds, label_ds))
-    return img_ds
+    return ds
 
 
 def load_image(
     path,
     image_size,
     num_channels,
     interpolation,
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/image_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/io_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/module_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/naming.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/progbar.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/python_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/text_dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,29 +254,36 @@
     max_length,
     shuffle=False,
     shuffle_buffer_size=None,
     seed=None,
 ):
     """Constructs a dataset of text strings and labels."""
     path_ds = tf.data.Dataset.from_tensor_slices(file_paths)
-    if shuffle:
-        path_ds = path_ds.shuffle(
-            buffer_size=shuffle_buffer_size or 1024, seed=seed
-        )
-
-    string_ds = path_ds.map(
-        lambda x: path_to_string_content(x, max_length),
-        num_parallel_calls=tf.data.AUTOTUNE,
-    )
     if label_mode:
         label_ds = dataset_utils.labels_to_dataset(
             labels, label_mode, num_classes
         )
-        string_ds = tf.data.Dataset.zip((string_ds, label_ds))
-    return string_ds
+        ds = tf.data.Dataset.zip((path_ds, label_ds))
+    else:
+        ds = path_ds
+
+    if shuffle:
+        ds = ds.shuffle(buffer_size=shuffle_buffer_size or 1024, seed=seed)
+
+    if label_mode:
+        ds = ds.map(
+            lambda x, y: (path_to_string_content(x, max_length), y),
+            num_parallel_calls=tf.data.AUTOTUNE,
+        )
+    else:
+        ds = ds.map(
+            lambda x: path_to_string_content(x, max_length),
+            num_parallel_calls=tf.data.AUTOTUNE,
+        )
+    return ds
 
 
 def path_to_string_content(path, max_length):
     txt = tf.io.read_file(path)
     if max_length is not None:
         txt = tf.strings.substr(txt, 0, max_length)
     return txt
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras/src/utils/tracking.py` & `keras_nightly-3.3.3.dev2024042703/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.3.dev2024042703/keras_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.2.dev2024042503
+Version: 3.3.3.dev2024042703
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.2.dev2024042503/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.3.dev2024042703/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.2.dev2024042503/setup.py` & `keras_nightly-3.3.3.dev2024042703/setup.py`

 * *Files identical despite different names*

