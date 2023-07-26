# Comparing `tmp/pyrfuniverse-0.9.10.tar.gz` & `tmp/pyrfuniverse-0.9.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfuniverse-0.9.10.tar", last modified: Mon Jul  3 04:47:49 2023, max compression
+gzip compressed data, was "pyrfuniverse-0.9.11.tar", last modified: Wed Jul 26 07:52:45 2023, max compression
```

## Comparing `pyrfuniverse-0.9.10.tar` & `pyrfuniverse-0.9.11.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.577521 pyrfuniverse-0.9.10/
--rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.9.10/LICENSE
--rw-rw-rw-   0        0        0      266 2023-07-03 04:47:49.577521 pyrfuniverse-0.9.10/PKG-INFO
--rw-rw-rw-   0        0        0     2758 2023-06-21 09:17:40.000000 pyrfuniverse-0.9.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.499034 pyrfuniverse-0.9.10/pyrfuniverse/
--rw-rw-rw-   0        0        0      759 2023-07-03 04:47:38.000000 pyrfuniverse-0.9.10/pyrfuniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.526229 pyrfuniverse-0.9.10/pyrfuniverse/attributes/
--rw-rw-rw-   0        0        0     1472 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-06-27 09:24:35.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/activelightsensor_attr.py
--rw-rw-rw-   0        0        0     8532 2023-06-26 07:46:59.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/base_attr.py
--rw-rw-rw-   0        0        0     8438 2023-06-27 09:30:40.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/camera_attr.py
--rw-rw-rw-   0        0        0      384 2023-06-26 03:15:33.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/cloth_attr.py
--rw-rw-rw-   0        0        0      601 2023-06-26 02:35:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/collider_attr.py
--rw-rw-rw-   0        0        0    15137 2023-07-03 03:38:52.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/controller_attr.py
--rw-rw-rw-   0        0        0      622 2023-06-26 02:41:17.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/custom_attr.py
--rw-rw-rw-   0        0        0      678 2023-06-26 03:18:21.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/digit_attr.py
--rw-rw-rw-   0        0        0      871 2023-06-26 02:43:24.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/fallingcloth_attr.py
--rw-rw-rw-   0        0        0     1533 2023-06-26 07:30:57.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/gameobject_attr.py
--rw-rw-rw-   0        0        0     4038 2023-06-26 06:02:42.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/graspsim_attr.py
--rw-rw-rw-   0        0        0     4520 2023-06-26 07:34:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/humanbody_attr.py
--rw-rw-rw-   0        0        0     2643 2023-06-26 07:41:38.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/light_attr.py
--rw-rw-rw-   0        0        0     8924 2023-06-27 09:47:18.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/omplmanager_attr.py
--rw-rw-rw-   0        0        0     1331 2023-06-27 08:46:11.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/pointcloud_attr.py
--rw-rw-rw-   0        0        0     1737 2023-06-26 03:12:07.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/rigidbody_attr.py
--rw-rw-rw-   0        0        0      387 2023-06-26 03:12:19.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/softbody_attr.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.534245 pyrfuniverse-0.9.10/pyrfuniverse/envs/
--rw-rw-rw-   0        0        0    14525 2023-06-26 03:42:24.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/__init__.py
--rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/balance_ball_env.py
--rw-rw-rw-   0        0        0    24046 2023-07-03 03:53:17.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/base_env.py
--rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/bouncer_env.py
--rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/franka_grasp_env.py
--rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/franka_push_env.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.539932 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/
--rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/__init__.py
--rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/nail_can_env.py
--rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/nail_card_env.py
--rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
--rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
--rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
--rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
--rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
--rw-rw-rw-   0        0        0      769 2023-06-26 03:45:35.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gym_goal_wrapper_env.py
--rw-rw-rw-   0        0        0      702 2023-06-26 03:45:35.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gym_wrapper_env.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.542004 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/
--rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/cleaner_env.py
--rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/navigation_env.py
--rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent_navigation_env.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.544004 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/
--rw-rw-rw-   0        0        0      871 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/__init__.py
--rw-rw-rw-   0        0        0    13868 2023-07-03 04:41:20.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
--rw-rw-rw-   0        0        0     8156 2023-06-28 05:32:14.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
--rw-rw-rw-   0        0        0    10075 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
--rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.549513 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/
--rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/__init__.py
--rw-rw-rw-   0        0        0     7276 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_cloth_env.py
--rw-rw-rw-   0        0        0     7476 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
--rw-rw-rw-   0        0        0     9654 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_robotics_env.py
--rw-rw-rw-   0        0        0     8014 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_softbody_env.py
--rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/pick_and_place_env.py
--rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/push_env.py
--rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/reach_env.py
--rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/roller_env.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.550512 pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotics/
--rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotics/__init__.py
--rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
--rw-rw-rw-   0        0        0     8629 2023-06-27 11:22:59.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
--rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/ur5_box_env.py
--rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/ur5_drawer_env.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.552021 pyrfuniverse-0.9.10/pyrfuniverse/side_channel/
--rw-rw-rw-   0        0        0      144 2023-06-26 02:33:27.000000 pyrfuniverse-0.9.10/pyrfuniverse/side_channel/__init__.py
--rw-rw-rw-   0        0        0     3244 2023-06-26 02:33:27.000000 pyrfuniverse-0.9.10/pyrfuniverse/side_channel/incoming_message.py
--rw-rw-rw-   0        0        0     1536 2023-06-26 02:33:27.000000 pyrfuniverse-0.9.10/pyrfuniverse/side_channel/outgoing_message.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.560049 pyrfuniverse-0.9.10/pyrfuniverse/utils/
--rw-rw-rw-   0        0        0        0 2023-07-03 03:57:44.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/__init__.py
--rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/active_depth_generate.py
--rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/controller.py
--rw-rw-rw-   0        0        0    11746 2023-06-27 09:15:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/depth_processor.py
--rw-rw-rw-   0        0        0     3227 2023-06-28 05:30:44.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/interpolate_utils.py
--rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/jaco_controller.py
--rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/kinova_controller.py
--rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/os_utils.py
--rw-rw-rw-   0        0        0     9072 2023-07-02 13:36:55.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/rfuniverse_communicator.py
--rw-rw-rw-   0        0        0     3569 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/rfuniverse_utility.py
--rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/stretch_controller.py
--rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/tobor_controller.py
--rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/ur5_controller.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.513716 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/
--rw-rw-rw-   0        0        0      266 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4088 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:32:20.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 04:47:49.577521 pyrfuniverse-0.9.10/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-07-03 03:43:45.000000 pyrfuniverse-0.9.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.576521 pyrfuniverse-0.9.10/test/
--rw-rw-rw-   0        0        0     5924 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_active_depth.py
--rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_articulation_ik.py
--rw-rw-rw-   0        0        0      943 2023-06-30 10:11:12.000000 pyrfuniverse-0.9.10/test/test_camera_image.py
--rw-rw-rw-   0        0        0     1939 2023-06-29 07:29:03.000000 pyrfuniverse-0.9.10/test/test_custom_message.py
--rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.9.10/test/test_debug.py
--rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.9.10/test/test_digit.py
--rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_grasp_pose.py
--rw-rw-rw-   0        0        0     2750 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_grasp_sim.py
--rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.9.10/test/test_heat_map.py
--rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_humanbody_ik.py
--rw-rw-rw-   0        0        0     1087 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_image_stream.py
--rw-rw-rw-   0        0        0     1984 2023-06-26 02:33:27.000000 pyrfuniverse-0.9.10/test/test_label.py
--rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_light.py
--rw-rw-rw-   0        0        0      589 2023-06-13 10:33:21.000000 pyrfuniverse-0.9.10/test/test_load_mesh.py
--rw-rw-rw-   0        0        0     1008 2023-06-27 08:00:59.000000 pyrfuniverse-0.9.10/test/test_load_urdf.py
--rw-rw-rw-   0        0        0      277 2023-06-26 07:47:27.000000 pyrfuniverse-0.9.10/test/test_load_urdf_akb.py
--rw-rw-rw-   0        0        0     1980 2023-06-27 08:13:05.000000 pyrfuniverse-0.9.10/test/test_object_data.py
--rw-rw-rw-   0        0        0     1646 2023-06-28 08:01:52.000000 pyrfuniverse-0.9.10/test/test_ompl.py
--rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.9.10/test/test_pick_and_place.py
--rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.9.10/test/test_pick_and_place_flexiv.py
--rw-rw-rw-   0        0        0     1658 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_point_cloud.py
--rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_point_cloud_render.py
--rw-rw-rw-   0        0        0     1830 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_point_cloud_with_intrinsic_matrix.py
--rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.9.10/test/test_save_gripper.py
--rw-rw-rw-   0        0        0      378 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_save_obj.py
--rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_scene.py
--rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.9.10/test/test_tobor_move.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.683002 pyrfuniverse-0.9.11/
+-rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.9.11/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-07-26 07:52:45.681499 pyrfuniverse-0.9.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2758 2023-06-21 09:17:40.000000 pyrfuniverse-0.9.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.158675 pyrfuniverse-0.9.11/pyrfuniverse/
+-rw-rw-rw-   0        0        0      759 2023-07-26 07:51:49.000000 pyrfuniverse-0.9.11/pyrfuniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.304711 pyrfuniverse-0.9.11/pyrfuniverse/attributes/
+-rw-rw-rw-   0        0        0     1472 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/activelightsensor_attr.py
+-rw-rw-rw-   0        0        0     9352 2023-07-12 10:53:12.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/base_attr.py
+-rw-rw-rw-   0        0        0     8438 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/camera_attr.py
+-rw-rw-rw-   0        0        0      384 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/cloth_attr.py
+-rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/collider_attr.py
+-rw-rw-rw-   0        0        0    15137 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/controller_attr.py
+-rw-rw-rw-   0        0        0      622 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/custom_attr.py
+-rw-rw-rw-   0        0        0      678 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/digit_attr.py
+-rw-rw-rw-   0        0        0      871 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/fallingcloth_attr.py
+-rw-rw-rw-   0        0        0     1533 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/gameobject_attr.py
+-rw-rw-rw-   0        0        0     4038 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/graspsim_attr.py
+-rw-rw-rw-   0        0        0     4520 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/humanbody_attr.py
+-rw-rw-rw-   0        0        0     2643 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/light_attr.py
+-rw-rw-rw-   0        0        0     8924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/omplmanager_attr.py
+-rw-rw-rw-   0        0        0     1331 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/pointcloud_attr.py
+-rw-rw-rw-   0        0        0     1737 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/rigidbody_attr.py
+-rw-rw-rw-   0        0        0      387 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/softbody_attr.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.363721 pyrfuniverse-0.9.11/pyrfuniverse/envs/
+-rw-rw-rw-   0        0        0    15241 2023-07-26 07:51:49.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/__init__.py
+-rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/balance_ball_env.py
+-rw-rw-rw-   0        0        0    24832 2023-07-14 07:27:36.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/base_env.py
+-rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/bouncer_env.py
+-rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/franka_grasp_env.py
+-rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/franka_push_env.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.407296 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/
+-rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/__init__.py
+-rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/nail_can_env.py
+-rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/nail_card_env.py
+-rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
+-rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
+-rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
+-rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
+-rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
+-rw-rw-rw-   0        0        0      769 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gym_goal_wrapper_env.py
+-rw-rw-rw-   0        0        0      702 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gym_wrapper_env.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.423828 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/
+-rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/cleaner_env.py
+-rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/navigation_env.py
+-rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent_navigation_env.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.444420 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/
+-rw-rw-rw-   0        0        0      871 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/__init__.py
+-rw-rw-rw-   0        0        0    13868 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
+-rw-rw-rw-   0        0        0     8156 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
+-rw-rw-rw-   0        0        0    10075 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
+-rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.479350 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/
+-rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/__init__.py
+-rw-rw-rw-   0        0        0     7488 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_cloth_env.py
+-rw-rw-rw-   0        0        0     7679 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
+-rw-rw-rw-   0        0        0     9654 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_robotics_env.py
+-rw-rw-rw-   0        0        0     8235 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_softbody_env.py
+-rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/pick_and_place_env.py
+-rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/push_env.py
+-rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/reach_env.py
+-rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/roller_env.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.488371 pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotics/
+-rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotics/__init__.py
+-rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
+-rw-rw-rw-   0        0        0     8876 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
+-rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/ur5_box_env.py
+-rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/ur5_drawer_env.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.503369 pyrfuniverse-0.9.11/pyrfuniverse/side_channel/
+-rw-rw-rw-   0        0        0      144 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/side_channel/__init__.py
+-rw-rw-rw-   0        0        0     3244 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/side_channel/incoming_message.py
+-rw-rw-rw-   0        0        0     1536 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/side_channel/outgoing_message.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.567667 pyrfuniverse-0.9.11/pyrfuniverse/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/active_depth_generate.py
+-rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/controller.py
+-rw-rw-rw-   0        0        0    11746 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/depth_processor.py
+-rw-rw-rw-   0        0        0     3314 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/interpolate_utils.py
+-rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/jaco_controller.py
+-rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/kinova_controller.py
+-rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/os_utils.py
+-rw-rw-rw-   0        0        0    10104 2023-07-21 18:14:17.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/rfuniverse_communicator.py
+-rw-rw-rw-   0        0        0     3569 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/rfuniverse_utility.py
+-rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/stretch_controller.py
+-rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/tobor_controller.py
+-rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/ur5_controller.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.170709 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4088 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:32:20.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 07:52:45.683002 pyrfuniverse-0.9.11/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.681499 pyrfuniverse-0.9.11/test/
+-rw-rw-rw-   0        0        0     5924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_active_depth.py
+-rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_articulation_ik.py
+-rw-rw-rw-   0        0        0      943 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_camera_image.py
+-rw-rw-rw-   0        0        0     1939 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_custom_message.py
+-rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.9.11/test/test_debug.py
+-rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.9.11/test/test_digit.py
+-rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_grasp_pose.py
+-rw-rw-rw-   0        0        0     2750 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_grasp_sim.py
+-rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.9.11/test/test_heat_map.py
+-rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_humanbody_ik.py
+-rw-rw-rw-   0        0        0     1087 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_image_stream.py
+-rw-rw-rw-   0        0        0     1984 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_label.py
+-rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_light.py
+-rw-rw-rw-   0        0        0      589 2023-06-13 10:33:21.000000 pyrfuniverse-0.9.11/test/test_load_mesh.py
+-rw-rw-rw-   0        0        0     1008 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_load_urdf.py
+-rw-rw-rw-   0        0        0      277 2023-07-10 14:17:21.000000 pyrfuniverse-0.9.11/test/test_load_urdf_akb.py
+-rw-rw-rw-   0        0        0     1980 2023-07-13 08:59:36.000000 pyrfuniverse-0.9.11/test/test_object_data.py
+-rw-rw-rw-   0        0        0     1646 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_ompl.py
+-rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.9.11/test/test_pick_and_place.py
+-rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.9.11/test/test_pick_and_place_flexiv.py
+-rw-rw-rw-   0        0        0     1658 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_point_cloud.py
+-rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_point_cloud_render.py
+-rw-rw-rw-   0        0        0     1830 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_point_cloud_with_intrinsic_matrix.py
+-rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.9.11/test/test_save_gripper.py
+-rw-rw-rw-   0        0        0      378 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_save_obj.py
+-rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_scene.py
+-rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.9.11/test/test_tobor_move.py
```

### Comparing `pyrfuniverse-0.9.10/LICENSE` & `pyrfuniverse-0.9.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/README.md` & `pyrfuniverse-0.9.11/README.md`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/__init__.py` & `pyrfuniverse-0.9.11/pyrfuniverse/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the library that will be used to upload to pypi
-__version__ = "0.9.10"
+__version__ = "0.9.11"
 
 import os.path
 import json
 
 def read_config():
     if not os.path.exists(config_path):
         config = {}
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/__init__.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/activelightsensor_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/activelightsensor_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/base_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/base_attr.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,29 @@
             is_world: Bool, True for world coordinate, False for local coordinate.
         """
         assert len(rotation) == 3, 'rotation length must be 3'
         rotation = [float(i) for i in rotation]
 
         self._send_data('Rotate', rotation, is_world)
 
+    def LookAt(self, target: list, world_up: list):
+        """
+        Rotates the transform so the forward vector points at target's current position.
+
+        Args:
+            target: A list of length 3, target to point towards.
+            world_up: A list of length 3, vector specifying the upward direction.
+        """
+        assert len(target) == 3, 'target length must be 3'
+        target = [float(i) for i in target]
+        assert len(world_up) == 3, 'world_up length must be 3'
+        world_up = [float(i) for i in world_up]
+
+        self._send_data('LookAt', target, world_up)
+
     def SetActive(self, active: bool):
         """
         Set the activeness of this obeject.
 
         Args:
             active: Bool, True for active, False for inactive.
         """
@@ -208,29 +223,29 @@
         Set the collider active or inactive in RFMove.
 
         Args:
             active: Bool, True for active and False for inactive.
         """
         self._send_data('SetRFMoveColliderActive', active)
 
-    def GetLoaclPointFromWorld(self, point: list):
+    def GetLocalPointFromWorld(self, point: list):
         """
-        Transform a point from local coordinate to world coordinate.
+        Transform a point from local coordinate to world coordinate. After calling this method and stepping once, the result will be saved in self.data['result_local_point']
 
         Args:
             point: A list of length 3, representing the position of a point.
         """
         assert len(point) == 3, 'point length must be 3'
         point = [float(i) for i in point]
 
-        self._send_data('GetLoaclPointFromWorld', point)
+        self._send_data('GetLocalPointFromWorld', point)
 
     def GetWorldPointFromLocal(self, point: list):
         """
-        Transform a point from world coordinate to local coordinate.
+        Transform a point from world coordinate to local coordinate. After calling this method and stepping once, the result will be saved in self.data['result_world_point']
 
         Args:
             point: A list of length 3, representing the position of a point.
         """
         assert len(point) == 3, 'point length must be 3'
         point = [float(i) for i in point]
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/camera_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/camera_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/collider_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/collider_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/controller_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/controller_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/custom_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/custom_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/digit_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/digit_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/fallingcloth_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/fallingcloth_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/gameobject_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/gameobject_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/graspsim_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/graspsim_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/humanbody_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/humanbody_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/light_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/light_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/omplmanager_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/omplmanager_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/pointcloud_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/pointcloud_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/attributes/rigidbody_attr.py` & `pyrfuniverse-0.9.11/pyrfuniverse/attributes/rigidbody_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/__init__.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,385 +19,385 @@
 # from pyrfuniverse.envs.ur5_box_env import Ur5BoxEnv
 # from pyrfuniverse.envs.ur5_drawer_env import Ur5DrawerEnv
 
 # Other projects based on RFUniverse
 # import pyrfuniverse.envs.robotube
 # import pyrfuniverse.envs.rcareworld
 
-__all__ = [
-    'RFUniverseBaseEnv', 'FrankaGraspEnv', 'FrankaPushEnv', 'BalanceBallEnv',
-    'RFUniverseGymWrapper', 'BalanceBallEnvV0', 'RFUniverseGymGoalWrapper',
-    'BouncerEnv', 'BouncerEnvV0', 'RollerEnv', 'RollerEnvV0', 'NailCardEnv',
-    'MultiAgentNavigationEnv', 'ToborRobotiq85ManipulationEnv', 'Ur5BoxEnv',
-    'Ur5DrawerEnv',
-]
-
-
-rfuniverse_build_base_root = '/home/haoyuan/workspace/rfuniverse/rfuniverse/rfuniverse_build/'
-
-try:
-    from gym.envs.registration import register
-
-    register(
-        id='BalanceBallEnv-v0',
-        entry_point='pyrfuniverse.envs:BalanceBallEnvV0'
-    )
-
-    register(
-        id='BouncerEnv-v0',
-        entry_point='pyrfuniverse.envs:BouncerEnvV0'
-    )
-
-    register(
-        id='RollerEnv-v0',
-        entry_point='pyrfuniverse.envs:RollerEnvV0'
-    )
-
-    register(
-        id='MultiAgentNavigation-v1',
-        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'num_agents': 5,
-        },
-    )
-
-    register(
-        id='MultiAgentNavigation-v2',
-        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'num_agents': 5,
-            'reset_on_collision': True
-        },
-    )
-
-    register(
-        id='MultiAgentNavigation-v3',
-        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'num_agents': 3,
-        },
-    )
-
-    register(
-        id='MultiAgentNavigation-v4',
-        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'num_agents': 3,
-            'reset_on_collision': True
-        },
-    )
-
-    # Franka robotics
-    for reward_type in ['sparse', 'dense']:
-        suffix = 'Dense' if reward_type == 'dense' else ''
-        kwargs = {
-            'executable_file': rfuniverse_build_base_root + 'FrankaRoboticsServer/RFUniverse.x86_64',
-            'max_episode_length': 50,
-            'reward_type': reward_type,
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody'
-        }
-
-        register(
-            id='FrankaPickAndPlace{}-v1'.format(suffix),
-            entry_point='pyrfuniverse.envs.robotics:FrankaPickAndPlaceEnv',
-            kwargs=kwargs,
-            max_episode_steps=50,
-        )
-
-        register(
-            id='FrankaReach{}-v1'.format(suffix),
-            entry_point='pyrfuniverse.envs.robotics:FrankaReachEnv',
-            kwargs=kwargs,
-            max_episode_steps=50,
-        )
-
-        register(
-            id='FrankaPush{}-v1'.format(suffix),
-            entry_point='pyrfuniverse.envs.robotics:FrankaPushEnv',
-            kwargs=kwargs,
-            max_episode_steps=50,
-        )
-
-    # Franka-Cloth env
-    franka_cloth_kwargs = {
-        'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/obi_cloth',
-        'executable_file': rfuniverse_build_base_root + 'FrankaCloth/RFUniverse.x86_64',
-        'reward_type': 'dense'
-    }
-    register(
-        id='FrankaCloth-v1',
-        entry_point='pyrfuniverse.envs.robotics:FrankaClothEnv',
-        kwargs=franka_cloth_kwargs,
-        max_episode_steps=50
-    )
-
-    # Franka-Softbody env
-    franka_softbody_kwargs = {
-        'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/softbody',
-        # 'executable_file': rfuniverse_build_base_root + 'FrankaSoftbodyServer/RFUniverse.x86_64',
-        'executable_file': None,
-        'reward_type': 'sparse'
-    }
-    register(
-        id='FrankaSoftbody-v1',
-        entry_point='pyrfuniverse.envs.robotics:FrankaSoftbodyEnv',
-        kwargs=franka_softbody_kwargs,
-        max_episode_steps=50
-    )
-
-    # Franka-ClothFold env
-    franka_cloth_fold_kwargs = {
-        'asset_bundle_file': '/home/haoyuan/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/obi_cloth',
-        # 'executable_file': rfuniverse_build_base_root + 'FrankaClothFoldServer/RFUniverse.x86_64',
-        'executable_file': None,
-        'reward_type': 'sparse'
-    }
-    register(
-        id='FrankaClothFold-v1',
-        entry_point='pyrfuniverse.envs.robotics:FrankaClothFoldEnv',
-        kwargs=franka_cloth_fold_kwargs,
-        max_episode_steps=20
-    )
-
-    # A relatively easy and naive NailCard environment
-    register(
-        id='NailCard-v1',
-        entry_point='pyrfuniverse.envs:NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
-            'rotation_factor': 0,
-            'goal_baseline': 0.02,
-        },
-        max_episode_steps=50,
-    )
-
-    # The normal version
-    register(
-        id='NailCard-v2',
-        entry_point='pyrfuniverse.envs:NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
-        },
-        max_episode_steps=50,
-    )
-
-    # Fixed the nail movement
-    register(
-        id='NailCard-v3',
-        entry_point='pyrfuniverse.envs:NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
-            'nail_movement_factor': 0
-        },
-        max_episode_steps=50,
-    )
-
-    # A relatively easy and naive NailCard environment
-    register(
-        id='Robotiq85NailCard-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
-            'rotation_factor': 0,
-            'goal_baseline': 0.02,
-        },
-        max_episode_steps=50,
-    )
-
-    # The normal version
-    register(
-        id='Robotiq85NailCard-v2',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
-        },
-        max_episode_steps=50,
-    )
-
-    # Fixed the nail movement
-    register(
-        id='Robotiq85NailCard-v3',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
-            'vertical_movement_factor': 0.02,
-            'nail_movement_factor': 0
-        },
-        max_episode_steps=50,
-    )
-
-    # Robotiq85 Nail Coin
-    register(
-        id='Robotiq85NailCoin-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCoinEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCoinServer/RFUniverse.x86_64',
-            'vertical_movement_factor': 0.02,
-            'nail_movement_factor': 0
-        },
-        max_episode_steps=50,
-    )
-
-    # Nail-Can environment
-    register(
-        id='NailCan-v1',
-        entry_point='pyrfuniverse.envs:NailCanEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'NailCanServer/RFUniverse.x86_64',
-        }
-    )
-
-    register(
-        id='Robotiq85NailCan-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCanEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCanServer/RFUniverse.x86_64',
-        }
-    )
-
-    register(
-        id='Robotiq85NailBook-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailBookEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailBook/RFUniverse.x86_64',
-        }
-    )
-
-    # Robotiq85 insert
-    register(
-        id='Robotiq85Insert-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85InsertEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85InsertServer/RFUniverse.x86_64',
-        }
-    )
-
-    register(
-        id='Cleaner-v1',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerServer/RFUniverse.x86_64'
-        }
-    )
-
-    register(
-        id='Cleaner-v2',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'reset_on_collision': False,
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerServer/RFUniverse.x86_64',
-        }
-    )
-
-    register(
-        id='Cleaner-v3',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64'
-        }
-    )
-
-    register(
-        id='Cleaner-v4',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'reset_on_collision': False,
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64'
-        }
-    )
-
-    register(
-        id='Cleaner-v5',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
-            'velocity_reward': True
-        }
-    )
-
-    register(
-        id='Cleaner-v6',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
-            'velocity_reward': True,
-            'collision_multiplier': 50,
-        }
-    )
-
-    register(
-        id='Cleaner-v7',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': '/home/haoyuan/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/rigidbody',
-            # 'executable_file': rfuniverse_build_base_root + 'CleanerWithWall/RFUniverse.x86_64',
-            'executable_file': None,
-            'velocity_reward': True,
-            'collision_multiplier': 50,
-            'obs_type': 'box',
-            'max_episode_length': 200
-        }
-    )
-
-    register(
-        id='Cleaner-v8',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
-            'grid_reward_per_step': True
-        }
-    )
-
-    register(
-        id='UR5Box-v1',
-        entry_point='pyrfuniverse.envs:Ur5BoxEnv',
-        kwargs={
-            'max_steps': 50,
-            'reward_type': 'sparse',
-            'min_open_angle': 30,
-            'executable_file': rfuniverse_build_base_root + 'UR5Box/RFUniverse.x86_64'
-        },
-        max_episode_steps=50,
-    )
-
-    register(
-        id='ToborPull-v1',
-        entry_point='pyrfuniverse.envs.tobor_robotics:ToborPushPullEnv',
-        kwargs={
-            'max_steps': 100,
-            'asset_bundle_file': '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/articulation',
-            'pull': True,
-            'executable_file': rfuniverse_build_base_root + 'ToborPushPull/RFUniverse.x86_64'
-        },
-        max_episode_steps=100
-    )
-
-    register(
-        id='ToborPush-v1',
-        entry_point='pyrfuniverse.envs.tobor_robotics:ToborPushPullEnv',
-        kwargs={
-            'max_steps': 100,
-            'asset_bundle_file': '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/articulation',
-            'pull': False,
-            'executable_file': rfuniverse_build_base_root + 'ToborPushPull/RFUniverse.x86_64'
-        },
-        max_episode_steps=100
-    )
-
-except ImportError:
-    print('No gym installed. Please install gym!')
-    pass
+# __all__ = [
+#     'RFUniverseBaseEnv', 'FrankaGraspEnv', 'FrankaPushEnv', 'BalanceBallEnv',
+#     'RFUniverseGymWrapper', 'BalanceBallEnvV0', 'RFUniverseGymGoalWrapper',
+#     'BouncerEnv', 'BouncerEnvV0', 'RollerEnv', 'RollerEnvV0', 'NailCardEnv',
+#     'MultiAgentNavigationEnv', 'ToborRobotiq85ManipulationEnv', 'Ur5BoxEnv',
+#     'Ur5DrawerEnv',
+# ]
+#
+#
+# rfuniverse_build_base_root = '/home/haoyuan/workspace/rfuniverse/rfuniverse/rfuniverse_build/'
+#
+# try:
+#     from gym.envs.registration import register
+#
+#     register(
+#         id='BalanceBallEnv-v0',
+#         entry_point='pyrfuniverse.envs:BalanceBallEnvV0'
+#     )
+#
+#     register(
+#         id='BouncerEnv-v0',
+#         entry_point='pyrfuniverse.envs:BouncerEnvV0'
+#     )
+#
+#     register(
+#         id='RollerEnv-v0',
+#         entry_point='pyrfuniverse.envs:RollerEnvV0'
+#     )
+#
+#     register(
+#         id='MultiAgentNavigation-v1',
+#         entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'num_agents': 5,
+#         },
+#     )
+#
+#     register(
+#         id='MultiAgentNavigation-v2',
+#         entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'num_agents': 5,
+#             'reset_on_collision': True
+#         },
+#     )
+#
+#     register(
+#         id='MultiAgentNavigation-v3',
+#         entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'num_agents': 3,
+#         },
+#     )
+#
+#     register(
+#         id='MultiAgentNavigation-v4',
+#         entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'num_agents': 3,
+#             'reset_on_collision': True
+#         },
+#     )
+#
+#     # Franka robotics
+#     for reward_type in ['sparse', 'dense']:
+#         suffix = 'Dense' if reward_type == 'dense' else ''
+#         kwargs = {
+#             'executable_file': rfuniverse_build_base_root + 'FrankaRoboticsServer/RFUniverse.x86_64',
+#             'max_episode_length': 50,
+#             'reward_type': reward_type,
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody'
+#         }
+#
+#         register(
+#             id='FrankaPickAndPlace{}-v1'.format(suffix),
+#             entry_point='pyrfuniverse.envs.robotics:FrankaPickAndPlaceEnv',
+#             kwargs=kwargs,
+#             max_episode_steps=50,
+#         )
+#
+#         register(
+#             id='FrankaReach{}-v1'.format(suffix),
+#             entry_point='pyrfuniverse.envs.robotics:FrankaReachEnv',
+#             kwargs=kwargs,
+#             max_episode_steps=50,
+#         )
+#
+#         register(
+#             id='FrankaPush{}-v1'.format(suffix),
+#             entry_point='pyrfuniverse.envs.robotics:FrankaPushEnv',
+#             kwargs=kwargs,
+#             max_episode_steps=50,
+#         )
+#
+#     # Franka-Cloth env
+#     franka_cloth_kwargs = {
+#         'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/obi_cloth',
+#         'executable_file': rfuniverse_build_base_root + 'FrankaCloth/RFUniverse.x86_64',
+#         'reward_type': 'dense'
+#     }
+#     register(
+#         id='FrankaCloth-v1',
+#         entry_point='pyrfuniverse.envs.robotics:FrankaClothEnv',
+#         kwargs=franka_cloth_kwargs,
+#         max_episode_steps=50
+#     )
+#
+#     # Franka-Softbody env
+#     franka_softbody_kwargs = {
+#         'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/softbody',
+#         # 'executable_file': rfuniverse_build_base_root + 'FrankaSoftbodyServer/RFUniverse.x86_64',
+#         'executable_file': None,
+#         'reward_type': 'sparse'
+#     }
+#     register(
+#         id='FrankaSoftbody-v1',
+#         entry_point='pyrfuniverse.envs.robotics:FrankaSoftbodyEnv',
+#         kwargs=franka_softbody_kwargs,
+#         max_episode_steps=50
+#     )
+#
+#     # Franka-ClothFold env
+#     franka_cloth_fold_kwargs = {
+#         'asset_bundle_file': '/home/haoyuan/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/obi_cloth',
+#         # 'executable_file': rfuniverse_build_base_root + 'FrankaClothFoldServer/RFUniverse.x86_64',
+#         'executable_file': None,
+#         'reward_type': 'sparse'
+#     }
+#     register(
+#         id='FrankaClothFold-v1',
+#         entry_point='pyrfuniverse.envs.robotics:FrankaClothFoldEnv',
+#         kwargs=franka_cloth_fold_kwargs,
+#         max_episode_steps=20
+#     )
+#
+#     # A relatively easy and naive NailCard environment
+#     register(
+#         id='NailCard-v1',
+#         entry_point='pyrfuniverse.envs:NailCardEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
+#             'rotation_factor': 0,
+#             'goal_baseline': 0.02,
+#         },
+#         max_episode_steps=50,
+#     )
+#
+#     # The normal version
+#     register(
+#         id='NailCard-v2',
+#         entry_point='pyrfuniverse.envs:NailCardEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
+#         },
+#         max_episode_steps=50,
+#     )
+#
+#     # Fixed the nail movement
+#     register(
+#         id='NailCard-v3',
+#         entry_point='pyrfuniverse.envs:NailCardEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
+#             'nail_movement_factor': 0
+#         },
+#         max_episode_steps=50,
+#     )
+#
+#     # A relatively easy and naive NailCard environment
+#     register(
+#         id='Robotiq85NailCard-v1',
+#         entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
+#             'rotation_factor': 0,
+#             'goal_baseline': 0.02,
+#         },
+#         max_episode_steps=50,
+#     )
+#
+#     # The normal version
+#     register(
+#         id='Robotiq85NailCard-v2',
+#         entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
+#         },
+#         max_episode_steps=50,
+#     )
+#
+#     # Fixed the nail movement
+#     register(
+#         id='Robotiq85NailCard-v3',
+#         entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
+#             'vertical_movement_factor': 0.02,
+#             'nail_movement_factor': 0
+#         },
+#         max_episode_steps=50,
+#     )
+#
+#     # Robotiq85 Nail Coin
+#     register(
+#         id='Robotiq85NailCoin-v1',
+#         entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCoinEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCoinServer/RFUniverse.x86_64',
+#             'vertical_movement_factor': 0.02,
+#             'nail_movement_factor': 0
+#         },
+#         max_episode_steps=50,
+#     )
+#
+#     # Nail-Can environment
+#     register(
+#         id='NailCan-v1',
+#         entry_point='pyrfuniverse.envs:NailCanEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'NailCanServer/RFUniverse.x86_64',
+#         }
+#     )
+#
+#     register(
+#         id='Robotiq85NailCan-v1',
+#         entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCanEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCanServer/RFUniverse.x86_64',
+#         }
+#     )
+#
+#     register(
+#         id='Robotiq85NailBook-v1',
+#         entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailBookEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'Robotiq85NailBook/RFUniverse.x86_64',
+#         }
+#     )
+#
+#     # Robotiq85 insert
+#     register(
+#         id='Robotiq85Insert-v1',
+#         entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85InsertEnv',
+#         kwargs={
+#             'executable_file': rfuniverse_build_base_root + 'Robotiq85InsertServer/RFUniverse.x86_64',
+#         }
+#     )
+#
+#     register(
+#         id='Cleaner-v1',
+#         entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+#         kwargs={
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'executable_file': rfuniverse_build_base_root + 'CleanerServer/RFUniverse.x86_64'
+#         }
+#     )
+#
+#     register(
+#         id='Cleaner-v2',
+#         entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+#         kwargs={
+#             'reset_on_collision': False,
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'executable_file': rfuniverse_build_base_root + 'CleanerServer/RFUniverse.x86_64',
+#         }
+#     )
+#
+#     register(
+#         id='Cleaner-v3',
+#         entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+#         kwargs={
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64'
+#         }
+#     )
+#
+#     register(
+#         id='Cleaner-v4',
+#         entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+#         kwargs={
+#             'reset_on_collision': False,
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64'
+#         }
+#     )
+#
+#     register(
+#         id='Cleaner-v5',
+#         entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+#         kwargs={
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
+#             'velocity_reward': True
+#         }
+#     )
+#
+#     register(
+#         id='Cleaner-v6',
+#         entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+#         kwargs={
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
+#             'velocity_reward': True,
+#             'collision_multiplier': 50,
+#         }
+#     )
+#
+#     register(
+#         id='Cleaner-v7',
+#         entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+#         kwargs={
+#             'asset_bundle_file': '/home/haoyuan/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/rigidbody',
+#             # 'executable_file': rfuniverse_build_base_root + 'CleanerWithWall/RFUniverse.x86_64',
+#             'executable_file': None,
+#             'velocity_reward': True,
+#             'collision_multiplier': 50,
+#             'obs_type': 'box',
+#             'max_episode_length': 200
+#         }
+#     )
+#
+#     register(
+#         id='Cleaner-v8',
+#         entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+#         kwargs={
+#             'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+#             'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
+#             'grid_reward_per_step': True
+#         }
+#     )
+#
+#     register(
+#         id='UR5Box-v1',
+#         entry_point='pyrfuniverse.envs:Ur5BoxEnv',
+#         kwargs={
+#             'max_steps': 50,
+#             'reward_type': 'sparse',
+#             'min_open_angle': 30,
+#             'executable_file': rfuniverse_build_base_root + 'UR5Box/RFUniverse.x86_64'
+#         },
+#         max_episode_steps=50,
+#     )
+#
+#     register(
+#         id='ToborPull-v1',
+#         entry_point='pyrfuniverse.envs.tobor_robotics:ToborPushPullEnv',
+#         kwargs={
+#             'max_steps': 100,
+#             'asset_bundle_file': '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/articulation',
+#             'pull': True,
+#             'executable_file': rfuniverse_build_base_root + 'ToborPushPull/RFUniverse.x86_64'
+#         },
+#         max_episode_steps=100
+#     )
+#
+#     register(
+#         id='ToborPush-v1',
+#         entry_point='pyrfuniverse.envs.tobor_robotics:ToborPushPullEnv',
+#         kwargs={
+#             'max_steps': 100,
+#             'asset_bundle_file': '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/articulation',
+#             'pull': False,
+#             'executable_file': rfuniverse_build_base_root + 'ToborPushPull/RFUniverse.x86_64'
+#         },
+#         max_episode_steps=100
+#     )
+#
+# except ImportError:
+#     print('No gym installed. Please install gym!')
+#     pass
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/balance_ball_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/balance_ball_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/base_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/base_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,27 +39,31 @@
 
         self.attrs = {}
         self.data = {}
         self.listen_messages = {}
         self.listen_object = {}
         self.port = port
 
+        self.log_level = 1
+        self.log_map = {'Log': 3, 'Warning': 2, 'Error': 1, 'Exception': 1, 'Assert': 1}
+
         if self.executable_file is None:
             self.executable_file = pyrfuniverse.executable_file
 
         if self.executable_file == '' or self.executable_file == '@editor':
-            print('Waiting for UnityEditor Play...')
+            print('Waiting for UnityEditor play...')
             self.process = None
         elif os.path.exists(self.executable_file):
             self.port = self._get_port()
             self.process = self._start_unity_env(self.executable_file, self.port)
         else:
             raise Exception('Executable file not exists')
-        self.communicator = RFUniverseCommunicator(port=self.port, receive_data_callback=self._receive_data)
-        self._send_debug_data('SendVersion', pyrfuniverse.__version__)
+        self.communicator = RFUniverseCommunicator(port=self.port,
+                                                   receive_data_callback=self._receive_data)
+        self._send_debug_data('SetPythonVersion', pyrfuniverse.__version__)
         if len(self.pre_load_assets) > 0:
             self.PreLoadAssetsAsync(assets, True)
         if self.scene_file is not None:
             self.LoadSceneAsync(self.scene_file, True)
 
     def _get_port(self) -> int:
         executable_port = 5005
@@ -77,40 +81,43 @@
         arg = [executable_file]
         if not self.graphics:
             arg.extend(["-nographics", "-batchmode"])
         arg.append(f'-port:{port}')
         return subprocess.Popen(arg)
 
     def _receive_data(self, objs: list) -> None:
-        type = objs[0]
+        msg = objs[0]
         objs = objs[1:]
-        if type == 'Env':
+        if msg == 'Env':
             self._parse_env_data(objs)
-        elif type == 'Instance':
+        elif msg == 'Instance':
             self._parse_instence_data(objs)
-        elif type == 'Debug':
+        elif msg == 'Debug':
             self._parse_debug_data(objs)
-        elif type == 'Message':
+        elif msg == 'Message':
             self._parse_message_data(objs)
-        elif type == 'Object':
+        elif msg == 'Object':
             self._parse_object_data(objs)
         return
+
     def _parse_env_data(self, objs: list) -> None:
-        type = objs[0]
+        msg = objs[0]
         objs = objs[1:]
-        if type == 'LoadDone':
+        if msg == 'Close':
+            self.close()
+        elif msg == 'LoadDone':
             self.data['load_done'] = True
-        elif type == 'PendDone':
+        elif msg == 'PendDone':
             self.data['pend_done'] = True
-        elif type == 'RFMoveColliders':
+        elif msg == 'RFMoveColliders':
             self.data['colliders'] = objs[0]
-        elif type == 'CurrentCollisionPairs':
+        elif msg == 'CurrentCollisionPairs':
             self.data['collision_pairs'] = objs[0]
         else:
-            print(f'unknown env data type: {type}')
+            print(f'unknown env data type: {msg}')
 
     def _parse_instence_data(self, objs: list) -> None:
         this_object_id = objs[0]
         this_object_type = objs[1]
         this_object_data = objs[2]
 
         attr_type = eval('attr.' + this_object_type)
@@ -118,14 +125,21 @@
             self.attrs[this_object_id] = attr_type(self, this_object_id)
         elif type(self.attrs[this_object_id]) != attr_type:
             self.attrs[this_object_id] = attr_type(self, this_object_id, self.attrs[this_object_id].data)
 
         self.data[this_object_id] = self.attrs[this_object_id].parse_message(this_object_data)
 
     def _parse_debug_data(self, objs: list) -> None:
+        msg = objs[0]
+        objs = objs[1:]
+        if msg == 'Log':
+            if self.log_map[objs[0]] <= self.log_level:
+                print(f'Unity Env Log Type:{objs[0]}\nCondition:{objs[1]}\nStackTrace:{objs[2]}')
+        else:
+            print(f'unknown debug data type: {msg}')
         return
 
     def _parse_message_data(self, objs: list) -> None:
         msg = objs[0]
         objs = objs[1:]
         if msg in self.listen_messages:
             self.listen_messages[msg](IncomingMessage(objs[0]))
@@ -148,14 +162,19 @@
     def _send_message_data(self, *args) -> None:
         self.communicator.send_object('Message', *args)
 
     def _send_object_data(self, *args) -> None:
         self.communicator.send_object('Object', *args)
 
     def _step(self):
+        """
+        Send the messages of called functions to Unity and simulate for a step, then accept the data from Unity.
+        """
+        if not self.communicator.connected:
+            raise Exception('Unity Env not connected')
         self.communicator.sync_step()
 
     def step(self, count: int = 1):
         """
         Send the messages of called functions to Unity and simulate for a step, then accept the data from Unity.
 
         Args:
@@ -168,14 +187,16 @@
 
     def close(self):
         """
         Close the environment
         """
         if self.process is not None:
             self.process.kill()
+        if self.communicator is not None:
+            self.communicator.close()
 
     def GetAttr(self, id: int):
         """
         Get the attribute instance by object id.
 
         Args:
             id: Int, object id.
@@ -401,15 +422,15 @@
             id = random.randint(100000, 999999)
 
         self._send_env_data('InstanceObject', name, id)
 
         self.attrs[id] = attr_type(self, id)
         return self.attrs[id]
 
-    def LoadURDF(self, path: str, id: int = None, native_ik: bool = True, axis: str = 'y') -> attr.ControllerAttr:
+    def LoadURDF(self, path: str, id: int = None, native_ik: bool = False, axis: str = 'y') -> attr.ControllerAttr:
         """
         Load a model from URDF file.
 
         Args:
             path: Str, the URDF file path.
             id: Int, object id.
             native_ik: Bool, True for enabling native IK; False for using custom IK.When it is True, through the IKTargetDo*** interface, according to the end pose.When it is False, through the SetJoint*** interface, according to the joint movement.
@@ -459,27 +480,21 @@
             layer2: Int, the layer number of the second layer.
             ignore: Bool, True for ignoring collision between two layers; False for enabling collision between two layers.
         """
         self._send_env_data('IgnoreLayerCollision', layer1, layer2, ignore)
 
     def GetCurrentCollisionPairs(self) -> None:
         """
-        Get the collision pairs of current collision.
-
-        Returns:
-            Call this function and `step()`, the collision pairs can be got from env.data['CurrentCollisionPairs'].
+        Get the collision pairs of current collision. After calling this method and stepping once, the result will be saved in env.data['CurrentCollisionPairs']
         """
         self._send_env_data('GetCurrentCollisionPairs')
 
     def GetRFMoveColliders(self) -> None:
         """
-        Get the RFMove colliders.
-
-        Returns:
-            Call this function and `step()`, the collision pairs can be got from env.data['RFMoveColliders'].
+        Get the RFMove colliders. After calling this method and stepping once, the result will be saved in env.data['RFMoveColliders']
         """
         self._send_env_data('GetRFMoveColliders')
 
     def SetGravity(self, x: float, y: float, z: float) -> None:
         """
         Set the gravity of environment.
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/bouncer_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/bouncer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/franka_grasp_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/franka_grasp_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/franka_push_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/franka_push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/__init__.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/nail_can_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/nail_card_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gym_goal_wrapper_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gym_goal_wrapper_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/gym_wrapper_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/gym_wrapper_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/cleaner_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/cleaner_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/navigation_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent_navigation_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent_navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/__init__.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/flexiv_cutting.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/flexiv_cutting.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/rfuniverse_robot_hub_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/rfuniverse_robot_hub_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/__init__.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_cloth_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_cloth_env.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
-import numpy as np
-import math
-import copy
-from gym import spaces
-from gym.utils import seeding
-
-
-class FrankaClothEnv(RFUniverseGymGoalWrapper):
-    metadata = {'render.modes': ['human']}
-
-    def __init__(
-            self,
-            asset_bundle_file,
-            reward_type,
-            tolerance=0.08,
-            target_x_range=(-0.1, -0.1),
-            target_z_range=(-0.1, 0.1),
-            executable_file=None
-    ):
-        super().__init__(
-            executable_file=executable_file,
-            articulation_channel=True,
-            game_object_channel=True,
-            obi_cloth_channel=True,
-        )
-        self.asset_bundle_file = asset_bundle_file
-        self.reward_type = reward_type
-        self.tolerance = tolerance
-        self.target_x_range = target_x_range
-        self.target_z_range = target_z_range
-
-        # Fixed parameters
-        self.obi_solver_position = np.array([-0.1, 0.31, -0.1])
-        self.number_of_particles = 289
-        self.number_of_sampled_particles = 10
-
-        # Env setup
-        self.load_cloth = False
-        self._load_obi_cloth()
-        self.ik_controller = RFUniverseController('franka', base_pos=np.array([-0.6, 0, 0]))
-        self.eef_orn = self.ik_controller.bullet_client.getQuaternionFromEuler([math.pi / 2, 0, math.pi / 2])
-
-        self.t = 0
-        self.goal = self._sample_goal()
-        self.action_space = spaces.Box(
-            low=-1, high=1, shape=(4,), dtype=np.float32
-        )
-        obs = self._get_obs()
-        self.observation_space = spaces.Dict({
-            'observation': spaces.Box(-np.inf, np.inf, shape=obs['observation'].shape, dtype=np.float32),
-            'desired_goal': spaces.Box(-np.inf, np.inf, shape=obs['desired_goal'].shape, dtype=np.float32),
-            'achieved_goal': spaces.Box(-np.inf, np.inf, shape=obs['achieved_goal'].shape, dtype=np.float32)
-        })
-
-    def step(self, action: np.ndarray):
-        pos_ctrl = action[:3] * 0.05
-        curr_pos = np.array(self.articulation_channel.data[1]['positions'][3])
-        pos_ctrl = curr_pos + pos_ctrl
-        joint_positions = self.ik_controller.calculate_ik(
-            pos_ctrl,
-            eef_orn=self.eef_orn
-        )
-
-        curr_gripper_width = self._get_gripper_width()
-        target_gripper_width = curr_gripper_width + action[3] * 0.2
-        target_gripper_width = np.clip(target_gripper_width, 0, 0.08)
-        joint_positions.append(target_gripper_width)
-
-        self._set_franka_joints(np.array(joint_positions))
-        self.t += 1
-
-        obs = self._get_obs()
-        done = False
-        info = {
-            'is_success': self._check_success(obs)
-        }
-        reward = self.compute_reward(obs['achieved_goal'], obs['desired_goal'], info)
-
-        return obs, reward, done, info
-
-    def reset(self):
-        super().reset()
-
-        self._destroy_obi_cloth()
-        self.env.reset()
-        self._load_obi_cloth()
-        self.goal = self._sample_goal()
-
-        self.t = 0
-        self.ik_controller.reset()
-        joint_positions = self.ik_controller.calculate_ik(
-            [0, 0.3, 0.1],
-            self.eef_orn
-        )
-        self.articulation_channel.set_action(
-            'SetJointPositionDirectly',
-            index=0,
-            joint_positions=joint_positions,
-        )
-
-        self.game_object_channel.set_action(
-            'SetTransform',
-            index=0,
-            position=list(self.goal.copy())
-        )
-
-        self._step()
-
-        return self._get_obs()
-
-    def seed(self, seed=None):
-        self.np_random, seed = seeding.np_random(seed)
-        return [seed]
-
-    def render(self, mode='human'):
-        self._step()
-
-    def compute_reward(self, achieved_goal, desired_goal, info):
-        distance = self._compute_goal_distance(achieved_goal, desired_goal)
-        if self.reward_type == 'sparse':
-            return -(distance > self.tolerance).astype(np.float32)
-        else:
-            return -distance
-
-    def _get_obs(self):
-        gripper_position = np.array(self.articulation_channel.data[1]['positions'][3])
-        gripper_velocity = np.array(self.articulation_channel.data[1]['velocities'][3])
-        gripper_width = self._get_gripper_width()
-        panda_obs = np.concatenate((gripper_position, gripper_velocity, [gripper_width]))
-
-        cloth_particles = np.array(self.obi_cloth_channel.data[0]['positions'])
-        random_indices = np.random.randint(0, self.number_of_particles, size=(self.number_of_sampled_particles,))
-        sampled_particles = cloth_particles[random_indices] + self.obi_solver_position
-        sampled_particles = np.reshape(sampled_particles, newshape=(3 * self.number_of_sampled_particles,))
-
-        obs = np.concatenate((panda_obs, sampled_particles))
-
-        cloth_center = np.average(cloth_particles, axis=0) + self.obi_solver_position
-
-        return {
-            'observation': obs.copy(),
-            'achieved_goal': cloth_center.copy(),
-            'desired_goal': self.goal.copy()
-        }
-
-    def _load_obi_cloth(self):
-        if self.load_cloth:
-            return
-        self.asset_channel.set_action(
-            'LoadObiCloth',
-            filename=self.asset_bundle_file,
-            name='Obi Solver',
-            position=list(self.obi_solver_position)
-        )
-        self._step()
-        self.load_cloth = True
-
-    def _destroy_obi_cloth(self):
-        if not self.load_cloth:
-            return
-        self.obi_cloth_channel.set_action(
-            'Destroy',
-            index=0
-        )
-        self._step()
-        self.load_cloth = False
-
-    def _get_gripper_width(self):
-        gripper_joint_positions = copy.deepcopy(self.articulation_channel.data[1]['joint_positions'])
-        return -1 * (gripper_joint_positions[0] + gripper_joint_positions[1])
-
-    def _set_franka_joints(self, a: np.ndarray):
-        self.articulation_channel.set_action(
-            'SetJointPosition',
-            index=0,
-            joint_positions=list(a[0:7]),
-        )
-        self._step()
-
-        a[7] = -1 * a[7] / 2
-        self.articulation_channel.set_action(
-            'SetJointPosition',
-            index=1,
-            joint_positions=[a[7], a[7]],
-        )
-        self._step()
-
-    def _generate_random_float(self, min: float, max: float) -> float:
-        assert min <= max, \
-            'Min value is {}, while max value is {}.'.format(min, max)
-        random_float = np.random.rand()
-        random_float = random_float * (max - min) + min
-
-        return random_float
-
-    def _compute_goal_distance(self, goal_a, goal_b):
-        assert goal_a.shape == goal_b.shape
-        return np.linalg.norm(goal_a - goal_b, axis=-1)
-
-    def _check_success(self, obs):
-        achieved_goal = obs['achieved_goal']
-        desired_goal = obs['desired_goal']
-        distance = self._compute_goal_distance(achieved_goal, desired_goal)
-
-        return (distance < self.tolerance).astype(np.float32)
-
-    def _sample_goal(self):
-        target_x = self._generate_random_float(self.target_x_range[0], self.target_x_range[1])
-        target_z = self._generate_random_float(self.target_z_range[0], self.target_z_range[1])
-
-        return np.array([target_x, 0.3, target_z])
+from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
+import numpy as np
+import math
+import copy
+from gym import spaces
+from gym.utils import seeding
+
+
+class FrankaClothEnv(RFUniverseGymGoalWrapper):
+    metadata = {'render.modes': ['human']}
+
+    def __init__(
+            self,
+            asset_bundle_file,
+            reward_type,
+            tolerance=0.08,
+            target_x_range=(-0.1, -0.1),
+            target_z_range=(-0.1, 0.1),
+            executable_file=None
+    ):
+        super().__init__(
+            executable_file=executable_file,
+            articulation_channel=True,
+            game_object_channel=True,
+            obi_cloth_channel=True,
+        )
+        self.asset_bundle_file = asset_bundle_file
+        self.reward_type = reward_type
+        self.tolerance = tolerance
+        self.target_x_range = target_x_range
+        self.target_z_range = target_z_range
+
+        # Fixed parameters
+        self.obi_solver_position = np.array([-0.1, 0.31, -0.1])
+        self.number_of_particles = 289
+        self.number_of_sampled_particles = 10
+
+        # Env setup
+        self.load_cloth = False
+        self._load_obi_cloth()
+        self.ik_controller = RFUniverseController('franka', base_pos=np.array([-0.6, 0, 0]))
+        self.eef_orn = self.ik_controller.bullet_client.getQuaternionFromEuler([math.pi / 2, 0, math.pi / 2])
+
+        self.t = 0
+        self.goal = self._sample_goal()
+        self.action_space = spaces.Box(
+            low=-1, high=1, shape=(4,), dtype=np.float32
+        )
+        obs = self._get_obs()
+        self.observation_space = spaces.Dict({
+            'observation': spaces.Box(-np.inf, np.inf, shape=obs['observation'].shape, dtype=np.float32),
+            'desired_goal': spaces.Box(-np.inf, np.inf, shape=obs['desired_goal'].shape, dtype=np.float32),
+            'achieved_goal': spaces.Box(-np.inf, np.inf, shape=obs['achieved_goal'].shape, dtype=np.float32)
+        })
+
+    def step(self, action: np.ndarray):
+        pos_ctrl = action[:3] * 0.05
+        curr_pos = np.array(self.articulation_channel.data[1]['positions'][3])
+        pos_ctrl = curr_pos + pos_ctrl
+        joint_positions = self.ik_controller.calculate_ik(
+            pos_ctrl,
+            eef_orn=self.eef_orn
+        )
+
+        curr_gripper_width = self._get_gripper_width()
+        target_gripper_width = curr_gripper_width + action[3] * 0.2
+        target_gripper_width = np.clip(target_gripper_width, 0, 0.08)
+        joint_positions.append(target_gripper_width)
+
+        self._set_franka_joints(np.array(joint_positions))
+        self.t += 1
+
+        obs = self._get_obs()
+        done = False
+        info = {
+            'is_success': self._check_success(obs)
+        }
+        reward = self.compute_reward(obs['achieved_goal'], obs['desired_goal'], info)
+
+        return obs, reward, done, info
+
+    def reset(self):
+        super().reset()
+
+        self._destroy_obi_cloth()
+        self.env.reset()
+        self._load_obi_cloth()
+        self.goal = self._sample_goal()
+
+        self.t = 0
+        self.ik_controller.reset()
+        joint_positions = self.ik_controller.calculate_ik(
+            [0, 0.3, 0.1],
+            self.eef_orn
+        )
+        self.articulation_channel.set_action(
+            'SetJointPositionDirectly',
+            index=0,
+            joint_positions=joint_positions,
+        )
+
+        self.game_object_channel.set_action(
+            'SetTransform',
+            index=0,
+            position=list(self.goal.copy())
+        )
+
+        self._step()
+
+        return self._get_obs()
+
+    def seed(self, seed=None):
+        self.np_random, seed = seeding.np_random(seed)
+        return [seed]
+
+    def render(self, mode='human'):
+        self._step()
+
+    def compute_reward(self, achieved_goal, desired_goal, info):
+        distance = self._compute_goal_distance(achieved_goal, desired_goal)
+        if self.reward_type == 'sparse':
+            return -(distance > self.tolerance).astype(np.float32)
+        else:
+            return -distance
+
+    def _get_obs(self):
+        gripper_position = np.array(self.articulation_channel.data[1]['positions'][3])
+        gripper_velocity = np.array(self.articulation_channel.data[1]['velocities'][3])
+        gripper_width = self._get_gripper_width()
+        panda_obs = np.concatenate((gripper_position, gripper_velocity, [gripper_width]))
+
+        cloth_particles = np.array(self.obi_cloth_channel.data[0]['positions'])
+        random_indices = np.random.randint(0, self.number_of_particles, size=(self.number_of_sampled_particles,))
+        sampled_particles = cloth_particles[random_indices] + self.obi_solver_position
+        sampled_particles = np.reshape(sampled_particles, newshape=(3 * self.number_of_sampled_particles,))
+
+        obs = np.concatenate((panda_obs, sampled_particles))
+
+        cloth_center = np.average(cloth_particles, axis=0) + self.obi_solver_position
+
+        return {
+            'observation': obs.copy(),
+            'achieved_goal': cloth_center.copy(),
+            'desired_goal': self.goal.copy()
+        }
+
+    def _load_obi_cloth(self):
+        if self.load_cloth:
+            return
+        self.asset_channel.set_action(
+            'LoadObiCloth',
+            filename=self.asset_bundle_file,
+            name='Obi Solver',
+            position=list(self.obi_solver_position)
+        )
+        self._step()
+        self.load_cloth = True
+
+    def _destroy_obi_cloth(self):
+        if not self.load_cloth:
+            return
+        self.obi_cloth_channel.set_action(
+            'Destroy',
+            index=0
+        )
+        self._step()
+        self.load_cloth = False
+
+    def _get_gripper_width(self):
+        gripper_joint_positions = copy.deepcopy(self.articulation_channel.data[1]['joint_positions'])
+        return -1 * (gripper_joint_positions[0] + gripper_joint_positions[1])
+
+    def _set_franka_joints(self, a: np.ndarray):
+        self.articulation_channel.set_action(
+            'SetJointPosition',
+            index=0,
+            joint_positions=list(a[0:7]),
+        )
+        self._step()
+
+        a[7] = -1 * a[7] / 2
+        self.articulation_channel.set_action(
+            'SetJointPosition',
+            index=1,
+            joint_positions=[a[7], a[7]],
+        )
+        self._step()
+
+    def _generate_random_float(self, min: float, max: float) -> float:
+        assert min <= max, \
+            'Min value is {}, while max value is {}.'.format(min, max)
+        random_float = np.random.rand()
+        random_float = random_float * (max - min) + min
+
+        return random_float
+
+    def _compute_goal_distance(self, goal_a, goal_b):
+        assert goal_a.shape == goal_b.shape
+        return np.linalg.norm(goal_a - goal_b, axis=-1)
+
+    def _check_success(self, obs):
+        achieved_goal = obs['achieved_goal']
+        desired_goal = obs['desired_goal']
+        distance = self._compute_goal_distance(achieved_goal, desired_goal)
+
+        return (distance < self.tolerance).astype(np.float32)
+
+    def _sample_goal(self):
+        target_x = self._generate_random_float(self.target_x_range[0], self.target_x_range[1])
+        target_z = self._generate_random_float(self.target_z_range[0], self.target_z_range[1])
+
+        return np.array([target_x, 0.3, target_z])
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
-# from pyrfuniverse.utils import RFUniverseController
-import numpy as np
-from gym import spaces
-from gym.utils import seeding
-import copy
-
-
-class FrankaClothFoldEnv(RFUniverseGymGoalWrapper):
-    metadata = {'render.modes': ['human']}
-    height_offset = 0.01
-
-    def __init__(
-            self,
-            asset_bundle_file,
-            executable_file=None,
-            reward_type='sparse',
-            tolerance=0.05,
-            object_xz_range=0.055,
-            object_rotation_range=180,
-    ):
-        super().__init__(
-            executable_file=executable_file,
-            articulation_channel=True,
-            obi_cloth_with_grasping_channel=True,
-        )
-        self.reward_type = reward_type
-        self.tolerance = tolerance
-        self.object_xz_range = object_xz_range
-        self.object_rotation_range = object_rotation_range
-        self.object_range_low = np.array([-object_xz_range, self.height_offset, -object_xz_range])
-        self.object_range_high = np.array([object_xz_range, self.height_offset, object_xz_range])
-        self.asset_bundle_file = asset_bundle_file
-        self.ik_controller = RFUniverseController('franka', base_pos=np.array([-0.6, 0, 0]))
-        self.t = 0
-
-        self.has_loaded_object = False
-        self.goal = None
-        self.seed()
-        self._load_object()
-
-        self.action_space = spaces.Box(
-            low=-1, high=1, shape=(4,), dtype=np.float32
-        )
-        obs = self._get_obs()
-        self.observation_space = spaces.Dict({
-            'observation': spaces.Box(-np.inf, np.inf, shape=obs['observation'].shape, dtype=np.float32),
-            'desired_goal': spaces.Box(-np.inf, np.inf, shape=obs['desired_goal'].shape, dtype=np.float32),
-            'achieved_goal': spaces.Box(-np.inf, np.inf, shape=obs['achieved_goal'].shape, dtype=np.float32)
-        })
-
-    def step(self, action: np.ndarray):
-        pos_ctrl = action[:3] * 0.05
-        curr_pos = np.array(self.articulation_channel.data[1]['positions'][3])
-        pos_ctrl = curr_pos + pos_ctrl
-        joint_positions = self.ik_controller.calculate_ik_recursive(pos_ctrl)
-
-        curr_gripper_width = self._get_gripper_width()
-        target_gripper_width = curr_gripper_width + action[3] * 0.2
-        target_gripper_width = np.clip(target_gripper_width, 0, 0.08)
-        joint_positions.append(target_gripper_width)
-
-        self._set_franka_joints(np.array(joint_positions))
-        self.t += 1
-
-        obs = self._get_obs()
-        done = False
-        info = {
-            'is_success': self._check_success(obs)
-        }
-        reward = self.compute_reward(obs['achieved_goal'], obs['desired_goal'], info)
-
-        return obs, reward, done, info
-
-    def reset(self):
-        super().reset()
-        self._destroy_object()
-        self.env.reset()
-        self.ik_controller.reset()
-        self.t = 0
-        self._load_object()
-
-        grasp_position = self._get_grasp_position()
-        joint_positions = self.ik_controller.calculate_ik_recursive(grasp_position)
-        self.articulation_channel.set_action(
-            'SetJointPositionDirectly',
-            index=0,
-            joint_positions=list(joint_positions),
-        )
-        self._step()
-
-        return self._get_obs()
-
-    def seed(self, seed=1234):
-        self.np_random, seed = seeding.np_random(seed)
-        return [seed]
-
-    def render(self, mode='human'):
-        self._step()
-
-    def compute_reward(self, achieved_goal, desired_goal, info):
-        distance = self._compute_goal_distance(achieved_goal, desired_goal)
-        if self.reward_type == 'sparse':
-            return -(distance > self.tolerance).astype(np.float32)
-        else:
-            return -distance
-
-    def _get_obs(self):
-        gripper_position = np.array(self.articulation_channel.data[1]['positions'][3])
-        gripper_velocity = np.array(self.articulation_channel.data[1]['velocities'][3])
-        gripper_width = self._get_gripper_width()
-
-        panda_obs = np.concatenate((gripper_position, gripper_velocity, [gripper_width]))
-
-        grasp_position = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_position'])
-        grasp_rotation = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_rotation'])
-        grasp_velocity = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_velocity'])
-        grasp_angular_vel = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_angular_vel'])
-        achieved_goal = grasp_position.copy()
-
-        object_obs = np.concatenate((grasp_position, grasp_rotation, grasp_velocity, grasp_angular_vel))
-
-        obs = np.concatenate((panda_obs, object_obs))
-
-        return {
-            'observation': obs.copy(),
-            'achieved_goal': achieved_goal.copy(),
-            'desired_goal': self.goal.copy()
-        }
-
-    def _generate_random_float(self, min: float, max: float) -> float:
-        assert min < max, \
-            'Min value is {}, while max value is {}.'.format(min, max)
-        random_float = np.random.rand()
-        random_float = random_float * (max - min) + min
-
-        return random_float
-
-    def _set_franka_joints(self, a: np.ndarray):
-        self.articulation_channel.set_action(
-            'SetJointPosition',
-            index=0,
-            joint_positions=list(a[0:7]),
-        )
-        self._step()
-
-        a[7] = -1 * a[7] / 2
-        self.articulation_channel.set_action(
-            'SetJointPosition',
-            index=1,
-            joint_positions=[a[7], a[7]],
-        )
-        self._step()
-
-    def _get_gripper_width(self):
-        gripper_joint_positions = copy.deepcopy(self.articulation_channel.data[1]['joint_positions'])
-        return -1 * (gripper_joint_positions[0] + gripper_joint_positions[1])
-
-    def _check_success(self, obs):
-        achieved_goal = obs['achieved_goal']
-        desired_goal = obs['desired_goal']
-        distance = self._compute_goal_distance(achieved_goal, desired_goal)
-
-        return (distance < self.tolerance).astype(np.float32)
-
-    def _compute_goal_distance(self, goal_a, goal_b):
-        assert goal_a.shape == goal_b.shape
-        return np.linalg.norm(goal_a - goal_b, axis=-1)
-
-    def _load_object(self):
-        assert self.asset_bundle_file is not None, \
-            'There must be an asset bundle file to load.'
-
-        object_name = 'Obi Solver For Grasp'
-        position = self.np_random.uniform(self.object_range_low, self.object_range_high)
-        rotation = [0, self._generate_random_float(-self.object_rotation_range, self.object_rotation_range), 0]
-
-        self.asset_channel.set_action(
-            'LoadObiClothWithGrasping',
-            filename=self.asset_bundle_file,
-            name=object_name,
-            position=position,
-            rotation=rotation
-        )
-        self._step()
-        self.has_loaded_object = True
-        self.goal = np.array(self.obi_cloth_with_grasping_channel.data[0]['target_position'])
-
-    def _destroy_object(self):
-        self.obi_cloth_with_grasping_channel.set_action(
-            'Destroy',
-            index=0
-        )
-        self._step()
-        self.has_loaded_object = False
-        self.goal = None
-
-    def _get_grasp_position(self):
-        assert self.has_loaded_object, \
-            'No object loaded.'
-        grasp_position = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_position'])
-
-        return grasp_position
+from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
+# from pyrfuniverse.utils import RFUniverseController
+import numpy as np
+from gym import spaces
+from gym.utils import seeding
+import copy
+
+
+class FrankaClothFoldEnv(RFUniverseGymGoalWrapper):
+    metadata = {'render.modes': ['human']}
+    height_offset = 0.01
+
+    def __init__(
+            self,
+            asset_bundle_file,
+            executable_file=None,
+            reward_type='sparse',
+            tolerance=0.05,
+            object_xz_range=0.055,
+            object_rotation_range=180,
+    ):
+        super().__init__(
+            executable_file=executable_file,
+            articulation_channel=True,
+            obi_cloth_with_grasping_channel=True,
+        )
+        self.reward_type = reward_type
+        self.tolerance = tolerance
+        self.object_xz_range = object_xz_range
+        self.object_rotation_range = object_rotation_range
+        self.object_range_low = np.array([-object_xz_range, self.height_offset, -object_xz_range])
+        self.object_range_high = np.array([object_xz_range, self.height_offset, object_xz_range])
+        self.asset_bundle_file = asset_bundle_file
+        self.ik_controller = RFUniverseController('franka', base_pos=np.array([-0.6, 0, 0]))
+        self.t = 0
+
+        self.has_loaded_object = False
+        self.goal = None
+        self.seed()
+        self._load_object()
+
+        self.action_space = spaces.Box(
+            low=-1, high=1, shape=(4,), dtype=np.float32
+        )
+        obs = self._get_obs()
+        self.observation_space = spaces.Dict({
+            'observation': spaces.Box(-np.inf, np.inf, shape=obs['observation'].shape, dtype=np.float32),
+            'desired_goal': spaces.Box(-np.inf, np.inf, shape=obs['desired_goal'].shape, dtype=np.float32),
+            'achieved_goal': spaces.Box(-np.inf, np.inf, shape=obs['achieved_goal'].shape, dtype=np.float32)
+        })
+
+    def step(self, action: np.ndarray):
+        pos_ctrl = action[:3] * 0.05
+        curr_pos = np.array(self.articulation_channel.data[1]['positions'][3])
+        pos_ctrl = curr_pos + pos_ctrl
+        joint_positions = self.ik_controller.calculate_ik_recursive(pos_ctrl)
+
+        curr_gripper_width = self._get_gripper_width()
+        target_gripper_width = curr_gripper_width + action[3] * 0.2
+        target_gripper_width = np.clip(target_gripper_width, 0, 0.08)
+        joint_positions.append(target_gripper_width)
+
+        self._set_franka_joints(np.array(joint_positions))
+        self.t += 1
+
+        obs = self._get_obs()
+        done = False
+        info = {
+            'is_success': self._check_success(obs)
+        }
+        reward = self.compute_reward(obs['achieved_goal'], obs['desired_goal'], info)
+
+        return obs, reward, done, info
+
+    def reset(self):
+        super().reset()
+        self._destroy_object()
+        self.env.reset()
+        self.ik_controller.reset()
+        self.t = 0
+        self._load_object()
+
+        grasp_position = self._get_grasp_position()
+        joint_positions = self.ik_controller.calculate_ik_recursive(grasp_position)
+        self.articulation_channel.set_action(
+            'SetJointPositionDirectly',
+            index=0,
+            joint_positions=list(joint_positions),
+        )
+        self._step()
+
+        return self._get_obs()
+
+    def seed(self, seed=1234):
+        self.np_random, seed = seeding.np_random(seed)
+        return [seed]
+
+    def render(self, mode='human'):
+        self._step()
+
+    def compute_reward(self, achieved_goal, desired_goal, info):
+        distance = self._compute_goal_distance(achieved_goal, desired_goal)
+        if self.reward_type == 'sparse':
+            return -(distance > self.tolerance).astype(np.float32)
+        else:
+            return -distance
+
+    def _get_obs(self):
+        gripper_position = np.array(self.articulation_channel.data[1]['positions'][3])
+        gripper_velocity = np.array(self.articulation_channel.data[1]['velocities'][3])
+        gripper_width = self._get_gripper_width()
+
+        panda_obs = np.concatenate((gripper_position, gripper_velocity, [gripper_width]))
+
+        grasp_position = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_position'])
+        grasp_rotation = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_rotation'])
+        grasp_velocity = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_velocity'])
+        grasp_angular_vel = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_angular_vel'])
+        achieved_goal = grasp_position.copy()
+
+        object_obs = np.concatenate((grasp_position, grasp_rotation, grasp_velocity, grasp_angular_vel))
+
+        obs = np.concatenate((panda_obs, object_obs))
+
+        return {
+            'observation': obs.copy(),
+            'achieved_goal': achieved_goal.copy(),
+            'desired_goal': self.goal.copy()
+        }
+
+    def _generate_random_float(self, min: float, max: float) -> float:
+        assert min < max, \
+            'Min value is {}, while max value is {}.'.format(min, max)
+        random_float = np.random.rand()
+        random_float = random_float * (max - min) + min
+
+        return random_float
+
+    def _set_franka_joints(self, a: np.ndarray):
+        self.articulation_channel.set_action(
+            'SetJointPosition',
+            index=0,
+            joint_positions=list(a[0:7]),
+        )
+        self._step()
+
+        a[7] = -1 * a[7] / 2
+        self.articulation_channel.set_action(
+            'SetJointPosition',
+            index=1,
+            joint_positions=[a[7], a[7]],
+        )
+        self._step()
+
+    def _get_gripper_width(self):
+        gripper_joint_positions = copy.deepcopy(self.articulation_channel.data[1]['joint_positions'])
+        return -1 * (gripper_joint_positions[0] + gripper_joint_positions[1])
+
+    def _check_success(self, obs):
+        achieved_goal = obs['achieved_goal']
+        desired_goal = obs['desired_goal']
+        distance = self._compute_goal_distance(achieved_goal, desired_goal)
+
+        return (distance < self.tolerance).astype(np.float32)
+
+    def _compute_goal_distance(self, goal_a, goal_b):
+        assert goal_a.shape == goal_b.shape
+        return np.linalg.norm(goal_a - goal_b, axis=-1)
+
+    def _load_object(self):
+        assert self.asset_bundle_file is not None, \
+            'There must be an asset bundle file to load.'
+
+        object_name = 'Obi Solver For Grasp'
+        position = self.np_random.uniform(self.object_range_low, self.object_range_high)
+        rotation = [0, self._generate_random_float(-self.object_rotation_range, self.object_rotation_range), 0]
+
+        self.asset_channel.set_action(
+            'LoadObiClothWithGrasping',
+            filename=self.asset_bundle_file,
+            name=object_name,
+            position=position,
+            rotation=rotation
+        )
+        self._step()
+        self.has_loaded_object = True
+        self.goal = np.array(self.obi_cloth_with_grasping_channel.data[0]['target_position'])
+
+    def _destroy_object(self):
+        self.obi_cloth_with_grasping_channel.set_action(
+            'Destroy',
+            index=0
+        )
+        self._step()
+        self.has_loaded_object = False
+        self.goal = None
+
+    def _get_grasp_position(self):
+        assert self.has_loaded_object, \
+            'No object loaded.'
+        grasp_position = np.array(self.obi_cloth_with_grasping_channel.data[0]['grasp_position'])
+
+        return grasp_position
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_robotics_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_robotics_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_softbody_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/ur5_drawer_env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,221 +1,259 @@
-from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
-# from pyrfuniverse.utils import RFUniverseController
+from pyrfuniverse.envs import RFUniverseGymGoalWrapper
+from pyrfuniverse.utils.ur5_controller import RFUniverseUR5Controller
+import pyrfuniverse
 import numpy as np
-import math
-import copy
 from gym import spaces
 from gym.utils import seeding
+import math
+import pybullet as p
+import os
 
 
-class FrankaSoftbodyEnv(RFUniverseGymGoalWrapper):
+class Ur5DrawerEnv(RFUniverseGymGoalWrapper):
     metadata = {'render.modes': ['human']}
 
     def __init__(
             self,
-            asset_bundle_file,
-            reward_type,
-            open_gripper=True,
-            tolerance=0.05,
-            goal_xz_range=0.15,
-            softbody_xz_range=0.15,
+            max_steps,
+            reward_type='dense',
+            min_open_distance=0.08,
+            seed=None,
             executable_file=None,
+            asset_bundle_file=None,
+            assets: list = []
     ):
         super().__init__(
             executable_file=executable_file,
+            camera_channel=True,
             articulation_channel=True,
-            game_object_channel=True,
-            obi_softbody_channel=True
+            assets=assets
         )
-        self.asset_bundle_file = asset_bundle_file
+        self.asset_channel.set_action(
+            'InstanceObject',
+            name='ur5_robotiq85',
+            id=123,
+        )
+        self.articulation_channel.set_action(
+            'SetTransform',
+            id=123,
+            position=[0, 0, 0],
+            rotation=[0, -90, 0],
+        )
+        self.asset_channel.set_action(
+            'InstanceObject',
+            name='handled_drawer',
+            id=456,
+        )
+        self.articulation_channel.set_action(
+            'SetTransform',
+            id=456,
+            position=[-0.721, 0.5, -0.538],
+            rotation=[-90, 180, 0],
+        )
+        self.camera_channel.set_action(
+            'AddCamera',
+            id=0,
+            position=[-0.25, 0.712, -0.914],
+            rotation=[26.997, -13.874, 0],
+        )
+        self._step()
+        self.max_steps = max_steps
         self.reward_type = reward_type
-        self.open_gripper = open_gripper
-        self.tolerance = tolerance
+        self.min_open_distance = min_open_distance
+        self.asset_bundle_file = asset_bundle_file
 
-        # Fixed parameters
-        self.scale = 10.0
-        self.goal_center_position = np.array([-0.6, 0.015, 0])
-        self.softbody_center_position = np.array([-0.6, 0.022, 0])
-        self.goal_range_low = self.goal_center_position - np.array([goal_xz_range, 0, goal_xz_range])
-        self.goal_range_high = self.goal_center_position + np.array([goal_xz_range, 0, goal_xz_range])
-        self.softbody_range_low = self.softbody_center_position - np.array([softbody_xz_range, 0, softbody_xz_range])
-        self.softbody_range_high = self.softbody_center_position + np.array([softbody_xz_range, 0, softbody_xz_range])
-
-        # Env setup
-        self.seed()
-        self.load_softbody = False
-        self._load_obi_softbody()
-        self.ik_controller = RFUniverseController('franka', base_pos=np.array([0, 0, 0]))
+        self.seed(seed)
+        self.ik_controller = RFUniverseUR5Controller(
+            robot_urdf=os.path.join(pyrfuniverse.assets_path, 'RoboTube/DrawerClosing/UR5/ur5_robotiq_85.urdf'),
+            init_joint_positions=[90, -60, 60, 90, 90, 0],
+        )
         self.t = 0
-        self.goal = self._sample_goal()
+        self.goal = np.array([self.min_open_distance])
         self.action_space = spaces.Box(
             low=-1, high=1, shape=(4,), dtype=np.float32
         )
         obs = self._get_obs()
         self.observation_space = spaces.Dict({
             'observation': spaces.Box(-np.inf, np.inf, shape=obs['observation'].shape, dtype=np.float32),
             'desired_goal': spaces.Box(-np.inf, np.inf, shape=obs['desired_goal'].shape, dtype=np.float32),
             'achieved_goal': spaces.Box(-np.inf, np.inf, shape=obs['achieved_goal'].shape, dtype=np.float32)
         })
+        self.eef_orn = p.getQuaternionFromEuler([math.pi, 0, 0])
 
     def step(self, action: np.ndarray):
-        pos_ctrl = action[:3] * 0.05
+        action_ctrl = action.copy()
+        pos_ctrl = action_ctrl[:3] * 0.05
         curr_pos = self._get_gripper_position()
-        pos_ctrl = curr_pos + pos_ctrl
-        joint_positions = self.ik_controller.calculate_ik(pos_ctrl)
+        pos_ctrl = pos_ctrl + curr_pos
+        joint_positions = self.ik_controller.calculate_ik_recursive(pos_ctrl, eef_orn=self.eef_orn)
 
-        if self.open_gripper:
-            curr_gripper_width = self._get_gripper_width()
-            target_gripper_width = curr_gripper_width + action[3] * 0.2
-            target_gripper_width = np.clip(target_gripper_width, 0, 0.08)
-            joint_positions.append(target_gripper_width)
-        else:
-            joint_positions.append(0)
+        gripper_width = self._get_gripper_width()
+        gripper_width_ctrl = np.clip(gripper_width + action_ctrl[3] * 0.2, 0, 0.085)
+        gripper_angle = self._compute_gripper_angle(gripper_width_ctrl)
+        joint_positions.append(gripper_angle)
 
-        self._set_franka_joints(np.array(joint_positions))
+        self._set_ur5_robotiq85_joints(joint_positions)
         self.t += 1
 
         obs = self._get_obs()
         done = False
         info = {
             'is_success': self._check_success(obs)
         }
-        # if info['is_success'] > 0:
-        #     print('Success')
         reward = self.compute_reward(obs['achieved_goal'], obs['desired_goal'], info)
 
+        if self.t == self.max_steps:
+            obs = self.reset()
+            done = True
+
         return obs, reward, done, info
 
     def reset(self):
         super().reset()
-
-        self._destroy_obi_softbody()
         self.env.reset()
-        if not self.open_gripper:
-            self.articulation_channel.set_action(
-                'SetJointPositionDirectly',
-                index=1,
-                joint_positions=[0, 0],
-            )
-
-        obi_softbody_solver_position = self._load_obi_softbody()
-        self.goal = self._sample_goal()
-        self.game_object_channel.set_action(
-            'SetTransform',
-            index=0,
-            position=list(self.goal * self.scale)
-        )
-
-        self.t = 0
         self.ik_controller.reset()
-        joint_positions = self.ik_controller.calculate_ik_recursive(
-            list(obi_softbody_solver_position),
-        )
-        self.articulation_channel.set_action(
-            'SetJointPositionDirectly',
-            index=0,
-            joint_positions=list(joint_positions),
-        )
-        self._step()
+        self.t = 0
+
+        handle_position = np.array(self.articulation_channel.data[456]['positions'][3])
+        joint_positions = self.ik_controller.calculate_ik_recursive(handle_position, eef_orn=self.eef_orn)
+        gripper_angle = self._compute_gripper_angle(0.085)
+        joint_positions.append(gripper_angle)
+        self._set_ur5_robotiq85_joints_directly(joint_positions)
 
         return self._get_obs()
 
     def seed(self, seed=1234):
         self.np_random, seed = seeding.np_random(seed)
         return [seed]
 
     def render(self, mode='human'):
+        self.camera_channel.set_action(
+            'GetImages',
+            rendering_params=[[0, 320, 240]]
+        )
+        self._step()
+        img = self.camera_channel.images.pop(0)
+
+        return img
+
+    def load_drawer(self, name, position, rotation):
+        self.asset_channel.set_action(
+            'LoadArticulationBody',
+            filename=self.asset_bundle_file,
+            name=name,
+            position=position,
+            rotation=rotation
+        )
+        self._step()
+
+    def destroy_drawer(self, index):
+        self.articulation_channel.set_action(
+            'Destroy',
+            index=index + 2
+        )
         self._step()
 
     def compute_reward(self, achieved_goal, desired_goal, info):
-        distance = self._compute_goal_distance(achieved_goal, desired_goal)
-        if self.reward_type == 'sparse':
-            return -(distance > self.tolerance).astype(np.float32)
+        if self.reward_type == 'dense':
+            return float(achieved_goal)
         else:
-            return -distance
+            overhead_angle = achieved_goal - desired_goal
+            return float(overhead_angle[0] > 0)
 
-    def _get_obs(self): #
-        gripper_position = np.array(self.articulation_channel.data[1]['positions'][3])
-        gripper_velocity = np.array(self.articulation_channel.data[1]['velocities'][3])
-        gripper_width = self._get_gripper_width()
-        panda_obs = np.concatenate((gripper_position, gripper_velocity, [gripper_width])) / self.scale
+    def add_camera(self, position, rotation):
+        self.camera_channel.set_action(
+            'AddCamera',
+            position=position,
+            rotation=rotation,
+        )
+        self._step()
 
-        softbody_position = np.array(self.obi_softbody_channel.data[0]['position']) / self.scale
-        softbody_orientation = np.array(self.obi_softbody_channel.data[0]['orientation'])
-        softbody_velocity = np.array(self.obi_softbody_channel.data[0]['velocity']) / self.scale
-        softbody_angular_vel = np.array(self.obi_softbody_channel.data[0]['angular_vel'])
-        softbody_obs = np.concatenate(
-            (softbody_position, softbody_orientation, softbody_velocity, softbody_angular_vel)
+    def get_images(self):
+        self.camera_channel.set_action(
+            'GetImages',
+            rendering_params=[[0, 320, 240], [1, 320, 240]]
         )
+        self._step()
+
+        img_rgb = self.camera_channel.images.pop(0)
+        img_depth = self.camera_channel.images.pop(0)
 
-        obs = np.concatenate((panda_obs, softbody_obs))
+        return img_rgb, img_depth
+
+    def _get_obs(self):
+        gripper_position = self._get_gripper_position()
+        gripper_width = self._get_gripper_width()
+
+        robot_obs = np.concatenate((gripper_position, [gripper_width]))
+
+        handle_position = np.array(self.articulation_channel.data[456]['positions'][3])
+        drawer_open_distance = np.array([self.articulation_channel.data[456]['joint_positions'][0]])
+
+        object_obs = np.concatenate((handle_position, drawer_open_distance))
+
+        obs = np.concatenate((robot_obs, object_obs))
 
         return {
             'observation': obs.copy(),
-            'achieved_goal': softbody_position.copy(),
+            'achieved_goal': drawer_open_distance.copy(),
             'desired_goal': self.goal.copy()
         }
 
-    def _load_obi_softbody(self):
-        if self.load_softbody:
-            return
-        obi_softbody_solver_position = self.np_random.uniform(
-            self.softbody_range_low, self.softbody_range_high
-        )
-        self.asset_channel.set_action(
-            'LoadObiSoftbody',
-            filename=self.asset_bundle_file,
-            name='Obi Softbody Solver',
-            position=list(obi_softbody_solver_position * self.scale)
-        )
-        self._step()
-        self.load_softbody = True
+    def _get_gripper_position(self):
+        return np.array(self.articulation_channel.data[1230]['positions'][11])
 
-        return obi_softbody_solver_position
+    def _get_gripper_width(self):
+        right_inner_finger_pos = np.array(self.articulation_channel.data[1230]['positions'][5])
+        left_inner_finger_pos = np.array(self.articulation_channel.data[1230]['positions'][10])
+        width = self._compute_distance(right_inner_finger_pos, left_inner_finger_pos)
 
-    def _destroy_obi_softbody(self):
-        if not self.load_softbody:
-            return
-        self.obi_softbody_channel.set_action(
-            'Destroy',
-            index=0
-        )
-        self._step()
-        self.load_softbody = False
+        # The position is at the center of inner_finger, so we must get rid of the width of inner finger,
+        # to get accurate gripper width
+        width = width - 0.00635
 
-    def _sample_goal(self):
-        goal = self.np_random.uniform(self.goal_range_low, self.goal_range_high)
-        return goal.copy()
+        return width
 
-    def _get_gripper_position(self):
-        return np.array(self.articulation_channel.data[1]['positions'][3]) / self.scale
+    def _compute_gripper_angle(self, width):
+        angle_rad = 0.715 - math.asin((width - 0.01) / 0.1143)
+        angle_deg = angle_rad * 180 / math.pi
 
-    def _get_gripper_width(self):
-        gripper_joint_positions = copy.deepcopy(self.articulation_channel.data[1]['joint_positions'])
-        return -1 * (gripper_joint_positions[0] + gripper_joint_positions[1]) / self.scale
+        return angle_deg
 
-    def _set_franka_joints(self, a: np.ndarray):
+    def _set_ur5_robotiq85_joints(self, joint_positions):
         self.articulation_channel.set_action(
             'SetJointPosition',
-            index=0,
-            joint_positions=list(a[0:7]),
+            id=123,
+            joint_positions=list(joint_positions[:6])
         )
-        self._step()
+        #self._step()
 
-        a[7] = -1 * a[7] / 2 * self.scale
         self.articulation_channel.set_action(
             'SetJointPosition',
-            index=1,
-            joint_positions=[a[7], a[7]],
+            id=1230,
+            joint_positions=[joint_positions[6], joint_positions[6]],
+        )
+        self._step()
+
+    def _set_ur5_robotiq85_joints_directly(self, joint_positions):
+        self.articulation_channel.set_action(
+            'SetJointPositionDirectly',
+            id=123,
+            joint_positions=list(joint_positions[:6])
+        )
+        #self._step()
+
+        self.articulation_channel.set_action(
+            'SetJointPositionDirectly',
+            id=1230,
+            joint_positions=[joint_positions[6], joint_positions[6]],
         )
         self._step()
 
-    def _compute_goal_distance(self, goal_a, goal_b):
-        assert goal_a.shape == goal_b.shape
-        return np.linalg.norm(goal_a - goal_b, axis=-1)
+    def _compute_distance(self, point_a, point_b):
+        return np.linalg.norm(point_a - point_b, axis=-1)
 
     def _check_success(self, obs):
-        achieved_goal = obs['achieved_goal']
-        desired_goal = obs['desired_goal']
-        distance = self._compute_goal_distance(achieved_goal, desired_goal)
+        achieved_goal = obs['achieved_goal'][0]
+        desired_goal = obs['desired_goal'][0]
 
-        return (distance < self.tolerance).astype(np.float32)
+        return (desired_goal < achieved_goal).astype(np.float32)
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/pick_and_place_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/pick_and_place_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/push_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/reach_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/reach_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/roller_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/roller_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-import pyrfuniverse
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-from pyrfuniverse.utils.tobor_controller import RFUniverseToborController
-import numpy as np
-
-
-class ToborRobotiq85ManipulationEnv(RFUniverseBaseEnv):
-    def __init__(
-            self,
-            task_name,
-            scene_file=None,
-            only_calculate=False,
-            left_init_joint_positions=[0] * 7,
-            right_init_joint_positions=[0] * 7
-    ):
-        super().__init__(
-            scene_file=scene_file,
-        )
-        self.GetAttr(9874610).EnabledNativeIK(enabled=False)
-        self.GetAttr(9874611).EnabledNativeIK(enabled=False)
-        self._step()
-        self.ik_controller = RFUniverseToborController(
-            urdf_folder='../URDF/tobor',
-            left_hand='robotiq85',
-            right_hand='robotiq85',
-            left_init_joint_positions=left_init_joint_positions,
-            right_init_joint_positions=right_init_joint_positions,
-            revise=True
-        )
-
-        # Init joint positions
-        self.left_init_joint_positions = left_init_joint_positions
-        self.left_joint_positions = self.left_init_joint_positions.copy()
-        self.right_init_joint_positions = right_init_joint_positions
-        self.right_joint_positions = self.right_init_joint_positions.copy()
-
-        self.left_gripper_open = True
-        self.right_gripper_open = True
-        self.task_name = task_name
-        self.record_file = '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/tobor_manipulation_{}.txt'.format(self.task_name)
-        self.only_calculate = only_calculate
-        #with open(self.record_file, 'w') as f:
-            #f.close()
-
-    def step(self, mode, position: np.ndarray, orientation=None):
-        if mode == 'left':
-            # Robotiq85
-            current_position = np.array(self.GetAttr(98746100).data['positions'][7])
-        else:
-            # Robotiq85
-            current_position = np.array(self.GetAttr(98746110).data['positions'][7])
-
-        distance = position - current_position
-        time_steps = int(np.abs(distance / 0.05).max()) + 1
-        unit_distance = distance / time_steps
-
-        for i in range(time_steps):
-            target_position = current_position + unit_distance * (i + 1)
-            joint_positions = self.ik_controller.calculate_ik(
-                mode,
-                target_position,
-                orientation
-            )
-
-            if mode == 'left':
-                self.left_joint_positions = joint_positions
-                if not self.only_calculate:
-                    self.GetAttr(9874610).SetJointPosition(
-                        joint_positions=list(joint_positions),
-                    )
-            else:
-                self.right_joint_positions = joint_positions
-                if not self.only_calculate:
-                    self.GetAttr(9874611).SetJointPosition(
-                        joint_positions=list(joint_positions),
-                    )
-
-            for j in range(20):
-                if not self.only_calculate:
-                    self._step()
-                self.write()
-
-
-    def double_step(self, left_pos, right_pos, left_orn=None, right_orn=None):
-        left_current_pos = np.array(self.GetAttr(98746100).data['positions'][7])
-        left_distance = left_pos - left_current_pos
-        left_time_steps = int(np.abs(left_distance / 0.05).max()) + 1
-
-        right_current_pos = np.array(self.GetAttr(98746110).data['positions'][7])
-        right_distance = right_pos - right_current_pos
-        right_time_steps = int(np.abs(right_distance / 0.05).max()) + 1
-
-        time_steps = max(left_time_steps, right_time_steps)
-        left_unit_distance = left_distance / time_steps
-        right_unit_distance = right_distance / time_steps
-
-        for i in range(time_steps):
-            left_target_position = left_current_pos + left_unit_distance * (i + 1)
-            right_target_position = right_current_pos + right_unit_distance * (i + 1)
-            left_joint_positions = self.ik_controller.calculate_ik(
-                'left',
-                left_target_position,
-                left_orn
-            )
-            self.left_joint_positions = left_joint_positions
-            right_joint_positions = self.ik_controller.calculate_ik(
-                'right',
-                right_target_position,
-                right_orn
-            )
-            self.right_joint_positions = right_joint_positions
-
-            if not self.only_calculate:
-                self.GetAttr(9874610).SetJointPosition(
-                    joint_positions=list(left_joint_positions),
-                )
-                self._step()
-                self.GetAttr(9874611).SetJointPosition(
-                    joint_positions=list(right_joint_positions),
-                )
-
-            for j in range(20):
-                if not self.only_calculate:
-                    self._step()
-                self.write()
-
-    def double_close(self):
-        if not self.only_calculate:
-            self.GetAttr(98746100).SetJointPosition(
-                joint_positions=[50, 50]
-            )
-            self.left_gripper_open = False
-            self._step()
-            self.GetAttr(98746110).SetJointPosition(
-                joint_positions=[50, 50]
-            )
-            self.right_gripper_open = False
-            self._step()
-
-        for i in range(20):
-            if not self.only_calculate:
-                self._step()
-            self.write()
-
-    def double_open(self):
-        if not self.only_calculate:
-            self.GetAttr(98746100).SetJointPosition(
-                joint_positions=[0, 0]
-            )
-            self.left_gripper_open = True
-            self._step()
-            self.GetAttr(98746110).SetJointPosition(
-                joint_positions=[0, 0]
-            )
-            self.right_gripper_open = True
-            self._step()
-
-        for i in range(20):
-            if not self.only_calculate:
-                self._step()
-            self.write()
-
-    def reset(self):
-        self.GetAttr(9874610).SetJointPositionDirectly(
-            joint_positions=self.left_init_joint_positions
-        )
-        self._step()
-        self.GetAttr(9874611).SetJointPositionDirectly(
-            joint_positions=self.right_init_joint_positions
-        )
-        self._step()
-
-    def close_gripper(self, mode):
-        if not self.only_calculate:
-            if mode == 'left':
-                self.GetAttr(98746100).SetJointPosition(
-                    joint_positions=[50, 50]
-                )
-                self.left_gripper_open = False
-            else:
-                self.GetAttr(98746110).SetJointPosition(
-                    joint_positions=[50, 50]
-                )
-                self.right_gripper_open = False
-        for i in range(20):
-            if not self.only_calculate:
-                self._step()
-            self.write()
-
-
-    def open_gripper(self, mode):
-        if not self.only_calculate:
-            if mode == 'left':
-                self.GetAttr(98746100).SetJointPosition(
-                    joint_positions=[0, 0]
-                )
-                self.left_gripper_open = True
-            else:
-                self.GetAttr(98746110).SetJointPosition(
-                    joint_positions=[0, 0]
-                )
-                self.right_gripper_open = True
-        for i in range(20):
-            if not self.only_calculate:
-                self._step()
-            self.write()
-
-
-    def wait(self, n_timesteps):
-        for i in range(n_timesteps):
-            if not self.only_calculate:
-                self._step()
-            self.write()
-
-
-    def write(self):
-        '''
-        with open(self.record_file, 'a+') as f:
-            line = ''
-            for joint_position in self.left_joint_positions:
-                line += str(joint_position) + ','
-            for joint_position in self.right_joint_positions:
-                line += str(joint_position) + ','
-
-            if self.left_gripper_open:
-                line += '0,0,'
-            else:
-                line += '50,50,'
-
-            if self.right_gripper_open:
-                line += '0,0\n'
-            else:
-                line += '50,50\n'
-
-            f.write(line)
-            '''
-
-    def write_raw(self, raw_str):
-        with open(self.record_file, 'a+') as f:
-            f.write(raw_str)
-
-    def get_current_position(self, mode):
-        if mode == 'left':
-            return np.array(self.GetAttr(98746100).data['positions'][7])
-        elif mode == 'right':
-            return np.array(self.GetAttr(98746110).data['positions'][7])
-
+import pyrfuniverse
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+from pyrfuniverse.utils.tobor_controller import RFUniverseToborController
+import numpy as np
+
+
+class ToborRobotiq85ManipulationEnv(RFUniverseBaseEnv):
+    def __init__(
+            self,
+            task_name,
+            scene_file=None,
+            only_calculate=False,
+            left_init_joint_positions=[0] * 7,
+            right_init_joint_positions=[0] * 7
+    ):
+        super().__init__(
+            scene_file=scene_file,
+        )
+        self.GetAttr(9874610).EnabledNativeIK(enabled=False)
+        self.GetAttr(9874611).EnabledNativeIK(enabled=False)
+        self._step()
+        self.ik_controller = RFUniverseToborController(
+            urdf_folder='../URDF/tobor',
+            left_hand='robotiq85',
+            right_hand='robotiq85',
+            left_init_joint_positions=left_init_joint_positions,
+            right_init_joint_positions=right_init_joint_positions,
+            revise=True
+        )
+
+        # Init joint positions
+        self.left_init_joint_positions = left_init_joint_positions
+        self.left_joint_positions = self.left_init_joint_positions.copy()
+        self.right_init_joint_positions = right_init_joint_positions
+        self.right_joint_positions = self.right_init_joint_positions.copy()
+
+        self.left_gripper_open = True
+        self.right_gripper_open = True
+        self.task_name = task_name
+        self.record_file = '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/tobor_manipulation_{}.txt'.format(self.task_name)
+        self.only_calculate = only_calculate
+        #with open(self.record_file, 'w') as f:
+            #f.close()
+
+    def step(self, mode, position: np.ndarray, orientation=None):
+        if mode == 'left':
+            # Robotiq85
+            current_position = np.array(self.GetAttr(98746100).data['positions'][7])
+        else:
+            # Robotiq85
+            current_position = np.array(self.GetAttr(98746110).data['positions'][7])
+
+        distance = position - current_position
+        time_steps = int(np.abs(distance / 0.05).max()) + 1
+        unit_distance = distance / time_steps
+
+        for i in range(time_steps):
+            target_position = current_position + unit_distance * (i + 1)
+            joint_positions = self.ik_controller.calculate_ik(
+                mode,
+                target_position,
+                orientation
+            )
+
+            if mode == 'left':
+                self.left_joint_positions = joint_positions
+                if not self.only_calculate:
+                    self.GetAttr(9874610).SetJointPosition(
+                        joint_positions=list(joint_positions),
+                    )
+            else:
+                self.right_joint_positions = joint_positions
+                if not self.only_calculate:
+                    self.GetAttr(9874611).SetJointPosition(
+                        joint_positions=list(joint_positions),
+                    )
+
+            for j in range(20):
+                if not self.only_calculate:
+                    self._step()
+                self.write()
+
+
+    def double_step(self, left_pos, right_pos, left_orn=None, right_orn=None):
+        left_current_pos = np.array(self.GetAttr(98746100).data['positions'][7])
+        left_distance = left_pos - left_current_pos
+        left_time_steps = int(np.abs(left_distance / 0.05).max()) + 1
+
+        right_current_pos = np.array(self.GetAttr(98746110).data['positions'][7])
+        right_distance = right_pos - right_current_pos
+        right_time_steps = int(np.abs(right_distance / 0.05).max()) + 1
+
+        time_steps = max(left_time_steps, right_time_steps)
+        left_unit_distance = left_distance / time_steps
+        right_unit_distance = right_distance / time_steps
+
+        for i in range(time_steps):
+            left_target_position = left_current_pos + left_unit_distance * (i + 1)
+            right_target_position = right_current_pos + right_unit_distance * (i + 1)
+            left_joint_positions = self.ik_controller.calculate_ik(
+                'left',
+                left_target_position,
+                left_orn
+            )
+            self.left_joint_positions = left_joint_positions
+            right_joint_positions = self.ik_controller.calculate_ik(
+                'right',
+                right_target_position,
+                right_orn
+            )
+            self.right_joint_positions = right_joint_positions
+
+            if not self.only_calculate:
+                self.GetAttr(9874610).SetJointPosition(
+                    joint_positions=list(left_joint_positions),
+                )
+                self._step()
+                self.GetAttr(9874611).SetJointPosition(
+                    joint_positions=list(right_joint_positions),
+                )
+
+            for j in range(20):
+                if not self.only_calculate:
+                    self._step()
+                self.write()
+
+    def double_close(self):
+        if not self.only_calculate:
+            self.GetAttr(98746100).SetJointPosition(
+                joint_positions=[50, 50]
+            )
+            self.left_gripper_open = False
+            self._step()
+            self.GetAttr(98746110).SetJointPosition(
+                joint_positions=[50, 50]
+            )
+            self.right_gripper_open = False
+            self._step()
+
+        for i in range(20):
+            if not self.only_calculate:
+                self._step()
+            self.write()
+
+    def double_open(self):
+        if not self.only_calculate:
+            self.GetAttr(98746100).SetJointPosition(
+                joint_positions=[0, 0]
+            )
+            self.left_gripper_open = True
+            self._step()
+            self.GetAttr(98746110).SetJointPosition(
+                joint_positions=[0, 0]
+            )
+            self.right_gripper_open = True
+            self._step()
+
+        for i in range(20):
+            if not self.only_calculate:
+                self._step()
+            self.write()
+
+    def reset(self):
+        self.GetAttr(9874610).SetJointPositionDirectly(
+            joint_positions=self.left_init_joint_positions
+        )
+        self._step()
+        self.GetAttr(9874611).SetJointPositionDirectly(
+            joint_positions=self.right_init_joint_positions
+        )
+        self._step()
+
+    def close_gripper(self, mode):
+        if not self.only_calculate:
+            if mode == 'left':
+                self.GetAttr(98746100).SetJointPosition(
+                    joint_positions=[50, 50]
+                )
+                self.left_gripper_open = False
+            else:
+                self.GetAttr(98746110).SetJointPosition(
+                    joint_positions=[50, 50]
+                )
+                self.right_gripper_open = False
+        for i in range(20):
+            if not self.only_calculate:
+                self._step()
+            self.write()
+
+
+    def open_gripper(self, mode):
+        if not self.only_calculate:
+            if mode == 'left':
+                self.GetAttr(98746100).SetJointPosition(
+                    joint_positions=[0, 0]
+                )
+                self.left_gripper_open = True
+            else:
+                self.GetAttr(98746110).SetJointPosition(
+                    joint_positions=[0, 0]
+                )
+                self.right_gripper_open = True
+        for i in range(20):
+            if not self.only_calculate:
+                self._step()
+            self.write()
+
+
+    def wait(self, n_timesteps):
+        for i in range(n_timesteps):
+            if not self.only_calculate:
+                self._step()
+            self.write()
+
+
+    def write(self):
+        '''
+        with open(self.record_file, 'a+') as f:
+            line = ''
+            for joint_position in self.left_joint_positions:
+                line += str(joint_position) + ','
+            for joint_position in self.right_joint_positions:
+                line += str(joint_position) + ','
+
+            if self.left_gripper_open:
+                line += '0,0,'
+            else:
+                line += '50,50,'
+
+            if self.right_gripper_open:
+                line += '0,0\n'
+            else:
+                line += '50,50\n'
+
+            f.write(line)
+            '''
+
+    def write_raw(self, raw_str):
+        with open(self.record_file, 'a+') as f:
+            f.write(raw_str)
+
+    def get_current_position(self, mode):
+        if mode == 'left':
+            return np.array(self.GetAttr(98746100).data['positions'][7])
+        elif mode == 'right':
+            return np.array(self.GetAttr(98746110).data['positions'][7])
+
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/ur5_box_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/ur5_box_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/envs/ur5_drawer_env.py` & `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_softbody_env.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,259 +1,221 @@
-from pyrfuniverse.envs import RFUniverseGymGoalWrapper
-from pyrfuniverse.utils.ur5_controller import RFUniverseUR5Controller
-import pyrfuniverse
-import numpy as np
-from gym import spaces
-from gym.utils import seeding
-import math
-import pybullet as p
-import os
-
-
-class Ur5DrawerEnv(RFUniverseGymGoalWrapper):
-    metadata = {'render.modes': ['human']}
-
-    def __init__(
-            self,
-            max_steps,
-            reward_type='dense',
-            min_open_distance=0.08,
-            seed=None,
-            executable_file=None,
-            asset_bundle_file=None,
-            assets: list = []
-    ):
-        super().__init__(
-            executable_file=executable_file,
-            camera_channel=True,
-            articulation_channel=True,
-            assets=assets
-        )
-        self.asset_channel.set_action(
-            'InstanceObject',
-            name='ur5_robotiq85',
-            id=123,
-        )
-        self.articulation_channel.set_action(
-            'SetTransform',
-            id=123,
-            position=[0, 0, 0],
-            rotation=[0, -90, 0],
-        )
-        self.asset_channel.set_action(
-            'InstanceObject',
-            name='handled_drawer',
-            id=456,
-        )
-        self.articulation_channel.set_action(
-            'SetTransform',
-            id=456,
-            position=[-0.721, 0.5, -0.538],
-            rotation=[-90, 180, 0],
-        )
-        self.camera_channel.set_action(
-            'AddCamera',
-            id=0,
-            position=[-0.25, 0.712, -0.914],
-            rotation=[26.997, -13.874, 0],
-        )
-        self._step()
-        self.max_steps = max_steps
-        self.reward_type = reward_type
-        self.min_open_distance = min_open_distance
-        self.asset_bundle_file = asset_bundle_file
-
-        self.seed(seed)
-        self.ik_controller = RFUniverseUR5Controller(
-            robot_urdf=os.path.join(pyrfuniverse.assets_path, 'RoboTube/DrawerClosing/UR5/ur5_robotiq_85.urdf'),
-            init_joint_positions=[90, -60, 60, 90, 90, 0],
-        )
-        self.t = 0
-        self.goal = np.array([self.min_open_distance])
-        self.action_space = spaces.Box(
-            low=-1, high=1, shape=(4,), dtype=np.float32
-        )
-        obs = self._get_obs()
-        self.observation_space = spaces.Dict({
-            'observation': spaces.Box(-np.inf, np.inf, shape=obs['observation'].shape, dtype=np.float32),
-            'desired_goal': spaces.Box(-np.inf, np.inf, shape=obs['desired_goal'].shape, dtype=np.float32),
-            'achieved_goal': spaces.Box(-np.inf, np.inf, shape=obs['achieved_goal'].shape, dtype=np.float32)
-        })
-        self.eef_orn = p.getQuaternionFromEuler([math.pi, 0, 0])
-
-    def step(self, action: np.ndarray):
-        action_ctrl = action.copy()
-        pos_ctrl = action_ctrl[:3] * 0.05
-        curr_pos = self._get_gripper_position()
-        pos_ctrl = pos_ctrl + curr_pos
-        joint_positions = self.ik_controller.calculate_ik_recursive(pos_ctrl, eef_orn=self.eef_orn)
-
-        gripper_width = self._get_gripper_width()
-        gripper_width_ctrl = np.clip(gripper_width + action_ctrl[3] * 0.2, 0, 0.085)
-        gripper_angle = self._compute_gripper_angle(gripper_width_ctrl)
-        joint_positions.append(gripper_angle)
-
-        self._set_ur5_robotiq85_joints(joint_positions)
-        self.t += 1
-
-        obs = self._get_obs()
-        done = False
-        info = {
-            'is_success': self._check_success(obs)
-        }
-        reward = self.compute_reward(obs['achieved_goal'], obs['desired_goal'], info)
-
-        if self.t == self.max_steps:
-            obs = self.reset()
-            done = True
-
-        return obs, reward, done, info
-
-    def reset(self):
-        super().reset()
-        self.env.reset()
-        self.ik_controller.reset()
-        self.t = 0
-
-        handle_position = np.array(self.articulation_channel.data[456]['positions'][3])
-        joint_positions = self.ik_controller.calculate_ik_recursive(handle_position, eef_orn=self.eef_orn)
-        gripper_angle = self._compute_gripper_angle(0.085)
-        joint_positions.append(gripper_angle)
-        self._set_ur5_robotiq85_joints_directly(joint_positions)
-
-        return self._get_obs()
-
-    def seed(self, seed=1234):
-        self.np_random, seed = seeding.np_random(seed)
-        return [seed]
-
-    def render(self, mode='human'):
-        self.camera_channel.set_action(
-            'GetImages',
-            rendering_params=[[0, 320, 240]]
-        )
-        self._step()
-        img = self.camera_channel.images.pop(0)
-
-        return img
-
-    def load_drawer(self, name, position, rotation):
-        self.asset_channel.set_action(
-            'LoadArticulationBody',
-            filename=self.asset_bundle_file,
-            name=name,
-            position=position,
-            rotation=rotation
-        )
-        self._step()
-
-    def destroy_drawer(self, index):
-        self.articulation_channel.set_action(
-            'Destroy',
-            index=index + 2
-        )
-        self._step()
-
-    def compute_reward(self, achieved_goal, desired_goal, info):
-        if self.reward_type == 'dense':
-            return float(achieved_goal)
-        else:
-            overhead_angle = achieved_goal - desired_goal
-            return float(overhead_angle[0] > 0)
-
-    def add_camera(self, position, rotation):
-        self.camera_channel.set_action(
-            'AddCamera',
-            position=position,
-            rotation=rotation,
-        )
-        self._step()
-
-    def get_images(self):
-        self.camera_channel.set_action(
-            'GetImages',
-            rendering_params=[[0, 320, 240], [1, 320, 240]]
-        )
-        self._step()
-
-        img_rgb = self.camera_channel.images.pop(0)
-        img_depth = self.camera_channel.images.pop(0)
-
-        return img_rgb, img_depth
-
-    def _get_obs(self):
-        gripper_position = self._get_gripper_position()
-        gripper_width = self._get_gripper_width()
-
-        robot_obs = np.concatenate((gripper_position, [gripper_width]))
-
-        handle_position = np.array(self.articulation_channel.data[456]['positions'][3])
-        drawer_open_distance = np.array([self.articulation_channel.data[456]['joint_positions'][0]])
-
-        object_obs = np.concatenate((handle_position, drawer_open_distance))
-
-        obs = np.concatenate((robot_obs, object_obs))
-
-        return {
-            'observation': obs.copy(),
-            'achieved_goal': drawer_open_distance.copy(),
-            'desired_goal': self.goal.copy()
-        }
-
-    def _get_gripper_position(self):
-        return np.array(self.articulation_channel.data[1230]['positions'][11])
-
-    def _get_gripper_width(self):
-        right_inner_finger_pos = np.array(self.articulation_channel.data[1230]['positions'][5])
-        left_inner_finger_pos = np.array(self.articulation_channel.data[1230]['positions'][10])
-        width = self._compute_distance(right_inner_finger_pos, left_inner_finger_pos)
-
-        # The position is at the center of inner_finger, so we must get rid of the width of inner finger,
-        # to get accurate gripper width
-        width = width - 0.00635
-
-        return width
-
-    def _compute_gripper_angle(self, width):
-        angle_rad = 0.715 - math.asin((width - 0.01) / 0.1143)
-        angle_deg = angle_rad * 180 / math.pi
-
-        return angle_deg
-
-    def _set_ur5_robotiq85_joints(self, joint_positions):
-        self.articulation_channel.set_action(
-            'SetJointPosition',
-            id=123,
-            joint_positions=list(joint_positions[:6])
-        )
-        #self._step()
-
-        self.articulation_channel.set_action(
-            'SetJointPosition',
-            id=1230,
-            joint_positions=[joint_positions[6], joint_positions[6]],
-        )
-        self._step()
-
-    def _set_ur5_robotiq85_joints_directly(self, joint_positions):
-        self.articulation_channel.set_action(
-            'SetJointPositionDirectly',
-            id=123,
-            joint_positions=list(joint_positions[:6])
-        )
-        #self._step()
-
-        self.articulation_channel.set_action(
-            'SetJointPositionDirectly',
-            id=1230,
-            joint_positions=[joint_positions[6], joint_positions[6]],
-        )
-        self._step()
-
-    def _compute_distance(self, point_a, point_b):
-        return np.linalg.norm(point_a - point_b, axis=-1)
-
-    def _check_success(self, obs):
-        achieved_goal = obs['achieved_goal'][0]
-        desired_goal = obs['desired_goal'][0]
-
-        return (desired_goal < achieved_goal).astype(np.float32)
+from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
+# from pyrfuniverse.utils import RFUniverseController
+import numpy as np
+import math
+import copy
+from gym import spaces
+from gym.utils import seeding
+
+
+class FrankaSoftbodyEnv(RFUniverseGymGoalWrapper):
+    metadata = {'render.modes': ['human']}
+
+    def __init__(
+            self,
+            asset_bundle_file,
+            reward_type,
+            open_gripper=True,
+            tolerance=0.05,
+            goal_xz_range=0.15,
+            softbody_xz_range=0.15,
+            executable_file=None,
+    ):
+        super().__init__(
+            executable_file=executable_file,
+            articulation_channel=True,
+            game_object_channel=True,
+            obi_softbody_channel=True
+        )
+        self.asset_bundle_file = asset_bundle_file
+        self.reward_type = reward_type
+        self.open_gripper = open_gripper
+        self.tolerance = tolerance
+
+        # Fixed parameters
+        self.scale = 10.0
+        self.goal_center_position = np.array([-0.6, 0.015, 0])
+        self.softbody_center_position = np.array([-0.6, 0.022, 0])
+        self.goal_range_low = self.goal_center_position - np.array([goal_xz_range, 0, goal_xz_range])
+        self.goal_range_high = self.goal_center_position + np.array([goal_xz_range, 0, goal_xz_range])
+        self.softbody_range_low = self.softbody_center_position - np.array([softbody_xz_range, 0, softbody_xz_range])
+        self.softbody_range_high = self.softbody_center_position + np.array([softbody_xz_range, 0, softbody_xz_range])
+
+        # Env setup
+        self.seed()
+        self.load_softbody = False
+        self._load_obi_softbody()
+        self.ik_controller = RFUniverseController('franka', base_pos=np.array([0, 0, 0]))
+        self.t = 0
+        self.goal = self._sample_goal()
+        self.action_space = spaces.Box(
+            low=-1, high=1, shape=(4,), dtype=np.float32
+        )
+        obs = self._get_obs()
+        self.observation_space = spaces.Dict({
+            'observation': spaces.Box(-np.inf, np.inf, shape=obs['observation'].shape, dtype=np.float32),
+            'desired_goal': spaces.Box(-np.inf, np.inf, shape=obs['desired_goal'].shape, dtype=np.float32),
+            'achieved_goal': spaces.Box(-np.inf, np.inf, shape=obs['achieved_goal'].shape, dtype=np.float32)
+        })
+
+    def step(self, action: np.ndarray):
+        pos_ctrl = action[:3] * 0.05
+        curr_pos = self._get_gripper_position()
+        pos_ctrl = curr_pos + pos_ctrl
+        joint_positions = self.ik_controller.calculate_ik(pos_ctrl)
+
+        if self.open_gripper:
+            curr_gripper_width = self._get_gripper_width()
+            target_gripper_width = curr_gripper_width + action[3] * 0.2
+            target_gripper_width = np.clip(target_gripper_width, 0, 0.08)
+            joint_positions.append(target_gripper_width)
+        else:
+            joint_positions.append(0)
+
+        self._set_franka_joints(np.array(joint_positions))
+        self.t += 1
+
+        obs = self._get_obs()
+        done = False
+        info = {
+            'is_success': self._check_success(obs)
+        }
+        # if info['is_success'] > 0:
+        #     print('Success')
+        reward = self.compute_reward(obs['achieved_goal'], obs['desired_goal'], info)
+
+        return obs, reward, done, info
+
+    def reset(self):
+        super().reset()
+
+        self._destroy_obi_softbody()
+        self.env.reset()
+        if not self.open_gripper:
+            self.articulation_channel.set_action(
+                'SetJointPositionDirectly',
+                index=1,
+                joint_positions=[0, 0],
+            )
+
+        obi_softbody_solver_position = self._load_obi_softbody()
+        self.goal = self._sample_goal()
+        self.game_object_channel.set_action(
+            'SetTransform',
+            index=0,
+            position=list(self.goal * self.scale)
+        )
+
+        self.t = 0
+        self.ik_controller.reset()
+        joint_positions = self.ik_controller.calculate_ik_recursive(
+            list(obi_softbody_solver_position),
+        )
+        self.articulation_channel.set_action(
+            'SetJointPositionDirectly',
+            index=0,
+            joint_positions=list(joint_positions),
+        )
+        self._step()
+
+        return self._get_obs()
+
+    def seed(self, seed=1234):
+        self.np_random, seed = seeding.np_random(seed)
+        return [seed]
+
+    def render(self, mode='human'):
+        self._step()
+
+    def compute_reward(self, achieved_goal, desired_goal, info):
+        distance = self._compute_goal_distance(achieved_goal, desired_goal)
+        if self.reward_type == 'sparse':
+            return -(distance > self.tolerance).astype(np.float32)
+        else:
+            return -distance
+
+    def _get_obs(self): #
+        gripper_position = np.array(self.articulation_channel.data[1]['positions'][3])
+        gripper_velocity = np.array(self.articulation_channel.data[1]['velocities'][3])
+        gripper_width = self._get_gripper_width()
+        panda_obs = np.concatenate((gripper_position, gripper_velocity, [gripper_width])) / self.scale
+
+        softbody_position = np.array(self.obi_softbody_channel.data[0]['position']) / self.scale
+        softbody_orientation = np.array(self.obi_softbody_channel.data[0]['orientation'])
+        softbody_velocity = np.array(self.obi_softbody_channel.data[0]['velocity']) / self.scale
+        softbody_angular_vel = np.array(self.obi_softbody_channel.data[0]['angular_vel'])
+        softbody_obs = np.concatenate(
+            (softbody_position, softbody_orientation, softbody_velocity, softbody_angular_vel)
+        )
+
+        obs = np.concatenate((panda_obs, softbody_obs))
+
+        return {
+            'observation': obs.copy(),
+            'achieved_goal': softbody_position.copy(),
+            'desired_goal': self.goal.copy()
+        }
+
+    def _load_obi_softbody(self):
+        if self.load_softbody:
+            return
+        obi_softbody_solver_position = self.np_random.uniform(
+            self.softbody_range_low, self.softbody_range_high
+        )
+        self.asset_channel.set_action(
+            'LoadObiSoftbody',
+            filename=self.asset_bundle_file,
+            name='Obi Softbody Solver',
+            position=list(obi_softbody_solver_position * self.scale)
+        )
+        self._step()
+        self.load_softbody = True
+
+        return obi_softbody_solver_position
+
+    def _destroy_obi_softbody(self):
+        if not self.load_softbody:
+            return
+        self.obi_softbody_channel.set_action(
+            'Destroy',
+            index=0
+        )
+        self._step()
+        self.load_softbody = False
+
+    def _sample_goal(self):
+        goal = self.np_random.uniform(self.goal_range_low, self.goal_range_high)
+        return goal.copy()
+
+    def _get_gripper_position(self):
+        return np.array(self.articulation_channel.data[1]['positions'][3]) / self.scale
+
+    def _get_gripper_width(self):
+        gripper_joint_positions = copy.deepcopy(self.articulation_channel.data[1]['joint_positions'])
+        return -1 * (gripper_joint_positions[0] + gripper_joint_positions[1]) / self.scale
+
+    def _set_franka_joints(self, a: np.ndarray):
+        self.articulation_channel.set_action(
+            'SetJointPosition',
+            index=0,
+            joint_positions=list(a[0:7]),
+        )
+        self._step()
+
+        a[7] = -1 * a[7] / 2 * self.scale
+        self.articulation_channel.set_action(
+            'SetJointPosition',
+            index=1,
+            joint_positions=[a[7], a[7]],
+        )
+        self._step()
+
+    def _compute_goal_distance(self, goal_a, goal_b):
+        assert goal_a.shape == goal_b.shape
+        return np.linalg.norm(goal_a - goal_b, axis=-1)
+
+    def _check_success(self, obs):
+        achieved_goal = obs['achieved_goal']
+        desired_goal = obs['desired_goal']
+        distance = self._compute_goal_distance(achieved_goal, desired_goal)
+
+        return (distance < self.tolerance).astype(np.float32)
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/side_channel/incoming_message.py` & `pyrfuniverse-0.9.11/pyrfuniverse/side_channel/incoming_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/side_channel/outgoing_message.py` & `pyrfuniverse-0.9.11/pyrfuniverse/side_channel/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/active_depth_generate.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/active_depth_generate.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/controller.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/depth_processor.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/depth_processor.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/interpolate_utils.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/interpolate_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-import numpy as np
-import math
-
-
-def average_interpolate_with_max_step_length(start: np.ndarray, terminal: np.ndarray, max_step_length):
-    assert start.shape == terminal.shape
-    distance = terminal - start
-    num_steps = int(abs(distance).max() / max_step_length) + 1
-    unit = distance / num_steps
-
-    intermediate_nodes = []
-    for i in range(num_steps):
-        intermediate_nodes.append(start + unit * (i + 1))
-    intermediate_nodes.append(terminal)
-
-    return np.array(intermediate_nodes)
-
-
-def average_interpolate(start: np.ndarray, terminal: np.ndarray, num_steps):
-    assert start.shape == terminal.shape
-    distance = terminal - start
-    unit = distance / num_steps
-
-    intermediate_nodes = []
-    for i in range(num_steps):
-        intermediate_nodes.append(start + unit * (i + 1))
-
-    return np.array(intermediate_nodes)
-
-
-def sine_interpolate(start: np.ndarray, terminal: np.ndarray, num_steps):
-    assert start.shape == terminal.shape
-    distance = terminal - start
-
-    intermediate_nodes = []
-    for i in range(num_steps):
-        step = distance / 2 * (math.sin(math.pi / num_steps * (i + 1) - math.pi / 2) + 1)
-        node = start + step
-        intermediate_nodes.append(node)
-
-    return np.array(intermediate_nodes)
-
-
-def rotate_by_y_axis_interpolate(start: np.array, center: np.array, moving_degree: float, num_steps: int):
-    """
-    The rotation is default to be anti-clockwise.
-    Args:
-        start: The start position in Unity.
-        center: The center position in Unity.
-        moving_degree: The amount of rotation need to rotate, in degree.
-        num_steps: The number of steps of this movement.
-
-    Returns:
-        The interpolated positions of this movement, in `np.ndarray` format
-    """
-    start_2d = np.array([start[0], start[2]])
-    center_2d = np.array([center[0], center[2]])
-    relative_2d = start_2d - center_2d
-    radius = np.linalg.norm(relative_2d)
-    init_radius = math.acos(float(relative_2d[0]) / radius)
-    if float(relative_2d[1]) < 0:
-        init_radius = -1 * init_radius
-    delta_radius = moving_degree * math.pi / 180 / num_steps
-    intermediate_nodes = []
-    for i in range(num_steps):
-        curr_target_radius = init_radius + delta_radius * (i + 1)
-        relative_x = radius * math.cos(curr_target_radius)
-        relative_z = radius * math.sin(curr_target_radius)
-        intermediate_node = np.array([center_2d[0] + relative_x, start[1], center_2d[1] + relative_z])
-        intermediate_nodes.append(intermediate_node)
-
-    return np.array(intermediate_nodes)
-
-
-def joint_positions_interpolation(env: RFUniverseBaseEnv, body_id, target_joint_positions, max_step_degree=3):
-    curr_jp = np.array(env.articulation_channel.data[body_id]['joint_positions'])
-    target_jp = np.array(target_joint_positions)
-    return average_interpolate(curr_jp, target_jp, max_step_degree)
-
-
-def pos_interpolation(env: RFUniverseBaseEnv, body_id, part_index, target_pos, max_step_length=0.05):
-    curr_pos = np.array(env.articulation_channel.data[body_id]['positions'][part_index])
-    targ_pos = np.array(target_pos)
-    return average_interpolate(curr_pos, targ_pos, max_step_length)
-
-
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+import numpy as np
+import math
+
+
+def average_interpolate_with_max_step_length(start: np.ndarray, terminal: np.ndarray, max_step_length):
+    assert start.shape == terminal.shape
+    distance = terminal - start
+    num_steps = int(abs(distance).max() / max_step_length) + 1
+    unit = distance / num_steps
+
+    intermediate_nodes = []
+    for i in range(num_steps):
+        intermediate_nodes.append(start + unit * (i + 1))
+    intermediate_nodes.append(terminal)
+
+    return np.array(intermediate_nodes)
+
+
+def average_interpolate(start: np.ndarray, terminal: np.ndarray, num_steps):
+    assert start.shape == terminal.shape
+    distance = terminal - start
+    unit = distance / num_steps
+
+    intermediate_nodes = []
+    for i in range(num_steps):
+        intermediate_nodes.append(start + unit * (i + 1))
+
+    return np.array(intermediate_nodes)
+
+
+def sine_interpolate(start: np.ndarray, terminal: np.ndarray, num_steps):
+    assert start.shape == terminal.shape
+    distance = terminal - start
+
+    intermediate_nodes = []
+    for i in range(num_steps):
+        step = distance / 2 * (math.sin(math.pi / num_steps * (i + 1) - math.pi / 2) + 1)
+        node = start + step
+        intermediate_nodes.append(node)
+
+    return np.array(intermediate_nodes)
+
+
+def rotate_by_y_axis_interpolate(start: np.array, center: np.array, moving_degree: float, num_steps: int):
+    """
+    The rotation is default to be anti-clockwise.
+    Args:
+        start: The start position in Unity.
+        center: The center position in Unity.
+        moving_degree: The amount of rotation need to rotate, in degree.
+        num_steps: The number of steps of this movement.
+
+    Returns:
+        The interpolated positions of this movement, in `np.ndarray` format
+    """
+    start_2d = np.array([start[0], start[2]])
+    center_2d = np.array([center[0], center[2]])
+    relative_2d = start_2d - center_2d
+    radius = np.linalg.norm(relative_2d)
+    init_radius = math.acos(float(relative_2d[0]) / radius)
+    if float(relative_2d[1]) < 0:
+        init_radius = -1 * init_radius
+    delta_radius = moving_degree * math.pi / 180 / num_steps
+    intermediate_nodes = []
+    for i in range(num_steps):
+        curr_target_radius = init_radius + delta_radius * (i + 1)
+        relative_x = radius * math.cos(curr_target_radius)
+        relative_z = radius * math.sin(curr_target_radius)
+        intermediate_node = np.array([center_2d[0] + relative_x, start[1], center_2d[1] + relative_z])
+        intermediate_nodes.append(intermediate_node)
+
+    return np.array(intermediate_nodes)
+
+
+def joint_positions_interpolation(env: RFUniverseBaseEnv, body_id, target_joint_positions, max_step_degree=3):
+    curr_jp = np.array(env.articulation_channel.data[body_id]['joint_positions'])
+    target_jp = np.array(target_joint_positions)
+    return average_interpolate(curr_jp, target_jp, max_step_degree)
+
+
+def pos_interpolation(env: RFUniverseBaseEnv, body_id, part_index, target_pos, max_step_length=0.05):
+    curr_pos = np.array(env.articulation_channel.data[body_id]['positions'][part_index])
+    targ_pos = np.array(target_pos)
+    return average_interpolate(curr_pos, targ_pos, max_step_length)
+
+
```

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/jaco_controller.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/jaco_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/kinova_controller.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/kinova_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/os_utils.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/rfuniverse_utility.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/rfuniverse_utility.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/stretch_controller.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/stretch_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/tobor_controller.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/tobor_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse/utils/ur5_controller.py` & `pyrfuniverse-0.9.11/pyrfuniverse/utils/ur5_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/pyrfuniverse.egg-info/SOURCES.txt` & `pyrfuniverse-0.9.11/pyrfuniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/setup.py` & `pyrfuniverse-0.9.11/setup.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_active_depth.py` & `pyrfuniverse-0.9.11/test/test_active_depth.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_articulation_ik.py` & `pyrfuniverse-0.9.11/test/test_articulation_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_camera_image.py` & `pyrfuniverse-0.9.11/test/test_camera_image.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_custom_message.py` & `pyrfuniverse-0.9.11/test/test_custom_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_debug.py` & `pyrfuniverse-0.9.11/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_grasp_pose.py` & `pyrfuniverse-0.9.11/test/test_grasp_pose.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_grasp_sim.py` & `pyrfuniverse-0.9.11/test/test_grasp_sim.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_heat_map.py` & `pyrfuniverse-0.9.11/test/test_heat_map.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_humanbody_ik.py` & `pyrfuniverse-0.9.11/test/test_humanbody_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_image_stream.py` & `pyrfuniverse-0.9.11/test/test_image_stream.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_label.py` & `pyrfuniverse-0.9.11/test/test_label.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_light.py` & `pyrfuniverse-0.9.11/test/test_light.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_load_mesh.py` & `pyrfuniverse-0.9.11/test/test_load_mesh.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_load_urdf.py` & `pyrfuniverse-0.9.11/test/test_load_urdf.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_object_data.py` & `pyrfuniverse-0.9.11/test/test_object_data.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_ompl.py` & `pyrfuniverse-0.9.11/test/test_ompl.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_pick_and_place.py` & `pyrfuniverse-0.9.11/test/test_pick_and_place.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_pick_and_place_flexiv.py` & `pyrfuniverse-0.9.11/test/test_pick_and_place_flexiv.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_point_cloud.py` & `pyrfuniverse-0.9.11/test/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_point_cloud_with_intrinsic_matrix.py` & `pyrfuniverse-0.9.11/test/test_point_cloud_with_intrinsic_matrix.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_save_gripper.py` & `pyrfuniverse-0.9.11/test/test_save_gripper.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_scene.py` & `pyrfuniverse-0.9.11/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.10/test/test_tobor_move.py` & `pyrfuniverse-0.9.11/test/test_tobor_move.py`

 * *Files identical despite different names*

