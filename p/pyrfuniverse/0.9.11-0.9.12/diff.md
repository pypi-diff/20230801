# Comparing `tmp/pyrfuniverse-0.9.11.tar.gz` & `tmp/pyrfuniverse-0.9.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfuniverse-0.9.11.tar", last modified: Wed Jul 26 07:52:45 2023, max compression
+gzip compressed data, was "pyrfuniverse-0.9.12.tar", last modified: Tue Aug  1 09:11:05 2023, max compression
```

## Comparing `pyrfuniverse-0.9.11.tar` & `pyrfuniverse-0.9.12.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.683002 pyrfuniverse-0.9.11/
--rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.9.11/LICENSE
--rw-rw-rw-   0        0        0      266 2023-07-26 07:52:45.681499 pyrfuniverse-0.9.11/PKG-INFO
--rw-rw-rw-   0        0        0     2758 2023-06-21 09:17:40.000000 pyrfuniverse-0.9.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.158675 pyrfuniverse-0.9.11/pyrfuniverse/
--rw-rw-rw-   0        0        0      759 2023-07-26 07:51:49.000000 pyrfuniverse-0.9.11/pyrfuniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.304711 pyrfuniverse-0.9.11/pyrfuniverse/attributes/
--rw-rw-rw-   0        0        0     1472 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/activelightsensor_attr.py
--rw-rw-rw-   0        0        0     9352 2023-07-12 10:53:12.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/base_attr.py
--rw-rw-rw-   0        0        0     8438 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/camera_attr.py
--rw-rw-rw-   0        0        0      384 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/cloth_attr.py
--rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/collider_attr.py
--rw-rw-rw-   0        0        0    15137 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/controller_attr.py
--rw-rw-rw-   0        0        0      622 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/custom_attr.py
--rw-rw-rw-   0        0        0      678 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/digit_attr.py
--rw-rw-rw-   0        0        0      871 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/fallingcloth_attr.py
--rw-rw-rw-   0        0        0     1533 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/gameobject_attr.py
--rw-rw-rw-   0        0        0     4038 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/graspsim_attr.py
--rw-rw-rw-   0        0        0     4520 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/humanbody_attr.py
--rw-rw-rw-   0        0        0     2643 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/light_attr.py
--rw-rw-rw-   0        0        0     8924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/omplmanager_attr.py
--rw-rw-rw-   0        0        0     1331 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/pointcloud_attr.py
--rw-rw-rw-   0        0        0     1737 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/rigidbody_attr.py
--rw-rw-rw-   0        0        0      387 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/attributes/softbody_attr.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.363721 pyrfuniverse-0.9.11/pyrfuniverse/envs/
--rw-rw-rw-   0        0        0    15241 2023-07-26 07:51:49.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/__init__.py
--rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/balance_ball_env.py
--rw-rw-rw-   0        0        0    24832 2023-07-14 07:27:36.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/base_env.py
--rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/bouncer_env.py
--rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/franka_grasp_env.py
--rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/franka_push_env.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.407296 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/
--rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/__init__.py
--rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/nail_can_env.py
--rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/nail_card_env.py
--rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
--rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
--rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
--rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
--rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
--rw-rw-rw-   0        0        0      769 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gym_goal_wrapper_env.py
--rw-rw-rw-   0        0        0      702 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/gym_wrapper_env.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.423828 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/
--rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/cleaner_env.py
--rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/navigation_env.py
--rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent_navigation_env.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.444420 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/
--rw-rw-rw-   0        0        0      871 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/__init__.py
--rw-rw-rw-   0        0        0    13868 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
--rw-rw-rw-   0        0        0     8156 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
--rw-rw-rw-   0        0        0    10075 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
--rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.479350 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/
--rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/__init__.py
--rw-rw-rw-   0        0        0     7488 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_cloth_env.py
--rw-rw-rw-   0        0        0     7679 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
--rw-rw-rw-   0        0        0     9654 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_robotics_env.py
--rw-rw-rw-   0        0        0     8235 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_softbody_env.py
--rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/pick_and_place_env.py
--rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/push_env.py
--rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/reach_env.py
--rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/roller_env.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.488371 pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotics/
--rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotics/__init__.py
--rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
--rw-rw-rw-   0        0        0     8876 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
--rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/ur5_box_env.py
--rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.11/pyrfuniverse/envs/ur5_drawer_env.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.503369 pyrfuniverse-0.9.11/pyrfuniverse/side_channel/
--rw-rw-rw-   0        0        0      144 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/side_channel/__init__.py
--rw-rw-rw-   0        0        0     3244 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/side_channel/incoming_message.py
--rw-rw-rw-   0        0        0     1536 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/side_channel/outgoing_message.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.567667 pyrfuniverse-0.9.11/pyrfuniverse/utils/
--rw-rw-rw-   0        0        0        0 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/__init__.py
--rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/active_depth_generate.py
--rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/controller.py
--rw-rw-rw-   0        0        0    11746 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/depth_processor.py
--rw-rw-rw-   0        0        0     3314 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/interpolate_utils.py
--rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/jaco_controller.py
--rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/kinova_controller.py
--rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/os_utils.py
--rw-rw-rw-   0        0        0    10104 2023-07-21 18:14:17.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/rfuniverse_communicator.py
--rw-rw-rw-   0        0        0     3569 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/rfuniverse_utility.py
--rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/stretch_controller.py
--rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/tobor_controller.py
--rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.11/pyrfuniverse/utils/ur5_controller.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.170709 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/
--rw-rw-rw-   0        0        0      266 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4088 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:32:20.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 07:52:45.000000 pyrfuniverse-0.9.11/pyrfuniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 07:52:45.683002 pyrfuniverse-0.9.11/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:52:45.681499 pyrfuniverse-0.9.11/test/
--rw-rw-rw-   0        0        0     5924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_active_depth.py
--rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_articulation_ik.py
--rw-rw-rw-   0        0        0      943 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_camera_image.py
--rw-rw-rw-   0        0        0     1939 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_custom_message.py
--rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.9.11/test/test_debug.py
--rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.9.11/test/test_digit.py
--rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_grasp_pose.py
--rw-rw-rw-   0        0        0     2750 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_grasp_sim.py
--rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.9.11/test/test_heat_map.py
--rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_humanbody_ik.py
--rw-rw-rw-   0        0        0     1087 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_image_stream.py
--rw-rw-rw-   0        0        0     1984 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_label.py
--rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_light.py
--rw-rw-rw-   0        0        0      589 2023-06-13 10:33:21.000000 pyrfuniverse-0.9.11/test/test_load_mesh.py
--rw-rw-rw-   0        0        0     1008 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_load_urdf.py
--rw-rw-rw-   0        0        0      277 2023-07-10 14:17:21.000000 pyrfuniverse-0.9.11/test/test_load_urdf_akb.py
--rw-rw-rw-   0        0        0     1980 2023-07-13 08:59:36.000000 pyrfuniverse-0.9.11/test/test_object_data.py
--rw-rw-rw-   0        0        0     1646 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_ompl.py
--rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.9.11/test/test_pick_and_place.py
--rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.9.11/test/test_pick_and_place_flexiv.py
--rw-rw-rw-   0        0        0     1658 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_point_cloud.py
--rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_point_cloud_render.py
--rw-rw-rw-   0        0        0     1830 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_point_cloud_with_intrinsic_matrix.py
--rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.9.11/test/test_save_gripper.py
--rw-rw-rw-   0        0        0      378 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.11/test/test_save_obj.py
--rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.11/test/test_scene.py
--rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.9.11/test/test_tobor_move.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.818441 pyrfuniverse-0.9.12/
+-rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.9.12/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-08-01 09:11:05.818441 pyrfuniverse-0.9.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2758 2023-06-21 09:17:40.000000 pyrfuniverse-0.9.12/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.309875 pyrfuniverse-0.9.12/pyrfuniverse/
+-rw-rw-rw-   0        0        0      759 2023-08-01 09:11:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.441479 pyrfuniverse-0.9.12/pyrfuniverse/attributes/
+-rw-rw-rw-   0        0        0     1472 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/activelightsensor_attr.py
+-rw-rw-rw-   0        0        0     9352 2023-07-12 10:53:12.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/base_attr.py
+-rw-rw-rw-   0        0        0     8438 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/camera_attr.py
+-rw-rw-rw-   0        0        0      384 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/cloth_attr.py
+-rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/collider_attr.py
+-rw-rw-rw-   0        0        0    15137 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/controller_attr.py
+-rw-rw-rw-   0        0        0      622 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/custom_attr.py
+-rw-rw-rw-   0        0        0      678 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/digit_attr.py
+-rw-rw-rw-   0        0        0      871 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/fallingcloth_attr.py
+-rw-rw-rw-   0        0        0     1533 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/gameobject_attr.py
+-rw-rw-rw-   0        0        0     4038 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/graspsim_attr.py
+-rw-rw-rw-   0        0        0     4520 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/humanbody_attr.py
+-rw-rw-rw-   0        0        0     2643 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/light_attr.py
+-rw-rw-rw-   0        0        0     8924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/omplmanager_attr.py
+-rw-rw-rw-   0        0        0     1331 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/pointcloud_attr.py
+-rw-rw-rw-   0        0        0     1737 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/rigidbody_attr.py
+-rw-rw-rw-   0        0        0      387 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/attributes/softbody_attr.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.496840 pyrfuniverse-0.9.12/pyrfuniverse/envs/
+-rw-rw-rw-   0        0        0    15241 2023-07-26 07:51:49.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/__init__.py
+-rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/balance_ball_env.py
+-rw-rw-rw-   0        0        0    24832 2023-07-14 07:27:36.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/base_env.py
+-rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/bouncer_env.py
+-rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/franka_grasp_env.py
+-rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/franka_push_env.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.538484 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/
+-rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/__init__.py
+-rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/nail_can_env.py
+-rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/nail_card_env.py
+-rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
+-rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
+-rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
+-rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
+-rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
+-rw-rw-rw-   0        0        0      769 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gym_goal_wrapper_env.py
+-rw-rw-rw-   0        0        0      702 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/gym_wrapper_env.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.554844 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_agent/
+-rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_agent/cleaner_env.py
+-rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_agent/navigation_env.py
+-rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_agent_navigation_env.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.573112 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/
+-rw-rw-rw-   0        0        0      871 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/__init__.py
+-rw-rw-rw-   0        0        0    13868 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
+-rw-rw-rw-   0        0        0     8156 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
+-rw-rw-rw-   0        0        0    10075 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
+-rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.612716 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/
+-rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/__init__.py
+-rw-rw-rw-   0        0        0     7488 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/franka_cloth_env.py
+-rw-rw-rw-   0        0        0     7679 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
+-rw-rw-rw-   0        0        0     9654 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/franka_robotics_env.py
+-rw-rw-rw-   0        0        0     8235 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/franka_softbody_env.py
+-rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/pick_and_place_env.py
+-rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/push_env.py
+-rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/reach_env.py
+-rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/roller_env.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.626791 pyrfuniverse-0.9.12/pyrfuniverse/envs/tobor_robotics/
+-rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/tobor_robotics/__init__.py
+-rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
+-rw-rw-rw-   0        0        0     8876 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
+-rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/ur5_box_env.py
+-rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.12/pyrfuniverse/envs/ur5_drawer_env.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.642454 pyrfuniverse-0.9.12/pyrfuniverse/side_channel/
+-rw-rw-rw-   0        0        0      144 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/side_channel/__init__.py
+-rw-rw-rw-   0        0        0     3244 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/side_channel/incoming_message.py
+-rw-rw-rw-   0        0        0     1536 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/side_channel/outgoing_message.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.694899 pyrfuniverse-0.9.12/pyrfuniverse/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/active_depth_generate.py
+-rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/controller.py
+-rw-rw-rw-   0        0        0    11746 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/depth_processor.py
+-rw-rw-rw-   0        0        0     3314 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/interpolate_utils.py
+-rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/jaco_controller.py
+-rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/kinova_controller.py
+-rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/os_utils.py
+-rw-rw-rw-   0        0        0     9915 2023-08-01 08:25:21.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/rfuniverse_communicator.py
+-rw-rw-rw-   0        0        0     3569 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/rfuniverse_utility.py
+-rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/stretch_controller.py
+-rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/tobor_controller.py
+-rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.12/pyrfuniverse/utils/ur5_controller.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.327627 pyrfuniverse-0.9.12/pyrfuniverse.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-08-01 09:11:05.000000 pyrfuniverse-0.9.12/pyrfuniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4080 2023-08-01 09:11:05.000000 pyrfuniverse-0.9.12/pyrfuniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:11:05.000000 pyrfuniverse-0.9.12/pyrfuniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:32:20.000000 pyrfuniverse-0.9.12/pyrfuniverse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-08-01 09:11:05.000000 pyrfuniverse-0.9.12/pyrfuniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 09:11:05.000000 pyrfuniverse-0.9.12/pyrfuniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:11:05.818441 pyrfuniverse-0.9.12/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:11:05.817441 pyrfuniverse-0.9.12/test/
+-rw-rw-rw-   0        0        0     5924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_active_depth.py
+-rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.12/test/test_articulation_ik.py
+-rw-rw-rw-   0        0        0      943 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_camera_image.py
+-rw-rw-rw-   0        0        0     1939 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_custom_message.py
+-rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.9.12/test/test_debug.py
+-rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.9.12/test/test_digit.py
+-rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.12/test/test_grasp_pose.py
+-rw-rw-rw-   0        0        0     2750 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_grasp_sim.py
+-rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.9.12/test/test_heat_map.py
+-rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.12/test/test_humanbody_ik.py
+-rw-rw-rw-   0        0        0     1087 2023-08-01 08:26:35.000000 pyrfuniverse-0.9.12/test/test_image_stream.py
+-rw-rw-rw-   0        0        0     1984 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_label.py
+-rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.12/test/test_light.py
+-rw-rw-rw-   0        0        0      589 2023-06-13 10:33:21.000000 pyrfuniverse-0.9.12/test/test_load_mesh.py
+-rw-rw-rw-   0        0        0     1008 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_load_urdf.py
+-rw-rw-rw-   0        0        0      277 2023-07-10 14:17:21.000000 pyrfuniverse-0.9.12/test/test_load_urdf_akb.py
+-rw-rw-rw-   0        0        0     1980 2023-07-13 08:59:36.000000 pyrfuniverse-0.9.12/test/test_object_data.py
+-rw-rw-rw-   0        0        0     1646 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_ompl.py
+-rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.9.12/test/test_pick_and_place.py
+-rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.9.12/test/test_pick_and_place_flexiv.py
+-rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.12/test/test_ply_render.py
+-rw-rw-rw-   0        0        0     1658 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_point_cloud.py
+-rw-rw-rw-   0        0        0     1830 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_point_cloud_with_intrinsic_matrix.py
+-rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.9.12/test/test_save_gripper.py
+-rw-rw-rw-   0        0        0      378 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.12/test/test_save_obj.py
+-rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.12/test/test_scene.py
+-rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.9.12/test/test_tobor_move.py
```

### Comparing `pyrfuniverse-0.9.11/LICENSE` & `pyrfuniverse-0.9.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/README.md` & `pyrfuniverse-0.9.12/README.md`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/__init__.py` & `pyrfuniverse-0.9.12/pyrfuniverse/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the library that will be used to upload to pypi
-__version__ = "0.9.11"
+__version__ = "0.9.12"
 
 import os.path
 import json
 
 def read_config():
     if not os.path.exists(config_path):
         config = {}
```

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/__init__.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/activelightsensor_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/activelightsensor_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/base_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/base_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/camera_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/camera_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/collider_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/collider_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/controller_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/controller_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/custom_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/custom_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/digit_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/digit_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/fallingcloth_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/fallingcloth_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/gameobject_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/gameobject_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/graspsim_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/graspsim_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/humanbody_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/humanbody_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/light_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/light_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/omplmanager_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/omplmanager_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/pointcloud_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/pointcloud_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/attributes/rigidbody_attr.py` & `pyrfuniverse-0.9.12/pyrfuniverse/attributes/rigidbody_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/__init__.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/balance_ball_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/balance_ball_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/base_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/base_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/bouncer_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/bouncer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/franka_grasp_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/franka_grasp_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/franka_push_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/franka_push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/__init__.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/nail_can_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/nail_card_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gym_goal_wrapper_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gym_goal_wrapper_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/gym_wrapper_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/gym_wrapper_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/cleaner_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_agent/cleaner_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent/navigation_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_agent/navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_agent_navigation_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_agent_navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/__init__.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/flexiv_cutting.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/flexiv_cutting.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/rfuniverse_robot_hub_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/rfuniverse_robot_hub_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/__init__.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_cloth_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/franka_cloth_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_robotics_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/franka_robotics_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/franka_softbody_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/franka_softbody_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/pick_and_place_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/pick_and_place_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/push_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/robotics/reach_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/robotics/reach_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/roller_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/roller_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/ur5_box_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/ur5_box_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/envs/ur5_drawer_env.py` & `pyrfuniverse-0.9.12/pyrfuniverse/envs/ur5_drawer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/side_channel/incoming_message.py` & `pyrfuniverse-0.9.12/pyrfuniverse/side_channel/incoming_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/side_channel/outgoing_message.py` & `pyrfuniverse-0.9.12/pyrfuniverse/side_channel/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/active_depth_generate.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/active_depth_generate.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/controller.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/depth_processor.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/depth_processor.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/interpolate_utils.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/interpolate_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/jaco_controller.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/jaco_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/kinova_controller.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/kinova_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/os_utils.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/rfuniverse_communicator.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/rfuniverse_communicator.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.server.bind(('localhost', self.port))
         print(f'Waiting for connections on port: {self.port}...')
         self.server.listen(1)
         self.client, self.addr = self.server.accept()
         print(f'Connected successfully')
         self.connected = True
         self.client.settimeout(None)
