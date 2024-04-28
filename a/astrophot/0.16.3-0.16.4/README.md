# Comparing `tmp/astrophot-0.16.3.tar.gz` & `tmp/astrophot-0.16.4.tar.gz`

## Comparing `astrophot-0.16.3.tar` & `astrophot-0.16.4.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 astrophot-0.16.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 astrophot-0.16.3/.readthedocs.yaml
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 astrophot-0.16.3/CITATION.cff
--rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 astrophot-0.16.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 astrophot-0.16.3/CONTRIBUTING.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 astrophot-0.16.3/MANIFEST.in
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 astrophot-0.16.3/requirements-dev.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 astrophot-0.16.3/requirements.txt
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/dependabot.yml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/ISSUE_TEMPLATE/refactor-request.md
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/workflows/cd.yaml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/workflows/testing.yaml
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/AP_config.py
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/__main__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/_version.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/base.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/fit.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/image.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/models.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/param.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/__init__.py
--rw-r--r--   0        0        0     6085 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/base.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/gp.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/gradient.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/hmc.py
--rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/iterative.py
--rw-r--r--   0        0        0    22641 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/lm.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/mhmcmc.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/minifit.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/nuts.py
--rw-r--r--   0        0        0    27868 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/oldlm.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/__init__.py
--rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/image_header.py
--rw-r--r--   0        0        0    25543 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/image_object.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/jacobian_image.py
--rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/model_image.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/psf_image.py
--rw-r--r--   0        0        0    24825 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/target_image.py
--rw-r--r--   0        0        0    31910 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/wcs.py
--rw-r--r--   0        0        0    25772 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/window_object.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/__init__.py
--rw-r--r--   0        0        0    17637 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/_model_methods.py
--rw-r--r--   0        0        0    22574 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/_shared_methods.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/airy_psf.py
--rw-r--r--   0        0        0    16918 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/core_model.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/edgeon_model.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/eigen_psf.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/exponential_model.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/flatsky_model.py
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/foureirellipse_model.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/galaxy_model_object.py
--rw-r--r--   0        0        0    12853 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/gaussian_model.py
--rw-r--r--   0        0        0    13220 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/group_model_object.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/group_psf_model.py
--rw-r--r--   0        0        0    18452 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/model_object.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/moffat_model.py
--rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/nuker_model.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/pixelated_psf_model.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/planesky_model.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/point_source.py
--rw-r--r--   0        0        0    12336 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/psf_model_object.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/ray_model.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/relspline_model.py
--rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/sersic_model.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/sky_model_object.py
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/spline_model.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/superellipse_model.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/warp_model.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/wedge_model.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/zernike_model.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/param/__init__.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/param/base.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/param/param_context.py
--rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/param/parameter.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/parse_config/__init__.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/parse_config/basic_config.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/parse_config/galfit_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/parse_config/shared_methods.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/__init__.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/diagnostic.py
--rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/image.py
--rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/profile.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/shared_elements.py
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/visuals.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/__init__.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/angle_operations.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/decorators.py
--rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/interpolate.py
--rw-r--r--   0        0        0     9067 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/operations.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/optimization.py
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/parametric_profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/__init__.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/coordinates.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/dict_to_hdf5.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/functions.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/optimization.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/units.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/__init__.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/center.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/construct_psf.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/initialize.py
--rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/segmentation_map.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/variance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/isophote/__init__.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/isophote/ellipse.py
--rw-r--r--   0        0        0     8423 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/isophote/extract.py
--rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/isophote/integrate.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/Makefile
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/requirements.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/media/AP_logo_favicon.ico
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/_config.yml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/_toc.yml
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/citation.rst
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/configfile_interface.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/contributing.rst
--rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/coordinates.rst
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/getting_started.rst
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/index.rst
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/install.rst
--rw-r--r--   0        0        0    36085 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/license.rst
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/modules.rst
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/troubleshooting.rst
--rw-r--r--   0        0        0    19814 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/AdvancedPSFModels.ipynb
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/BasicPSFModels.ipynb
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/ConstrainedModels.ipynb
--rw-r--r--   0        0        0    18299 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/CustomModels.ipynb
--rw-r--r--   0        0        0    33534 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/FittingMethods.ipynb
--rw-r--r--   0        0        0    27921 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/GettingStarted.ipynb
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/GroupModels.ipynb
--rw-r--r--   0        0        0    23851 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/JointModels.ipynb
--rw-r--r--   0        0        0    53209 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/ModelZoo.ipynb
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/index.rst
--rw-r--r--   0        0        0    86041 2020-02-02 00:00:00.000000 astrophot-0.16.3/media/AP_logo.png
--rw-r--r--   0        0        0    90111 2020-02-02 00:00:00.000000 astrophot-0.16.3/media/AP_logo_white.png
--rw-r--r--   0        0        0    89580 2020-02-02 00:00:00.000000 astrophot-0.16.3/media/AstroPhotModelOrgchart.png
--rw-r--r--   0        0        0    67356 2020-02-02 00:00:00.000000 astrophot-0.16.3/media/groupjointmodels.png
--rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_fit.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_group_models.py
--rw-r--r--   0        0        0    22789 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_image.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_image_header.py
--rw-r--r--   0        0        0    15586 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_image_list.py
--rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_model.py
--rw-r--r--   0        0        0    20550 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_parameter.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_plots.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_psfmodel.py
--rw-r--r--   0        0        0    18920 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_utils.py
--rw-r--r--   0        0        0    18903 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_wcs.py
--rw-r--r--   0        0        0    14405 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_window.py
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_window_list.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/utils.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 astrophot-0.16.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 astrophot-0.16.3/LICENSE
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 astrophot-0.16.3/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 astrophot-0.16.3/pyproject.toml
--rw-r--r--   0        0        0    45182 2020-02-02 00:00:00.000000 astrophot-0.16.3/PKG-INFO
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 astrophot-0.16.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 astrophot-0.16.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 astrophot-0.16.4/CITATION.cff
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 astrophot-0.16.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 astrophot-0.16.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 astrophot-0.16.4/MANIFEST.in
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 astrophot-0.16.4/requirements-dev.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 astrophot-0.16.4/requirements.txt
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 astrophot-0.16.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 astrophot-0.16.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 astrophot-0.16.4/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 astrophot-0.16.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 astrophot-0.16.4/.github/ISSUE_TEMPLATE/refactor-request.md
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 astrophot-0.16.4/.github/workflows/cd.yaml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 astrophot-0.16.4/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 astrophot-0.16.4/.github/workflows/testing.yaml
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/AP_config.py
+-rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/__main__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/_version.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/errors/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/errors/base.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/errors/fit.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/errors/image.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/errors/models.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/errors/param.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/__init__.py
+-rw-r--r--   0        0        0     6085 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/base.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/gp.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/gradient.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/hmc.py
+-rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/iterative.py
+-rw-r--r--   0        0        0    22641 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/lm.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/mhmcmc.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/minifit.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/nuts.py
+-rw-r--r--   0        0        0    27868 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/fit/oldlm.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/__init__.py
+-rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/image_header.py
+-rw-r--r--   0        0        0    25543 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/image_object.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/jacobian_image.py
+-rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/model_image.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/psf_image.py
+-rw-r--r--   0        0        0    24825 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/target_image.py
+-rw-r--r--   0        0        0    31910 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/wcs.py
+-rw-r--r--   0        0        0    25772 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/image/window_object.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/__init__.py
+-rw-r--r--   0        0        0    17637 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/_model_methods.py
+-rw-r--r--   0        0        0    22574 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/_shared_methods.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/airy_psf.py
+-rw-r--r--   0        0        0    16918 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/core_model.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/edgeon_model.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/eigen_psf.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/exponential_model.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/flatsky_model.py
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/foureirellipse_model.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/galaxy_model_object.py
+-rw-r--r--   0        0        0    12853 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/gaussian_model.py
+-rw-r--r--   0        0        0    13220 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/group_model_object.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/group_psf_model.py
+-rw-r--r--   0        0        0    18452 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/model_object.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/moffat_model.py
+-rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/nuker_model.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/pixelated_psf_model.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/planesky_model.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/point_source.py
+-rw-r--r--   0        0        0    12336 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/psf_model_object.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/ray_model.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/relspline_model.py
+-rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/sersic_model.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/sky_model_object.py
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/spline_model.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/superellipse_model.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/warp_model.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/wedge_model.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/models/zernike_model.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/param/__init__.py
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/param/base.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/param/param_context.py
+-rw-r--r--   0        0        0    29575 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/param/parameter.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/parse_config/__init__.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/parse_config/basic_config.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/parse_config/galfit_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/parse_config/shared_methods.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/plots/__init__.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/plots/diagnostic.py
+-rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/plots/image.py
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/plots/profile.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/plots/shared_elements.py
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/plots/visuals.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/__init__.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/angle_operations.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/decorators.py
+-rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/interpolate.py
+-rw-r--r--   0        0        0     9067 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/operations.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/optimization.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/parametric_profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/conversions/__init__.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/conversions/coordinates.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/conversions/dict_to_hdf5.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/conversions/functions.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/conversions/optimization.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/conversions/units.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/initialize/__init__.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/initialize/center.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/initialize/construct_psf.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/initialize/initialize.py
+-rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/initialize/segmentation_map.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/initialize/variance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/isophote/__init__.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/isophote/ellipse.py
+-rw-r--r--   0        0        0     8423 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/isophote/extract.py
+-rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 astrophot-0.16.4/astrophot/utils/isophote/integrate.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/Makefile
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/requirements.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/media/AP_logo_favicon.ico
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/_config.yml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/_toc.yml
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/citation.rst
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/configfile_interface.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/contributing.rst
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/coordinates.rst
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/getting_started.rst
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/index.rst
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/install.rst
+-rw-r--r--   0        0        0    36085 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/license.rst
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/modules.rst
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/troubleshooting.rst
+-rw-r--r--   0        0        0    19814 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/AdvancedPSFModels.ipynb
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/BasicPSFModels.ipynb
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/ConstrainedModels.ipynb
+-rw-r--r--   0        0        0    18299 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/CustomModels.ipynb
+-rw-r--r--   0        0        0    33534 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/FittingMethods.ipynb
+-rw-r--r--   0        0        0    27921 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/GettingStarted.ipynb
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/GroupModels.ipynb
+-rw-r--r--   0        0        0    23851 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/JointModels.ipynb
+-rw-r--r--   0        0        0    53209 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/ModelZoo.ipynb
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 astrophot-0.16.4/docs/source/tutorials/index.rst
+-rw-r--r--   0        0        0    86041 2020-02-02 00:00:00.000000 astrophot-0.16.4/media/AP_logo.png
+-rw-r--r--   0        0        0    90111 2020-02-02 00:00:00.000000 astrophot-0.16.4/media/AP_logo_white.png
+-rw-r--r--   0        0        0    89580 2020-02-02 00:00:00.000000 astrophot-0.16.4/media/AstroPhotModelOrgchart.png
+-rw-r--r--   0        0        0    67356 2020-02-02 00:00:00.000000 astrophot-0.16.4/media/groupjointmodels.png
+-rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_fit.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_group_models.py
+-rw-r--r--   0        0        0    22789 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_image.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_image_header.py
+-rw-r--r--   0        0        0    15586 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_image_list.py
+-rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_model.py
+-rw-r--r--   0        0        0    20527 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_parameter.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_plots.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_psfmodel.py
+-rw-r--r--   0        0        0    18920 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_utils.py
+-rw-r--r--   0        0        0    18903 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_wcs.py
+-rw-r--r--   0        0        0    14405 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_window.py
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/test_window_list.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 astrophot-0.16.4/tests/utils.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 astrophot-0.16.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 astrophot-0.16.4/LICENSE
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 astrophot-0.16.4/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 astrophot-0.16.4/pyproject.toml
+-rw-r--r--   0        0        0    45182 2020-02-02 00:00:00.000000 astrophot-0.16.4/PKG-INFO
```

### Comparing `astrophot-0.16.3/.pre-commit-config.yaml` & `astrophot-0.16.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/.readthedocs.yaml` & `astrophot-0.16.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/CITATION.cff` & `astrophot-0.16.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/CODE_OF_CONDUCT.md` & `astrophot-0.16.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/CONTRIBUTING.md` & `astrophot-0.16.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/.github/dependabot.yml` & `astrophot-0.16.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/.github/ISSUE_TEMPLATE/bug_report.md` & `astrophot-0.16.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/.github/ISSUE_TEMPLATE/feature_request.md` & `astrophot-0.16.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/.github/ISSUE_TEMPLATE/refactor-request.md` & `astrophot-0.16.4/.github/ISSUE_TEMPLATE/refactor-request.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/.github/workflows/cd.yaml` & `astrophot-0.16.4/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/.github/workflows/coverage.yaml` & `astrophot-0.16.4/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/.github/workflows/testing.yaml` & `astrophot-0.16.4/.github/workflows/testing.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/AP_config.py` & `astrophot-0.16.4/astrophot/AP_config.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/__init__.py` & `astrophot-0.16.4/astrophot/__init__.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/errors/image.py` & `astrophot-0.16.4/astrophot/errors/image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/__init__.py` & `astrophot-0.16.4/astrophot/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/base.py` & `astrophot-0.16.4/astrophot/fit/base.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/gradient.py` & `astrophot-0.16.4/astrophot/fit/gradient.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/hmc.py` & `astrophot-0.16.4/astrophot/fit/hmc.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/iterative.py` & `astrophot-0.16.4/astrophot/fit/iterative.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/lm.py` & `astrophot-0.16.4/astrophot/fit/lm.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/mhmcmc.py` & `astrophot-0.16.4/astrophot/fit/mhmcmc.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/minifit.py` & `astrophot-0.16.4/astrophot/fit/minifit.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/nuts.py` & `astrophot-0.16.4/astrophot/fit/nuts.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/fit/oldlm.py` & `astrophot-0.16.4/astrophot/fit/oldlm.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/image/image_header.py` & `astrophot-0.16.4/astrophot/image/image_header.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/image/image_object.py` & `astrophot-0.16.4/astrophot/image/image_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/image/jacobian_image.py` & `astrophot-0.16.4/astrophot/image/jacobian_image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/image/model_image.py` & `astrophot-0.16.4/astrophot/image/model_image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/image/psf_image.py` & `astrophot-0.16.4/astrophot/image/psf_image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/image/target_image.py` & `astrophot-0.16.4/astrophot/image/target_image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/image/wcs.py` & `astrophot-0.16.4/astrophot/image/wcs.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/image/window_object.py` & `astrophot-0.16.4/astrophot/image/window_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/__init__.py` & `astrophot-0.16.4/astrophot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/_model_methods.py` & `astrophot-0.16.4/astrophot/models/_model_methods.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/_shared_methods.py` & `astrophot-0.16.4/astrophot/models/_shared_methods.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/airy_psf.py` & `astrophot-0.16.4/astrophot/models/airy_psf.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/core_model.py` & `astrophot-0.16.4/astrophot/models/core_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/edgeon_model.py` & `astrophot-0.16.4/astrophot/models/edgeon_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/eigen_psf.py` & `astrophot-0.16.4/astrophot/models/eigen_psf.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/exponential_model.py` & `astrophot-0.16.4/astrophot/models/exponential_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/flatsky_model.py` & `astrophot-0.16.4/astrophot/models/flatsky_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/foureirellipse_model.py` & `astrophot-0.16.4/astrophot/models/foureirellipse_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/galaxy_model_object.py` & `astrophot-0.16.4/astrophot/models/galaxy_model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/gaussian_model.py` & `astrophot-0.16.4/astrophot/models/gaussian_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/group_model_object.py` & `astrophot-0.16.4/astrophot/models/group_model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/group_psf_model.py` & `astrophot-0.16.4/astrophot/models/group_psf_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/model_object.py` & `astrophot-0.16.4/astrophot/models/model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/moffat_model.py` & `astrophot-0.16.4/astrophot/models/moffat_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/nuker_model.py` & `astrophot-0.16.4/astrophot/models/nuker_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/pixelated_psf_model.py` & `astrophot-0.16.4/astrophot/models/pixelated_psf_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/planesky_model.py` & `astrophot-0.16.4/astrophot/models/planesky_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/point_source.py` & `astrophot-0.16.4/astrophot/models/point_source.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/psf_model_object.py` & `astrophot-0.16.4/astrophot/models/psf_model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/ray_model.py` & `astrophot-0.16.4/astrophot/models/ray_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/relspline_model.py` & `astrophot-0.16.4/astrophot/models/relspline_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/sersic_model.py` & `astrophot-0.16.4/astrophot/models/sersic_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/sky_model_object.py` & `astrophot-0.16.4/astrophot/models/sky_model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/spline_model.py` & `astrophot-0.16.4/astrophot/models/spline_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/superellipse_model.py` & `astrophot-0.16.4/astrophot/models/superellipse_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/warp_model.py` & `astrophot-0.16.4/astrophot/models/warp_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/wedge_model.py` & `astrophot-0.16.4/astrophot/models/wedge_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/models/zernike_model.py` & `astrophot-0.16.4/astrophot/models/zernike_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/param/base.py` & `astrophot-0.16.4/astrophot/param/base.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/param/param_context.py` & `astrophot-0.16.4/astrophot/param/param_context.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/param/parameter.py` & `astrophot-0.16.4/astrophot/param/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,23 +340,23 @@
         one-sided then the transformation: ``newvalue = value - 1 /
         (value - limit)`` is used.
 
         """
         rep = torch.as_tensor(rep, dtype=AP_config.ap_dtype, device=AP_config.ap_device)
         if self.leaf:
             if self.cyclic:
-                val = cyclic_boundaries(rep, (self.limits[0][self.mask], self.limits[1][self.mask]))
+                val = cyclic_boundaries(rep, (self.limits[0], self.limits[1]))
             elif self.limits[0] is None and self.limits[1] is None:
                 val = rep
             else:
                 val = inv_boundaries(
                     rep,
                     (
-                        None if self.limits[0] is None else self.limits[0][self.mask],
-                        None if self.limits[1] is None else self.limits[1][self.mask],
+                        None if self.limits[0] is None else self.limits[0],
+                        None if self.limits[1] is None else self.limits[1],
                     ),
                 )
             return val
 
         mask = self.vector_mask()
         flat = self.flat(include_locked=False, include_links=False)
 
@@ -386,23 +386,23 @@
         one-sided then the transformation: ``newvalue = value - 1 /
         (value - limit)`` is used.
 
         """
         val = torch.as_tensor(val, dtype=AP_config.ap_dtype, device=AP_config.ap_device)
         if self.leaf:
             if self.cyclic:
