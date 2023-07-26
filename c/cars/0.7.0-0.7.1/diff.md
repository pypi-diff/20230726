# Comparing `tmp/cars-0.7.0.tar.gz` & `tmp/cars-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/CAMPUS/users/youssefd/Development/cars-master/dist/.tmp-okesd4qt/cars-0.7.0.tar", last modified: Thu Jun 22 09:33:12 2023, max compression
+gzip compressed data, was "/work/softs/rh8/projets/3d/installer/cars/dist/.tmp-puywxr65/cars-0.7.1.tar", last modified: Wed Jul 26 06:52:08 2023, max compression
```

## Comparing `cars-0.7.0.tar` & `cars-0.7.1.tar`

### file list

```diff
@@ -1,227 +1,228 @@
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.493550 cars-0.7.0/
--rw-------   0 youssefd  (7412) campus    (9585)       85 2021-09-29 14:51:03.000000 cars-0.7.0/.coveragerc
--rw-------   0 youssefd  (7412) campus    (9585)     1107 2022-10-07 19:31:52.000000 cars-0.7.0/.gitignore
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.620084 cars-0.7.0/.gitlab/
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.677879 cars-0.7.0/.gitlab/issue_templates/
--rw-------   0 youssefd  (7412) campus    (9585)     1009 2022-10-07 19:31:52.000000 cars-0.7.0/.gitlab/issue_templates/Bug.md
--rw-------   0 youssefd  (7412) campus    (9585)      442 2022-10-07 19:31:52.000000 cars-0.7.0/.gitlab/issue_templates/Proposal.md
--rw-------   0 youssefd  (7412) campus    (9585)     1821 2022-10-07 19:31:52.000000 cars-0.7.0/.gitlab/issue_templates/Refacto.md
--rw-------   0 youssefd  (7412) campus    (9585)      810 2022-10-07 19:31:52.000000 cars-0.7.0/.gitlab/issue_templates/Release.md
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.678789 cars-0.7.0/.gitlab/merge_request_templates/
--rw-------   0 youssefd  (7412) campus    (9585)     2345 2022-10-07 19:31:52.000000 cars-0.7.0/.gitlab/merge_request_templates/MR.md
--rw-------   0 youssefd  (7412) campus    (9585)      864 2023-06-02 19:05:31.000000 cars-0.7.0/.pre-commit-config.yaml
--rw-------   0 youssefd  (7412) campus    (9585)    16149 2023-06-05 15:54:23.000000 cars-0.7.0/.pylintrc
--rw-------   0 youssefd  (7412) campus    (9585)      510 2023-03-23 12:49:31.000000 cars-0.7.0/.readthedocs.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     1719 2023-06-20 07:07:34.000000 cars-0.7.0/AUTHORS.md
--rw-------   0 youssefd  (7412) campus    (9585)     8444 2023-06-20 12:46:58.000000 cars-0.7.0/CHANGELOG.md
--rw-------   0 youssefd  (7412) campus    (9585)     4509 2023-03-10 14:58:43.000000 cars-0.7.0/CONTRIBUTING.md
--rw-------   0 youssefd  (7412) campus    (9585)      907 2023-01-02 09:39:32.000000 cars-0.7.0/Dockerfile
--rw-------   0 youssefd  (7412) campus    (9585)     4039 2023-06-20 07:07:34.000000 cars-0.7.0/Dockerfile.deps
--rw-------   0 youssefd  (7412) campus    (9585)      547 2022-11-24 15:16:29.000000 cars-0.7.0/Dockerfile.jupyter
--rw-------   0 youssefd  (7412) campus    (9585)      384 2022-11-24 15:16:29.000000 cars-0.7.0/Dockerfile.tutorial
--rw-------   0 youssefd  (7412) campus    (9585)    11358 2020-12-16 10:57:27.000000 cars-0.7.0/LICENSE
--rw-------   0 youssefd  (7412) campus    (9585)       38 2023-06-07 07:59:03.000000 cars-0.7.0/MANIFEST.in
--rw-------   0 youssefd  (7412) campus    (9585)    16061 2023-06-07 07:59:03.000000 cars-0.7.0/Makefile
--rw-------   0 youssefd  (7412) campus    (9585)     5750 2022-10-07 19:31:52.000000 cars-0.7.0/NOTICE
--rw-------   0 youssefd  (7412) campus    (9585)     5997 2023-06-22 09:33:12.493945 cars-0.7.0/PKG-INFO
--rw-------   0 youssefd  (7412) campus    (9585)     4936 2023-06-07 07:59:03.000000 cars-0.7.0/README.md
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.688153 cars-0.7.0/cars/
--rw-------   0 youssefd  (7412) campus    (9585)     1026 2022-10-07 19:31:52.000000 cars-0.7.0/cars/__init__.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.709047 cars-0.7.0/cars/applications/
--rw-------   0 youssefd  (7412) campus    (9585)     1819 2023-06-07 07:59:03.000000 cars-0.7.0/cars/applications/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     2999 2022-11-30 10:16:57.000000 cars-0.7.0/cars/applications/application.py
--rw-------   0 youssefd  (7412) campus    (9585)      830 2022-10-07 19:31:52.000000 cars-0.7.0/cars/applications/application_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)     2478 2022-11-30 17:19:59.000000 cars-0.7.0/cars/applications/application_template.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.718425 cars-0.7.0/cars/applications/dense_matches_filling/
--rw-------   0 youssefd  (7412) campus    (9585)      935 2023-03-30 16:01:54.000000 cars-0.7.0/cars/applications/dense_matches_filling/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     7204 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/dense_matches_filling/dense_matches_filling.py
--rw-------   0 youssefd  (7412) campus    (9585)     1300 2023-02-22 08:13:12.000000 cars-0.7.0/cars/applications/dense_matches_filling/fill_disp_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    26358 2023-03-30 16:01:54.000000 cars-0.7.0/cars/applications/dense_matches_filling/fill_disp_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    18341 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/dense_matches_filling/plane.py
--rw-------   0 youssefd  (7412) campus    (9585)     8914 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/dense_matches_filling/zero_padding.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.724997 cars-0.7.0/cars/applications/dense_matching/
--rw-------   0 youssefd  (7412) campus    (9585)      898 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/dense_matching/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    21477 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/dense_matching/census_mccnn_sgm.py
--rw-------   0 youssefd  (7412) campus    (9585)     6258 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/dense_matching/dense_matching.py
--rw-------   0 youssefd  (7412) campus    (9585)     2610 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/dense_matching/dense_matching_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    17411 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/dense_matching/dense_matching_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.730773 cars-0.7.0/cars/applications/dense_matching/loaders/
--rw-------   0 youssefd  (7412) campus    (9585)      770 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/dense_matching/loaders/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)      964 2023-03-30 16:01:54.000000 cars-0.7.0/cars/applications/dense_matching/loaders/config_census_sgm.json
--rw-------   0 youssefd  (7412) campus    (9585)      881 2023-03-30 16:01:54.000000 cars-0.7.0/cars/applications/dense_matching/loaders/config_mccnn.json
--rw-------   0 youssefd  (7412) campus    (9585)     8193 2023-03-30 16:01:54.000000 cars-0.7.0/cars/applications/dense_matching/loaders/pandora_loader.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.738832 cars-0.7.0/cars/applications/grid_generation/
--rw-------   0 youssefd  (7412) campus    (9585)      905 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/grid_generation/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    10415 2023-06-20 12:46:58.000000 cars-0.7.0/cars/applications/grid_generation/epipolar_grid_generation.py
--rw-------   0 youssefd  (7412) campus    (9585)     1503 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/grid_generation/grid_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    16110 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/grid_generation/grid_correction.py
--rw-------   0 youssefd  (7412) campus    (9585)     3949 2023-01-02 09:39:32.000000 cars-0.7.0/cars/applications/grid_generation/grid_generation.py
--rw-------   0 youssefd  (7412) campus    (9585)     9461 2023-06-05 15:54:23.000000 cars-0.7.0/cars/applications/grid_generation/grids.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.746900 cars-0.7.0/cars/applications/holes_detection/
--rw-------   0 youssefd  (7412) campus    (9585)      894 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/holes_detection/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    10712 2023-03-30 16:01:54.000000 cars-0.7.0/cars/applications/holes_detection/cloud_to_bbox.py
--rw-------   0 youssefd  (7412) campus    (9585)     4011 2023-01-02 09:39:32.000000 cars-0.7.0/cars/applications/holes_detection/holes_detection.py
--rw-------   0 youssefd  (7412) campus    (9585)     5512 2023-04-19 14:45:10.000000 cars-0.7.0/cars/applications/holes_detection/holes_detection_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.754496 cars-0.7.0/cars/applications/point_cloud_fusion/
--rw-------   0 youssefd  (7412) campus    (9585)      924 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/point_cloud_fusion/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     1078 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/point_cloud_fusion/cloud_fusion_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    18953 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py
--rw-------   0 youssefd  (7412) campus    (9585)    30076 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/point_cloud_fusion/pc_tif_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)     3950 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/point_cloud_fusion/point_cloud_fusion.py
--rw-------   0 youssefd  (7412) campus    (9585)    35071 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/point_cloud_fusion/point_cloud_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.027009 cars-0.7.0/cars/applications/point_cloud_outliers_removing/
--rw-------   0 youssefd  (7412) campus    (9585)      957 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/point_cloud_outliers_removing/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    14832 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/point_cloud_outliers_removing/outlier_removing_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)     6413 2023-03-10 14:57:02.000000 cars-0.7.0/cars/applications/point_cloud_outliers_removing/pc_out_removing.py
--rw-------   0 youssefd  (7412) campus    (9585)     1298 2022-11-30 17:19:59.000000 cars-0.7.0/cars/applications/point_cloud_outliers_removing/points_removing_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    14034 2023-06-20 12:46:58.000000 cars-0.7.0/cars/applications/point_cloud_outliers_removing/small_components.py
--rw-------   0 youssefd  (7412) campus    (9585)    12600 2023-06-20 12:46:58.000000 cars-0.7.0/cars/applications/point_cloud_outliers_removing/statistical.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.034635 cars-0.7.0/cars/applications/rasterization/
--rw-------   0 youssefd  (7412) campus    (9585)      925 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/rasterization/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     4805 2023-03-10 14:57:02.000000 cars-0.7.0/cars/applications/rasterization/point_cloud_rasterization.py
--rw-------   0 youssefd  (7412) campus    (9585)     1305 2023-03-21 16:35:08.000000 cars-0.7.0/cars/applications/rasterization/rasterization_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    18268 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/rasterization/rasterization_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    23161 2023-06-20 12:46:58.000000 cars-0.7.0/cars/applications/rasterization/simple_gaussian.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.042777 cars-0.7.0/cars/applications/resampling/
--rw-------   0 youssefd  (7412) campus    (9585)      885 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/resampling/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    31038 2023-06-20 12:46:58.000000 cars-0.7.0/cars/applications/resampling/bicubic_resampling.py
--rw-------   0 youssefd  (7412) campus    (9585)     4399 2023-01-02 09:39:32.000000 cars-0.7.0/cars/applications/resampling/resampling.py
--rw-------   0 youssefd  (7412) campus    (9585)      906 2022-11-30 17:19:59.000000 cars-0.7.0/cars/applications/resampling/resampling_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    12931 2023-06-20 12:42:56.000000 cars-0.7.0/cars/applications/resampling/resampling_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.048892 cars-0.7.0/cars/applications/sparse_matching/
--rw-------   0 youssefd  (7412) campus    (9585)      883 2022-12-02 15:26:27.000000 cars-0.7.0/cars/applications/sparse_matching/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    28570 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/sparse_matching/sift.py
--rw-------   0 youssefd  (7412) campus    (9585)     5113 2023-01-02 09:39:32.000000 cars-0.7.0/cars/applications/sparse_matching/sparse_matching.py
--rw-------   0 youssefd  (7412) campus    (9585)     2281 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/sparse_matching/sparse_matching_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    15407 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/sparse_matching/sparse_matching_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.055143 cars-0.7.0/cars/applications/triangulation/
--rw-------   0 youssefd  (7412) campus    (9585)      944 2022-10-07 19:31:52.000000 cars-0.7.0/cars/applications/triangulation/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    22170 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/triangulation/line_of_sight_intersection.py
--rw-------   0 youssefd  (7412) campus    (9585)     4898 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/triangulation/triangulation.py
--rw-------   0 youssefd  (7412) campus    (9585)     1047 2022-11-30 17:19:59.000000 cars-0.7.0/cars/applications/triangulation/triangulation_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    14267 2023-06-20 07:07:34.000000 cars-0.7.0/cars/applications/triangulation/triangulation_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)     6332 2023-06-20 12:46:58.000000 cars-0.7.0/cars/cars.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.058649 cars-0.7.0/cars/conf/
--rw-------   0 youssefd  (7412) campus    (9585)      754 2021-09-29 14:51:03.000000 cars-0.7.0/cars/conf/__init__.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.213957 cars-0.7.0/cars/conf/geoid/
--rw-------   0 youssefd  (7412) campus    (9585)  4155868 2021-09-29 14:51:03.000000 cars-0.7.0/cars/conf/geoid/egm96.grd
--rw-------   0 youssefd  (7412) campus    (9585)      454 2022-10-07 19:31:52.000000 cars-0.7.0/cars/conf/geoid/egm96.grd.hdr
--rw-------   0 youssefd  (7412) campus    (9585)     5042 2023-06-20 07:07:34.000000 cars-0.7.0/cars/conf/input_parameters.py
--rw-------   0 youssefd  (7412) campus    (9585)     1010 2023-02-22 08:13:12.000000 cars-0.7.0/cars/conf/mask_cst.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.255679 cars-0.7.0/cars/core/
--rw-------   0 youssefd  (7412) campus    (9585)      754 2021-09-29 14:51:03.000000 cars-0.7.0/cars/core/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     5536 2023-06-20 12:46:58.000000 cars-0.7.0/cars/core/cars_logging.py
--rw-------   0 youssefd  (7412) campus    (9585)     2654 2023-06-05 15:54:23.000000 cars-0.7.0/cars/core/constants.py
--rw-------   0 youssefd  (7412) campus    (9585)     1269 2023-03-21 16:35:08.000000 cars-0.7.0/cars/core/constants_disparity.py
--rw-------   0 youssefd  (7412) campus    (9585)     4504 2023-06-05 15:54:23.000000 cars-0.7.0/cars/core/datasets.py
--rw-------   0 youssefd  (7412) campus    (9585)     3210 2022-10-07 19:31:52.000000 cars-0.7.0/cars/core/former_confs_utils.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.260838 cars-0.7.0/cars/core/geometry/
--rw-------   0 youssefd  (7412) campus    (9585)    19087 2023-06-20 07:07:34.000000 cars-0.7.0/cars/core/geometry/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    18175 2023-06-20 07:07:34.000000 cars-0.7.0/cars/core/geometry/otb_geometry.py
--rw-------   0 youssefd  (7412) campus    (9585)    14269 2023-06-05 15:54:23.000000 cars-0.7.0/cars/core/geometry/shareloc_geometry.py
--rw-------   0 youssefd  (7412) campus    (9585)     7404 2023-06-20 07:07:34.000000 cars-0.7.0/cars/core/inputs.py
--rw-------   0 youssefd  (7412) campus    (9585)     3476 2023-06-20 07:07:34.000000 cars-0.7.0/cars/core/otb_adapters.py
--rw-------   0 youssefd  (7412) campus    (9585)     5662 2023-06-05 15:54:23.000000 cars-0.7.0/cars/core/outputs.py
--rw-------   0 youssefd  (7412) campus    (9585)    27094 2023-06-05 15:54:23.000000 cars-0.7.0/cars/core/preprocessing.py
--rw-------   0 youssefd  (7412) campus    (9585)    30353 2023-06-07 07:59:03.000000 cars-0.7.0/cars/core/projection.py
--rw-------   0 youssefd  (7412) campus    (9585)     5096 2023-03-02 09:45:46.000000 cars-0.7.0/cars/core/roi_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    22683 2023-06-20 07:07:34.000000 cars-0.7.0/cars/core/tiling.py
--rw-------   0 youssefd  (7412) campus    (9585)     4944 2022-11-22 10:23:47.000000 cars-0.7.0/cars/core/utils.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.271648 cars-0.7.0/cars/data_structures/
--rw-------   0 youssefd  (7412) campus    (9585)      765 2022-10-07 19:31:52.000000 cars-0.7.0/cars/data_structures/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    40155 2023-06-20 07:07:34.000000 cars-0.7.0/cars/data_structures/cars_dataset.py
--rw-------   0 youssefd  (7412) campus    (9585)     1857 2023-03-10 14:57:03.000000 cars-0.7.0/cars/data_structures/cars_dict.py
--rw-------   0 youssefd  (7412) campus    (9585)     8954 2023-06-05 15:54:23.000000 cars-0.7.0/cars/data_structures/corresponding_tiles_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)     4202 2023-01-02 09:39:32.000000 cars-0.7.0/cars/data_structures/dataframe_converter.py
--rw-------   0 youssefd  (7412) campus    (9585)     5331 2023-01-02 09:39:32.000000 cars-0.7.0/cars/data_structures/format_transformation.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.276394 cars-0.7.0/cars/orchestrator/
--rw-------   0 youssefd  (7412) campus    (9585)      762 2022-10-07 19:31:52.000000 cars-0.7.0/cars/orchestrator/__init__.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.290753 cars-0.7.0/cars/orchestrator/cluster/
--rw-------   0 youssefd  (7412) campus    (9585)      997 2023-03-21 16:35:08.000000 cars-0.7.0/cars/orchestrator/cluster/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     7191 2023-06-20 07:07:34.000000 cars-0.7.0/cars/orchestrator/cluster/abstract_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)    12173 2023-06-20 07:07:34.000000 cars-0.7.0/cars/orchestrator/cluster/abstract_dask_cluster.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.296789 cars-0.7.0/cars/orchestrator/cluster/dask_config/
--rw-------   0 youssefd  (7412) campus    (9585)     7009 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/README.md
--rw-------   0 youssefd  (7412) campus    (9585)     1016 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/dask.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     3120 2023-06-20 07:07:34.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/distributed.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     1427 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/jobqueue.yaml
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.305560 cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/
--rw-------   0 youssefd  (7412) campus    (9585)     4711 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml
--rw-------   0 youssefd  (7412) campus    (9585)      989 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml
--rw-------   0 youssefd  (7412) campus    (9585)    38310 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml
--rw-------   0 youssefd  (7412) campus    (9585)    11637 2023-02-22 08:13:13.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/distributed.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     7566 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/jobqueue.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     2619 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/local_dask_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)     8632 2023-06-20 12:46:58.000000 cars-0.7.0/cars/orchestrator/cluster/log_wrapper.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.314254 cars-0.7.0/cars/orchestrator/cluster/mp_cluster/
--rw-------   0 youssefd  (7412) campus    (9585)      834 2023-03-21 16:35:08.000000 cars-0.7.0/cars/orchestrator/cluster/mp_cluster/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    11870 2023-03-30 16:01:54.000000 cars-0.7.0/cars/orchestrator/cluster/mp_cluster/mp_factorizer.py
--rw-------   0 youssefd  (7412) campus    (9585)     7547 2023-06-20 12:46:58.000000 cars-0.7.0/cars/orchestrator/cluster/mp_cluster/mp_objects.py
--rw-------   0 youssefd  (7412) campus    (9585)     1906 2023-03-21 16:35:08.000000 cars-0.7.0/cars/orchestrator/cluster/mp_cluster/mp_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    10308 2023-06-20 12:46:58.000000 cars-0.7.0/cars/orchestrator/cluster/mp_cluster/mp_wrapper.py
--rw-------   0 youssefd  (7412) campus    (9585)    20976 2023-06-20 12:46:58.000000 cars-0.7.0/cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)     9545 2023-06-05 15:54:23.000000 cars-0.7.0/cars/orchestrator/cluster/pbs_dask_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)     3316 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/cluster/sequential_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)    12286 2023-06-20 12:46:58.000000 cars-0.7.0/cars/orchestrator/orchestrator.py
--rw-------   0 youssefd  (7412) campus    (9585)      894 2022-10-07 19:31:52.000000 cars-0.7.0/cars/orchestrator/orchestrator_constants.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.323823 cars-0.7.0/cars/orchestrator/registry/
--rw-------   0 youssefd  (7412) campus    (9585)      758 2022-10-07 19:31:52.000000 cars-0.7.0/cars/orchestrator/registry/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     3740 2022-12-02 15:26:27.000000 cars-0.7.0/cars/orchestrator/registry/abstract_registry.py
--rw-------   0 youssefd  (7412) campus    (9585)     3090 2022-10-07 19:31:52.000000 cars-0.7.0/cars/orchestrator/registry/id_generator.py
--rw-------   0 youssefd  (7412) campus    (9585)     4661 2023-01-02 09:39:32.000000 cars-0.7.0/cars/orchestrator/registry/replacer_registry.py
--rw-------   0 youssefd  (7412) campus    (9585)    11756 2023-06-05 15:54:23.000000 cars-0.7.0/cars/orchestrator/registry/saver_registry.py
--rw-------   0 youssefd  (7412) campus    (9585)     2977 2022-10-07 19:31:52.000000 cars-0.7.0/cars/orchestrator/registry/unseen_registry.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.329855 cars-0.7.0/cars/pipelines/
--rw-------   0 youssefd  (7412) campus    (9585)      973 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/__init__.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.336081 cars-0.7.0/cars/pipelines/conf_pipeline/
--rw-------   0 youssefd  (7412) campus    (9585)      765 2022-11-02 08:44:18.000000 cars-0.7.0/cars/pipelines/conf_pipeline/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)        8 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/conf_pipeline/point_clouds_to_dsm.json
--rw-------   0 youssefd  (7412) campus    (9585)       13 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/conf_pipeline/sensor_to_dense_dsm.json
--rw-------   0 youssefd  (7412) campus    (9585)      158 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/conf_pipeline/sensor_to_pc.json
--rw-------   0 youssefd  (7412) campus    (9585)      223 2023-06-05 15:54:23.000000 cars-0.7.0/cars/pipelines/conf_pipeline/sensor_to_sparse_dsm.json
--rw-------   0 youssefd  (7412) campus    (9585)     3445 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/pipeline.py
--rw-------   0 youssefd  (7412) campus    (9585)      920 2022-11-24 15:16:29.000000 cars-0.7.0/cars/pipelines/pipeline_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)     4330 2023-06-20 12:42:56.000000 cars-0.7.0/cars/pipelines/pipeline_template.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.343379 cars-0.7.0/cars/pipelines/point_clouds_to_dsm/
--rw-------   0 youssefd  (7412) campus    (9585)      892 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/point_clouds_to_dsm/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)      822 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/point_clouds_to_dsm/pc_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)     9678 2023-06-05 15:54:23.000000 cars-0.7.0/cars/pipelines/point_clouds_to_dsm/pc_inputs.py
--rw-------   0 youssefd  (7412) campus    (9585)    12529 2023-06-20 07:07:34.000000 cars-0.7.0/cars/pipelines/point_clouds_to_dsm/point_cloud_to_dsm_pipeline.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.353046 cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/
--rw-------   0 youssefd  (7412) campus    (9585)      893 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     2225 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/dsm_output.py
--rw-------   0 youssefd  (7412) campus    (9585)     1573 2023-06-05 15:54:23.000000 cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/sensor_dense_dsm_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    35334 2023-06-20 12:46:58.000000 cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/sensor_to_dense_dsm_pipeline.py
--rw-------   0 youssefd  (7412) campus    (9585)    14612 2023-06-05 15:54:23.000000 cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/sensors_inputs.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.355960 cars-0.7.0/cars/pipelines/sensor_to_sparse_dsm/
--rw-------   0 youssefd  (7412) campus    (9585)      895 2023-03-10 14:57:03.000000 cars-0.7.0/cars/pipelines/sensor_to_sparse_dsm/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    20353 2023-06-20 07:07:34.000000 cars-0.7.0/cars/pipelines/sensor_to_sparse_dsm/sensor_to_sparse_dsm_pipeline.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:11.699766 cars-0.7.0/cars.egg-info/
--rw-------   0 youssefd  (7412) campus    (9585)     5997 2023-06-22 09:33:05.000000 cars-0.7.0/cars.egg-info/PKG-INFO
--rw-------   0 youssefd  (7412) campus    (9585)     7881 2023-06-22 09:33:11.690868 cars-0.7.0/cars.egg-info/SOURCES.txt
--rw-------   0 youssefd  (7412) campus    (9585)        1 2023-06-22 09:33:05.000000 cars-0.7.0/cars.egg-info/dependency_links.txt
--rw-------   0 youssefd  (7412) campus    (9585)       40 2023-06-22 09:33:05.000000 cars-0.7.0/cars.egg-info/entry_points.txt
--rw-------   0 youssefd  (7412) campus    (9585)      802 2023-06-22 09:33:05.000000 cars-0.7.0/cars.egg-info/requires.txt
--rw-------   0 youssefd  (7412) campus    (9585)       11 2023-06-22 09:33:05.000000 cars-0.7.0/cars.egg-info/top_level.txt
--rwx------   0 youssefd  (7412) campus    (9585)     2254 2023-01-02 09:39:32.000000 cars-0.7.0/env_cars.sh
--rw-------   0 youssefd  (7412) campus    (9585)     2771 2022-10-07 19:31:52.000000 cars-0.7.0/gdal-config
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.358884 cars-0.7.0/otb_remote_module/
--rw-------   0 youssefd  (7412) campus    (9585)      374 2023-03-21 16:35:08.000000 cars-0.7.0/otb_remote_module/CMakeLists.txt
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.364104 cars-0.7.0/otb_remote_module/app/
--rw-------   0 youssefd  (7412) campus    (9585)      368 2023-06-05 15:54:23.000000 cars-0.7.0/otb_remote_module/app/CMakeLists.txt
--rw-------   0 youssefd  (7412) campus    (9585)     7630 2023-02-27 10:57:22.000000 cars-0.7.0/otb_remote_module/app/otbConvertSensorToGeoPointFast.cxx
--rw-------   0 youssefd  (7412) campus    (9585)     7228 2023-02-27 10:57:22.000000 cars-0.7.0/otb_remote_module/app/otbEpipolarTriangulation.cxx
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.487317 cars-0.7.0/otb_remote_module/data/
--rw-------   0 youssefd  (7412) campus    (9585)   323046 2020-12-16 10:57:27.000000 cars-0.7.0/otb_remote_module/data/rectified_ref.tif
--rw-------   0 youssefd  (7412) campus    (9585)    81136 2020-12-16 10:57:27.000000 cars-0.7.0/otb_remote_module/data/rectified_ref_mask.tif
--rw-------   0 youssefd  (7412) campus    (9585)   322610 2020-12-16 10:57:27.000000 cars-0.7.0/otb_remote_module/data/rectified_sec.tif
--rw-------   0 youssefd  (7412) campus    (9585)    75835 2020-12-16 10:57:27.000000 cars-0.7.0/otb_remote_module/data/rectified_sec_mask.tif
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2023-06-22 09:33:12.492272 cars-0.7.0/otb_remote_module/include/
--rw-------   0 youssefd  (7412) campus    (9585)    13784 2023-02-27 10:57:22.000000 cars-0.7.0/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.h
--rw-------   0 youssefd  (7412) campus    (9585)    13094 2023-02-27 10:57:22.000000 cars-0.7.0/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.hxx
--rw-------   0 youssefd  (7412) campus    (9585)      506 2020-12-16 10:57:27.000000 cars-0.7.0/otb_remote_module/otb-module.cmake
--rw-------   0 youssefd  (7412) campus    (9585)      407 2022-10-07 19:31:52.000000 cars-0.7.0/pyproject.toml
--rw-------   0 youssefd  (7412) campus    (9585)      266 2021-09-29 14:51:04.000000 cars-0.7.0/pytest.ini
--rw-------   0 youssefd  (7412) campus    (9585)     3091 2023-06-22 09:33:12.495705 cars-0.7.0/setup.cfg
--rw-------   0 youssefd  (7412) campus    (9585)     1084 2023-06-07 07:59:04.000000 cars-0.7.0/setup.py
--rw-------   0 youssefd  (7412) campus    (9585)     1000 2023-03-10 14:57:04.000000 cars-0.7.0/sonar-project.properties
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.714587 cars-0.7.1/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)       85 2023-07-26 06:48:01.000000 cars-0.7.1/.coveragerc
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1107 2023-07-26 06:48:01.000000 cars-0.7.1/.gitignore
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.204376 cars-0.7.1/.gitlab/
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.271782 cars-0.7.1/.gitlab/issue_templates/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1009 2023-07-26 06:48:01.000000 cars-0.7.1/.gitlab/issue_templates/Bug.md
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      442 2023-07-26 06:48:01.000000 cars-0.7.1/.gitlab/issue_templates/Proposal.md
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1821 2023-07-26 06:48:01.000000 cars-0.7.1/.gitlab/issue_templates/Refacto.md
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      810 2023-07-26 06:48:01.000000 cars-0.7.1/.gitlab/issue_templates/Release.md
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.272331 cars-0.7.1/.gitlab/merge_request_templates/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2345 2023-07-26 06:48:01.000000 cars-0.7.1/.gitlab/merge_request_templates/MR.md
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      864 2023-07-26 06:48:01.000000 cars-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    16149 2023-07-26 06:48:01.000000 cars-0.7.1/.pylintrc
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      510 2023-07-26 06:48:01.000000 cars-0.7.1/.readthedocs.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1719 2023-07-26 06:48:01.000000 cars-0.7.1/AUTHORS.md
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     8837 2023-07-26 06:48:01.000000 cars-0.7.1/CHANGELOG.md
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4509 2023-07-26 06:48:01.000000 cars-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      907 2023-07-26 06:48:01.000000 cars-0.7.1/Dockerfile
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4039 2023-07-26 06:48:01.000000 cars-0.7.1/Dockerfile.deps
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      573 2023-07-26 06:48:01.000000 cars-0.7.1/Dockerfile.jupyter
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    11358 2023-07-26 06:48:01.000000 cars-0.7.1/LICENSE
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)       38 2023-07-26 06:48:01.000000 cars-0.7.1/MANIFEST.in
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    15440 2023-07-26 06:48:01.000000 cars-0.7.1/Makefile
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5750 2023-07-26 06:48:01.000000 cars-0.7.1/NOTICE
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5997 2023-07-26 06:52:08.714925 cars-0.7.1/PKG-INFO
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4936 2023-07-26 06:48:01.000000 cars-0.7.1/README.md
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.273404 cars-0.7.1/cars/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1026 2023-07-26 06:48:01.000000 cars-0.7.1/cars/__init__.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.293314 cars-0.7.1/cars/applications/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1819 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2999 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/application.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      830 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/application_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2478 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/application_template.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.319436 cars-0.7.1/cars/applications/dense_matches_filling/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      935 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matches_filling/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7204 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matches_filling/dense_matches_filling.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1300 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matches_filling/fill_disp_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    26358 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matches_filling/fill_disp_tools.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    18341 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matches_filling/plane.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     8914 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matches_filling/zero_padding.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.334904 cars-0.7.1/cars/applications/dense_matching/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      898 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    23181 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/census_mccnn_sgm.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     6258 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/dense_matching.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2610 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/dense_matching_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    17411 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/dense_matching_tools.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.337589 cars-0.7.1/cars/applications/dense_matching/loaders/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      770 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/loaders/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      964 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/loaders/config_census_sgm.json
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      881 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/loaders/config_mccnn.json
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     8193 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/dense_matching/loaders/pandora_loader.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.362548 cars-0.7.1/cars/applications/grid_generation/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      905 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/grid_generation/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    10826 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/grid_generation/epipolar_grid_generation.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1503 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/grid_generation/grid_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    16110 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/grid_generation/grid_correction.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3949 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/grid_generation/grid_generation.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     9461 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/grid_generation/grids.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.373983 cars-0.7.1/cars/applications/holes_detection/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      894 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/holes_detection/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    11216 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/holes_detection/cloud_to_bbox.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4011 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/holes_detection/holes_detection.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5512 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/holes_detection/holes_detection_tools.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.385924 cars-0.7.1/cars/applications/point_cloud_fusion/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      924 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_fusion/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1078 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_fusion/cloud_fusion_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    18259 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    30623 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_fusion/pc_tif_tools.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3950 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_fusion/point_cloud_fusion.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    35722 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_fusion/point_cloud_tools.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.392604 cars-0.7.1/cars/applications/point_cloud_outliers_removing/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      957 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_outliers_removing/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    14827 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_outliers_removing/outlier_removing_tools.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     6413 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_outliers_removing/pc_out_removing.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1298 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_outliers_removing/points_removing_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    14034 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_outliers_removing/small_components.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    12600 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/point_cloud_outliers_removing/statistical.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.416762 cars-0.7.1/cars/applications/rasterization/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      925 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/rasterization/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4805 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/rasterization/point_cloud_rasterization.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1305 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/rasterization/rasterization_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    20623 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/rasterization/rasterization_tools.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    24331 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/rasterization/simple_gaussian.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.421611 cars-0.7.1/cars/applications/resampling/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      885 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/resampling/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    31038 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/resampling/bicubic_resampling.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4399 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/resampling/resampling.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      906 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/resampling/resampling_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    12931 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/resampling/resampling_tools.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.426076 cars-0.7.1/cars/applications/sparse_matching/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      883 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/sparse_matching/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    28570 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/sparse_matching/sift.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5113 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/sparse_matching/sparse_matching.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2281 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/sparse_matching/sparse_matching_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    15407 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/sparse_matching/sparse_matching_tools.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.451690 cars-0.7.1/cars/applications/triangulation/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      944 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/triangulation/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    22581 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/triangulation/line_of_sight_intersection.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4898 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/triangulation/triangulation.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1047 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/triangulation/triangulation_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    14267 2023-07-26 06:48:01.000000 cars-0.7.1/cars/applications/triangulation/triangulation_tools.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     6332 2023-07-26 06:48:01.000000 cars-0.7.1/cars/cars.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.454187 cars-0.7.1/cars/conf/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      754 2023-07-26 06:48:01.000000 cars-0.7.1/cars/conf/__init__.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.484001 cars-0.7.1/cars/conf/geoid/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)  4155868 2023-07-26 06:48:01.000000 cars-0.7.1/cars/conf/geoid/egm96.grd
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      454 2023-07-26 06:48:01.000000 cars-0.7.1/cars/conf/geoid/egm96.grd.hdr
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5042 2023-07-26 06:48:01.000000 cars-0.7.1/cars/conf/input_parameters.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1010 2023-07-26 06:48:01.000000 cars-0.7.1/cars/conf/mask_cst.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.549118 cars-0.7.1/cars/core/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      754 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5411 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/cars_logging.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2801 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1269 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/constants_disparity.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4504 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/datasets.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3210 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/former_confs_utils.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.555371 cars-0.7.1/cars/core/geometry/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    19087 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/geometry/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    18617 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/geometry/otb_geometry.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    14269 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/geometry/shareloc_geometry.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7404 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/inputs.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3476 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/otb_adapters.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5662 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/outputs.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    27094 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/preprocessing.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    30353 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/projection.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5096 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/roi_tools.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    22826 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/tiling.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4944 2023-07-26 06:48:01.000000 cars-0.7.1/cars/core/utils.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.560478 cars-0.7.1/cars/data_structures/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      765 2023-07-26 06:48:01.000000 cars-0.7.1/cars/data_structures/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    40270 2023-07-26 06:48:01.000000 cars-0.7.1/cars/data_structures/cars_dataset.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1857 2023-07-26 06:48:01.000000 cars-0.7.1/cars/data_structures/cars_dict.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     8954 2023-07-26 06:48:01.000000 cars-0.7.1/cars/data_structures/corresponding_tiles_tools.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4202 2023-07-26 06:48:01.000000 cars-0.7.1/cars/data_structures/dataframe_converter.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5331 2023-07-26 06:48:01.000000 cars-0.7.1/cars/data_structures/format_transformation.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.562990 cars-0.7.1/cars/orchestrator/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      762 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/__init__.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.570295 cars-0.7.1/cars/orchestrator/cluster/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1021 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7191 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/abstract_cluster.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    12173 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/abstract_dask_cluster.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.573383 cars-0.7.1/cars/orchestrator/cluster/dask_config/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7009 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/README.md
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1016 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/dask.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3120 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/distributed.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1427 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/jobqueue.yaml
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.591008 cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4711 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      989 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    38310 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    11637 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/distributed.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7566 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/jobqueue.yaml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     6470 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/dask_jobqueue_utils.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2619 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/local_dask_cluster.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     8632 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/log_wrapper.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.596750 cars-0.7.1/cars/orchestrator/cluster/mp_cluster/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      834 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/mp_cluster/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    11870 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/mp_cluster/mp_factorizer.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7547 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/mp_cluster/mp_objects.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1906 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/mp_cluster/mp_tools.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    10308 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/mp_cluster/mp_wrapper.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    23651 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5359 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/pbs_dask_cluster.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3316 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/sequential_cluster.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5341 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/cluster/slurm_dask_cluster.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    12327 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/orchestrator.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      894 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/orchestrator_constants.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.618855 cars-0.7.1/cars/orchestrator/registry/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      758 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/registry/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3740 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/registry/abstract_registry.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3090 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/registry/id_generator.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4661 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/registry/replacer_registry.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    11756 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/registry/saver_registry.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2977 2023-07-26 06:48:01.000000 cars-0.7.1/cars/orchestrator/registry/unseen_registry.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.621022 cars-0.7.1/cars/pipelines/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      973 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/__init__.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.624194 cars-0.7.1/cars/pipelines/conf_pipeline/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      765 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/conf_pipeline/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)        8 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/conf_pipeline/point_clouds_to_dsm.json
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)       13 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/conf_pipeline/sensor_to_dense_dsm.json
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      158 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/conf_pipeline/sensor_to_pc.json
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      223 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/conf_pipeline/sensor_to_sparse_dsm.json
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3445 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/pipeline.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      920 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/pipeline_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     4207 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/pipeline_template.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.627161 cars-0.7.1/cars/pipelines/point_clouds_to_dsm/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      892 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/point_clouds_to_dsm/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      822 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/point_clouds_to_dsm/pc_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     9678 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/point_clouds_to_dsm/pc_inputs.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    12738 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/point_clouds_to_dsm/point_cloud_to_dsm_pipeline.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.630920 cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      893 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2225 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/dsm_output.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1573 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/sensor_dense_dsm_constants.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    35606 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/sensor_to_dense_dsm_pipeline.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    14612 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/sensors_inputs.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.632764 cars-0.7.1/cars/pipelines/sensor_to_sparse_dsm/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      895 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/sensor_to_sparse_dsm/__init__.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    20577 2023-07-26 06:48:01.000000 cars-0.7.1/cars/pipelines/sensor_to_sparse_dsm/sensor_to_sparse_dsm_pipeline.py
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.291120 cars-0.7.1/cars.egg-info/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     5997 2023-07-26 06:52:04.000000 cars-0.7.1/cars.egg-info/PKG-INFO
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7958 2023-07-26 06:52:08.289068 cars-0.7.1/cars.egg-info/SOURCES.txt
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)        1 2023-07-26 06:52:04.000000 cars-0.7.1/cars.egg-info/dependency_links.txt
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)       40 2023-07-26 06:52:04.000000 cars-0.7.1/cars.egg-info/entry_points.txt
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      808 2023-07-26 06:52:04.000000 cars-0.7.1/cars.egg-info/requires.txt
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)       11 2023-07-26 06:52:04.000000 cars-0.7.1/cars.egg-info/top_level.txt
+-rwxr-xr-x   0 cars_admin  (9833) at3d_admin  (8192)     2254 2023-07-26 06:48:01.000000 cars-0.7.1/env_cars.sh
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     2771 2023-07-26 06:48:01.000000 cars-0.7.1/gdal-config
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.634405 cars-0.7.1/otb_remote_module/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      374 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/CMakeLists.txt
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.636520 cars-0.7.1/otb_remote_module/app/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      368 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/app/CMakeLists.txt
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7630 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/app/otbConvertSensorToGeoPointFast.cxx
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     7228 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/app/otbEpipolarTriangulation.cxx
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.678073 cars-0.7.1/otb_remote_module/data/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)   323046 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/data/rectified_ref.tif
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    81136 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/data/rectified_ref_mask.tif
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)   322610 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/data/rectified_sec.tif
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    75835 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/data/rectified_sec_mask.tif
+drwxr-sr-x   0 cars_admin  (9833) at3d_admin  (8192)        0 2023-07-26 06:52:08.693618 cars-0.7.1/otb_remote_module/include/
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    13784 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.h
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)    13094 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.hxx
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      506 2023-07-26 06:48:01.000000 cars-0.7.1/otb_remote_module/otb-module.cmake
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      407 2023-07-26 06:48:01.000000 cars-0.7.1/pyproject.toml
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)      316 2023-07-26 06:48:01.000000 cars-0.7.1/pytest.ini
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     3091 2023-07-26 06:52:08.716085 cars-0.7.1/setup.cfg
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1084 2023-07-26 06:48:01.000000 cars-0.7.1/setup.py
+-rw-r--r--   0 cars_admin  (9833) at3d_admin  (8192)     1000 2023-07-26 06:48:01.000000 cars-0.7.1/sonar-project.properties
```

### Comparing `cars-0.7.0/.gitignore` & `cars-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/.gitlab/issue_templates/Bug.md` & `cars-0.7.1/.gitlab/issue_templates/Bug.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/.gitlab/issue_templates/Refacto.md` & `cars-0.7.1/.gitlab/issue_templates/Refacto.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/.gitlab/issue_templates/Release.md` & `cars-0.7.1/.gitlab/issue_templates/Release.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/.gitlab/merge_request_templates/MR.md` & `cars-0.7.1/.gitlab/merge_request_templates/MR.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/.pre-commit-config.yaml` & `cars-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/.pylintrc` & `cars-0.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/AUTHORS.md` & `cars-0.7.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/CHANGELOG.md` & `cars-0.7.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # Changelog
 