-        self.buffer_size = 1024 * 10
+        # self.buffer_size = 1024 * 10
         # self.client.setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, self.buffer_size)
         # self.client.setsockopt(socket.SOL_SOCKET, socket.SO_RCVBUF, self.buffer_size)
         self.client.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         if self.is_async:
             self.start()
         else:
             self.receive_step()
@@ -58,53 +58,51 @@
         # sync_receive_objects_queue = []
         while True:
             if not self.connected:
                 return
             data = self.receive_bytes()
             objs = self.receive_object(data)
             if len(objs) > 0 and objs[0] == "StepEnd":
+
                 break
             self.on_receive_data(objs)
         #     sync_receive_objects_queue.append(objs)
         # if self.on_receive_data is not None:
         #     for item in sync_receive_objects_queue:
         #         self.on_receive_data(item)
         # sync_receive_objects_queue.clear()
 
     def receive_bytes(self):
-        if not self.connected:
-            return
         data = self.client.recv(4)
-        length = int.from_bytes(data, byteorder='little', signed=True)
-        buffer = bytearray(length)
-        offset = 0
-        while offset < length:
-            offset_max = offset + self.buffer_size
-            if offset_max > length:
-                offset_max = length
-            buffer[offset: offset_max] = self.client.recv(offset_max-offset)
-            offset = offset_max
-        return bytes(buffer)
-        # return self.client.recv(length)
+        length = int.from_bytes(data, byteorder='little', signed=False)
+
+        buf = bytearray()
+        while len(buf) < length:
+            tmp = self.client.recv(length - len(buf))
+            buf.extend(tmp)
+        assert len(buf) == length
+        return buf
 
     def send_bytes(self, data: bytes):
         if not self.connected:
             return
         length = len(data).to_bytes(4, byteorder='little', signed=False)
         self.client.send(length)