-                rep = cyclic_boundaries(val, (self.limits[0][self.mask], self.limits[1][self.mask]))
+                rep = cyclic_boundaries(val, (self.limits[0], self.limits[1]))
             elif self.limits[0] is None and self.limits[1] is None:
                 rep = val
             else:
                 rep = boundaries(
                     val,
                     (
-                        None if self.limits[0] is None else self.limits[0][self.mask],
-                        None if self.limits[1] is None else self.limits[1][self.mask],
+                        None if self.limits[0] is None else self.limits[0],
+                        None if self.limits[1] is None else self.limits[1],
                     ),
                 )
             return rep
 
         mask = self.vector_mask()
         flat = self.flat(include_locked=False, include_links=False)
```

### Comparing `astrophot-0.16.3/astrophot/parse_config/basic_config.py` & `astrophot-0.16.4/astrophot/parse_config/basic_config.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/parse_config/galfit_config.py` & `astrophot-0.16.4/astrophot/parse_config/galfit_config.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/plots/diagnostic.py` & `astrophot-0.16.4/astrophot/plots/diagnostic.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/plots/image.py` & `astrophot-0.16.4/astrophot/plots/image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/plots/profile.py` & `astrophot-0.16.4/astrophot/plots/profile.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/plots/shared_elements.py` & `astrophot-0.16.4/astrophot/plots/shared_elements.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/plots/visuals.py` & `astrophot-0.16.4/astrophot/plots/visuals.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/angle_operations.py` & `astrophot-0.16.4/astrophot/utils/angle_operations.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/decorators.py` & `astrophot-0.16.4/astrophot/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/interpolate.py` & `astrophot-0.16.4/astrophot/utils/interpolate.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/operations.py` & `astrophot-0.16.4/astrophot/utils/operations.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/optimization.py` & `astrophot-0.16.4/astrophot/utils/optimization.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/parametric_profiles.py` & `astrophot-0.16.4/astrophot/utils/parametric_profiles.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/conversions/coordinates.py` & `astrophot-0.16.4/astrophot/utils/conversions/coordinates.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/conversions/dict_to_hdf5.py` & `astrophot-0.16.4/astrophot/utils/conversions/dict_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/conversions/functions.py` & `astrophot-0.16.4/astrophot/utils/conversions/functions.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/conversions/optimization.py` & `astrophot-0.16.4/astrophot/utils/conversions/optimization.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/conversions/units.py` & `astrophot-0.16.4/astrophot/utils/conversions/units.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/initialize/__init__.py` & `astrophot-0.16.4/astrophot/utils/initialize/__init__.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/initialize/center.py` & `astrophot-0.16.4/astrophot/utils/initialize/center.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/initialize/construct_psf.py` & `astrophot-0.16.4/astrophot/utils/initialize/construct_psf.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/initialize/initialize.py` & `astrophot-0.16.4/astrophot/utils/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/initialize/segmentation_map.py` & `astrophot-0.16.4/astrophot/utils/initialize/segmentation_map.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/initialize/variance.py` & `astrophot-0.16.4/astrophot/utils/initialize/variance.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/isophote/ellipse.py` & `astrophot-0.16.4/astrophot/utils/isophote/ellipse.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/isophote/extract.py` & `astrophot-0.16.4/astrophot/utils/isophote/extract.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/astrophot/utils/isophote/integrate.py` & `astrophot-0.16.4/astrophot/utils/isophote/integrate.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/Makefile` & `astrophot-0.16.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/media/AP_logo_favicon.ico` & `astrophot-0.16.4/docs/media/AP_logo_favicon.ico`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/_config.yml` & `astrophot-0.16.4/docs/source/_config.yml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/citation.rst` & `astrophot-0.16.4/docs/source/citation.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/configfile_interface.rst` & `astrophot-0.16.4/docs/source/configfile_interface.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/coordinates.rst` & `astrophot-0.16.4/docs/source/coordinates.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/getting_started.rst` & `astrophot-0.16.4/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/index.rst` & `astrophot-0.16.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/install.rst` & `astrophot-0.16.4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/license.rst` & `astrophot-0.16.4/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/troubleshooting.rst` & `astrophot-0.16.4/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/AdvancedPSFModels.ipynb` & `astrophot-0.16.4/docs/source/tutorials/AdvancedPSFModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/BasicPSFModels.ipynb` & `astrophot-0.16.4/docs/source/tutorials/BasicPSFModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/ConstrainedModels.ipynb` & `astrophot-0.16.4/docs/source/tutorials/ConstrainedModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/CustomModels.ipynb` & `astrophot-0.16.4/docs/source/tutorials/CustomModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/FittingMethods.ipynb` & `astrophot-0.16.4/docs/source/tutorials/FittingMethods.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/GettingStarted.ipynb` & `astrophot-0.16.4/docs/source/tutorials/GettingStarted.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/GroupModels.ipynb` & `astrophot-0.16.4/docs/source/tutorials/GroupModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/JointModels.ipynb` & `astrophot-0.16.4/docs/source/tutorials/JointModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/docs/source/tutorials/ModelZoo.ipynb` & `astrophot-0.16.4/docs/source/tutorials/ModelZoo.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/media/AP_logo.png` & `astrophot-0.16.4/media/AP_logo.png`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/media/AP_logo_white.png` & `astrophot-0.16.4/media/AP_logo_white.png`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/media/AstroPhotModelOrgchart.png` & `astrophot-0.16.4/media/AstroPhotModelOrgchart.png`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/media/groupjointmodels.png` & `astrophot-0.16.4/media/groupjointmodels.png`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_fit.py` & `astrophot-0.16.4/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_group_models.py` & `astrophot-0.16.4/tests/test_group_models.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_image.py` & `astrophot-0.16.4/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_image_header.py` & `astrophot-0.16.4/tests/test_image_header.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_image_list.py` & `astrophot-0.16.4/tests/test_image_list.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_model.py` & `astrophot-0.16.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_parameter.py` & `astrophot-0.16.4/tests/test_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,24 +382,24 @@
             "test1", value=0.5, uncertainty=0.3, limits=(-1, 1), locked=False, prof=1.0
         )
         P2 = Parameter_Node("test2", value=2.0, uncertainty=1.0, locked=False)
         P3 = Parameter_Node(
             "test3",
             value=[4.0, 5.0],
             uncertainty=[5.0, 3.0],
-            limits=((0.0, 1.0), None),
+            limits=(1.0, None),
             locked=False,
         )
         P4 = Parameter_Node("test4", value=P2)
         P5 = Parameter_Node("test5", value=lambda P: P["test1"].value ** 2, link=(P1,))
         P6 = Parameter_Node(
             "test6",
             value=((5, 6), (7, 8)),
             uncertainty=0.1 * np.zeros((2, 2)),
-            limits=(None, 10 * np.ones((2, 2))),
+            limits=(None, 10.0),
         )
         PG = Parameter_Node("testgroup", link=(P1, P2, P3, P4, P5, P6))
 
         mask = torch.tensor([1, 1, 0, 1, 0, 1, 0, 1], dtype=torch.bool, device=P1.value.device)
 
         self.assertEqual(
             len(PG.vector_representation()),
```

### Comparing `astrophot-0.16.3/tests/test_plots.py` & `astrophot-0.16.4/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_psfmodel.py` & `astrophot-0.16.4/tests/test_psfmodel.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_utils.py` & `astrophot-0.16.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_wcs.py` & `astrophot-0.16.4/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_window.py` & `astrophot-0.16.4/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/test_window_list.py` & `astrophot-0.16.4/tests/test_window_list.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/tests/utils.py` & `astrophot-0.16.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/LICENSE` & `astrophot-0.16.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/README.md` & `astrophot-0.16.4/README.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/pyproject.toml` & `astrophot-0.16.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.3/PKG-INFO` & `astrophot-0.16.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astrophot
-Version: 0.16.3
+Version: 0.16.4
 Summary: A fast, flexible, automated, and differentiable astronomical image 2D forward modelling tool for precise parallel multi-wavelength photometry.
 Project-URL: Homepage, https://autostronomy.github.io/AstroPhot/
 Project-URL: Documentation, https://autostronomy.github.io/AstroPhot/
 Project-URL: Repository, https://github.com/Autostronomy/AstroPhot
 Project-URL: Issues, https://github.com/Autostronomy/AstroPhot/issues
 Author-email: Connor Stone <connorstone628@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
```