+
+## 0.7.1 Slurm Cluster (July 2023)
+
+### Added
+- Dask Slurm cluster [#624]
+- Crop disparity range with thresholds [#626]
+- Used source information map generated [#648]
+
+### Changed
+- Write workers logs in one single file [#659]
+- Use tempfile to generate default orchestrator folder instead of /tmp [#663]
+
+### Fixed
+- Cython upgrade bug [#674]
+- Too much used disk memory in MP mode [#632]
+
+
 ## 0.7.0 CARS installable without OTB (June 2023)
 
 ### Added
 - Notebook: add masks and classification options [#615]
 - Option: Set python interpreter to use in PBS Dask Cluster [#611]
 - DensePointCloudToDenseDSM Pipeline: now re-entrance with confidence and classification [#602]
 - Shareloc Geometry plugin is now internal [#618]
```

### Comparing `cars-0.7.0/CONTRIBUTING.md` & `cars-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/Dockerfile` & `cars-0.7.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/Dockerfile.deps` & `cars-0.7.1/Dockerfile.deps`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     libossim-dev=2.9.1-2build3 \
     libtinyxml-dev=2.6.2-4build1 \
     libmuparser-dev=2.2.6.1+dfsg-1build1 \
     libmuparserx-dev=4.0.7+dfsg-3build1 \
     libsvm-dev=3.24+ds-3build1 \
     swig=4.0.1-5build1 \
     libfftw3-dev=3.3.8-2ubuntu1 \
-    openssh-client=1:8.2p1-4ubuntu0.7 \
-    curl=7.68.0-1ubuntu2.18 \
+    openssh-client=1:8.2p1-4ubuntu0.8 \
+    curl=7.68.0-1ubuntu2.19 \
     vim=2:8.1.2269-1ubuntu5.15 \
     nano=4.8-1ubuntu1 \
     && rm -rf /var/lib/apt/lists/*
 
 # install orfeo toolbox
 WORKDIR /opt/otb
 RUN wget -q https://www.orfeo-toolbox.org/packages/archives/OTB/OTB-7.4.1.zip -O /tmp/OTB-7.4.1.zip && \
```

### Comparing `cars-0.7.0/Dockerfile.jupyter` & `cars-0.7.1/Dockerfile.jupyter`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-FROM cnes/cars:0.5.0
+# hadolint ignore=DL3007
+FROM cnes/cars:latest
 LABEL maintainer="CNES"
 
 WORKDIR /cars/tutorials/
 
 # install and Enable rise Jupyter slideshow extension https://rise.readthedocs.io/
 # and Jupyter kernel cars creation
 RUN jupyter-nbextension install rise --py --sys-prefix \
```

### Comparing `cars-0.7.0/LICENSE` & `cars-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/Makefile` & `cars-0.7.1/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
 # Check Docker
 CHECK_DOCKER = $(shell docker -v)
 
 # CARS version from setup.py
 CARS_VERSION = $(shell python3 -c 'from cars import __version__; print(__version__)')
 CARS_VERSION_MIN =$(shell echo ${CARS_VERSION} | cut -d . -f 1,2,3)
-CARS_VERSION_TUTO = 0.5.0
 
 ################ MAKE targets by sections ######################
 
 .PHONY: help
 help: ## this help
 	@echo "      CARS MAKE HELP  LOGLEVEL=${LOGLEVEL}"
 	@echo "  Dependencies: Install OTB and VLFEAT before !"
@@ -75,67 +74,62 @@
 	@cd vlfeat && make MEX=$MATLABROOT/bin/
 	@echo "vlfeat is installed. Please set the following environment variables:"
 	@echo "export VLFEAT_INCLUDE_DIR=${PWD}/vlfeat"
 	@echo "export VLFEAT_LIBRARY_DIR=${PWD}/vlfeat/bin/glnxa64"
 	@echo "export LD_LIBRARY_PATH=${PWD}/vlfeat/bin/glnxa64:$$""LD_LIBRARY_PATH"
 
 .PHONY: otb-remote-module
-otb-remote-module:
+otb-remote-module: ## install remote module otb
 	@[ "${CHECK_CMAKE}" ] || ( echo ">> cmake not found"; exit 1 )
 	@[ "${CHECK_OTB}" ] || ( echo ">> OTB not found"; exit 1 )
 	@[ "${OTB_APPLICATION_PATH}" ] || ( echo ">> OTB_APPLICATION_PATH is not set"; exit 1 )
 	@mkdir -p build
 	@cd build && cmake -DCMAKE_INSTALL_PREFIX=${CARS_VENV} -DOTB_BUILD_MODULE_AS_STANDALONE=ON -DCMAKE_BUILD_TYPE=Release ../otb_remote_module && make install
-	@cp env_cars.sh ${CARS_VENV}/bin/.
 
 .PHONY: install-deps
-install-deps: venv otb-remote-module
-	@[ "${CHECK_NUMPY}" ] ||${CARS_VENV}/bin/python -m pip install --upgrade cython numpy
-	@[ "${CHECK_FIONA}" ] ||${CARS_VENV}/bin/python -m pip install --no-binary fiona fiona
-	@[ "${CHECK_RASTERIO}" ] ||${CARS_VENV}/bin/python -m pip install --no-binary rasterio rasterio
+install-deps: venv ## install python libs
+	@[ "${CHECK_NUMPY}" ] ||${CARS_VENV}/bin/python -m pip install --upgrade "cython<3.0.0" numpy
 	@[ "${CHECK_TBB}" ] ||${CARS_VENV}/bin/python -m pip install tbb==$(TBB_VERSION_SETUP)
 	@[ "${CHECK_NUMBA}" ] ||${CARS_VENV}/bin/python -m pip install --upgrade numba
 	@[ "${CHECK_CYVLFEAT}" ] ||CFLAGS="-I${VLFEAT_INCLUDE_DIR}" LDFLAGS="-L${VLFEAT_LIBRARY_DIR}" ${CARS_VENV}/bin/python -m pip install --no-binary cyvlfeat cyvlfeat
 
+.PHONY: install-deps-gdal
+install-deps-gdal: install-deps ## create an healthy python environment for OTB / GDAL
+	@[ "${CHECK_FIONA}" ] ||${CARS_VENV}/bin/python -m pip install --no-binary fiona fiona
+	@[ "${CHECK_RASTERIO}" ] ||${CARS_VENV}/bin/python -m pip install --no-binary rasterio rasterio
+
 .PHONY: install
-install: install-deps  ## install cars (not editable) with dev, docs, notebook dependencies
+install: install-deps-gdal otb-remote-module ## install cars (not editable) with dev, docs, notebook dependencies
 	@test -f ${CARS_VENV}/bin/cars || ${CARS_VENV}/bin/pip install .[dev,docs,notebook]
 	@test -f .git/hooks/pre-commit || echo "  Install pre-commit hook"
 	@test -f .git/hooks/pre-commit || ${CARS_VENV}/bin/pre-commit install -t pre-commit
 	@test -f .git/hooks/pre-push || ${CARS_VENV}/bin/pre-commit install -t pre-push
 	@echo "CARS ${CARS_VERSION} installed in virtualenv ${CARS_VENV}"
 	@echo "CARS venv usage: source ${CARS_VENV}/bin/activate; source ${CARS_VENV}/bin/env_cars.sh; cars -h"
 
 .PHONY: install-pandora-mccnn
-install-pandora-mccnn: install-deps  ## install cars (not editable) with dev, docs, notebook dependencies
+install-pandora-mccnn: install-deps-gdal otb-remote-module  ## install cars (not editable) with dev, docs, notebook dependencies
 	@test -f ${CARS_VENV}/bin/cars || ${CARS_VENV}/bin/pip install .[dev,docs,notebook,pandora_mccnn]
 	@test -f .git/hooks/pre-commit || echo "  Install pre-commit hook"
 	@test -f .git/hooks/pre-commit || ${CARS_VENV}/bin/pre-commit install -t pre-commit
 	@test -f .git/hooks/pre-push || ${CARS_VENV}/bin/pre-commit install -t pre-push
 	@echo "CARS ${CARS_VERSION} installed in virtualenv ${CARS_VENV}"
 	@echo "CARS venv usage: source ${CARS_VENV}/bin/activate; source ${CARS_VENV}/bin/env_cars.sh; cars -h"
 
 .PHONY: install-dev
-install-dev: install-deps ## install cars in dev editable mode (pip install -e .)
+install-dev: install-deps-gdal otb-remote-module ## install cars in dev editable mode (pip install -e .)
 	@test -f ${CARS_VENV}/bin/cars || ${CARS_VENV}/bin/pip install -e .[dev,docs,notebook]
 	@test -f .git/hooks/pre-commit || echo "  Install pre-commit hook"
 	@test -f .git/hooks/pre-commit || ${CARS_VENV}/bin/pre-commit install -t pre-commit
 	@test -f .git/hooks/pre-push || ${CARS_VENV}/bin/pre-commit install -t pre-push
 	@echo "CARS ${CARS_VERSION} installed in dev mode in virtualenv ${CARS_VENV}"
 	@echo "CARS venv usage: source ${CARS_VENV}/bin/activate; source ${CARS_VENV}/bin/env_cars.sh; cars -h"
 
-.PHONY: install-deps-otb-free
-install-deps-otb-free: venv
-	@[ "${CHECK_NUMPY}" ] ||${CARS_VENV}/bin/python -m pip install --upgrade cython numpy
-	@[ "${CHECK_TBB}" ] ||${CARS_VENV}/bin/python -m pip install tbb==$(TBB_VERSION_SETUP)
-	@[ "${CHECK_NUMBA}" ] ||${CARS_VENV}/bin/python -m pip install --upgrade numba
-	@[ "${CHECK_CYVLFEAT}" ] ||CFLAGS="-I${VLFEAT_INCLUDE_DIR}" LDFLAGS="-L${VLFEAT_LIBRARY_DIR}" ${CARS_VENV}/bin/python -m pip install --no-binary cyvlfeat cyvlfeat
-
 .PHONY: install-dev-otb-free
-install-dev-otb-free: install-deps-otb-free ## install cars in dev editable mode (pip install -e .) without otb
+install-dev-otb-free: install-deps ## install cars in dev editable mode (pip install -e .) without recompiling otb remote modules, rasterio, fiona
 	@test -f ${CARS_VENV}/bin/cars || ${CARS_VENV}/bin/pip install -e .[dev,docs,notebook]
 	@test -f .git/hooks/pre-commit || echo "  Install pre-commit hook"
 	@test -f .git/hooks/pre-commit || ${CARS_VENV}/bin/pre-commit install -t pre-commit
 	@test -f .git/hooks/pre-push || ${CARS_VENV}/bin/pre-commit install -t pre-push
 	@echo "CARS ${CARS_VERSION} installed in dev mode in virtualenv ${CARS_VENV}"
 	@echo "CARS venv usage: source ${CARS_VENV}/bin/activate; cars -h"
 
@@ -162,14 +156,19 @@
 	@${CARS_VENV}/bin/pytest -m "unit_tests" -o log_cli=true -o log_cli_level=${LOGLEVEL}
 
 .PHONY: test-pbs-cluster
 test-pbs-cluster: ## run pbs cluster tests only
 	@echo "Please source ${CARS_VENV}/bin/env_cars.sh before launching tests\n"
 	@${CARS_VENV}/bin/pytest -m "pbs_cluster_tests" -o log_cli=true -o log_cli_level=${LOGLEVEL}
 
+.PHONY: test-slurm-cluster
+test-slurm-cluster: ## run slurm cluster tests only
+	@echo "Please source ${CARS_VENV}/bin/env_cars.sh before launching tests\n"
+	@${CARS_VENV}/bin/pytest -m "slurm_cluster_tests" -o log_cli=true -o log_cli_level=${LOGLEVEL}
+
 .PHONY: test-notebook
 test-notebook: ## run notebook tests only
 	@echo "Please source ${CARS_VENV}/bin/env_cars.sh before launching tests\n"
 	@${CARS_VENV}/bin/pytest -m "notebook_tests" -o log_cli=true -o log_cli_level=${LOGLEVEL}
 
 ## Code quality, linting section
 
@@ -230,15 +229,15 @@
 	@echo " --> After CARS virtualenv activation, please use following command to launch local jupyter notebook to open CARS Notebooks:"
 	@echo "jupyter notebook"
 
 
 # Dev section
 
 .PHONY: dev
-dev: install-dev docs notebook ## Install CARS in dev mode : install-dev, notebook and docs
+dev: install-dev docs notebook ## install CARS in dev mode : install-dev, notebook and docs
 
 ## Docker section
 
 .PHONY: docker-deps
 docker-deps: ## Check and build docker image cnes/cars-deps
 	@@[ "${CHECK_DOCKER}" ] || ( echo ">> docker not found"; exit 1 )
 	@docker pull hadolint/hadolint
@@ -260,36 +259,28 @@
 # Set docker options like --build-arg
 ifndef DOCKER_OPTIONS
 	@docker build -t cnes/cars:${CARS_VERSION_MIN} -t cnes/cars:latest . -f Dockerfile
 else
 	@docker build ${DOCKER_OPTIONS} -t cnes/cars:${CARS_VERSION_MIN} -t cnes/cars:latest . -f Dockerfile
 endif
 
-.PHONY: docker-tuto
-docker-tuto: ## Check and build docker image cnes/cars-jupyter and cnes/tutorials
+.PHONY: docker-jupyter
+docker-jupyter: ## Check and build docker image cnes/cars-jupyter
 	@@[ "${CHECK_DOCKER}" ] || ( echo ">> docker not found"; exit 1 )
 	@docker pull hadolint/hadolint
 	@echo "Check Dockerfile.jupyter with hadolint"
 	@docker run --rm -i hadolint/hadolint < Dockerfile.jupyter
-	@echo "Check Dockerfile.tutorial with hadolint"
-	@docker run --rm -i hadolint/hadolint < Dockerfile.tutorial
 	@echo "Build Docker jupyter notebook image from CARS"
 # Set docker options like --build-arg
 ifndef DOCKER_OPTIONS
-	@docker build -t cnes/cars-jupyter:$(CARS_VERSION_TUTO) -t cnes/cars-jupyter:latest . -f Dockerfile.jupyter
-else
-	@docker build ${DOCKER_OPTIONS} -t cnes/cars-jupyter:$(CARS_VERSION_TUTO) -t cnes/cars-jupyter:latest . -f Dockerfile.jupyter
-endif
-	@echo "Build Docker jupyter tutorial notebook image from CARS"
-# Set docker options like --build-arg
-ifndef DOCKER_OPTIONS
-	@docker build -t cnes/cars-tutorial:$(CARS_VERSION_TUTO) -t cnes/cars-tutorial:latest . -f Dockerfile.tutorial
+	@docker build -t cnes/cars-jupyter:$(CARS_VERSION_MIN) -t cnes/cars-jupyter:latest . -f Dockerfile.jupyter
 else
-	@docker build ${DOCKER_OPTIONS} -t cnes/cars-tutorial:$(CARS_VERSION_TUTO) -t cnes/cars-tutorial:latest . -f Dockerfile.tutorial
+	@docker build ${DOCKER_OPTIONS} -t cnes/cars-jupyter:$(CARS_VERSION_MIN) -t cnes/cars-jupyter:latest . -f Dockerfile.jupyter
 endif
+	@echo "Build Docker jupyter notebook image from CARS"
 
 ## Clean section
 
 .PHONY: clean
 clean: clean-venv clean-build clean-vlfeat clean-precommit clean-pyc clean-test clean-docs clean-notebook clean-dask ## remove all build, test, coverage and Python artifacts
 
 .PHONY: clean-venv
@@ -347,23 +338,21 @@
 	@echo "+ $@"
 	@find . -type d -name "dask-worker-space" -exec rm -fr {} +
 
 
 .PHONY: clean-docker
 clean-docker: ## clean docker image
 	@@[ "${CHECK_DOCKER}" ] || ( echo ">> docker not found"; exit 1 )
-	@echo "Clean Docker images cars-deps, cars ${CARS_VERSION_MIN} + cars-jupyter, cars-tutorial $(CARS_VERSION_TUTO)"
+	@echo "Clean Docker images cars-deps, cars, cars-jupyter ${CARS_VERSION_MIN}"
 	@docker image rm -f cnes/cars-deps:${CARS_VERSION_MIN}
 	@docker image rm -f cnes/cars-deps:latest
 	@docker image rm -f cnes/cars:${CARS_VERSION_MIN}
 	@docker image rm -f cnes/cars:latest
-	@docker image rm -f cnes/cars-jupyter:${CARS_VERSION_TUTO}
+	@docker image rm -f cnes/cars-jupyter:${CARS_VERSION_MIN}
 	@docker image rm -f cnes/cars-jupyter:latest
-	@docker image rm -f cnes/cars-tutorial:${CARS_VERSION_TUTO}
-	@docker image rm -f cnes/cars-tutorial:latest
 
 .PHONY: clean-vlfeat
 clean-vlfeat:
 	@echo "+ $@"
 	@rm -rf vlfeat
 
 .PHONY: profile-memory-report
```

### Comparing `cars-0.7.0/NOTICE` & `cars-0.7.1/NOTICE`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/PKG-INFO` & `cars-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cars
-Version: 0.7.0
+Version: 0.7.1
 Summary: A satellite multi view stereo pipeline
 Home-page: https://cars.readthedocs.io/
 Author: CNES
 Author-email: cars@cnes.fr
 License: Apache License 2.0
 Project-URL: Source, https://github.com/CNES/cars
 Project-URL: Documentation, https://cars.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cars Version: 0.7.0 Summary: A satellite multi view
+Metadata-Version: 2.1 Name: cars Version: 0.7.1 Summary: A satellite multi view
 stereo pipeline Home-page: https://cars.readthedocs.io/ Author: CNES Author-
 email: cars@cnes.fr License: Apache License 2.0 Project-URL: Source, https://
 github.com/CNES/cars Project-URL: Documentation, https://cars.readthedocs.io/
 en/latest/ Keywords: cars,3D,DEM,pandora,photogrammetry Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 Intended Audience :: Science/Research Classifier: Environment :: Console
```

### Comparing `cars-0.7.0/README.md` & `cars-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/__init__.py` & `cars-0.7.1/cars/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/__init__.py` & `cars-0.7.1/cars/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/application.py` & `cars-0.7.1/cars/applications/application.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/application_constants.py` & `cars-0.7.1/cars/applications/application_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/application_template.py` & `cars-0.7.1/cars/applications/application_template.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matches_filling/__init__.py` & `cars-0.7.1/cars/applications/dense_matches_filling/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matches_filling/dense_matches_filling.py` & `cars-0.7.1/cars/applications/dense_matches_filling/dense_matches_filling.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matches_filling/fill_disp_constants.py` & `cars-0.7.1/cars/applications/dense_matches_filling/fill_disp_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matches_filling/fill_disp_tools.py` & `cars-0.7.1/cars/applications/dense_matches_filling/fill_disp_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matches_filling/plane.py` & `cars-0.7.1/cars/applications/dense_matches_filling/plane.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matches_filling/zero_padding.py` & `cars-0.7.1/cars/applications/dense_matches_filling/zero_padding.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matching/__init__.py` & `cars-0.7.1/cars/applications/dense_matching/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matching/census_mccnn_sgm.py` & `cars-0.7.1/cars/applications/dense_matching/census_mccnn_sgm.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,19 @@
         self.min_epi_tile_size = self.used_config["min_epi_tile_size"]
         self.max_epi_tile_size = self.used_config["max_epi_tile_size"]
         self.epipolar_tile_margin_in_percent = self.used_config[
             "epipolar_tile_margin_in_percent"
         ]
         self.min_elevation_offset = self.used_config["min_elevation_offset"]
         self.max_elevation_offset = self.used_config["max_elevation_offset"]
+
+        # Disparity threshold
+        self.disp_min_threshold = self.used_config["disp_min_threshold"]
+        self.disp_max_threshold = self.used_config["disp_max_threshold"]
+
         # Performance map
         self.generate_performance_map = self.used_config[
             "generate_performance_map"
         ]
         self.perf_ambiguity_threshold = self.used_config[
             "perf_ambiguity_threshold"
         ]
@@ -125,14 +130,23 @@
         )
         overloaded_conf["min_elevation_offset"] = conf.get(
             "min_elevation_offset", None
         )
         overloaded_conf["max_elevation_offset"] = conf.get(
             "max_elevation_offset", None
         )
+
+        # Disparity threshold
+        overloaded_conf["disp_min_threshold"] = conf.get(
+            "disp_min_threshold", None
+        )
+        overloaded_conf["disp_max_threshold"] = conf.get(
+            "disp_max_threshold", None
+        )
+
         # Permormance map parameters
         overloaded_conf["generate_performance_map"] = conf.get(
             "generate_performance_map", False
         )
         overloaded_conf["perf_eta_max_ambiguity"] = conf.get(
             "perf_eta_max_ambiguity", 0.99
         )
@@ -170,14 +184,16 @@
         application_schema = {
             "method": str,
             "min_epi_tile_size": And(int, lambda x: x > 0),
             "max_epi_tile_size": And(int, lambda x: x > 0),
             "epipolar_tile_margin_in_percent": int,
             "min_elevation_offset": Or(None, int),
             "max_elevation_offset": Or(None, int),
+            "disp_min_threshold": Or(None, int),
+            "disp_max_threshold": Or(None, int),
             "save_disparity_map": bool,
             "generate_performance_map": bool,
             "perf_eta_max_ambiguity": float,
             "perf_eta_max_risk": float,
             "perf_eta_step": float,
             "perf_ambiguity_threshold": float,
             "loader_conf": dict,
@@ -206,27 +222,56 @@
             and min_elevation_offset > max_elevation_offset
         ):
             raise ValueError(
                 "Maximal elevation should be bigger than "
                 "minimal elevation for dense matching"
             )
 
+        disp_min_threshold = overloaded_conf["disp_min_threshold"]
+        disp_max_threshold = overloaded_conf["disp_max_threshold"]
+        if (
+            disp_min_threshold is not None
+            and disp_max_threshold is not None
+            and disp_min_threshold > disp_max_threshold
+        ):
+            raise ValueError(
+                "Maximal disparity should be bigger than "
+                "minimal disparity for dense matching"
+            )
+
         return overloaded_conf
 
     def get_margins(self, grid_left, disp_min=None, disp_max=None):
         """
         Get Margins needed by matching method, to use during resampling
 
         :param grid_left: left epipolar grid
         :param disp_min: minimum disparity
         :param disp_max: maximum disparity
         :return: margins, updated disp_min, updated disp_max
 
         """
 
+        if self.disp_min_threshold is not None:
+            if disp_min < self.disp_min_threshold:
+                logging.warning(
+                    "Override disp_min {} with disp_min_threshold {}".format(
+                        disp_min, self.disp_min_threshold
+                    )
+                )
+                disp_min = self.disp_min_threshold
+        if self.disp_max_threshold is not None:
+            if disp_max > self.disp_max_threshold:
+                logging.warning(
+                    "Override disp_max {} with disp_max_threshold {}".format(
+                        disp_max, self.disp_max_threshold
+                    )
+                )
+                disp_max = self.disp_max_threshold
+
         # get disp_to_alt_ratio
         disp_to_alt_ratio = grid_left.attributes["disp_to_alt_ratio"]
 
         # Check if we need to override disp_min
         if self.min_elevation_offset is not None:
             user_disp_min = self.min_elevation_offset / disp_to_alt_ratio
             if user_disp_min > disp_min:
```

### Comparing `cars-0.7.0/cars/applications/dense_matching/dense_matching.py` & `cars-0.7.1/cars/applications/dense_matching/dense_matching.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matching/dense_matching_constants.py` & `cars-0.7.1/cars/applications/dense_matching/dense_matching_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matching/dense_matching_tools.py` & `cars-0.7.1/cars/applications/dense_matching/dense_matching_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matching/loaders/__init__.py` & `cars-0.7.1/cars/applications/dense_matching/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matching/loaders/config_census_sgm.json` & `cars-0.7.1/cars/applications/dense_matching/loaders/config_census_sgm.json`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matching/loaders/config_mccnn.json` & `cars-0.7.1/cars/applications/dense_matching/loaders/config_mccnn.json`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/dense_matching/loaders/pandora_loader.py` & `cars-0.7.1/cars/applications/dense_matching/loaders/pandora_loader.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/grid_generation/__init__.py` & `cars-0.7.1/cars/applications/grid_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/grid_generation/epipolar_grid_generation.py` & `cars-0.7.1/cars/applications/grid_generation/epipolar_grid_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,29 @@
 
         # Overload conf
         overloaded_conf["method"] = conf.get("method", "epipolar")
         overloaded_conf["epi_step"] = conf.get("epi_step", 30)
         overloaded_conf["save_grids"] = conf.get("save_grids", False)
 
         # check geometry tool availability
+        geometry = "OTBGeometry"
+
+        # 1/ check otbApplication python module
         otb_app = importlib.util.find_spec("otbApplication")
-        geometry = "OTBGeometry" if otb_app is not None else "SharelocGeometry"
+        # 2/ check remote modules
+        if otb_app is not None:
+            otb_geometry = (
+                AbstractGeometry(  # pylint: disable=abstract-class-instantiated
+                    "OTBGeometry"
+                )
+            )
+            missing_remote = otb_geometry.check_otb_remote_modules()
+
+        if otb_app is None or len(missing_remote) > 0:
+            geometry = "SharelocGeometry"
 
         # Overloader loader
         overloaded_conf["geometry_loader"] = conf.get(
             "geometry_loader", geometry
         )
 
         grid_generation_schema = {
```

### Comparing `cars-0.7.0/cars/applications/grid_generation/grid_constants.py` & `cars-0.7.1/cars/applications/grid_generation/grid_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/grid_generation/grid_correction.py` & `cars-0.7.1/cars/applications/grid_generation/grid_correction.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/grid_generation/grid_generation.py` & `cars-0.7.1/cars/applications/grid_generation/grid_generation.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/grid_generation/grids.py` & `cars-0.7.1/cars/applications/grid_generation/grids.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/holes_detection/__init__.py` & `cars-0.7.1/cars/applications/holes_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/holes_detection/cloud_to_bbox.py` & `cars-0.7.1/cars/applications/holes_detection/cloud_to_bbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,54 +190,57 @@
                 self.orchestrator.add_to_replace_lists(
                     right_bbox_cars_ds, cars_ds_name="epi_msk_bbox_right"
                 )
 
                 # Generate disparity maps
                 for col in range(epipolar_images_left.shape[1]):
                     for row in range(epipolar_images_left.shape[0]):
-                        # update saving_info with row and col needed for
-                        # replacement
-                        full_saving_info_left = ocht.update_saving_infos(
-                            saving_info_left, row=row, col=col
-                        )
-                        full_saving_info_right = ocht.update_saving_infos(
-                            saving_info_right, row=row, col=col
-                        )
-
-                        # get window and overlaps
-                        window_left = epipolar_images_left.tiling_grid[
-                            row, col, :
-                        ]
-                        window_right = epipolar_images_right.tiling_grid[
-                            row, col, :
-                        ]
-                        overlap_left = epipolar_images_left.overlaps[
-                            row, col, :
-                        ]
-                        overlap_right = epipolar_images_right.overlaps[
-                            row, col, :
-                        ]
-
-                        # Compute bbox
-                        (
-                            left_bbox_cars_ds[row, col],
-                            right_bbox_cars_ds[row, col],
-                        ) = self.orchestrator.cluster.create_task(
-                            compute_mask_bboxes, nout=2
-                        )(
-                            epipolar_images_left[row, col],
-                            epipolar_images_right[row, col],
-                            window_left,
-                            window_right,
-                            overlap_left,
-                            overlap_right,
-                            classification,
-                            saving_info_left=full_saving_info_left,
-                            saving_info_right=full_saving_info_right,
-                        )
+                        if (epipolar_images_left[row, col] is not None) or (
+                            epipolar_images_right[row, col] is not None
+                        ):
+                            # update saving_info with row and col needed for
+                            # replacement
+                            full_saving_info_left = ocht.update_saving_infos(
+                                saving_info_left, row=row, col=col
+                            )
+                            full_saving_info_right = ocht.update_saving_infos(
+                                saving_info_right, row=row, col=col
+                            )
+
+                            # get window and overlaps
+                            window_left = epipolar_images_left.tiling_grid[
+                                row, col, :
+                            ]
+                            window_right = epipolar_images_right.tiling_grid[
+                                row, col, :
+                            ]
+                            overlap_left = epipolar_images_left.overlaps[
+                                row, col, :
+                            ]
+                            overlap_right = epipolar_images_right.overlaps[
+                                row, col, :
+                            ]
+
+                            # Compute bbox
+                            (
+                                left_bbox_cars_ds[row, col],
+                                right_bbox_cars_ds[row, col],
+                            ) = self.orchestrator.cluster.create_task(
+                                compute_mask_bboxes, nout=2
+                            )(
+                                epipolar_images_left[row, col],
+                                epipolar_images_right[row, col],
+                                window_left,
+                                window_right,
+                                overlap_left,
+                                overlap_right,
+                                classification,
+                                saving_info_left=full_saving_info_left,
+                                saving_info_right=full_saving_info_right,
+                            )
         else:
             logging.error(
                 "CloudToBbox application doesn't "
                 "support this input data format"
             )
 
         return left_bbox_cars_ds, right_bbox_cars_ds
@@ -300,29 +303,35 @@
 
     # compute offsets
     row_offset_left = window_left[0] - overlap_left[0]
     col_offset_left = window_left[2] - overlap_left[2]
     row_offset_right = window_right[0] - overlap_right[0]
     col_offset_right = window_right[2] - overlap_right[2]
 
-    bbox_left = holes_detection_tools.localize_masked_areas(
-        left_image_dataset,
-        classification,
-        row_offset=row_offset_left,
-        col_offset=col_offset_left,
-        margin=margin,
-    )
-
-    bbox_right = holes_detection_tools.localize_masked_areas(
-        right_image_dataset,
-        classification,
-        row_offset=row_offset_right,
-        col_offset=col_offset_right,
-        margin=margin,
-    )
+    bbox_left = {}
+
+    if left_image_dataset is not None:
+        bbox_left = holes_detection_tools.localize_masked_areas(
+            left_image_dataset,
+            classification,
+            row_offset=row_offset_left,
+            col_offset=col_offset_left,
+            margin=margin,
+        )
+
+    bbox_right = {}
+
+    if right_image_dataset is not None:
+        bbox_right = holes_detection_tools.localize_masked_areas(
+            right_image_dataset,
+            classification,
+            row_offset=row_offset_right,
+            col_offset=col_offset_right,
+            margin=margin,
+        )
 
     # add saving infos
     bbox_left_dict = cars_dict.CarsDict({"list_bbox": bbox_left})
     cars_dataset.fill_dict(bbox_left_dict, saving_info=saving_info_left)
 
     bbox_right_dict = cars_dict.CarsDict({"list_bbox": bbox_right})
     cars_dataset.fill_dict(bbox_right_dict, saving_info=saving_info_right)
```

### Comparing `cars-0.7.0/cars/applications/holes_detection/holes_detection.py` & `cars-0.7.1/cars/applications/holes_detection/holes_detection.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/holes_detection/holes_detection_tools.py` & `cars-0.7.1/cars/applications/holes_detection/holes_detection_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/point_cloud_fusion/__init__.py` & `cars-0.7.1/cars/applications/point_cloud_fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/point_cloud_fusion/cloud_fusion_constants.py` & `cars-0.7.1/cars/applications/point_cloud_fusion/cloud_fusion_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py` & `cars-0.7.1/cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,30 +143,17 @@
             - N x M Delayed tiles. \
                 Each tile will be a future xarray Dataset containing:
 
                 - data : with keys : "x", "y", "z", "corr_msk" \
                     optional: "color", "msk",
                 - attrs with keys: "margins", "epi_full_size", "epsg"
             - attributes containing: "disp_lower_bound",  "disp_upper_bound" \
-                "elevation_delta_lower_bound","elevation_delta_upper_bound"
+                "elevation_delta_lower_bound", "elevation_delta_upper_bound"
         :type list_epipolar_points_cloud: list(CarsDataset) filled with
           xr.Dataset
-        :param list_epipolar_points_cloud_right: list with right points clouds.\
-            Each CarsDataset contains:
-
-            - N x M Delayed tiles.\
-                Each tile will be a future xarray Dataset containing:
-
-                - data : with keys : "x", "y", "z", "corr_msk" \
-                    optional: "color", "msk",
-                - attrs with keys: "margins", "epi_full_size", "epsg"
-            - attributes containing: "disp_lower_bound",  "disp_upper_bound",\
-                "elevation_delta_lower_bound","elevation_delta_upper_bound"
-        :type list_epipolar_points_cloud_right: list(CarsDataset) filled with
-          xr.Dataset
         :param bounds: terrain bounds
         :type bounds: list
         :param epsg: epsg to use
         :type epsg: str
         :param orchestrator: orchestrator used
         :type orchestrator: Orchestrator
         :param margins: margins needed for tiles, meter or degree
@@ -211,15 +198,18 @@
             ymin,
             xmax,
             ymax,
             optimal_terrain_tile_width,
             optimal_terrain_tile_width,
         )
 
-        if list_epipolar_points_cloud[0].dataset_type in (
+        # Get dataset type of first item in list_epipolar_points_cloud
+        pc_dataset_type = list_epipolar_points_cloud[0].dataset_type
+
+        if pc_dataset_type in (
             "arrays",
             "dict",
             "points",
         ):
             # Create CarsDataset
             merged_point_cloud = cars_dataset.CarsDataset("points")
 
@@ -242,19 +232,19 @@
                     merged_point_cloud.shape[0],
                     merged_point_cloud.shape[1],
                 )
             )
 
             number_of_epipolar_tiles_per_terrain_tiles = []
 
-            if list_epipolar_points_cloud[0].dataset_type in (
+            if pc_dataset_type in (
                 "arrays",
                 "points",
             ):
-                # deall with delayed tiles, with a priori disp min and max
+                # deal with delayed tiles, with a priori disp min and max
 
                 # Add epipolar_points_min and epipolar_points_max used
                 #  in point_cloud_fusion
                 # , to get corresponding tiles (terrain)
                 # TODO change method for corresponding tiles
                 list_points_min = []
                 list_points_max = []
@@ -288,18 +278,17 @@
             logging.info(
                 "Point clouds: Merged points number: {}".format(
                     merged_point_cloud.shape[1] * merged_point_cloud.shape[0]
                 )
             )
 
             # Compute corresponing tiles in parallel if from tif files
-            # list_epipolar_points_cloud_right is empty
-            if list_epipolar_points_cloud[0].dataset_type == "dict":
+            if pc_dataset_type == "dict":
                 corresponding_tiles_cars_ds = (
-                    pc_tif_tools.get_tiles_corresponding_tiles_tif(
+                    pc_tif_tools.get_corresponding_tiles_tif(
                         terrain_tiling_grid,
                         list_epipolar_points_cloud,
                         margins=margins,
                         orchestrator=self.orchestrator,
                     )
                 )
 
@@ -325,15 +314,15 @@
 
             for col in range(merged_point_cloud.shape[1]):
                 for row in range(merged_point_cloud.shape[0]):
                     # update saving infos  for potential replacement
                     full_saving_info = ocht.update_saving_infos(
                         saving_info, row=row, col=col
                     )
-                    if list_epipolar_points_cloud[0].dataset_type in (
+                    if pc_dataset_type in (
                         "arrays",
                         "points",
                     ):
                         # Get required point clouds
                         (
                             terrain_region,
                             required_point_clouds,
@@ -344,28 +333,27 @@
                             row,
                             col,
                             list_epipolar_points_cloud,
                             list_points_min,
                             list_points_max,
                         )
                     else:
-                        # required_point_clouds_right will be empty
                         # Get correspondances previously computed
                         terrain_region = corresponding_tiles_cars_ds[row, col][
                             "terrain_region"
                         ]
                         required_point_clouds = corresponding_tiles_cars_ds[
                             row, col
                         ]["required_point_clouds"]
 
                     if (
                         len(
                             [
                                 value
-                                for value in required_point_clouds
+                                for value, _ in required_point_clouds
                                 if not isinstance(value, type(None))
                             ]
                         )
                         > 0
                     ):
                         logging.debug(
                             "Number of clouds to process for this terrain"
@@ -451,21 +439,20 @@
     save_pc_as_csv: bool = False,
     saving_info=None,
 ):
     """
     Wrapper for points clouds fusion step :
     - Convert a list of clouds to correct epsg
 
-    :param point_clouds: list of clouds, list of datasets with :
-
+    :param point_clouds: list of clouds, list of (dataset, dataset_id) with :
             - cst.X
             - cst.Y
             - cst.Z
             - cst.EPI_COLOR
-    :type point_clouds: list(xr.Dataset)
+    :type point_clouds: list((xr.Dataset, int))
     :param  epsg_code: epsg code for the CRS of the output DSM
     :type epsg_code: int
     :param  stereo_out_epsg: epsg code to convert point cloud to, if needed
     :type stereo_out_epsg: int
     :param xmin: xmin of the rasterization grid
         (if None, will be estimated by the function)
     :param xmin: xmin of the rasterization grid
@@ -487,27 +474,29 @@
             - cst.X
             - cst.Y
             - cst.Z
             - cst.EPI_COLOR
             - attrs : xmin, xmax, ymin, ymax, saving_info
     :rtype: pandas.DataFrame
     """
-    # Unpack list of clouds from tuple, and project them to correct EPSG if
-    # needed
-    clouds = point_clouds
-
     # Remove None tiles
-    clouds = [value for value in clouds if value is not None]
+    clouds = []
+    clouds_ids = []
+    for value, pc_id in point_clouds:
+        if value is not None:
+            clouds.append(value)
+            clouds_ids.append(pc_id)
     if len(clouds) == 0:
         raise RuntimeError("All clouds are None")
 
     # combine clouds
     if not isinstance(clouds[0], dict):
         pc_pandas, cloud_epsg = point_cloud_tools.create_combined_cloud(
             clouds,
+            clouds_ids,
             epsg,
             xmin=xmin,
             xmax=xmax,
             ymin=ymin,
             ymax=ymax,
             margin=margins,
             epipolar_border_margin=0,
@@ -519,14 +508,15 @@
         # combined pc from tif files
         (
             pc_pandas,
             cloud_epsg,
             color_type,
         ) = pc_tif_tools.create_combined_cloud_from_tif(
             clouds,
+            clouds_ids,
             epsg,
             xmin=xmin,
             xmax=xmax,
             ymin=ymin,
             ymax=ymax,
             margin=margins,
         )
```

### Comparing `cars-0.7.0/cars/applications/point_cloud_fusion/pc_tif_tools.py` & `cars-0.7.1/cars/applications/point_cloud_fusion/pc_tif_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,21 +266,30 @@
     cond_y_max = pd_cloud[cst.Y] > bounds[3]
     pd_cloud = pd_cloud.drop(
         pd_cloud.index[cond_x_min | cond_x_max | cond_y_min | cond_y_max]
     )
 
 
 def create_combined_cloud_from_tif(
-    clouds, epsg, xmin=None, xmax=None, ymin=None, ymax=None, margin=0
+    clouds,
+    clouds_id,
+    epsg,
+    xmin=None,
+    xmax=None,
+    ymin=None,
+    ymax=None,
+    margin=0,
 ):
     """
     Create combined cloud from tif point clouds
 
     :param clouds: list of clouds
     :type clouds: list(dict)
+    :param clouds_id: list of global identificators associated to clouds
+    :type clouds_id: list(str)
     :param epsg: epsg to convert point clouds to
     :type epsg: int or str
     :param xmin: min x coordinate
     :type xmin: float
     :param xmax: max x coordinate
     :type xmax: float
     :param ymin: min y coordinate
@@ -294,15 +303,15 @@
 
     clouds_pd_list = []
     color_types = []
     for cloud in clouds:
         for type_band in cloud["data"].keys():
             band_path = cloud["data"][type_band]
     # Create multiple pc pandas dataframes
-    for cloud in clouds:
+    for cloud_file_id, cloud in zip(clouds_id, clouds):  # noqa: B905
         window = cloud["window"]
         cloud_epsg = cloud["cloud_epsg"]
         cloud_data_bands = []
         cloud_data = {}
         for type_band in cloud["data"].keys():
             # open file and get data
             band_path = cloud["data"][type_band]
@@ -337,14 +346,20 @@
         # add mask if not given
         if cst.POINTS_CLOUD_VALID_DATA not in cloud_data_bands:
             cloud_data[cst.POINTS_CLOUD_VALID_DATA] = np.ones(
                 cloud_data[cst.X].shape
             )
             cloud_data_bands.append(cst.POINTS_CLOUD_VALID_DATA)
 
+        # add source file id
+        cloud_data[cst.POINTS_CLOUD_GLOBAL_ID] = (
+            np.ones(cloud_data[cst.X].shape) * cloud_file_id
+        )
+        cloud_data_bands.append(cst.POINTS_CLOUD_GLOBAL_ID)
+
         # Create cloud pandas
         cloud_pd = pd.DataFrame(cloud_data, columns=cloud_data_bands)
 
         # Post processing if 0 in data
         cloud_pd = cloud_pd.drop(
             cloud_pd.index[
                 (cloud_pd[cst.X] == 0.0)  # pylint: disable=E1136
@@ -720,15 +735,15 @@
     # add saving infos
     res = cars_dict.CarsDict(tile)
     cars_dataset.fill_dict(res, saving_info=saving_info)
 
     return res
 
 
-def get_tiles_corresponding_tiles_tif(
+def get_corresponding_tiles_tif(
     terrain_tiling_grid,
     list_epipolar_points_cloud_with_loc,
     margins=0,
     orchestrator=None,
 ):
     """
     Get point cloud tiles to use for terrain region
@@ -749,15 +764,15 @@
     :rtype: CarsDataset
 
     """
 
     if orchestrator is None:
         # Create default sequential orchestrator for current
         # application
-        # be awere, no out_json will be shared between orchestrators
+        # be aware, no out_json will be shared between orchestrators
         # No files saved
         cars_orchestrator = ocht.Orchestrator(
             orchestrator_conf={"mode": "sequential"}
         )
     else:
         cars_orchestrator = orchestrator
 
@@ -792,14 +807,15 @@
 
         list_corresp_cars_ds[
             row_fake_cars_ds, 0
         ] = cars_orchestrator.cluster.create_task(
             compute_correspondance_single_pc_terrain, nout=1
         )(
             list_epipolar_points_cloud_with_loc[row_fake_cars_ds],
+            row_fake_cars_ds,
             terrain_tiling_grid,
             margins=margins,
             saving_info=full_saving_info_pc,
         )
 
     # Breakpoint : compute
     # /!\ BE AWARE : this is not the conventionnal way
@@ -821,41 +837,44 @@
                 terrain_tiling_grid[row, col, 2],
                 terrain_tiling_grid[row, col, 1],
                 terrain_tiling_grid[row, col, 3],
             ]
 
             # Get required_point_clouds_left
             required_point_clouds = []
-            for correp_row in range(list_corresp_cars_ds.shape[0]):
+            for corresp_row in range(list_corresp_cars_ds.shape[0]):
                 # each tile in list_corresp contains a CarsDict,
                 # containing a CarsDataset filled with list
-                corresp = list_corresp_cars_ds[correp_row, 0].data[
+                corresp = list_corresp_cars_ds[corresp_row, 0].data[
                     "corresp_cars_ds"
                 ][row, col]
                 required_point_clouds += corresp
 
             terrain_correspondances[row, col] = {
                 "terrain_region": terrain_region,
                 "required_point_clouds": required_point_clouds,
             }
 
     return terrain_correspondances
 
 
 def compute_correspondance_single_pc_terrain(
     epi_pc,
+    epi_pc_id,
     terrain_tiling_grid,
     margins=0,
     saving_info=None,
 ):
     """
     Compute correspondances for each terrain tile, with current point cloud
 
     :param epi_pc: point cloud
     :type epi_pc: dict
+    :param epi_pc_id: identificator of the file of the point cloud
+    :type epi_pc_id: int
     :param terrain_tiling_grid: tiling grid
     :type terrain_tiling_grid: np.ndarray
     :param margins: margin to use in point clouds
     :type margins: float
 
     :return: CarsDict containing list of point cloud tiles to use for each
          terrain tile:
@@ -911,15 +930,15 @@
                     point_cloud_tile_polygon = convert_to_polygon(x_y_min_max)
 
                     if intersect_polygons(
                         terrain_tile_polygon, point_cloud_tile_polygon
                     ):
                         # add to required
                         terrain_corresp[terrain_row, terrain_col].append(
-                            epi_pc[tile_row, tile_col]
+                            (epi_pc[tile_row, tile_col], epi_pc_id)
                         )
 
     # add saving infos
     dict_with_corresp_cars_ds = cars_dict.CarsDict(
         {"corresp_cars_ds": terrain_corresp}
     )
     cars_dataset.fill_dict(dict_with_corresp_cars_ds, saving_info=saving_info)
```

### Comparing `cars-0.7.0/cars/applications/point_cloud_fusion/point_cloud_fusion.py` & `cars-0.7.1/cars/applications/point_cloud_fusion/point_cloud_fusion.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/point_cloud_fusion/point_cloud_tools.py` & `cars-0.7.1/cars/applications/point_cloud_fusion/point_cloud_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 # CARS imports
 from cars.core import constants as cst
 from cars.core import projection
 
 
 def create_combined_cloud(  # noqa: C901
     cloud_list: List[xr.Dataset] or List[pandas.DataFrame],
+    cloud_ids: List[int],
     dsm_epsg: int,
     xmin: float = None,
     xmax: float = None,
     ymin: int = None,
     ymax: int = None,
     epipolar_border_margin: int = 0,
     margin: float = 0,
@@ -51,14 +52,16 @@
 ) -> Tuple[pandas.DataFrame, int]:
     """
     Combine a list of clouds from sparse or dense matching
     into a pandas dataframe.
     The detailed cases for each cloud type are in the derived function
     create_combined_sparse_cloud and create_combined_dense_cloud.
 
+    :param cloud_list: list of every point cloud to merge
+    :param cloud_ids: list of global identificators of clouds in cloud_list
     :param dsm_epsg: epsg code for the CRS of the final output raster
     :param xmin: xmin of the rasterization grid
         (if None, the whole clouds are combined)
     :param xmax: xmax of the rasterization grid
         (if None, the whole clouds are combined)
     :param ymin: ymin of the rasterization grid
         (if None, the whole clouds are combined)
@@ -73,39 +76,42 @@
         in the original epipolar images
     :return: Tuple formed with the combined clouds and color
         in a single pandas dataframe and the epsg code
     """
     if isinstance(cloud_list[0], xr.Dataset):
         return create_combined_dense_cloud(
             cloud_list,
+            cloud_ids,
             dsm_epsg,
             xmin,
             xmax,
             ymin,
             ymax,
             epipolar_border_margin,
             margin,
             with_coords,
         )
     # case of pandas.DataFrame cloud
     return create_combined_sparse_cloud(
         cloud_list,
+        cloud_ids,
         dsm_epsg,
         xmin,
         xmax,
         ymin,
         ymax,
         epipolar_border_margin,
         margin,
         with_coords,
     )
 
 
 def create_combined_sparse_cloud(  # noqa: C901
     cloud_list: List[pandas.DataFrame],
+    cloud_ids: List[int],
     dsm_epsg: int,
     xmin: float = None,
     xmax: float = None,
     ymin: int = None,
     ymax: int = None,
     epipolar_border_margin: int = 0,
     margin: float = 0,
@@ -161,15 +167,17 @@
 
     if with_coords:
         nb_data.extend([cst.POINTS_CLOUD_COORD_EPI_GEOM_I])
 
     # iterate through input clouds
     cloud = np.zeros((0, len(nb_data)), dtype=np.float64)
     nb_points = 0
-    for _, cloud_list_item in enumerate(cloud_list):
+    for cloud_global_id, cloud_list_item in zip(  # noqa: B905
+        cloud_ids, cloud_list
+    ):
         full_x = cloud_list_item[cst.X]
         full_y = cloud_list_item[cst.Y]
         full_z = cloud_list_item[cst.Z]
 
         # get mask of points inside the roi (plus margins)
         if roi:
             # Compute terrain tile bounds
@@ -236,14 +244,17 @@
             ] = True
 
         c_epipolar_margin_mask = epipolar_margin_mask[bbox[0] : bbox[1] + 1]
         c_cloud[nb_data.index(cst.POINTS_CLOUD_VALID_DATA), :] = np.ravel(
             c_epipolar_margin_mask
         )
 
+        # add index of original point cloud
+        c_cloud[nb_data.index(cst.POINTS_CLOUD_GLOBAL_ID), :] = cloud_global_id
+
         # add the original image coordinates information to the current cloud
         if with_coords:
             coords_line = np.linspace(
                 bbox[0], bbox[1], num=bbox[1] - bbox[0] + 1
             )
             c_cloud[
                 nb_data.index(cst.POINTS_CLOUD_COORD_EPI_GEOM_I), :
@@ -366,14 +377,15 @@
     terrain_tile_data_msk_pos = terrain_tile_data_msk.astype(np.int8).nonzero()
 
     return terrain_tile_data_msk, terrain_tile_data_msk_pos
 
 
 def create_combined_dense_cloud(  # noqa: C901
     cloud_list: List[xr.Dataset],
+    cloud_id: List[int],
     dsm_epsg: int,
     xmin: float = None,
     xmax: float = None,
     ymin: int = None,
     ymax: int = None,
     epipolar_border_margin: int = 0,
     margin: float = 0,
@@ -409,15 +421,15 @@
              labels=[cst.POINTS_CLOUD_VALID_DATA,\
                      cst.X, cst.Y, cst.Z, cst.POINTS_CLOUD_MSK,\
                      cst.POINTS_CLOUD_CLR_KEY_ROOT+"0",\
                     cst.POINTS_CLOUD_CLR_KEY_ROOT+"1",\
                     cst.POINTS_CLOUD_CLR_KEY_ROOT+"2"\
                      cst.POINTS_CLOUD_COORD_EPI_GEOM_I,\
                      cst.POINTS_CLOUD_COORD_EPI_GEOM_J,\
-                     cst.POINTS_CLOUD_IDX_IM_EPI]\
+                     cst.POINTS_CLOUD_ID_IM_EPI]\
             The pixel position of the xyz point in the original epipolar\
             image (coord_epi_geom_i, coord_epi_geom_j) are added\
             to the dataframe along with the index of its original cloud\
             in the cloud_list input.
 
 
     :param dsm_epsg: epsg code for the CRS of the final output raster
@@ -435,15 +447,14 @@
         to invalidate cells too close to epipolar border. (default value: 0)
     :param with_coords: Option enabling the adding to the combined cloud
         of information of each point to retrieve their positions
         in the original epipolar images
     :return: Tuple formed with the combined clouds and color
         in a single pandas dataframe and the epsg code
     """
-
     epsg = get_epsg(cloud_list)
 
     # compute margin/roi and final number of data to add to the combined cloud
     roi = (
         xmin is not None
         and xmax is not None
         and ymin is not None
@@ -465,15 +476,15 @@
     nb_data.extend(list_clr)
 
     if with_coords:
         nb_data.extend(
             [
                 cst.POINTS_CLOUD_COORD_EPI_GEOM_I,
                 cst.POINTS_CLOUD_COORD_EPI_GEOM_J,
-                cst.POINTS_CLOUD_IDX_IM_EPI,
+                cst.POINTS_CLOUD_ID_IM_EPI,
             ]
         )
 
     # add classif indexes
     band_classif = None
     if cst.EPI_CLASSIFICATION in cloud_list[0]:
         band_classif = list(cloud_list[0].coords[cst.BAND_CLASSIF].to_numpy())
@@ -490,15 +501,17 @@
         if cst.POINTS_CLOUD_CONFIDENCE in key:
             nb_data.append(key)
             confidence_list.append(key)
 
     # iterate through input clouds
     cloud = np.zeros((0, len(nb_data)), dtype=np.float64)
     nb_points = 0
-    for cloud_list_idx, cloud_list_item in enumerate(cloud_list):
+    for cloud_global_id, (cloud_list_id, cloud_list_item) in zip(  # noqa: B905
+        cloud_id, enumerate(cloud_list)
+    ):
         full_x = cloud_list_item[cst.X].values
         full_y = cloud_list_item[cst.Y].values
         full_z = cloud_list_item[cst.Z].values
 
         # get mask of points inside the roi (plus margins)
         if roi:
             # Compute terrain tile bounds
@@ -593,41 +606,44 @@
         c_epipolar_margin_mask = epipolar_margin_mask[
             bbox[0] : bbox[2] + 1, bbox[1] : bbox[3] + 1
         ]
         c_cloud[nb_data.index(cst.POINTS_CLOUD_VALID_DATA), :] = np.ravel(
             c_epipolar_margin_mask
         )
 
+        # add index of original point cloud
+        c_cloud[nb_data.index(cst.POINTS_CLOUD_GLOBAL_ID), :] = cloud_global_id
+
         # add the color information to the current cloud
-        if cst.EPI_COLOR in cloud_list[cloud_list_idx]:
+        if cst.EPI_COLOR in cloud_list[cloud_list_id]:
             add_color_information(
                 cloud_list,
                 nb_data,
                 nb_band_clr,
-                cloud_list_idx,
+                cloud_list_id,
                 bbox,
                 c_cloud,
             )
 
         # add classification to the current cloud
-        if cst.EPI_CLASSIFICATION in cloud_list[cloud_list_idx]:
+        if cst.EPI_CLASSIFICATION in cloud_list[cloud_list_id]:
             add_classification_information(
                 cloud_list,
                 nb_data,
                 band_classif,
-                cloud_list_idx,
+                cloud_list_id,
                 bbox,
                 c_cloud,
             )
         # add mask to the current cloud
-        if cst.EPI_COLOR_MSK in cloud_list[cloud_list_idx]:
+        if cst.EPI_COLOR_MSK in cloud_list[cloud_list_id]:
             add_msk_information(
                 cloud_list,
                 nb_data,
-                cloud_list_idx,
+                cloud_list_id,
                 bbox,
                 c_cloud,
             )
         # add the original image coordinates information to the current cloud
         if with_coords:
             coords_line = np.linspace(bbox[0], bbox[2], bbox[2] - bbox[0] + 1)
             coords_col = np.linspace(bbox[1], bbox[3], bbox[3] - bbox[1] + 1)
@@ -636,16 +652,16 @@
             c_cloud[
                 nb_data.index(cst.POINTS_CLOUD_COORD_EPI_GEOM_I), :
             ] = np.ravel(coords_line)
             c_cloud[
                 nb_data.index(cst.POINTS_CLOUD_COORD_EPI_GEOM_J), :
             ] = np.ravel(coords_col)
             c_cloud[
-                nb_data.index(cst.POINTS_CLOUD_IDX_IM_EPI), :
-            ] = cloud_list_idx
+                nb_data.index(cst.POINTS_CLOUD_ID_IM_EPI), :
+            ] = cloud_list_id
 
         # remove masked data (pandora + out of the terrain tile points)
         c_terrain_tile_data_msk = (
             cloud_list_item[cst.POINTS_CLOUD_CORR_MSK].values[
                 bbox[0] : bbox[2] + 1, bbox[1] : bbox[3] + 1
             ]
             == 255
@@ -677,15 +693,21 @@
     return pd_cloud, epsg
 
 
 def create_point_cloud_index(cloud_list):
     """
     Create point cloud index from cloud list keys and color inputs
     """
-    nb_data = [cst.POINTS_CLOUD_VALID_DATA, cst.X, cst.Y, cst.Z]
+    nb_data = [
+        cst.POINTS_CLOUD_GLOBAL_ID,
+        cst.POINTS_CLOUD_VALID_DATA,
+        cst.X,
+        cst.Y,
+        cst.Z,
+    ]
 
     # check if the input mask values are present in the dataset
     for cloud_list_item in cloud_list:
         ds_values_list = [key for key, _ in cloud_list_item.items()]
         if cst.POINTS_CLOUD_MSK in ds_values_list:
             nb_data.append(cst.POINTS_CLOUD_MSK)
             break
@@ -693,50 +715,50 @@
     return nb_data
 
 
 def add_color_information(
     cloud_list,
     nb_data,
     nb_band_clr,
-    cloud_list_idx,
+    cloud_list_id,
     bbox,
     c_cloud,
 ):
     """
     Add color information for a current cloud_list item
 
     :param cloud_list: point cloud dataset
     :type cloud_list: List(Dataset)
     :param nb_data: list of band data
     :type nb_data: list[str]
     :param nb_band_clr: number of color band
     :type nb_band_clr: int
-    :param cloud_list_idx: index of the current point cloud
-    :type cloud_list_idx: int
+    :param cloud_list_id: index of the current point cloud
+    :type cloud_list_id: int
     :param bbox: bbox of interest
     :type bbox: list[int]
     :param c_cloud: arranged point cloud
     :type c_cloud: NDArray[float64]
     """
     if nb_band_clr == 1:
-        if len(cloud_list[cloud_list_idx][cst.EPI_COLOR].values.shape) == 3:
+        if len(cloud_list[cloud_list_id][cst.EPI_COLOR].values.shape) == 3:
             c_color = np.squeeze(
-                cloud_list[cloud_list_idx][cst.EPI_COLOR].values
+                cloud_list[cloud_list_id][cst.EPI_COLOR].values
             )[bbox[0] : bbox[2] + 1, bbox[1] : bbox[3] + 1]
         else:
-            c_color = cloud_list[cloud_list_idx][cst.EPI_COLOR].values[
+            c_color = cloud_list[cloud_list_id][cst.EPI_COLOR].values[
                 bbox[0] : bbox[2] + 1, bbox[1] : bbox[3] + 1
             ]
 
         c_cloud[
             nb_data.index("{}{}".format(cst.POINTS_CLOUD_CLR_KEY_ROOT, 0)),
             :,
         ] = np.ravel(c_color[:, :])
     else:
-        color_array = cloud_list[cloud_list_idx][cst.EPI_COLOR].values
+        color_array = cloud_list[cloud_list_id][cst.EPI_COLOR].values
         if len(color_array.shape) == 2:
             # point cloud created with pancro, needs to duplicate
             logging.debug(
                 "Not the same number of color bands for all point clouds"
             )
             color_array = np.stack(
                 [color_array for _ in range(nb_band_clr)], axis=0
@@ -752,66 +774,66 @@
             ] = np.ravel(c_color[band, :, :])
 
 
 def add_classification_information(
     cloud_list,
     nb_data,
     band_classif,
-    cloud_list_idx,
+    cloud_list_id,
     bbox,
     c_cloud,
 ):
     """
     Add color information for a current cloud_list item
 
     :param cloud_list: point cloud dataset
     :type cloud_list: List(Dataset)
     :param band_classif: list of band classif
     :type band_classif: list[str]
     :param nb_data: list of band data
     :type nb_data: list[str]
-    :param cloud_list_idx: index of the current point cloud
-    :type cloud_list_idx: int
+    :param cloud_list_id: index of the current point cloud
+    :type cloud_list_id: int
     :param bbox: bbox of interest
     :type bbox: list[int]
     :param c_cloud: arranged point cloud
     :type c_cloud: NDArray[float64]
     """
-    classif_array = cloud_list[cloud_list_idx][cst.EPI_CLASSIFICATION].values
+    classif_array = cloud_list[cloud_list_id][cst.EPI_CLASSIFICATION].values
     c_classif = classif_array[:, bbox[0] : bbox[2] + 1, bbox[1] : bbox[3] + 1]
     for idx, band in enumerate(band_classif):
         band_index = "{}_{}".format(cst.POINTS_CLOUD_CLASSIF_KEY_ROOT, band)
         c_cloud[
             nb_data.index(band_index),
             :,
         ] = np.ravel(c_classif[idx, :, :])
 
 
 def add_msk_information(
     cloud_list,
     nb_data,
-    cloud_list_idx,
+    cloud_list_id,
     bbox,
     c_cloud,
 ):
     """
     Add mask information for a current cloud_list item
 
     :param cloud_list: point cloud dataset
     :type cloud_list: List(Dataset)
     :param nb_data: list of band data
     :type nb_data: list[str]
-    :param cloud_list_idx: index of the current point cloud
-    :type cloud_list_idx: int
+    :param cloud_list_id: index of the current point cloud
+    :type cloud_list_id: int
     :param bbox: bbox of interest
     :type bbox: list[int]
     :param c_cloud: arranged point cloud
     :type c_cloud: NDArray[float64]
     """
-    msk_array = cloud_list[cloud_list_idx][cst.EPI_COLOR_MSK].values
+    msk_array = cloud_list[cloud_list_id][cst.EPI_COLOR_MSK].values
     c_msk = msk_array[bbox[0] : bbox[2] + 1, bbox[1] : bbox[3] + 1]
     c_cloud[
         nb_data.index(cst.POINTS_CLOUD_MSK),
         :,
     ] = np.ravel(c_msk[:, :])
 
 
@@ -823,16 +845,16 @@
     :type cloud_list: xarray Dataset
 
     :return: color type of the tiles list
     :rtype: str
 
     """
     color_types = []
-    for cloud_idx, cloud_item in enumerate(clouds):
-        if cst.EPI_COLOR in clouds[cloud_idx]:
+    for cloud_id, cloud_item in enumerate(clouds):
+        if cst.EPI_COLOR in clouds[cloud_id]:
             if "color_type" in cloud_item.attrs:
                 color_types.append(cloud_item.attrs["color_type"])
     if color_types:
         color_type_set = set(color_types)
         if len(color_type_set) > 1:
             logging.warning("The tiles colors don't have the same type.")
         return color_types[0]
@@ -897,29 +919,29 @@
         the filtered elements epipolar position information
         (or None for the latter if filtered_elt_pos is set to False
         or if the cloud Dataframe has not been build with with_coords option)
     """
     if filtered_elt_pos and not (
         cst.POINTS_CLOUD_COORD_EPI_GEOM_I in cloud.columns
         and cst.POINTS_CLOUD_COORD_EPI_GEOM_J in cloud.columns
-        and cst.POINTS_CLOUD_IDX_IM_EPI in cloud.columns
+        and cst.POINTS_CLOUD_ID_IM_EPI in cloud.columns
     ):
         logging.warning(
             "In filter_cloud: the filtered_elt_pos has been activated but "
             "the cloud Datafram has not been build with option with_coords. "
             "The positions cannot be retrieved."
         )
         filtered_elt_pos = False
 
     # retrieve removed points position in their original epipolar images
     if filtered_elt_pos:
         labels = [
             cst.POINTS_CLOUD_COORD_EPI_GEOM_I,
             cst.POINTS_CLOUD_COORD_EPI_GEOM_J,
-            cst.POINTS_CLOUD_IDX_IM_EPI,
+            cst.POINTS_CLOUD_ID_IM_EPI,
         ]
 
         removed_elt_pos_infos = cloud.loc[
             cloud.index.values[index_elt_to_remove], labels
         ].values
 
         removed_elt_pos_infos = pandas.DataFrame(
@@ -945,57 +967,57 @@
     (in-line function)
 
     TODO only used in tests
 
     :param clouds_list: Input list of clouds
     :param elt_pos_infos: pandas dataframe
         composed of cst.POINTS_CLOUD_COORD_EPI_GEOM_I,
-        cst.POINTS_CLOUD_COORD_EPI_GEOM_J, cst.POINTS_CLOUD_IDX_IM_EPI columns
+        cst.POINTS_CLOUD_COORD_EPI_GEOM_J, cst.POINTS_CLOUD_ID_IM_EPI columns
         as computed in the create_combined_cloud function.
         Those information are used to retrieve the point position
         in its original epipolar image.
     :param mask_label: label to give to the mask in the datasets
     :param mask_value: filtered elements value in the mask
     """
 
     # Verify that the elt_pos_infos is consistent
     if (
         elt_pos_infos is None
         or cst.POINTS_CLOUD_COORD_EPI_GEOM_I not in elt_pos_infos.columns
         or cst.POINTS_CLOUD_COORD_EPI_GEOM_J not in elt_pos_infos.columns
-        or cst.POINTS_CLOUD_IDX_IM_EPI not in elt_pos_infos.columns
+        or cst.POINTS_CLOUD_ID_IM_EPI not in elt_pos_infos.columns
     ):
         logging.warning(
             "Cannot generate filtered elements mask, "
             "no information about the point's"
             " original position in the epipolar image is given"
         )
 
     else:
-        elt_index = elt_pos_infos.loc[:, cst.POINTS_CLOUD_IDX_IM_EPI].to_numpy()
+        elt_index = elt_pos_infos.loc[:, cst.POINTS_CLOUD_ID_IM_EPI].to_numpy()
 
         min_elt_index = np.min(elt_index)
         max_elt_index = np.max(elt_index)
 
         if min_elt_index < 0 or max_elt_index > len(clouds_list) - 1:
             raise RuntimeError(
                 "Index indicated in the elt_pos_infos pandas. "
                 "DataFrame is not coherent with the clouds list given in input"
             )
 
         # create and add mask to each element of clouds_list
-        for cloud_idx, cloud_item in enumerate(clouds_list):
+        for cloud_id, cloud_item in enumerate(clouds_list):
             if mask_label not in cloud_item:
                 nb_row = cloud_item.coords[cst.ROW].data.shape[0]
                 nb_col = cloud_item.coords[cst.COL].data.shape[0]
                 msk = np.zeros((nb_row, nb_col), dtype=np.uint16)
             else:
                 msk = cloud_item[mask_label].values
 
-            cur_elt_index = np.argwhere(elt_index == cloud_idx)
+            cur_elt_index = np.argwhere(elt_index == cloud_id)
 
             for elt_pos in range(cur_elt_index.shape[0]):
                 i = int(
                     elt_pos_infos.loc[
                         cur_elt_index[elt_pos],
                         cst.POINTS_CLOUD_COORD_EPI_GEOM_I,
                     ].iat[0]
```

### Comparing `cars-0.7.0/cars/applications/point_cloud_outliers_removing/__init__.py` & `cars-0.7.1/cars/applications/point_cloud_outliers_removing/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/point_cloud_outliers_removing/outlier_removing_tools.py` & `cars-0.7.1/cars/applications/point_cloud_outliers_removing/outlier_removing_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,29 +279,29 @@
         the filtered elements epipolar position information
         (or None for the latter if filtered_elt_pos is set to False
         or if the cloud Dataframe has not been build with with_coords option)
     """
     if filtered_elt_pos and not (
         cst.POINTS_CLOUD_COORD_EPI_GEOM_I in cloud.columns
         and cst.POINTS_CLOUD_COORD_EPI_GEOM_J in cloud.columns
-        and cst.POINTS_CLOUD_IDX_IM_EPI in cloud.columns
+        and cst.POINTS_CLOUD_ID_IM_EPI in cloud.columns
     ):
         logging.warning(
             "In filter_cloud: the filtered_elt_pos has been activated but "
             "the cloud Datafram has not been build with option with_coords. "
             "The positions cannot be retrieved."
         )
         filtered_elt_pos = False
 
     # retrieve removed points position in their original epipolar images
     if filtered_elt_pos:
         labels = [
             cst.POINTS_CLOUD_COORD_EPI_GEOM_I,
             cst.POINTS_CLOUD_COORD_EPI_GEOM_J,
-            cst.POINTS_CLOUD_IDX_IM_EPI,
+            cst.POINTS_CLOUD_ID_IM_EPI,
         ]
 
         removed_elt_pos_infos = cloud.loc[
             cloud.index.values[index_elt_to_remove], labels
         ].values
 
         removed_elt_pos_infos = pandas.DataFrame(
@@ -325,37 +325,37 @@
     """
     Add a uint16 mask labeled 'mask_label' to the clouds in clouds_list.
     (in-line function)
 
     :param clouds_list: Input list of clouds
     :param elt_pos_infos: pandas dataframe
         composed of cst.POINTS_CLOUD_COORD_EPI_GEOM_I,
-        cst.POINTS_CLOUD_COORD_EPI_GEOM_J, cst.POINTS_CLOUD_IDX_IM_EPI columns
+        cst.POINTS_CLOUD_COORD_EPI_GEOM_J, cst.POINTS_CLOUD_ID_IM_EPI columns
         as computed in the create_combined_cloud function.
         Those information are used to retrieve the point position
         in its original epipolar image.
     :param mask_label: label to give to the mask in the datasets
     :param mask_value: filtered elements value in the mask
     """
 
     # Verify that the elt_pos_infos is consistent
     if (
         elt_pos_infos is None
         or cst.POINTS_CLOUD_COORD_EPI_GEOM_I not in elt_pos_infos.columns
         or cst.POINTS_CLOUD_COORD_EPI_GEOM_J not in elt_pos_infos.columns
-        or cst.POINTS_CLOUD_IDX_IM_EPI not in elt_pos_infos.columns
+        or cst.POINTS_CLOUD_ID_IM_EPI not in elt_pos_infos.columns
     ):
         logging.warning(
             "Cannot generate filtered elements mask, "
             "no information about the point's"
             " original position in the epipolar image is given"
         )
 
     else:
-        elt_index = elt_pos_infos.loc[:, cst.POINTS_CLOUD_IDX_IM_EPI].to_numpy()
+        elt_index = elt_pos_infos.loc[:, cst.POINTS_CLOUD_ID_IM_EPI].to_numpy()
 
         min_elt_index = np.min(elt_index)
         max_elt_index = np.max(elt_index)
 
         if min_elt_index < 0 or max_elt_index > len(clouds_list) - 1:
             raise RuntimeError(
                 "Index indicated in the elt_pos_infos pandas. "
```

### Comparing `cars-0.7.0/cars/applications/point_cloud_outliers_removing/pc_out_removing.py` & `cars-0.7.1/cars/applications/point_cloud_outliers_removing/pc_out_removing.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/point_cloud_outliers_removing/points_removing_constants.py` & `cars-0.7.1/cars/applications/point_cloud_outliers_removing/points_removing_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/point_cloud_outliers_removing/small_components.py` & `cars-0.7.1/cars/applications/point_cloud_outliers_removing/small_components.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/point_cloud_outliers_removing/statistical.py` & `cars-0.7.1/cars/applications/point_cloud_outliers_removing/statistical.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/rasterization/__init__.py` & `cars-0.7.1/cars/applications/rasterization/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/rasterization/point_cloud_rasterization.py` & `cars-0.7.1/cars/applications/rasterization/point_cloud_rasterization.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/rasterization/rasterization_constants.py` & `cars-0.7.1/cars/applications/rasterization/rasterization_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/rasterization/rasterization_tools.py` & `cars-0.7.1/cars/applications/rasterization/rasterization_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # limitations under the License.
 #
 """
 This module is responsible for the rasterization step:
 - it contains all functions related to 3D representation on a 2D raster grid
 TODO: refactor in several files and remove too-many-lines
 """
-# pylint: disable=C0302
 
 # Standard imports
 import logging
 from typing import List, Tuple, Union
 
 # Third party imports
 import numpy as np
@@ -86,14 +85,15 @@
     ysize: int = None,
     sigma: float = None,
     radius: int = 1,
     dsm_no_data: int = np.nan,
     color_no_data: int = np.nan,
     msk_no_data: int = 65535,
     list_computed_layers: List[str] = None,
+    source_pc_names: List[str] = None,
 ) -> xr.Dataset:
     """
     Wrapper of simple_rasterization
     that has xarray.Dataset as inputs and outputs.
 
     :param cloud: cloud to rasterize
     :param resolution: Resolution of rasterized cells,
@@ -112,14 +112,16 @@
     :param sigma: sigma for gaussian interpolation.
         (If None, set to resolution)
     :param radius: Radius for hole filling.
     :param dsm_no_data: no data value to use in the final raster
     :param color_no_data: no data value to use in the final colored raster
     :param msk_no_data: no data value to use in the final mask image
     :param list_computed_layers: list of computed output data
+    :param source_pc_names: list of names of points cloud before merging :
+        name of sensors pair or name of point cloud file
     :return: Rasterized cloud
     """
 
     # combined clouds
     roi = (
         resolution is not None
         and xstart is not None
@@ -148,14 +150,15 @@
         y_size=ysize,
         sigma=sigma,
         radius=radius,
         hgt_no_data=dsm_no_data,
         color_no_data=color_no_data,
         msk_no_data=msk_no_data,
         list_computed_layers=list_computed_layers,
+        source_pc_names=source_pc_names,
     )
 
     return raster
 
 
 def compute_values_1d(
     x_start: float, y_start: float, x_size: int, y_size: int, resolution: float
@@ -183,15 +186,44 @@
         y_size,
         endpoint=False,
     )
 
     return x_values_1d, y_values_1d
 
 
-def compute_vector_raster_and_stats(
+def substring_in_list(src_list, substring):
+    """
+    Check if the list contains substring
+    """
+    res = list(filter(lambda x: substring in x, src_list))
+    return len(res) > 0
+
+
+def find_indexes_in_point_cloud(
+    cloud: pandas.DataFrame, tag: str, list_computed_layers: List[str]
+) -> List[str]:
+    """
+    Find all indexes in point cloud that contains the key tag
+    if it needs to be computed
+    :param cloud: Combined cloud
+    :param tag: substring of desired columns in cloud
+    :param list_computed_layers: list of computed output data
+    """
+    indexes = []
+    if substring_in_list(cloud.columns, tag) and (
+        (list_computed_layers is None)
+        or substring_in_list(list_computed_layers, tag)
+    ):
+        for key in cloud.columns:
+            if tag in key:
+                indexes.append(key)
+    return indexes
+
+
+def compute_vector_raster_and_stats(  # noqa: C901
     cloud: pandas.DataFrame,
     data_valid: np.ndarray,
     x_start: float,
     y_start: float,
     x_size: int,
     y_size: int,
     resolution: float,
@@ -225,15 +257,14 @@
     :param resolution: Resolution of rasterized cells,
         expressed in cloud CRS units or None.
     :param sigma: Sigma for gaussian interpolation. If None, set to resolution
     :param radius: Radius for hole filling.
     :param list_computed_layers: list of computed output data
     :return: a tuple with rasterization results and statistics.
     """
-
     # get points corresponding to (X, Y positions) + data_valid
     points = cloud.loc[:, [cst.X, cst.Y]].values.T
     valid = data_valid[np.newaxis, :]
     nb_points = points.shape[1]
 
     # create values: 1. altitudes and colors, 2. confidences, 3. masks
     # split_indexes allows to keep indexes separating values
@@ -246,51 +277,59 @@
         for band in cloud
         if str.find(band, cst.POINTS_CLOUD_CLR_KEY_ROOT) >= 0
     ]
     values_bands.extend(clr_bands)
     split_indexes.append(len(values_bands))
 
     # 2. confidences
-    confidences_indexes = []
-    if substring_in_list(cloud.columns, cst.POINTS_CLOUD_CONFIDENCE) and (
-        (list_computed_layers is None)
-        or substring_in_list(list_computed_layers, cst.POINTS_CLOUD_CONFIDENCE)
-    ):
-        for key in cloud.columns:
-            if cst.POINTS_CLOUD_CONFIDENCE in key:
-                confidences_indexes.append(key)
-                values_bands.append(key)
+    confidences_indexes = find_indexes_in_point_cloud(
+        cloud, cst.POINTS_CLOUD_CONFIDENCE, list_computed_layers
+    )
+    values_bands.extend(confidences_indexes)
     split_indexes.append(len(confidences_indexes))
 
     # 3. mask
-    msk_indexes = []
-    if substring_in_list(cloud.columns, cst.POINTS_CLOUD_MSK) and (
-        (list_computed_layers is None)
-        or substring_in_list(list_computed_layers, cst.POINTS_CLOUD_MSK)
-    ):
-        for key in cloud.columns:
-            if cst.POINTS_CLOUD_MSK in key:
-                msk_indexes.append(key)
-                values_bands.append(key)
+    msk_indexes = find_indexes_in_point_cloud(
+        cloud, cst.POINTS_CLOUD_MSK, list_computed_layers
+    )
+    values_bands.extend(msk_indexes)
     split_indexes.append(len(msk_indexes))
 
     # 4. classification
-    classif_indexes = []
-    if substring_in_list(cloud.columns, cst.POINTS_CLOUD_CLASSIF_KEY_ROOT) and (
+    classif_indexes = find_indexes_in_point_cloud(
+        cloud, cst.POINTS_CLOUD_CLASSIF_KEY_ROOT, list_computed_layers
+    )
+    values_bands.extend(classif_indexes)
+    split_indexes.append(len(classif_indexes))
+
+    # 5. source point cloud
+    # Fill the dataframe with additional column :
+    # each column refers to a point cloud id
+    if cst.POINTS_CLOUD_GLOBAL_ID in cloud.columns and (
         (list_computed_layers is None)
         or substring_in_list(
-            list_computed_layers, cst.POINTS_CLOUD_CLASSIF_KEY_ROOT
+            list_computed_layers, cst.POINTS_CLOUD_SOURCE_KEY_ROOT
         )
     ):
-        classif_indexes = []
+        number_of_pc = (
+            int(np.round(np.max(cloud[cst.POINTS_CLOUD_GLOBAL_ID]))) + 1
+        )
+        for pc_id in range(number_of_pc):
+            # Create binary list that indicates from each point whether it comes
+            # from point cloud number "pc_id"
+            point_is_from_pc = list(
+                map(int, cloud[cst.POINTS_CLOUD_GLOBAL_ID] == pc_id)
+            )
+            pc_key = "{}{}".format(cst.POINTS_CLOUD_SOURCE_KEY_ROOT, pc_id)
+            cloud[pc_key] = point_is_from_pc
 
-        for key in cloud.columns:
-            if cst.POINTS_CLOUD_CLASSIF_KEY_ROOT in key:
-                classif_indexes.append(key)
-                values_bands.append(key)
+    source_pc_indexes = find_indexes_in_point_cloud(
+        cloud, cst.POINTS_CLOUD_SOURCE_KEY_ROOT, list_computed_layers
+    )
+    values_bands.extend(source_pc_indexes)
 
     values = (
         cloud.loc[:, values_bands].values.T
         if len(values_bands) > 0
         else np.empty((0, nb_points))
     )
 
@@ -302,16 +341,17 @@
         y_start,
         x_size,
         y_size,
         resolution,
         radius,
         sigma,
     )
+
     # pylint: disable=unbalanced-tuple-unpacking
-    out, confidences, msk, classif = np.split(
+    out, confidences, msk, classif, source_pc = np.split(
         out, np.cumsum(split_indexes), axis=-1
     )
 
     confidences_out = None
     if len(confidences_indexes) > 0:
         confidences_out = {}
         for k, key in enumerate(confidences_indexes):
@@ -321,35 +361,31 @@
     if len(msk_indexes) > 0:
         msk_out = msk
 
     classif_out = None
     if len(classif_indexes) > 0:
         classif_out = classif
 
+    # Change values of source_pc to one if positive and 0 otherwise
+    source_pc_out = np.ceil(source_pc)
+
     return (
         out,
         mean,
         stdev,
         nb_pts_in_disc,
         nb_pts_in_cell,
         msk_out,
         classif_out,
         classif_indexes,
         confidences_out,
+        source_pc_out,
     )
 
 
-def substring_in_list(src_list, substring):
-    """
-    Check if the list contains substring
-    """
-    res = list(filter(lambda x: substring in x, src_list))
-    return len(res) > 0
-
-
 def create_raster_dataset(
     raster: np.ndarray,
     x_start: float,
     y_start: float,
     x_size: int,
     y_size: int,
     resolution: float,
@@ -361,14 +397,16 @@
     stdev: np.ndarray,
     n_pts: np.ndarray,
     n_in_cell: np.ndarray,
     msk: np.ndarray = None,
     classif: np.ndarray = None,
     band_classif: List[str] = None,
     confidences: np.ndarray = None,
+    source_pc: np.ndarray = None,
+    source_pc_names: List[str] = None,
 ) -> xr.Dataset:
     """
     Create final raster xarray dataset
 
     :param raster: height and colors
     :param x_start: x start of the rasterization grid
     :param y_start: y start of the rasterization grid
@@ -383,14 +421,17 @@
     :param mean: mean of height and colors
     :param stdev: standard deviation of height and colors
     :param n_pts: number of points that are stricty in a cell
     :param n_in_cell: number of points which contribute to a cell
     :param msk: raster msk
     :param classif: raster classif
     :param confidence_from_ambiguity: raster msk
+    :param source_pc: binary raster with source point cloud information
+    :param source_pc_names: list of names of points cloud before merging :
+        name of sensors pair or name of point cloud file
     :return: the raster xarray dataset
     """
     raster_dims = (cst.Y, cst.X)
     n_layers = raster.shape[-1]
     x_values_1d, y_values_1d = compute_values_1d(
         x_start, y_start, x_size, y_size, resolution
     )
@@ -437,14 +478,15 @@
     raster_out[cst.RASTER_NB_PTS_IN_CELL] = xr.DataArray(
         n_in_cell, dims=raster_dims
     )
 
     if msk is not None:
         msk = np.nan_to_num(msk, nan=msk_no_data)
         raster_out[cst.RASTER_MSK] = xr.DataArray(msk, dims=raster_dims)
+
     if classif is not None:
         if classif.shape[-1] > 1:  # rasterizer produced classif output
             classif = np.nan_to_num(classif, nan=msk_no_data)
             for idx, band_name in enumerate(band_classif):
                 band_classif[idx] = band_name.replace("classif_", "")
             classif_out = xr.Dataset(
                 {
@@ -457,14 +499,29 @@
             )
             # update raster output with classification data
             raster_out = xr.merge((raster_out, classif_out))
 
     if confidences is not None:
         for key in confidences:
             raster_out[key] = xr.DataArray(confidences[key], dims=raster_dims)
+
+    if source_pc is not None and source_pc_names is not None:
+        source_pc = np.nan_to_num(np.rollaxis(source_pc, 2), nan=msk_no_data)
+        source_pc_out = xr.Dataset(
+            {
+                cst.RASTER_SOURCE_PC: (
+                    [cst.BAND_SOURCE_PC, cst.Y, cst.X],
+                    source_pc,
+                )
+            },
+            coords={**raster_coords, cst.BAND_SOURCE_PC: source_pc_names},
+        )
+        # update raster output with classification data
+        raster_out = xr.merge((raster_out, source_pc_out))
+
     return raster_out
 
 
 def rasterize(
     cloud: pandas.DataFrame,
     resolution: float,
     epsg: int,
@@ -474,14 +531,15 @@
     y_size: int,
     sigma: float = None,
     radius: int = 1,
     hgt_no_data: int = -32768,
     color_no_data: int = 0,
     msk_no_data: int = 65535,
     list_computed_layers: List[str] = None,
+    source_pc_names: List[str] = None,
 ) -> Union[xr.Dataset, None]:
     """
     Rasterize a point cloud with its color bands to a Dataset
     that also contains quality statistics.
 
     :param cloud: Combined cloud
         as returned by the create_combined_cloud function
@@ -524,14 +582,15 @@
         stdev,
         n_pts,
         n_in_cell,
         msk,
         classif,
         band_list,
         confidences,
+        source_pc,
     ) = compute_vector_raster_and_stats(
         cloud,
         data_valid,
         x_start,
         y_start,
         x_size,
         y_size,
@@ -544,24 +603,29 @@
     # reshape data as a 2d grid.
     shape_out = (y_size, x_size)
     out = out.reshape(shape_out + (-1,))
     mean = mean.reshape(shape_out + (-1,))
     stdev = stdev.reshape(shape_out + (-1,))
     n_pts = n_pts.reshape(shape_out)
     n_in_cell = n_in_cell.reshape(shape_out)
+
     if classif is not None:
         classif = classif.reshape(shape_out + (-1,))
         classif = np.moveaxis(classif, 2, 0)
 
     if msk is not None:
         msk = msk.reshape(shape_out)
 
     if confidences is not None:
         for key in confidences:
             confidences[key] = confidences[key].reshape(shape_out)
+
+    if source_pc is not None:
+        source_pc = source_pc.reshape(shape_out + (-1,))
+
     # build output dataset
     raster_out = create_raster_dataset(
         out,
         x_start,
         y_start,
         x_size,
         y_size,
@@ -574,10 +638,12 @@
         stdev,
         n_pts,
         n_in_cell,
         msk,
         classif,
         band_list,
         confidences,
+        source_pc,
+        source_pc_names,
     )
 
     return raster_out
```

### Comparing `cars-0.7.0/cars/applications/rasterization/simple_gaussian.py` & `cars-0.7.1/cars/applications/rasterization/simple_gaussian.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         # Get if color, mask and stats are saved
         self.save_color = self.used_config["save_color"]
         self.save_stats = self.used_config["save_stats"]
         self.save_mask = self.used_config["save_msk"]
         self.save_classif = self.used_config["save_classif"]
         self.save_dsm = self.used_config["save_dsm"]
         self.save_confidence = self.used_config["save_confidence"]
+        self.save_source_pc = self.used_config["save_source_pc"]
 
         # Init orchestrator
         self.orchestrator = None
 
     def check_conf(self, conf):
         """
         Check configuration
@@ -137,14 +138,15 @@
         # Get if color, mask and stats are saved
         overloaded_conf["save_color"] = conf.get("save_color", True)
         overloaded_conf["save_stats"] = conf.get("save_stats", False)
         overloaded_conf["save_msk"] = conf.get("save_msk", False)
         overloaded_conf["save_classif"] = conf.get("save_classif", False)
         overloaded_conf["save_dsm"] = conf.get("save_dsm", True)
         overloaded_conf["save_confidence"] = conf.get("save_confidence", False)
+        overloaded_conf["save_source_pc"] = conf.get("save_source_pc", False)
 
         overloaded_conf["compute_all"] = conf.get("compute_all", False)
         if overloaded_conf["compute_all"]:
             # all the layers will computed
             self.list_computed_layers = None
         else:
             # only the saved layers will be saved
@@ -165,14 +167,15 @@
             "color_dtype": str,
             "save_color": bool,
             "save_msk": bool,
             "save_classif": bool,
             "save_stats": bool,
             "save_dsm": bool,
             "save_confidence": bool,
+            "save_source_pc": bool,
             "compute_all": bool,
         }
 
         # Check conf
         checker = Checker(rasterization_schema)
         checker.validate(overloaded_conf)
 
@@ -229,15 +232,15 @@
         logging.info(
             "Estimated optimal tile size for rasterization: {} meters".format(
                 tile_size
             )
         )
         return tile_size
 
-    def run(
+    def run(  # noqa: C901 function is too complex
         self,
         merged_points_cloud,
         epsg,
         orchestrator=None,
         dsm_file_name=None,
         color_file_name=None,
     ):
@@ -308,14 +311,21 @@
             xsize, ysize = tiling.roi_to_start_and_size(
                 bounds, self.resolution
             )[2:]
             logging.info(
                 "DSM output image size: {}x{} pixels".format(xsize, ysize)
             )
 
+            if self.save_source_pc:
+                source_pc_names = merged_points_cloud.attributes[
+                    "source_pc_names"
+                ]
+            else:
+                source_pc_names = None
+
             # Save objects
             # Initialize files names
             # TODO get from config ?
             out_dsm_file_name = None
             out_clr_file_name = None
             out_msk_file_name = None
             out_confidence = None
@@ -433,14 +443,27 @@
                     cst.RASTER_CONFIDENCE,
                     terrain_raster,
                     dtype=np.float32,
                     nodata=self.msk_no_data,
                     cars_ds_name="confidence",
                 )
 
+            if self.save_source_pc:
+                out_source_pc = os.path.join(
+                    self.orchestrator.out_dir, "source_pc.tif"
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_source_pc,
+                    cst.RASTER_SOURCE_PC,
+                    terrain_raster,
+                    dtype=np.float32,
+                    nodata=self.msk_no_data,
+                    cars_ds_name="source_pc",
+                )
+
             # Get saving infos in order to save tiles when they are computed
             [saving_info] = self.orchestrator.get_saving_infos([terrain_raster])
 
             # Generate profile
             geotransform = (
                 bounds[0],
                 self.resolution,
@@ -544,14 +567,15 @@
                             list_computed_layers=self.list_computed_layers,
                             saving_info=full_saving_info,
                             radius=self.dsm_radius,
                             sigma=self.sigma,
                             dsm_no_data=self.dsm_no_data,
                             color_no_data=self.color_no_data,
                             msk_no_data=self.msk_no_data,
+                            source_pc_names=source_pc_names,
                         )
 
             # Sort tiles according to rank TODO remove or implement it ?
 
         else:
             logging.error(
                 "PointsCloudRasterisation application doesn't support"
@@ -572,14 +596,15 @@
     list_computed_layers: List[str] = None,
     saving_info=None,
     sigma: float = None,
     radius: int = 1,
     dsm_no_data: int = np.nan,
     color_no_data: int = np.nan,
     msk_no_data: int = 65535,
+    source_pc_names=None,
 ):
     """
     Wrapper for rasterization step :
     - Convert a list of clouds to correct epsg
     - Rasterize it with associated colors
 
     :param cloud: combined cloud
@@ -598,14 +623,16 @@
     :type saving_info: dict
     :param sigma: sigma for gaussian interpolation.
         (If None, set to resolution)
     :param radius: Radius for hole filling.
     :param dsm_no_data: no data value to use in the final raster
     :param color_no_data: no data value to use in the final colored raster
     :param msk_no_data: no data value to use in the final mask image
+    :param source_pc_names: list of names of points cloud before merging :
+        name of sensors pair or name of point cloud file
     :return: digital surface model + projected colors
     :rtype: xr.Dataset
     """
 
     cloud_attributes = cars_dataset.get_attributes_dataframe(cloud)
     cloud_epsg = cloud_attributes["epsg"]
 
@@ -630,14 +657,15 @@
         ysize=ysize,
         sigma=sigma,
         radius=radius,
         dsm_no_data=dsm_no_data,
         color_no_data=color_no_data,
         msk_no_data=msk_no_data,
         list_computed_layers=list_computed_layers,
+        source_pc_names=source_pc_names,
     )
 
     # Fill raster
     if raster is not None:
         cars_dataset.fill_dataset(
             raster,
             saving_info=saving_info,
```

### Comparing `cars-0.7.0/cars/applications/resampling/__init__.py` & `cars-0.7.1/cars/applications/resampling/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/resampling/bicubic_resampling.py` & `cars-0.7.1/cars/applications/resampling/bicubic_resampling.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/resampling/resampling.py` & `cars-0.7.1/cars/applications/resampling/resampling.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/resampling/resampling_constants.py` & `cars-0.7.1/cars/applications/resampling/resampling_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/resampling/resampling_tools.py` & `cars-0.7.1/cars/applications/resampling/resampling_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/sparse_matching/__init__.py` & `cars-0.7.1/cars/applications/sparse_matching/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/sparse_matching/sift.py` & `cars-0.7.1/cars/applications/sparse_matching/sift.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/sparse_matching/sparse_matching.py` & `cars-0.7.1/cars/applications/sparse_matching/sparse_matching.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/sparse_matching/sparse_matching_constants.py` & `cars-0.7.1/cars/applications/sparse_matching/sparse_matching_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/sparse_matching/sparse_matching_tools.py` & `cars-0.7.1/cars/applications/sparse_matching/sparse_matching_tools.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -318,16 +318,16 @@
     mindisp = np.percentile(disparity, percent)
     maxdisp = np.percentile(disparity, 100 - percent)
 
     return mindisp, maxdisp
 
 
 def compute_disp_min_disp_max(
-    sensor_image_right,
     sensor_image_left,
+    sensor_image_right,
     grid_left,
     corrected_grid_right,
     grid_right,
     matches,
     orchestrator,
     geometry_loader,
     srtm_dir,
```

### Comparing `cars-0.7.0/cars/applications/triangulation/__init__.py` & `cars-0.7.1/cars/applications/triangulation/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/triangulation/line_of_sight_intersection.py` & `cars-0.7.1/cars/applications/triangulation/line_of_sight_intersection.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,16 +117,29 @@
             "method", "line_of_sight_intersection"
         )
         overloaded_conf["use_geoid_alt"] = conf.get("use_geoid_alt", False)
         overloaded_conf["snap_to_img1"] = conf.get("snap_to_img1", False)
         overloaded_conf["add_msk_info"] = conf.get("add_msk_info", True)
 
         # check geometry tool availability
+        geometry = "OTBGeometry"
+
+        # 1/ check otbApplication python module
         otb_app = importlib.util.find_spec("otbApplication")
-        geometry = "OTBGeometry" if otb_app is not None else "SharelocGeometry"
+        # 2/ check remote modules
+        if otb_app is not None:
+            otb_geometry = (
+                AbstractGeometry(  # pylint: disable=abstract-class-instantiated
+                    "OTBGeometry"
+                )
+            )
+            missing_remote = otb_geometry.check_otb_remote_modules()
+
+        if otb_app is None or len(missing_remote) > 0:
+            geometry = "SharelocGeometry"
 
         # Overloader loader
         overloaded_conf["geometry_loader"] = conf.get(
             "geometry_loader", geometry
         )
 
         # Saving files
```

### Comparing `cars-0.7.0/cars/applications/triangulation/triangulation.py` & `cars-0.7.1/cars/applications/triangulation/triangulation.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/triangulation/triangulation_constants.py` & `cars-0.7.1/cars/applications/triangulation/triangulation_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/applications/triangulation/triangulation_tools.py` & `cars-0.7.1/cars/applications/triangulation/triangulation_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/cars.py` & `cars-0.7.1/cars/cars.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/conf/__init__.py` & `cars-0.7.1/cars/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/conf/geoid/egm96.grd` & `cars-0.7.1/cars/conf/geoid/egm96.grd`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/conf/input_parameters.py` & `cars-0.7.1/cars/conf/input_parameters.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/conf/mask_cst.py` & `cars-0.7.1/cars/conf/mask_cst.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/__init__.py` & `cars-0.7.1/cars/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/cars_logging.py` & `cars-0.7.1/cars/core/cars_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,21 +173,18 @@
         if log_level == logging.DEBUG:
             formatter = logging.Formatter(
                 fmt="%(asctime)s :: %(module)s "
                 + ":: %(levelname)s :: %(thread)d "
                 + ":: %(process)d :: %(message)s",
                 datefmt="%y-%m-%d %H:%M:%S",
             )
-        now = datetime.now()
         if os.path.exists(log_dir):
             h_log_file = logging.FileHandler(
                 os.path.join(
                     log_dir,
-                    "{}_{}.log".format(
-                        now.strftime("%y-%m-%d_%Hh%Mm"), "workers"
-                    ),
-                ),
+                    "workers.log",
+                )
             )
             h_log_file.setFormatter(formatter)
             h_log_file.setLevel(log_level)
             cars_logger.addHandler(h_log_file)
             cars_logger.setLevel(log_level)
```

### Comparing `cars-0.7.0/cars/core/constants.py` & `cars-0.7.1/cars/core/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 # general
 ROW = "row"  # cannot be changed because of PANDORA input format
 COL = "col"  # cannot be changed because of PANDORA input format
 BAND = "band"
 BAND_IM = "band_im"
 BAND_CLASSIF = "classes"
+BAND_SOURCE_PC = "source_point_cloud"
 X = "x"
 Y = "y"
 Z = "z"
 RESOLUTION = "resolution"
 EPI_FULL_SIZE = "full_epipolar_size"
 ROI = "roi"
 ROI_WITH_MARGINS = "roi_with_margins"
@@ -64,17 +65,19 @@
 
 # points cloud fields (xarray Dataset and pandas Dataframe)
 POINTS_CLOUD_CORR_MSK = "corr_msk"
 POINTS_CLOUD_MSK = "msk"
 POINTS_CLOUD_VALID_DATA = "data_valid"
 POINTS_CLOUD_CLR_KEY_ROOT = "clr"
 POINTS_CLOUD_CLASSIF_KEY_ROOT = "classif"
+POINTS_CLOUD_SOURCE_KEY_ROOT = "source_pc"
 POINTS_CLOUD_COORD_EPI_GEOM_I = "coord_epi_geom_i"
 POINTS_CLOUD_COORD_EPI_GEOM_J = "coord_epi_geom_j"
-POINTS_CLOUD_IDX_IM_EPI = "idx_im_epi"
+POINTS_CLOUD_ID_IM_EPI = "id_im_epi"
+POINTS_CLOUD_GLOBAL_ID = "global_id"
 POINTS_CLOUD_MATCHES = "points_cloud_matches"
 POINTS_CLOUD_CONFIDENCE = "confidence"
 
 # raster fields (xarray Dataset)
 RASTER_HGT = "hgt"
 RASTER_COLOR_IMG = "img"
 RASTER_MSK = "raster_msk"
@@ -82,10 +85,11 @@
 RASTER_NB_PTS = "n_pts"
 RASTER_NB_PTS_IN_CELL = "pts_in_cell"
 RASTER_HGT_MEAN = "hgt_mean"
 RASTER_HGT_STD_DEV = "hgt_stdev"
 RASTER_BAND_MEAN = "band_mean"
 RASTER_BAND_STD_DEV = "band_stdev"
 RASTER_CONFIDENCE = "confidence"
+RASTER_SOURCE_PC = "source_pc"
 # Geometry constants
 DISP_MODE = "disp"
 MATCHES_MODE = "matches"
```

### Comparing `cars-0.7.0/cars/core/constants_disparity.py` & `cars-0.7.1/cars/core/constants_disparity.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/datasets.py` & `cars-0.7.1/cars/core/datasets.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/former_confs_utils.py` & `cars-0.7.1/cars/core/former_confs_utils.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/geometry/__init__.py` & `cars-0.7.1/cars/core/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/geometry/otb_geometry.py` & `cars-0.7.1/cars/core/geometry/otb_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,26 @@
             input_parameters.IMG1_TAG: And(str, inputs.rasterio_can_open),
             input_parameters.IMG2_TAG: And(str, inputs.rasterio_can_open),
         }
 
         return geo_conf_schema
 
     @staticmethod
+    def check_otb_remote_modules() -> List[str]:
+        """
+        Check all remote module compiled by cars
+        :return list of not available modules
+        """
+        not_available = []
+        for module in ["ConvertSensorToGeoPointFast", "EpipolarTriangulation"]:
+            if otbApplication.Registry.CreateApplication(module) is None:
+                not_available.append(module)
+        return not_available
+
+    @staticmethod
     def check_products_consistency(cars_conf) -> bool:
         """
         Test if the product is readable by the OTB
 
         :param: cars_conf: cars input configuration dictionary
         :return: True if the products are readable, False otherwise
         """
```

### Comparing `cars-0.7.0/cars/core/geometry/shareloc_geometry.py` & `cars-0.7.1/cars/core/geometry/shareloc_geometry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/inputs.py` & `cars-0.7.1/cars/core/inputs.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/otb_adapters.py` & `cars-0.7.1/cars/core/otb_adapters.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/outputs.py` & `cars-0.7.1/cars/core/outputs.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/preprocessing.py` & `cars-0.7.1/cars/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/projection.py` & `cars-0.7.1/cars/core/projection.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/roi_tools.py` & `cars-0.7.1/cars/core/roi_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/core/tiling.py` & `cars-0.7.1/cars/core/tiling.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,17 +533,19 @@
     :param terrain_tiling_grid: terrain grid positions
     :param row: row
     :param col: column
            epipolar input tiles where keys are image pairs index and values are
            epipolar_points_min, epipolar_points_max, largest_epipolar_region,
            opt_epipolar_tile_size
 
-    :return: Terrain regions, Corresponding tiles selected from
-             delayed_point_clouds and Terrain regions "rank" allowing to
-             sorting tiles for dask processing
+    :return: Terrain regions
+             Corresponding tiles selected from delayed_point_clouds with
+             associated id
+             Terrain regions "rank" allowing to sorting tiles for dask
+             processing
     """
 
     logging.debug(
         "Processing tile located at {},{} in tile grid".format(row, col)
     )
 
     # Terrain grid [row, j, :] = [xmin, xmax, ymin, ymax]
@@ -564,22 +566,24 @@
     # This list will hold the required points clouds for this terrain tile
     required_point_clouds = []
 
     # This list contains indexes of tiles (debug purpose)
     list_indexes = []
 
     # For each stereo configuration
-    for (
+    for pc_id, (
         points_cloud,
         epipolar_points_min,
         epipolar_points_max,
-    ) in zip(  # noqa: B905
-        list_points_clouds,
-        list_epipolar_points_min,
-        list_epipolar_points_max,
+    ) in enumerate(
+        zip(  # noqa: B905
+            list_points_clouds,
+            list_epipolar_points_min,
+            list_epipolar_points_max,
+        )
     ):
         largest_epipolar_region = points_cloud.attributes[
             "largest_epipolar_region"
         ]
         opt_epipolar_tile_size = points_cloud.attributes[
             "opt_epipolar_tile_size"
         ]
@@ -668,15 +672,17 @@
 
                 epi_grid_shape = points_cloud.tiling_grid.shape
 
                 if (
                     0 <= id_x < epi_grid_shape[1]
                     and 0 <= id_y < epi_grid_shape[0]
                 ):
-                    required_point_clouds.append(points_cloud[id_y, id_x])
+                    required_point_clouds.append(
+                        (points_cloud[id_y, id_x], pc_id)
+                    )
                     list_indexes.append([id_y, id_x])
 
     rank = col * col + row * row
 
     return (
         terrain_region,
         required_point_clouds,
```

### Comparing `cars-0.7.0/cars/core/utils.py` & `cars-0.7.1/cars/core/utils.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/data_structures/__init__.py` & `cars-0.7.1/cars/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/data_structures/cars_dataset.py` & `cars-0.7.1/cars/data_structures/cars_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1041,17 +1041,19 @@
         new_profile = DefaultGTiffProfile(count=new_profile["count"])
         new_profile["height"] = data.shape[0]
         new_profile["width"] = data.shape[1]
         new_profile["dtype"] = "float32"
 
     bands_description = None
     if tag in (cst.EPI_CLASSIFICATION, cst.RASTER_CLASSIF):
-        bands_description = dataset.coords["classes"].values
+        bands_description = dataset.coords[cst.BAND_CLASSIF].values
     if tag in (cst.EPI_COLOR, cst.POINTS_CLOUD_CLR_KEY_ROOT):
-        bands_description = dataset.coords["band_im"].values
+        bands_description = dataset.coords[cst.BAND_IM].values
+    if tag == cst.RASTER_SOURCE_PC:
+        bands_description = dataset.coords[cst.BAND_SOURCE_PC].values
 
     outputs.rasterio_write_georaster(
         file_name,
         data,
         new_profile,
         window=rio_window,
         descriptor=descriptor,
```

### Comparing `cars-0.7.0/cars/data_structures/cars_dict.py` & `cars-0.7.1/cars/data_structures/cars_dict.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/data_structures/corresponding_tiles_tools.py` & `cars-0.7.1/cars/data_structures/corresponding_tiles_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/data_structures/dataframe_converter.py` & `cars-0.7.1/cars/data_structures/dataframe_converter.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/data_structures/format_transformation.py` & `cars-0.7.1/cars/data_structures/format_transformation.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/__init__.py` & `cars-0.7.1/cars/orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/__init__.py` & `cars-0.7.1/cars/orchestrator/cluster/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 
 from . import (
     abstract_dask_cluster,
     local_dask_cluster,
     mp_cluster,
     pbs_dask_cluster,
     sequential_cluster,
+    slurm_dask_cluster,
 )
```

### Comparing `cars-0.7.0/cars/orchestrator/cluster/abstract_cluster.py` & `cars-0.7.1/cars/orchestrator/cluster/abstract_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/abstract_dask_cluster.py` & `cars-0.7.1/cars/orchestrator/cluster/abstract_dask_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/README.md` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/README.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/dask.yaml` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/dask.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/distributed.yaml` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/distributed.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/jobqueue.yaml` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/jobqueue.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/distributed.yaml` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/distributed.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/dask_config/reference_confs/jobqueue.yaml` & `cars-0.7.1/cars/orchestrator/cluster/dask_config/reference_confs/jobqueue.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/local_dask_cluster.py` & `cars-0.7.1/cars/orchestrator/cluster/local_dask_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/log_wrapper.py` & `cars-0.7.1/cars/orchestrator/cluster/log_wrapper.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/mp_cluster/__init__.py` & `cars-0.7.1/cars/orchestrator/cluster/mp_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/mp_cluster/mp_factorizer.py` & `cars-0.7.1/cars/orchestrator/cluster/mp_cluster/mp_factorizer.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/mp_cluster/mp_objects.py` & `cars-0.7.1/cars/orchestrator/cluster/mp_cluster/mp_objects.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/mp_cluster/mp_tools.py` & `cars-0.7.1/cars/orchestrator/cluster/mp_cluster/mp_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/mp_cluster/mp_wrapper.py` & `cars-0.7.1/cars/orchestrator/cluster/mp_cluster/mp_wrapper.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py` & `cars-0.7.1/cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 
             # Create pool
             self.pool = mp.get_context(mp_mode).Pool(
                 self.nb_workers,
                 initializer=freeze_support,
                 maxtasksperchild=100,
             )
+
             self.queue = Queue()
             self.task_cache = {}
 
             # Variable used for cleaning
             # Clone of iterator future list
             self.cl_future_list = []
 
@@ -128,14 +129,15 @@
                 args=(
                     self.pool,
                     self.task_cache,
                     self.queue,
                     self.per_job_timeout,
                     self.cl_future_list,
                     self.wrapper,
+                    self.nb_workers,
                 ),
             )
             self.refresh_worker.daemon = True
             self.refresh_worker._state = RUN
             self.refresh_worker.start()
 
     def check_conf(self, conf):
@@ -360,129 +362,148 @@
                     task_future, other_delayed_obj.return_index
                 )
 
         return object_future
 
     @staticmethod  # noqa: C901
     def refresh_task_cache(  # noqa: C901
-        pool, task_cache, in_queue, per_job_timeout, cl_future_list, wrapper_obj
+        pool,
+        task_cache,
+        in_queue,
+        per_job_timeout,
+        cl_future_list,
+        wrapper_obj,
+        nb_workers,
     ):
         """
         Refresh task cache
 
         :param task_cache: task cache list
         :param in_queue: queue
         :param per_job_timeout: per job timeout
         :param cl_future_list: current future list used in iterator
         :param wrapper_obj: wrapper (disk or None)
+        :param nb_workers:  number of workers
         :type wrapper_obj: AbstractWrapper
         """
         thread = threading.current_thread()
 
         # initialize lists
         wait_list = {}
         in_progress_list = {}
         dependances_list = {}
         done_task_results = {}
-
         while thread._state == RUN:  # pylint: disable=W0212
             # wait before next iteration
             time.sleep(REFRESH_TIME)
             # get new task from queue
             if not in_queue.empty():
-                # get all task from this batch
+                # get nb_workers task from this batch
                 for job_id, can_run, func, args, kw_args in iter(
                     in_queue.get, "END_BATCH"
                 ):
-                    if can_run:
+                    if can_run and len(in_progress_list) < nb_workers:
                         in_progress_list[job_id] = pool.apply_async(
                             func, args=args, kwds=kw_args
                         )
-                        # add to dependances
-                        dependances_list[job_id] = []
+                        # add to dependances (-1 to identify initial tasks)
+                        dependances_list[job_id] = [-1]
                     else:
                         # add to wait list
                         wait_list[job_id] = [func, args, kw_args]
                         # get dependances
                         dependances_list[job_id] = compute_dependances(
                             args, kw_args
                         )
+                        if len(dependances_list[job_id]) == 0:
+                            dependances_list[job_id] = [-1]
 
             # check for ready results
             done_list = []
+            next_priority_task = []
             for job_id, job_id_progress in in_progress_list.items():
                 if job_id_progress.ready():
                     try:
                         res = job_id_progress.get(timeout=per_job_timeout)
                         success = True
                     except:  # pylint: disable=W0702 # noqa: B001, E722
                         res = traceback.format_exc()
                         success = False
                         logging.error("Exception in worker: {}".format(res))
                     done_list.append(job_id)
                     done_task_results[job_id] = [success, res]
+
                     # remove from dependance list
                     dependances_list.pop(job_id)
 
+                # search related priority task
+                for job_id2 in wait_list.keys():  # pylint: disable=C0201
+                    depending_tasks = list(dependances_list[job_id2])
+                    if job_id in depending_tasks:
+                        next_priority_task += depending_tasks
+            # remove duplicate dependance task
+            next_priority_task = list(dict.fromkeys(next_priority_task))
+
             # clean done jobs
             for job_id in done_list:
                 # delete
                 del in_progress_list[job_id]
                 # copy results to futures
                 # (they remove themselves from task_cache
                 task_cache[job_id].set(done_task_results[job_id])
 
-            # check wait_list for dependent tasks
+            (
+                ready_list,
+                failed_list,
+            ) = MultiprocessingCluster.get_ready_failed_tasks(
+                wait_list, dependances_list, done_task_results
+            )
 
-            ready_list = []
-            failed_list = []
-            done_task_result_keys = done_task_results.keys()
-            for job_id in wait_list.keys():  # pylint: disable=C0201
-                depending_tasks = dependances_list[job_id]
-                # check if all tasks are finished
-                can_run = True
-                failed = False
-                for depend in depending_tasks:
-                    if depend not in done_task_result_keys:
-                        can_run = False
-                    else:
-                        if not done_task_results[depend][0]:
-                            # not a success
-                            can_run = False
-                            failed = True
-
-                if failed:
-                    # Add to done list with failed status
-                    failed_list.append(job_id)
-                if can_run:
-                    ready_list.append(job_id)
+            priority_list = []
+            nb_ready_task = nb_workers - len(priority_list)
+
+            priority_list += MultiprocessingCluster.get_tasks_without_deps(
+                dependances_list, ready_list, nb_ready_task
+            )
+            # add ready task in next_priority_task
+            priority_list += list(
+                filter(lambda job_id: job_id in next_priority_task, ready_list)
+            )
+            # if the priority task have finished
+            # continue with the rest of task (initial task)
+            if len(priority_list) == 0:
+                priority_list += ready_list
+            priority_list = list(dict.fromkeys(priority_list))
 
             # Deal with failed tasks
             for job_id in failed_list:
                 done_list.append(job_id)
                 done_task_results[job_id] = [
                     False,
                     "Failed depending task",
                 ]
                 # copy results to futures
                 # (they remove themselves from task_cache
                 task_cache[job_id].set(done_task_results[job_id])
                 del wait_list[job_id]
 
             # launch tasks ready to run
-            for job_id in ready_list:
-                func, args, kw_args = wait_list[job_id]
-                # replace jobs by real data
-                new_args = replace_job_by_data(args, done_task_results)
-                new_kw_args = replace_job_by_data(kw_args, done_task_results)
-                # launch task
-                in_progress_list[job_id] = pool.apply_async(
-                    func, args=new_args, kwds=new_kw_args
-                )
-                del wait_list[job_id]
+            for job_id in priority_list:
+                if len(in_progress_list) < nb_workers:
+                    func, args, kw_args = wait_list[job_id]
+                    # replace jobs by real data
+                    new_args = replace_job_by_data(args, done_task_results)
+                    new_kw_args = replace_job_by_data(
+                        kw_args, done_task_results
+                    )
+                    # launch task
+                    in_progress_list[job_id] = pool.apply_async(
+                        func, args=new_args, kwds=new_kw_args
+                    )
+                    del wait_list[job_id]
 
             # find done jobs that can be cleaned
             cleanable_jobid = []
 
             for job_id in done_task_results.keys():  # pylint: disable=C0201
                 # check if needed
                 still_need = False
@@ -501,14 +522,63 @@
                     # Cleanup with wrapper
                     wrapper_obj.cleanup_future_res(
                         done_task_results[job_id_to_clean][1]
                     )
                     # cleanup list
                     done_task_results.pop(job_id_to_clean)
 
+    @staticmethod
+    def get_ready_failed_tasks(wait_list, dependances_list, done_task_results):
+        """
+        Return the new ready tasks without constraint
+        and failed tasks
+        """
+        ready_list = []
+        failed_list = []
+        done_task_result_keys = done_task_results.keys()
+        for job_id in wait_list.keys():  # pylint: disable=C0201
+            depending_tasks = dependances_list[job_id]
+            # check if all tasks are finished
+            can_run = True
+            failed = False
+            for depend in list(filter(lambda dep: dep != -1, depending_tasks)):
+                if depend not in done_task_result_keys:
+                    can_run = False
+                else:
+                    if not done_task_results[depend][0]:
+                        # not a success
+                        can_run = False
+                        failed = True
+            if failed:
+                # Add to done list with failed status
+                failed_list.append(job_id)
+            if can_run:
+                ready_list.append(job_id)
+        return ready_list, failed_list
+
+    @staticmethod
+    def get_tasks_without_deps(dependances_list, ready_list, nb_ready_task):
+        """
+        Return the list of ready tasks without dependances
+        and not considered like initial task (dependance = -1)
+        """
+        priority_list = []
+        for _ in range(nb_ready_task):
+            task_id = next(
+                filter(
+                    lambda job_id: len(dependances_list[job_id]) != 1
+                    and dependances_list[job_id][0] != -1,
+                    ready_list,
+                ),
+                None,
+            )
+            if task_id:
+                priority_list.append(task_id)
+        return priority_list
+
     def future_iterator(self, future_list):
         """
         Start all tasks
 
         :param future_list: future_list list
         """
 
@@ -628,15 +698,15 @@
                 list_ids.append(current_id)
 
         return list_ids
 
     # compute dependances
     dependances = get_ids_rec(args) + get_ids_rec(kw_args)
 
-    return dependances
+    return list(dict.fromkeys(dependances))
 
 
 class MpFutureTask:  # pylint: disable=R0903
     """
     multiprocessing version of distributed.future
     """
```

### Comparing `cars-0.7.0/cars/orchestrator/cluster/pbs_dask_cluster.py` & `cars-0.7.1/cars/orchestrator/cluster/dask_jobqueue_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,128 +15,67 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-Contains abstract function for PBS dask Cluster
+Contains functions for dask jobqueue cluster (PBS, SLURM)
 """
 
-# Standard imports
 import logging
 import math
 import os
 import sys
 import warnings
 from datetime import timedelta
 
-# Third party imports
-from dask.distributed import Client
 
-with warnings.catch_warnings():
-    # Ignore some internal dask_jobqueue warnings
-    warnings.filterwarnings(
-        "ignore",
-        category=FutureWarning,
-        message=".*format_bytes is deprecated.*",
-    )
-    warnings.filterwarnings(
-        "ignore",
-        category=FutureWarning,
-        message=".*parse_bytes is deprecated.*",
-    )
-    warnings.filterwarnings(
-        "ignore",
-        category=FutureWarning,
-        message=".*tmpfile is deprecated.*",
-    )
-    from dask_jobqueue import PBSCluster
-
-# CARS imports
-from cars.orchestrator.cluster import abstract_cluster, abstract_dask_cluster
-
-
-@abstract_cluster.AbstractCluster.register_subclass("pbs_dask")
-class PbsDaskCluster(abstract_dask_cluster.AbstractDaskCluster):
+def init_cluster_variables(
+    nb_workers, walltime, out_dir, activate_dashboard, python, core_memory
+):
     """
-    PbsDaskCluster
+    Initialize global cluster variables
+    :param nb_workers: number of workers
+    :param walltime: workers walltime
+    :param out_dir: ouput result directory
+    :param activate_dashboard: option to activate dashboard mode
+    :param python: target python used by workers (retrun system python if None)
+    :param core_memory: cluster node memory (Mo)
+    :return: all cluster parameters (python,
+    nb_workers_per_job,
+    memory,
+    nb_cpus,
+    stagger,
+    lifetime_with_margin,
+    scheduler_options,
+    envs,
+    log_directory,
+    local_directory)
     """
 
-    def start_dask_cluster(self):
-        """
-        Start dask cluster
-        """
-
-        return start_cluster(
-            self.nb_workers,
-            self.walltime,
-            self.out_dir,
-            activate_dashboard=self.activate_dashboard,
-            python=self.python,
-        )
-
-    def cleanup(self):
-        """
-        Cleanup cluster
-
-        """
-        stop_cluster(self.cluster, self.client)
-        logging.info("Dask cluster closed")
-
-
-def start_cluster(
-    nb_workers,
-    walltime,
-    out_dir,
-    timeout=600,
-    activate_dashboard=False,
-    python=None,
-):
-    """Create a Dask cluster.
-
-    Each worker will be spawned in an independent job with a single CPU
-    allocated to it, and will use a single process. This is done to maximize
-    CPU utilization and minimize scheduling delay.
-
-    The CARS_PBS_QUEUE environment variable, if defined, is used to specify the
-    queue in which worker jobs are scheduled.
-
-    :param nb_workers: Number of dask workers
-    :type nb_workers: int
-    :param walltime: Walltime for each dask worker
-    :type walltime: string
-    :param out_dir: Output directory
-    :type out_dir: string
-    :return: Dask cluster and dask client
-    :rtype: (dask_jobqueue.PBSCluster, dask.distributed.Client) tuple
-    """
-    # retrieve current python path if None
     if python is None:
         python = sys.executable
 
-    # Retrieve PBS queue
-    pbs_queue = os.environ.get("CARS_PBS_QUEUE")
-
     # Configure worker distribution.
     # Workers are mostly running single-threaded, GIL-holding functions, so we
     # dedicate a single thread for each worker to maximize CPU utilization.
     nb_threads_per_worker = 1
 
     # Network latency is not the bottleneck, so we dedicate a single worker for
     # each job in order to minimize the requested resources, which reduces our
     # scheduling delay.
     nb_workers_per_job = 1
 
     # Total number of CPUs is multi-threading factor times size of batch
     # (number of workers per job)
     nb_cpus = nb_threads_per_worker * nb_workers_per_job
     nb_jobs = int(math.ceil(nb_workers / nb_workers_per_job))
-    # Cluster nodes have 5GB per core
-    memory = nb_cpus * 5000
+    # Cluster nodes have core_memory Mo per core
+    memory = nb_cpus * core_memory
 
     # Configure worker lifetime for adaptative scaling.
     # See https://jobqueue.dask.org/en/latest/advanced-tips-and-tricks.html
     hours, minutes, seconds = map(int, walltime.split(":"))
     lifetime = timedelta(seconds=3600 * hours + 60 * minutes + seconds)
     # Use hardcoded stagger of 3 minutes. The actual lifetime will be selected
     # uniformly at random between lifetime +/- stagger.
@@ -145,31 +84,31 @@
     shutdown_margin = timedelta(minutes=2)
     min_walltime = stagger + shutdown_margin
     lifetime_with_margin = lifetime - min_walltime
     if lifetime_with_margin.total_seconds() < 0:
         min_walltime_minutes = min_walltime.total_seconds() / 60
         logging.warning(
             "Could not add worker lifetime margin because specified walltime "
-            "is too short. Workers might get killed by PBS before they can "
+            "is too short. Workers might get killed by SLURM before they can "
             "cleanly exit, which might break adaptative scaling. Please "
             "specify a lifetime greater than {} minutes.".format(
                 min_walltime_minutes
             )
         )
         lifetime_with_margin = lifetime
 
     logging.info(
-        "Starting Dask PBS cluster with {} workers "
-        "({} workers with {} cores each per PBS job)".format(
+        "Starting Dask SLURM cluster with {} workers "
+        "({} workers with {} cores each per SLURM job)".format(
             nb_workers, nb_workers_per_job, nb_threads_per_worker
         )
     )
 
     logging.info(
-        "Submitting {} PBS jobs "
+        "Submitting {} SLURM jobs "
         "with configuration cpu={}, mem={}, walltime={}".format(
             nb_jobs, nb_cpus, memory, walltime
         )
     )
 
     if activate_dashboard:
         scheduler_options = None
@@ -193,60 +132,26 @@
         "DASK_CONFIG",
         "NUMBA_THREADING_LAYER",
     ]
     names = [name for name in names if os.environ.get(name)]
     envs = ["export {}={}".format(name, os.environ[name]) for name in names]
     log_directory = os.path.join(os.path.abspath(out_dir), "dask_log")
     local_directory = "$TMPDIR"
-    with warnings.catch_warnings():
-        # Ignore some internal dask_jobqueue warnings
-        # TODO remove when Future warning do not exist anymore
-        warnings.filterwarnings(
-            "ignore",
-            category=FutureWarning,
-            message=".*extra has been renamed to worker_extra_args*",
-        )
-        warnings.filterwarnings(
-            "ignore",
-            category=FutureWarning,
-            message=".*job_extra has been renamed to job_extra_directives*",
-        )
-        warnings.filterwarnings(
-            "ignore",
-            category=FutureWarning,
-            message=".*env_extra has been renamed to job_script_prologue*",
-        )
-        cluster = PBSCluster(
-            processes=nb_workers_per_job,
-            cores=nb_workers_per_job,
-            memory="{}MiB".format(memory),
-            local_directory=local_directory,
-            account="dask-test",
-            walltime=walltime,
-            interface="ib0",
-            queue=pbs_queue,
-            job_script_prologue=envs,
-            log_directory=log_directory,
-            python=python,
-            worker_extra_args=[
-                "--lifetime",
-                f"{int(lifetime_with_margin.total_seconds())}s",
-                "--lifetime-stagger",
-                f"{int(stagger.total_seconds())}s",
-            ],
-            scheduler_options=scheduler_options,
-            resource_spec="select=1:ncpus={}:mem={}MB".format(nb_cpus, memory),
-        )
-        logging.info("Dask cluster started")
-        cluster.adapt(minimum=nb_workers, maximum=nb_workers)
-        client = Client(cluster, timeout=timeout)
-        logging.info(
-            "Dashboard started at {}".format(get_dashboard_link(cluster))
-        )
-    return cluster, client
+    return (
+        python,
+        nb_workers_per_job,
+        memory,
+        nb_cpus,
+        stagger,
+        lifetime_with_margin,
+        scheduler_options,
+        envs,
+        log_directory,
+        local_directory,
+    )
 
 
 def get_dashboard_link(cluster):
     """
     This function returns the dashboard address.
 
     :param cluster: Dask cluster
```

### Comparing `cars-0.7.0/cars/orchestrator/cluster/sequential_cluster.py` & `cars-0.7.1/cars/orchestrator/cluster/sequential_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/orchestrator.py` & `cars-0.7.1/cars/orchestrator/orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 
 # Standard imports
 import collections
 import logging
 import os
 import shutil
 import sys
-import traceback
 
 # Third party imports
+import tempfile
+import traceback
+
 from tqdm import tqdm
 
 # CARS imports
 from cars.core.cars_logging import add_progress_message
 from cars.data_structures import cars_dataset
 from cars.orchestrator.cluster.abstract_cluster import AbstractCluster
 from cars.orchestrator.orchestrator_constants import CARS_DS_COL, CARS_DS_ROW
@@ -60,20 +62,23 @@
         """
         Init function of Orchestrator.
         Creates Cluster and Registry for CarsDatasets
 
         :param orchestrator_conf: configuration of distribution
 
         """
+        # init list of path to clean at the end
+        self.tmp_dir_list = []
 
         # out_dir
         if out_dir is not None:
             self.out_dir = out_dir
         else:
-            self.out_dir = os.path.join("/tmp/", "cars_tmp_dir")
+            self.out_dir = tempfile.mkdtemp()
+            self.add_to_clean(self.out_dir)
             logging.debug("No out_dir defined")
 
         self.launch_worker = launch_worker
 
         # overload orchestrator_conf
         if orchestrator_conf is None:
             orchestrator_conf = {"mode": "local_dask"}
@@ -102,17 +107,14 @@
         self.cars_ds_replacer_registry = (
             replacer_registry.CarsDatasetRegistryReplacer(self.id_generator)
         )
 
         # init cars_ds_names_info for pbar printing
         self.cars_ds_names_info = []
 
-        # init list of path to clean at the end
-        self.tmp_dir_list = []
-
         # outjson
         self.out_json_path = out_json_path
         if self.out_json_path is None:
             os.path.join(self.out_dir, "content.json")
         self.out_json = {}
 
     def add_to_clean(self, tmp_dir):
```

### Comparing `cars-0.7.0/cars/orchestrator/orchestrator_constants.py` & `cars-0.7.1/cars/orchestrator/orchestrator_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/registry/__init__.py` & `cars-0.7.1/cars/orchestrator/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/registry/abstract_registry.py` & `cars-0.7.1/cars/orchestrator/registry/abstract_registry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/registry/id_generator.py` & `cars-0.7.1/cars/orchestrator/registry/id_generator.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/registry/replacer_registry.py` & `cars-0.7.1/cars/orchestrator/registry/replacer_registry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/registry/saver_registry.py` & `cars-0.7.1/cars/orchestrator/registry/saver_registry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/orchestrator/registry/unseen_registry.py` & `cars-0.7.1/cars/orchestrator/registry/unseen_registry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/__init__.py` & `cars-0.7.1/cars/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/conf_pipeline/__init__.py` & `cars-0.7.1/cars/pipelines/conf_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/pipeline.py` & `cars-0.7.1/cars/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/pipeline_constants.py` & `cars-0.7.1/cars/pipelines/pipeline_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/pipeline_template.py` & `cars-0.7.1/cars/pipelines/pipeline_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 # limitations under the License.
 #
 """
 This module contains class pipeline template for
 templating the pipeline concept.
 """
 
-import os
-import tempfile
 from abc import ABCMeta, abstractmethod
 
 from json_checker import Checker, OptionalKey
 
 # CARS imports
 from cars.orchestrator import orchestrator
 from cars.pipelines import pipeline_constants
@@ -47,20 +45,19 @@
 
         :param conf: configuration of orchestrator
         :type conf: dict
         :return: overloaded orchestrator conf
         :rtype: dict
         """
 
-        with tempfile.TemporaryDirectory(dir=os.getcwd()) as directory:
-            with orchestrator.Orchestrator(
-                orchestrator_conf=conf, out_dir=directory, launch_worker=False
-            ) as orchestrator_obj:
-                conf = orchestrator_obj.get_conf()
-            return conf
+        with orchestrator.Orchestrator(
+            orchestrator_conf=conf, out_dir=None, launch_worker=False
+        ) as orchestrator_obj:
+            conf = orchestrator_obj.get_conf()
+        return conf
 
     def check_global_schema(self, conf):
         """
         Check the given global configuration
 
         :param conf: configuration
         :type conf: dict
```

### Comparing `cars-0.7.0/cars/pipelines/point_clouds_to_dsm/__init__.py` & `cars-0.7.1/cars/pipelines/point_clouds_to_dsm/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/point_clouds_to_dsm/pc_constants.py` & `cars-0.7.1/cars/pipelines/point_clouds_to_dsm/pc_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/point_clouds_to_dsm/pc_inputs.py` & `cars-0.7.1/cars/pipelines/point_clouds_to_dsm/pc_inputs.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/point_clouds_to_dsm/point_cloud_to_dsm_pipeline.py` & `cars-0.7.1/cars/pipelines/point_clouds_to_dsm/point_cloud_to_dsm_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,15 @@
                     self.inputs["point_clouds"]
                 )
             # Compute roi polygon, in input EPSG
             roi_poly = preprocessing.compute_roi_poly(
                 self.input_roi_poly, self.input_roi_epsg, epsg
             )
 
-            # compute terrain bounds and transform point clouds
+            # Compute terrain bounds and transform point clouds
             (
                 terrain_bounds,
                 list_epipolar_points_cloud_by_tiles,
             ) = pc_tif_tools.transform_input_pc(
                 self.inputs["point_clouds"],
                 epsg,
                 roi_poly=roi_poly,
@@ -341,14 +341,18 @@
                             max_number_superposing_point_clouds
                         ),
                         point_cloud_resolution=average_distance_point_cloud,
                     ),
                 ),
             )
 
+            # Add file names to retrieve source file of each point
+            pc_file_names = list(self.inputs["point_clouds"])
+            merged_points_clouds.attributes["source_pc_names"] = pc_file_names
+
             # Remove outliers with small components method
             filtered_1_merged_points_clouds = (
                 self.pc_outliers_removing_1_app.run(
                     merged_points_clouds,
                     orchestrator=cars_orchestrator,
                 )
             )
```

### Comparing `cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/__init__.py` & `cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/dsm_output.py` & `cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/dsm_output.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/sensor_dense_dsm_constants.py` & `cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/sensor_dense_dsm_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/sensor_to_dense_dsm_pipeline.py` & `cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/sensor_to_dense_dsm_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
                     )
                     # Compute roi polygon, in input EPSG
                     roi_poly = preprocessing.compute_roi_poly(
                         self.input_roi_poly, self.input_roi_epsg, epsg
                     )
 
                 # Run epipolar triangulation application
-                (epipolar_points_cloud) = self.triangulation_application.run(
+                epipolar_points_cloud = self.triangulation_application.run(
                     sensor_image_left,
                     sensor_image_right,
                     new_epipolar_image_left,
                     grid_left,
                     corrected_grid_right,
                     filled_with_2_epipolar_disparity_map,
                     epsg,
@@ -848,14 +848,20 @@
                             )
                         )
                         + self.rasterization_application.get_margins()
                     ),
                     optimal_terrain_tile_width=optimal_terrain_tile_width,
                 )
 
+                # Add pair names to retrieve source pair of each point
+                pairs_names = [
+                    pair_name for pair_name, _, _ in list_sensor_pairs
+                ]
+                merged_points_clouds.attributes["source_pc_names"] = pairs_names
+
                 # Remove outliers with small components method
                 filtered_1_merged_points_clouds = (
                     self.pc_outliers_removing_1_app.run(
                         merged_points_clouds,
                         orchestrator=cars_orchestrator,
                     )
                 )
```

### Comparing `cars-0.7.0/cars/pipelines/sensor_to_dense_dsm/sensors_inputs.py` & `cars-0.7.1/cars/pipelines/sensor_to_dense_dsm/sensors_inputs.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/sensor_to_sparse_dsm/__init__.py` & `cars-0.7.1/cars/pipelines/sensor_to_sparse_dsm/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/cars/pipelines/sensor_to_sparse_dsm/sensor_to_sparse_dsm_pipeline.py` & `cars-0.7.1/cars/pipelines/sensor_to_sparse_dsm/sensor_to_sparse_dsm_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,14 +528,18 @@
                 terrain_bounds,
                 epsg,
                 orchestrator=cars_orchestrator,
                 margins=self.rasterization_application.get_margins(),
                 optimal_terrain_tile_width=optimal_terrain_tile_width,
             )
 
+            # Add pair names to retrieve source pair of each point
+            pairs_names = [pair_name for pair_name, _, _ in list_sensor_pairs]
+            merged_points_clouds.attributes["source_pc_names"] = pairs_names
+
             # rasterize point cloud
             _ = self.rasterization_application.run(
                 merged_points_clouds,
                 epsg,
                 orchestrator=cars_orchestrator,
                 dsm_file_name=os.path.join(
                     self.used_conf[OUTPUT]["out_dir"],
```

### Comparing `cars-0.7.0/cars.egg-info/PKG-INFO` & `cars-0.7.1/cars.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cars
-Version: 0.7.0
+Version: 0.7.1
 Summary: A satellite multi view stereo pipeline
 Home-page: https://cars.readthedocs.io/
 Author: CNES
 Author-email: cars@cnes.fr
 License: Apache License 2.0
 Project-URL: Source, https://github.com/CNES/cars
 Project-URL: Documentation, https://cars.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cars Version: 0.7.0 Summary: A satellite multi view
+Metadata-Version: 2.1 Name: cars Version: 0.7.1 Summary: A satellite multi view
 stereo pipeline Home-page: https://cars.readthedocs.io/ Author: CNES Author-
 email: cars@cnes.fr License: Apache License 2.0 Project-URL: Source, https://
 github.com/CNES/cars Project-URL: Documentation, https://cars.readthedocs.io/
 en/latest/ Keywords: cars,3D,DEM,pandora,photogrammetry Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 Intended Audience :: Science/Research Classifier: Environment :: Console
```

### Comparing `cars-0.7.0/cars.egg-info/SOURCES.txt` & `cars-0.7.1/cars.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 .readthedocs.yaml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 Dockerfile
 Dockerfile.deps
 Dockerfile.jupyter
-Dockerfile.tutorial
 LICENSE
 MANIFEST.in
 Makefile
 NOTICE
 README.md
 env_cars.sh
 gdal-config
@@ -126,18 +125,20 @@
 cars/data_structures/format_transformation.py
 cars/orchestrator/__init__.py
 cars/orchestrator/orchestrator.py
 cars/orchestrator/orchestrator_constants.py
 cars/orchestrator/cluster/__init__.py
 cars/orchestrator/cluster/abstract_cluster.py
 cars/orchestrator/cluster/abstract_dask_cluster.py
+cars/orchestrator/cluster/dask_jobqueue_utils.py
 cars/orchestrator/cluster/local_dask_cluster.py
 cars/orchestrator/cluster/log_wrapper.py
 cars/orchestrator/cluster/pbs_dask_cluster.py
 cars/orchestrator/cluster/sequential_cluster.py
+cars/orchestrator/cluster/slurm_dask_cluster.py
 cars/orchestrator/cluster/dask_config/README.md
 cars/orchestrator/cluster/dask_config/dask.yaml
 cars/orchestrator/cluster/dask_config/distributed.yaml
 cars/orchestrator/cluster/dask_config/jobqueue.yaml
 cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml
 cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml
 cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml
```

### Comparing `cars-0.7.0/cars.egg-info/requires.txt` & `cars-0.7.1/cars.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 numpy>=1.17.0
 scipy!=1.10.0,>=1.7.1
 matplotlib
 affine
-rasterio>=1.1.3
+rasterio>=1.3.0
 dask>=2021.10.0
 distributed>=2021.10.0
 dask-jobqueue>=0.7.3
 json-checker
 xarray
 tqdm
 netCDF4>=1.5.3
@@ -36,15 +36,15 @@
 flake8-bugbear>=21.4.3
 jupyter_contrib_nbextensions
 pylint>=2.8.2
 setuptools_scm
 virtualenv
 configupdater
 twine
-notebook
+notebook<7.0.0
 bokeh==2.4.3
 sphinx
 sphinx-rtd-theme
 graphviz
 memory_profiler
 memray
```

### Comparing `cars-0.7.0/env_cars.sh` & `cars-0.7.1/env_cars.sh`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/gdal-config` & `cars-0.7.1/gdal-config`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/otb_remote_module/app/otbConvertSensorToGeoPointFast.cxx` & `cars-0.7.1/otb_remote_module/app/otbConvertSensorToGeoPointFast.cxx`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/otb_remote_module/app/otbEpipolarTriangulation.cxx` & `cars-0.7.1/otb_remote_module/app/otbEpipolarTriangulation.cxx`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/otb_remote_module/data/rectified_ref.tif` & `cars-0.7.1/otb_remote_module/data/rectified_ref.tif`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/otb_remote_module/data/rectified_ref_mask.tif` & `cars-0.7.1/otb_remote_module/data/rectified_ref_mask.tif`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/otb_remote_module/data/rectified_sec.tif` & `cars-0.7.1/otb_remote_module/data/rectified_sec.tif`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/otb_remote_module/data/rectified_sec_mask.tif` & `cars-0.7.1/otb_remote_module/data/rectified_sec_mask.tif`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.h` & `cars-0.7.1/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.h`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.hxx` & `cars-0.7.1/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.hxx`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/setup.cfg` & `cars-0.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 	wheel
 	setuptools_scm[toml]>=6.2 # Following https://pypi.org/project/setuptools-scm/
 install_requires = 
 	numpy>=1.17.0
 	scipy>=1.7.1,!=1.10.0
 	matplotlib
 	affine
-	rasterio>=1.1.3
+	rasterio>=1.3.0
 	dask>=2021.10.0
 	distributed>=2021.10.0
 	dask-jobqueue>=0.7.3
 	json-checker
 	xarray
 	tqdm
 	netCDF4>=1.5.3
@@ -76,15 +76,15 @@
 	flake8-bugbear>=21.4.3        # Add some rules to flake8
 	jupyter_contrib_nbextensions  # Clean notebooks
 	pylint>=2.8.2                 # General linter with more rules
 	setuptools_scm                # version from git tag
 	virtualenv
 	configupdater
 	twine                         # for pypi upload
-	notebook                      # for pytest test_notebooks.py
+	notebook<7.0.0                # for pytest test_notebooks.py
 	bokeh==2.4.3                  # for pytest test_notebooks.py
 	sphinx                        # for cars doc
 	sphinx-rtd-theme              # for cars doc
 	graphviz                      # for cars doc
 	memory_profiler
 	memray
 docs =
```

### Comparing `cars-0.7.0/setup.py` & `cars-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.0/sonar-project.properties` & `cars-0.7.1/sonar-project.properties`

 * *Files identical despite different names*