-        offset = 0
-        while offset < len(data):
-            offset_max = offset + self.buffer_size
-            if offset_max > len(data):
-                offset_max = len(data)
-            self.client.send(data[offset: offset_max])
-            offset = offset_max
-        # self.client.send(data)
-        if platform == 'linux':
-            self.client.setsockopt(socket.IPPROTO_TCP, socket.TCP_QUICKACK, 1)
+        self.client.send(data)
+
+        # offset = 0
+        # while offset < len(data):
+        #     offset_max = offset + self.buffer_size
+        #     if offset_max > len(data):
+        #         offset_max = len(data)
+        #     self.client.send(data[offset: offset_max])
+        #     offset = offset_max
+        # # self.client.send(data)
+        # if platform == 'linux':
+        #     self.client.setsockopt(socket.IPPROTO_TCP, socket.TCP_QUICKACK, 1)
 
     def receive_object(self, data: bytes) -> list:
         self.read_offset = 0
         count = self.read_int(data)
         objs = []
         for i in range(count):
             objs.append(self.read_object(data))
```

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/rfuniverse_utility.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/rfuniverse_utility.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/stretch_controller.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/stretch_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/tobor_controller.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/tobor_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse/utils/ur5_controller.py` & `pyrfuniverse-0.9.12/pyrfuniverse/utils/ur5_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/pyrfuniverse.egg-info/SOURCES.txt` & `pyrfuniverse-0.9.12/pyrfuniverse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,14 @@
 test/test_load_mesh.py
 test/test_load_urdf.py
 test/test_load_urdf_akb.py
 test/test_object_data.py
 test/test_ompl.py
 test/test_pick_and_place.py
 test/test_pick_and_place_flexiv.py
+test/test_ply_render.py
 test/test_point_cloud.py
-test/test_point_cloud_render.py
 test/test_point_cloud_with_intrinsic_matrix.py
 test/test_save_gripper.py
 test/test_save_obj.py
 test/test_scene.py
 test/test_tobor_move.py
```

### Comparing `pyrfuniverse-0.9.11/setup.py` & `pyrfuniverse-0.9.12/setup.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_active_depth.py` & `pyrfuniverse-0.9.12/test/test_active_depth.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_articulation_ik.py` & `pyrfuniverse-0.9.12/test/test_articulation_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_camera_image.py` & `pyrfuniverse-0.9.12/test/test_camera_image.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_custom_message.py` & `pyrfuniverse-0.9.12/test/test_custom_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_debug.py` & `pyrfuniverse-0.9.12/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_grasp_pose.py` & `pyrfuniverse-0.9.12/test/test_grasp_pose.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_grasp_sim.py` & `pyrfuniverse-0.9.12/test/test_grasp_sim.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_heat_map.py` & `pyrfuniverse-0.9.12/test/test_heat_map.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_humanbody_ik.py` & `pyrfuniverse-0.9.12/test/test_humanbody_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_image_stream.py` & `pyrfuniverse-0.9.12/test/test_image_stream.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_label.py` & `pyrfuniverse-0.9.12/test/test_label.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_light.py` & `pyrfuniverse-0.9.12/test/test_light.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_load_mesh.py` & `pyrfuniverse-0.9.12/test/test_load_mesh.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_load_urdf.py` & `pyrfuniverse-0.9.12/test/test_load_urdf.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_object_data.py` & `pyrfuniverse-0.9.12/test/test_object_data.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_ompl.py` & `pyrfuniverse-0.9.12/test/test_ompl.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_pick_and_place.py` & `pyrfuniverse-0.9.12/test/test_pick_and_place.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_pick_and_place_flexiv.py` & `pyrfuniverse-0.9.12/test/test_pick_and_place_flexiv.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_point_cloud.py` & `pyrfuniverse-0.9.12/test/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_point_cloud_with_intrinsic_matrix.py` & `pyrfuniverse-0.9.12/test/test_point_cloud_with_intrinsic_matrix.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_save_gripper.py` & `pyrfuniverse-0.9.12/test/test_save_gripper.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_scene.py` & `pyrfuniverse-0.9.12/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.11/test/test_tobor_move.py` & `pyrfuniverse-0.9.12/test/test_tobor_move.py`

 * *Files identical despite different names*

