# Comparing `tmp/redvox-3.5.0.tar.gz` & `tmp/redvox-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-3.5.0.tar", last modified: Tue Jul 11 21:03:45 2023, max compression
+gzip compressed data, was "redvox-3.5.1.tar", last modified: Tue Aug  1 00:09:13 2023, max compression
```

## Comparing `redvox-3.5.0.tar` & `redvox-3.5.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.439884 redvox-3.5.0/
--rw-r--r--   0 anthony    (501) staff       (20)    11343 2023-05-10 20:30:19.000000 redvox-3.5.0/LICENSE
--rw-r--r--   0 anthony    (501) staff       (20)    13906 2023-07-11 21:03:45.439712 redvox-3.5.0/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)      517 2021-12-29 23:42:43.000000 redvox-3.5.0/README.md
--rw-r--r--   0 anthony    (501) staff       (20)     1375 2023-05-10 20:30:19.000000 redvox-3.5.0/pyproject.toml
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.424030 redvox-3.5.0/redvox/
--rw-r--r--   0 anthony    (501) staff       (20)      728 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/__init__.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.424859 redvox-3.5.0/redvox/api1000/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/__init__.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.425680 redvox-3.5.0/redvox/api1000/common/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    20204 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/common.py
--rw-r--r--   0 anthony    (501) staff       (20)     1050 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/decorators.py
--rw-r--r--   0 anthony    (501) staff       (20)     5359 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/generic.py
--rw-r--r--   0 anthony    (501) staff       (20)      875 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/lz4.py
--rw-r--r--   0 anthony    (501) staff       (20)     2570 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/mapping.py
--rw-r--r--   0 anthony    (501) staff       (20)     2237 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/metadata.py
--rw-r--r--   0 anthony    (501) staff       (20)     2435 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/typing.py
--rw-r--r--   0 anthony    (501) staff       (20)     2114 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/errors.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.425862 redvox-3.5.0/redvox/api1000/gui/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/gui/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     4672 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/gui/image_viewer.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.426053 redvox-3.5.0/redvox/api1000/proto/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/proto/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    39434 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/api1000/proto/redvox_api_m_pb2.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.426749 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     5639 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/event_streams.py
--rw-r--r--   0 anthony    (501) staff       (20)    10817 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/ml.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.427576 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    11949 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.427772 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    14890 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
--rw-r--r--   0 anthony    (501) staff       (20)     7398 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/image.py
--rw-r--r--   0 anthony    (501) staff       (20)    40936 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/location.py
--rw-r--r--   0 anthony    (501) staff       (20)    42236 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
--rw-r--r--   0 anthony    (501) staff       (20)     3425 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/single.py
--rw-r--r--   0 anthony    (501) staff       (20)     5576 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
--rw-r--r--   0 anthony    (501) staff       (20)    50437 2022-08-04 18:31:21.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/station_information.py
--rw-r--r--   0 anthony    (501) staff       (20)    19060 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/timing_information.py
--rw-r--r--   0 anthony    (501) staff       (20)    21971 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.429228 redvox-3.5.0/redvox/api900/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    17514 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/concat.py
--rw-r--r--   0 anthony    (501) staff       (20)      494 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/constants.py
--rw-r--r--   0 anthony    (501) staff       (20)     1689 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/deprecation.py
--rw-r--r--   0 anthony    (501) staff       (20)      351 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/exceptions.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.429453 redvox-3.5.0/redvox/api900/lib/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/lib/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     7591 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/api900/lib/api900_pb2.py
--rw-r--r--   0 anthony    (501) staff       (20)    43091 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/location_analyzer.py
--rw-r--r--   0 anthony    (501) staff       (20)     2597 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/migrations.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.429653 redvox-3.5.0/redvox/api900/qa/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/qa/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     2813 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/qa/gap_detection.py
--rw-r--r--   0 anthony    (501) staff       (20)    16939 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/reader.py
--rw-r--r--   0 anthony    (501) staff       (20)    17096 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/reader_utils.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.431541 redvox-3.5.0/redvox/api900/sensors/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     2113 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/accelerometer_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     2298 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/barometer_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     2665 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/evenly_sampled_channel.py
--rw-r--r--   0 anthony    (501) staff       (20)     6283 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/evenly_sampled_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     1989 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/gyroscope_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     4854 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/image_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     2264 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/infrared_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)    16540 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/interleaved_channel.py
--rw-r--r--   0 anthony    (501) staff       (20)     2261 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/light_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)    10051 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/location_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     2022 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/magnetometer_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     3209 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/microphone_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     4655 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/time_synchronization_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     3536 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/unevenly_sampled_channel.py
--rw-r--r--   0 anthony    (501) staff       (20)     6619 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/unevenly_sampled_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     5907 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
--rw-r--r--   0 anthony    (501) staff       (20)     1128 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/stat_utils.py
--rw-r--r--   0 anthony    (501) staff       (20)     8780 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/summarize.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.431899 redvox-3.5.0/redvox/api900/timesync/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/timesync/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    27606 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/timesync/api900_timesync.py
--rw-r--r--   0 anthony    (501) staff       (20)    13824 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/timesync/tri_message_stats.py
--rw-r--r--   0 anthony    (501) staff       (20)     1537 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/types.py
--rw-r--r--   0 anthony    (501) staff       (20)    54392 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/wrapped_redvox_packet.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.433731 redvox-3.5.0/redvox/cli/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cli/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    22678 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cli/cli.py
--rw-r--r--   0 anthony    (501) staff       (20)     6683 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cli/conversions.py
--rw-r--r--   0 anthony    (501) staff       (20)     1797 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cli/data_req.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.435441 redvox-3.5.0/redvox/cloud/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     2267 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/api.py
--rw-r--r--   0 anthony    (501) staff       (20)   142063 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/api_m_fqns.py
--rw-r--r--   0 anthony    (501) staff       (20)     4334 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/auth_api.py
--rw-r--r--   0 anthony    (501) staff       (20)    29429 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/cloud/client.py
--rw-r--r--   0 anthony    (501) staff       (20)     5905 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/config.py
--rw-r--r--   0 anthony    (501) staff       (20)     6088 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/data_api.py
--rw-r--r--   0 anthony    (501) staff       (20)     3829 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/data_client.py
--rw-r--r--   0 anthony    (501) staff       (20)     3266 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/cloud/data_io.py
--rw-r--r--   0 anthony    (501) staff       (20)      487 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/errors.py
--rw-r--r--   0 anthony    (501) staff       (20)    18946 2022-08-04 18:31:21.000000 redvox-3.5.0/redvox/cloud/metadata_api.py
--rw-r--r--   0 anthony    (501) staff       (20)     3770 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/query_timing_correction.py
--rw-r--r--   0 anthony    (501) staff       (20)     1086 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/cloud/routes.py
--rw-r--r--   0 anthony    (501) staff       (20)    10985 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/cloud/session_model_api.py
--rw-r--r--   0 anthony    (501) staff       (20)     4262 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/station_stats.py
--rw-r--r--   0 anthony    (501) staff       (20)     7707 2022-08-04 18:31:21.000000 redvox-3.5.0/redvox/cloud/subscription.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.439330 redvox-3.5.0/redvox/common/
--rw-r--r--   0 anthony    (501) staff       (20)      195 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    55240 2023-03-01 21:44:51.000000 redvox-3.5.0/redvox/common/api_conversions.py
--rw-r--r--   0 anthony    (501) staff       (20)    23894 2023-07-11 21:00:08.000000 redvox-3.5.0/redvox/common/api_reader.py
--rw-r--r--   0 anthony    (501) staff       (20)     5249 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/api_reader_dw.py
--rw-r--r--   0 anthony    (501) staff       (20)     1173 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/constants.py
--rw-r--r--   0 anthony    (501) staff       (20)     4126 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/cross_stats.py
--rw-r--r--   0 anthony    (501) staff       (20)    42995 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/data_window.py
--rw-r--r--   0 anthony    (501) staff       (20)     8266 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/data_window_configuration.py
--rw-r--r--   0 anthony    (501) staff       (20)     7154 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/data_window_io.py
--rw-r--r--   0 anthony    (501) staff       (20)    16785 2023-03-01 21:44:51.000000 redvox-3.5.0/redvox/common/date_time_utils.py
--rw-r--r--   0 anthony    (501) staff       (20)     3252 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/errors.py
--rw-r--r--   0 anthony    (501) staff       (20)    41889 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/event_stream.py
--rw-r--r--   0 anthony    (501) staff       (20)     3104 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/event_stream_io.py
--rw-r--r--   0 anthony    (501) staff       (20)    13655 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/file_statistics.py
--rw-r--r--   0 anthony    (501) staff       (20)    17541 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/gap_and_pad_utils.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.439517 redvox-3.5.0/redvox/common/gui/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/gui/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)    16251 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/gui/cloud_data_retrieval.py
--rw-r--r--   0 anthony    (501) staff       (20)    56756 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/io.py
--rw-r--r--   0 anthony    (501) staff       (20)    26597 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/offset_model.py
--rw-r--r--   0 anthony    (501) staff       (20)    26988 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/packet_to_pyarrow.py
--rw-r--r--   0 anthony    (501) staff       (20)     5022 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/parallel_utils.py
--rw-r--r--   0 anthony    (501) staff       (20)     1256 2022-08-04 18:31:21.000000 redvox-3.5.0/redvox/common/run_me.py
--rw-r--r--   0 anthony    (501) staff       (20)    94752 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/sensor_data.py
--rw-r--r--   0 anthony    (501) staff       (20)     1086 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/sensor_io.py
--rw-r--r--   0 anthony    (501) staff       (20)    17894 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/sensor_reader_utils.py
--rw-r--r--   0 anthony    (501) staff       (20)     2947 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/session_io.py
--rw-r--r--   0 anthony    (501) staff       (20)    17172 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/session_model.py
--rw-r--r--   0 anthony    (501) staff       (20)    15794 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/session_model_utils.py
--rw-r--r--   0 anthony    (501) staff       (20)    70537 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/station.py
--rw-r--r--   0 anthony    (501) staff       (20)     1441 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/station_io.py
--rw-r--r--   0 anthony    (501) staff       (20)     4909 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/station_model.py
--rw-r--r--   0 anthony    (501) staff       (20)    17541 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/station_utils.py
--rw-r--r--   0 anthony    (501) staff       (20)     3964 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/stats_helper.py
--rw-r--r--   0 anthony    (501) staff       (20)    21550 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/timesync.py
--rw-r--r--   0 anthony    (501) staff       (20)     1175 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/timesync_io.py
--rw-r--r--   0 anthony    (501) staff       (20)    13810 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/tri_message_stats.py
--rw-r--r--   0 anthony    (501) staff       (20)     1867 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/versioning.py
--rw-r--r--   0 anthony    (501) staff       (20)     2205 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/settings.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.424660 redvox-3.5.0/redvox.egg-info/
--rw-r--r--   0 anthony    (501) staff       (20)    13906 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)     4560 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/SOURCES.txt
--rw-r--r--   0 anthony    (501) staff       (20)        1 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/dependency_links.txt
--rw-r--r--   0 anthony    (501) staff       (20)       51 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/entry_points.txt
--rw-r--r--   0 anthony    (501) staff       (20)      386 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/requires.txt
--rw-r--r--   0 anthony    (501) staff       (20)        7 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/top_level.txt
--rw-r--r--   0 anthony    (501) staff       (20)       38 2023-07-11 21:03:45.439917 redvox-3.5.0/setup.cfg
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.911962 redvox-3.5.1/
+-rw-r--r--   0 tyler      (501) staff       (20)    11343 2023-05-23 21:20:02.000000 redvox-3.5.1/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)    13906 2023-08-01 00:09:13.911332 redvox-3.5.1/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      517 2021-06-16 20:22:36.000000 redvox-3.5.1/README.md
+-rw-r--r--   0 tyler      (501) staff       (20)     1375 2023-05-23 21:20:02.000000 redvox-3.5.1/pyproject.toml
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.779610 redvox-3.5.1/redvox/
+-rw-r--r--   0 tyler      (501) staff       (20)      728 2023-07-31 23:52:22.000000 redvox-3.5.1/redvox/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.783371 redvox-3.5.1/redvox/api1000/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.789498 redvox-3.5.1/redvox/api1000/common/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/common/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    20204 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/api1000/common/common.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1050 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/common/decorators.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5359 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/common/generic.py
+-rw-r--r--   0 tyler      (501) staff       (20)      875 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/common/lz4.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2570 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/common/mapping.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2237 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/common/metadata.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2435 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/common/typing.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2114 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/errors.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.790563 redvox-3.5.1/redvox/api1000/gui/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/gui/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4672 2021-04-09 20:02:21.000000 redvox-3.5.1/redvox/api1000/gui/image_viewer.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.792017 redvox-3.5.1/redvox/api1000/proto/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/proto/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    39434 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/api1000/proto/redvox_api_m_pb2.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.799227 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5639 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/event_streams.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10817 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/ml.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.806385 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    11949 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.807840 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14890 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7398 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/image.py
+-rw-r--r--   0 tyler      (501) staff       (20)    40936 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/location.py
+-rw-r--r--   0 tyler      (501) staff       (20)    42236 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3425 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/single.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5576 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
+-rw-r--r--   0 tyler      (501) staff       (20)    50437 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/station_information.py
+-rw-r--r--   0 tyler      (501) staff       (20)    19060 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/timing_information.py
+-rw-r--r--   0 tyler      (501) staff       (20)    21971 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.821483 redvox-3.5.1/redvox/api900/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17514 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/api900/concat.py
+-rw-r--r--   0 tyler      (501) staff       (20)      494 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/constants.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1689 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/deprecation.py
+-rw-r--r--   0 tyler      (501) staff       (20)      351 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/exceptions.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.823281 redvox-3.5.1/redvox/api900/lib/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/lib/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7591 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/api900/lib/api900_pb2.py
+-rw-r--r--   0 tyler      (501) staff       (20)    43091 2023-06-26 20:48:33.000000 redvox-3.5.1/redvox/api900/location_analyzer.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2597 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/migrations.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.824887 redvox-3.5.1/redvox/api900/qa/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/qa/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2813 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/qa/gap_detection.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16939 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/reader.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17096 2021-06-01 21:32:52.000000 redvox-3.5.1/redvox/api900/reader_utils.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.841610 redvox-3.5.1/redvox/api900/sensors/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2113 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/accelerometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2298 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/barometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2665 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/evenly_sampled_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6283 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/evenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1989 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/gyroscope_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4854 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/image_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2264 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/infrared_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16540 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/interleaved_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2261 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/light_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10051 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/location_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2022 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/magnetometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3209 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/microphone_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4655 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/time_synchronization_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3536 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/unevenly_sampled_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6619 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/unevenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5907 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1128 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/stat_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8780 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/api900/summarize.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.844653 redvox-3.5.1/redvox/api900/timesync/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/timesync/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    27606 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/timesync/api900_timesync.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13824 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/timesync/tri_message_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1537 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/api900/types.py
+-rw-r--r--   0 tyler      (501) staff       (20)    54392 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/api900/wrapped_redvox_packet.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.849928 redvox-3.5.1/redvox/cli/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/cli/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    22678 2021-04-09 20:02:21.000000 redvox-3.5.1/redvox/cli/cli.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6683 2021-06-01 21:32:52.000000 redvox-3.5.1/redvox/cli/conversions.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1797 2021-04-09 20:02:21.000000 redvox-3.5.1/redvox/cli/data_req.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.869431 redvox-3.5.1/redvox/cloud/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/cloud/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2267 2023-06-26 20:48:55.000000 redvox-3.5.1/redvox/cloud/api.py
+-rw-r--r--   0 tyler      (501) staff       (20)   142063 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/cloud/api_m_fqns.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4334 2021-03-31 23:04:52.000000 redvox-3.5.1/redvox/cloud/auth_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)    29429 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/cloud/client.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5905 2022-12-15 01:35:54.000000 redvox-3.5.1/redvox/cloud/config.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6088 2021-04-09 20:02:21.000000 redvox-3.5.1/redvox/cloud/data_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3829 2022-12-15 01:35:54.000000 redvox-3.5.1/redvox/cloud/data_client.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3266 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/cloud/data_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)      487 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/cloud/errors.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18946 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/cloud/metadata_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3770 2021-04-14 22:44:11.000000 redvox-3.5.1/redvox/cloud/query_timing_correction.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1086 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/cloud/routes.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10985 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/cloud/session_model_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4262 2021-04-14 22:44:11.000000 redvox-3.5.1/redvox/cloud/station_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7707 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/cloud/subscription.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.908565 redvox-3.5.1/redvox/common/
+-rw-r--r--   0 tyler      (501) staff       (20)      195 2021-03-30 21:57:13.000000 redvox-3.5.1/redvox/common/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    55240 2023-06-23 23:40:13.000000 redvox-3.5.1/redvox/common/api_conversions.py
+-rw-r--r--   0 tyler      (501) staff       (20)    23894 2023-07-11 20:47:20.000000 redvox-3.5.1/redvox/common/api_reader.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5249 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/api_reader_dw.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1173 2021-04-19 23:26:28.000000 redvox-3.5.1/redvox/common/constants.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4126 2021-06-29 20:11:21.000000 redvox-3.5.1/redvox/common/cross_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)    42995 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/data_window.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8266 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/data_window_configuration.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7154 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/data_window_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16785 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/common/date_time_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3252 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/errors.py
+-rw-r--r--   0 tyler      (501) staff       (20)    41889 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/event_stream.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3104 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/event_stream_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13655 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/common/file_statistics.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17541 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/gap_and_pad_utils.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.910192 redvox-3.5.1/redvox/common/gui/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-04-09 20:02:21.000000 redvox-3.5.1/redvox/common/gui/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16251 2021-04-15 01:00:48.000000 redvox-3.5.1/redvox/common/gui/cloud_data_retrieval.py
+-rw-r--r--   0 tyler      (501) staff       (20)    56756 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    26597 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/offset_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    26988 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/packet_to_pyarrow.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5022 2022-12-15 01:35:54.000000 redvox-3.5.1/redvox/common/parallel_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1256 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/common/run_me.py
+-rw-r--r--   0 tyler      (501) staff       (20)    94752 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/sensor_data.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1086 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/sensor_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17894 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/sensor_reader_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2947 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/session_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17172 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/session_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15794 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/session_model_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)    70576 2023-07-31 20:50:36.000000 redvox-3.5.1/redvox/common/station.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1441 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/station_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4909 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/station_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17605 2023-07-21 01:59:50.000000 redvox-3.5.1/redvox/common/station_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3964 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/stats_helper.py
+-rw-r--r--   0 tyler      (501) staff       (20)    21550 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/timesync.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1175 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/timesync_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13810 2023-07-11 20:25:06.000000 redvox-3.5.1/redvox/common/tri_message_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1867 2021-06-29 20:11:21.000000 redvox-3.5.1/redvox/common/versioning.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2205 2023-05-23 21:20:02.000000 redvox-3.5.1/redvox/settings.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-01 00:09:13.782657 redvox-3.5.1/redvox.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)    13906 2023-08-01 00:09:13.000000 redvox-3.5.1/redvox.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)     4560 2023-08-01 00:09:13.000000 redvox-3.5.1/redvox.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2023-08-01 00:09:13.000000 redvox-3.5.1/redvox.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       51 2023-08-01 00:09:13.000000 redvox-3.5.1/redvox.egg-info/entry_points.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      386 2023-08-01 00:09:13.000000 redvox-3.5.1/redvox.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        7 2023-08-01 00:09:13.000000 redvox-3.5.1/redvox.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       38 2023-08-01 00:09:13.912142 redvox-3.5.1/setup.cfg
```

### Comparing `redvox-3.5.0/LICENSE` & `redvox-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/PKG-INFO` & `redvox-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.5.0
+Version: 3.5.1
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.5.0/README.md` & `redvox-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/pyproject.toml` & `redvox-3.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/__init__.py` & `redvox-3.5.1/redvox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Provides library level metadata and constants.
 """
 
 NAME: str = "redvox"
-VERSION: str = "3.5.0"
+VERSION: str = "3.5.1"
 
 
 def version() -> str:
     """Returns the version number of this library."""
     return VERSION
```

### Comparing `redvox-3.5.0/redvox/api1000/common/common.py` & `redvox-3.5.1/redvox/api1000/common/common.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/common/decorators.py` & `redvox-3.5.1/redvox/api1000/common/decorators.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/common/generic.py` & `redvox-3.5.1/redvox/api1000/common/generic.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/common/lz4.py` & `redvox-3.5.1/redvox/api1000/common/lz4.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/common/mapping.py` & `redvox-3.5.1/redvox/api1000/common/mapping.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/common/metadata.py` & `redvox-3.5.1/redvox/api1000/common/metadata.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/common/typing.py` & `redvox-3.5.1/redvox/api1000/common/typing.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/errors.py` & `redvox-3.5.1/redvox/api1000/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/gui/image_viewer.py` & `redvox-3.5.1/redvox/api1000/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/proto/redvox_api_m_pb2.py` & `redvox-3.5.1/redvox/api1000/proto/redvox_api_m_pb2.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/event_streams.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/event_streams.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/ml.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/ml.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/audio.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/audio.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/image.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/image.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/location.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/location.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/single.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/single.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/station_information.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/station_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/timing_information.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/timing_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py` & `redvox-3.5.1/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/concat.py` & `redvox-3.5.1/redvox/api900/concat.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/deprecation.py` & `redvox-3.5.1/redvox/api900/deprecation.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/lib/api900_pb2.py` & `redvox-3.5.1/redvox/api900/lib/api900_pb2.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/location_analyzer.py` & `redvox-3.5.1/redvox/api900/location_analyzer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/migrations.py` & `redvox-3.5.1/redvox/api900/migrations.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/qa/gap_detection.py` & `redvox-3.5.1/redvox/api900/qa/gap_detection.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/reader.py` & `redvox-3.5.1/redvox/api900/reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/reader_utils.py` & `redvox-3.5.1/redvox/api900/reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/accelerometer_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/accelerometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/barometer_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/barometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/evenly_sampled_channel.py` & `redvox-3.5.1/redvox/api900/sensors/evenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/evenly_sampled_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/evenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/gyroscope_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/gyroscope_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/image_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/image_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/infrared_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/infrared_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/interleaved_channel.py` & `redvox-3.5.1/redvox/api900/sensors/interleaved_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/light_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/light_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/location_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/location_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/magnetometer_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/magnetometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/microphone_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/microphone_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/time_synchronization_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/time_synchronization_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/unevenly_sampled_channel.py` & `redvox-3.5.1/redvox/api900/sensors/unevenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/unevenly_sampled_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py` & `redvox-3.5.1/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/stat_utils.py` & `redvox-3.5.1/redvox/api900/stat_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/summarize.py` & `redvox-3.5.1/redvox/api900/summarize.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/timesync/api900_timesync.py` & `redvox-3.5.1/redvox/api900/timesync/api900_timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/timesync/tri_message_stats.py` & `redvox-3.5.1/redvox/api900/timesync/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/types.py` & `redvox-3.5.1/redvox/api900/types.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/api900/wrapped_redvox_packet.py` & `redvox-3.5.1/redvox/api900/wrapped_redvox_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cli/cli.py` & `redvox-3.5.1/redvox/cli/cli.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cli/conversions.py` & `redvox-3.5.1/redvox/cli/conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cli/data_req.py` & `redvox-3.5.1/redvox/cli/data_req.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/api.py` & `redvox-3.5.1/redvox/cloud/api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/api_m_fqns.py` & `redvox-3.5.1/redvox/cloud/api_m_fqns.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/auth_api.py` & `redvox-3.5.1/redvox/cloud/auth_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/client.py` & `redvox-3.5.1/redvox/cloud/client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/config.py` & `redvox-3.5.1/redvox/cloud/config.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/data_api.py` & `redvox-3.5.1/redvox/cloud/data_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/data_client.py` & `redvox-3.5.1/redvox/cloud/data_client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/data_io.py` & `redvox-3.5.1/redvox/cloud/data_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/metadata_api.py` & `redvox-3.5.1/redvox/cloud/metadata_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/query_timing_correction.py` & `redvox-3.5.1/redvox/cloud/query_timing_correction.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/routes.py` & `redvox-3.5.1/redvox/cloud/routes.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/session_model_api.py` & `redvox-3.5.1/redvox/cloud/session_model_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/station_stats.py` & `redvox-3.5.1/redvox/cloud/station_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/cloud/subscription.py` & `redvox-3.5.1/redvox/cloud/subscription.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/api_conversions.py` & `redvox-3.5.1/redvox/common/api_conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/api_reader.py` & `redvox-3.5.1/redvox/common/api_reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/api_reader_dw.py` & `redvox-3.5.1/redvox/common/api_reader_dw.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/constants.py` & `redvox-3.5.1/redvox/common/constants.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/cross_stats.py` & `redvox-3.5.1/redvox/common/cross_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/data_window.py` & `redvox-3.5.1/redvox/common/data_window.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/data_window_configuration.py` & `redvox-3.5.1/redvox/common/data_window_configuration.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/data_window_io.py` & `redvox-3.5.1/redvox/common/data_window_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/date_time_utils.py` & `redvox-3.5.1/redvox/common/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/errors.py` & `redvox-3.5.1/redvox/common/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/event_stream.py` & `redvox-3.5.1/redvox/common/event_stream.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/event_stream_io.py` & `redvox-3.5.1/redvox/common/event_stream_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/file_statistics.py` & `redvox-3.5.1/redvox/common/file_statistics.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/gap_and_pad_utils.py` & `redvox-3.5.1/redvox/common/gap_and_pad_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/gui/cloud_data_retrieval.py` & `redvox-3.5.1/redvox/common/gui/cloud_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/io.py` & `redvox-3.5.1/redvox/common/io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/offset_model.py` & `redvox-3.5.1/redvox/common/offset_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/packet_to_pyarrow.py` & `redvox-3.5.1/redvox/common/packet_to_pyarrow.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/parallel_utils.py` & `redvox-3.5.1/redvox/common/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/run_me.py` & `redvox-3.5.1/redvox/common/run_me.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/sensor_data.py` & `redvox-3.5.1/redvox/common/sensor_data.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/sensor_io.py` & `redvox-3.5.1/redvox/common/sensor_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/sensor_reader_utils.py` & `redvox-3.5.1/redvox/common/sensor_reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/session_io.py` & `redvox-3.5.1/redvox/common/session_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/session_model.py` & `redvox-3.5.1/redvox/common/session_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/session_model_utils.py` & `redvox-3.5.1/redvox/common/session_model_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/station.py` & `redvox-3.5.1/redvox/common/station.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         }
 
     def default_station_json_file_name(self) -> str:
         """
         :return: default station json file name (id_startdate), with startdate as integer of microseconds
                     since epoch UTC
         """
-        return f"{self._id}_{0 if np.isnan(self._start_date) else int(self._start_date)}"
+        return self._get_id_key()
 
     def to_json_file(self, file_name: Optional[str] = None) -> Path:
         """
         saves the station as json in station.base_dir, then creates directories and the json for the metadata
         and data in the same base_dir.
 
         :param file_name: the optional base file name.  Do not include a file extension.
@@ -402,15 +402,15 @@
         """
         fill station using data from a list of Indexes
 
         :param indexes: List of indexes of the files to read
         """
         self._load_metadata_from_packet(indexes[0].read_first_packet())
         self._timesync_data.arrow_dir = os.path.join(self.save_dir(), "timesync")
-        self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
+        self._timesync_data.arrow_file = f"timesync_{self.start_date_as_str()}"
         all_summaries = ptp.AggregateSummary()
         self._event_data.set_save_dir(os.path.join(self.save_dir(), "events"))
         for idx in indexes:
             pkts = idx.read_contents()
             self._packet_metadata.extend([st_utils.StationPacketMetadata(packet) for packet in pkts])
             self._timesync_data.append_timesync_arrow(TimeSync().from_raw_packets(pkts))
             self._event_data.read_from_packets_list(pkts)
@@ -489,15 +489,15 @@
         """
         if packets and st_utils.validate_station_key_list(packets, self._errors):
             # noinspection Mypy
             self._load_metadata_from_packet(packets[0])
             self._packet_metadata = [st_utils.StationPacketMetadata(packet) for packet in packets]
             self._timesync_data = TimeSync().from_raw_packets(packets)
             self._timesync_data.arrow_dir = os.path.join(self.save_dir(), "timesync")
-            self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
+            self._timesync_data.arrow_file = f"timesync_{self.start_date_as_str()}"
             summaries = ptp.stream_to_pyarrow(packets, self._fs_writer.get_temp() if self.is_save_to_disk() else None)
             summaries.merge_all_summaries()
             self._set_pyarrow_sensors(summaries)
             if self._correct_timestamps:
                 self.update_timestamps()
             self._event_data.set_save_dir(os.path.join(self.save_dir(), "events"))
             self._event_data.read_from_packets_list(packets)
@@ -509,15 +509,15 @@
         :param packet: API-M redvox packet to load metadata from
         """
         self._id = packet.station_information.id.zfill(STATION_ID_LENGTH)
         self._uuid = packet.station_information.uuid
         self._start_date = packet.timing_information.app_start_mach_timestamp
         if self._start_date < 0:
             self._errors.append(
-                f"Station {self._id} has station start date before epoch.  " f"Station start date reset to np.nan"
+                f"Station {self._id} has station start date before epoch.  Station start date reset to np.nan"
             )
             self._start_date = np.nan
         self._metadata = st_utils.StationMetadata("Redvox", packet)
         if isinstance(packet, api_m.RedvoxPacketM) and packet.sensors.HasField("audio"):
             self._audio_sample_rate_nominal_hz = packet.sensors.audio.sample_rate
             self._is_audio_scrambled = packet.sensors.audio.is_scrambled
         else:
@@ -581,14 +581,20 @@
 
     def start_date(self) -> float:
         """
         :return: the station start timestamp or np.nan if it doesn't exist
         """
         return self._start_date
 
+    def start_date_as_str(self) -> str:
+        """
+        :return: station start timestamp as integer string or 0 if it doesn't exist
+        """
+        return f"{0 if np.isnan(self._start_date) else int(self._start_date)}"
+
     def check_key(self) -> bool:
         """
         check if the station has enough information to set its key.
 
         :return: True if key can be set, False if not enough information
         """
         if self._id:
@@ -618,24 +624,22 @@
 
     def append_station(self, new_station: "Station"):
         """
         append a new station to the current station; does nothing if keys do not match
 
         :param new_station: Station to append to current station
         """
-        if (
-            self.get_key() is not None
-            and new_station.get_key() == self.get_key()
-            and self._metadata.validate_metadata(new_station._metadata)
-        ):
+        key = self.get_key()
+        if key and key.compare_key(new_station.get_key()) and self._metadata.validate_metadata(new_station._metadata):
             self._errors.extend_error(new_station.errors())
             self.append_station_data(new_station._data)
             self._packet_metadata.extend(new_station._packet_metadata)
             self._sort_metadata_packets()
             self._timesync_data.append_timesync_arrow(new_station._timesync_data)
+            self._set_gps_offset()
             if not hasattr(self, "_event_data"):
                 self._event_data = EventStreams()
             self._event_data.append_streams(new_station.event_data())
             self.update_first_and_last_data_timestamps()
 
     def append_station_data(self, new_station_data: List[sd.SensorData]):
         """
@@ -1390,17 +1394,15 @@
         """
         return os.path.join(self.save_dir(), "events")
 
     def _get_id_key(self) -> str:
         """
         :return: the station's id and start time as a string
         """
-        if np.isnan(self._start_date):
-            return f"{self._id}_0"
-        return f"{self._id}_{int(self._start_date)}"
+        return f"{self._id}_{self.start_date_as_str()}"
 
     def _fix_sensor_data(self, sensor_type: sd.SensorType, data_table: pa.Table) -> pa.Table:
         """
         fix any problems with the data in data_table due to app/OS version
 
         :param sensor_type: type of sensor
         :param data_table: the data to edit
@@ -1596,14 +1598,16 @@
         """
         self._timesync_data = timesync
 
     def gps_offset_model(self) -> OffsetModel:
         """
         :return: the gps offset model
         """
+        if not hasattr(self, "_gps_offset_model"):
+            self._set_gps_offset()
         return self._gps_offset_model
 
     def errors(self) -> RedVoxExceptions:
         """
         :return: errors of the station
         """
         return self._errors
@@ -1718,15 +1722,15 @@
                     old_name = self.save_dir()
                     self.set_save_dir(self._fs_writer.base_dir)
                     if old_name != "." and os.path.exists(old_name):
                         os.rename(old_name, self.save_dir())
                 else:
                     self._fs_writer.file_name = self._get_id_key()
             self.update_first_and_last_data_timestamps()
-            self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
+            self._timesync_data.arrow_file = f"timesync_{self.start_date_as_str()}"
             self._is_timestamps_updated = True
         return self
 
     def undo_update_timestamps(self) -> "Station":
         """
         undoes non-sensor timestamp updates of the timestamps in the station using the offset model
         sensors already have unaltered timestamps
@@ -1755,10 +1759,10 @@
                     old_name = self.save_dir()
                     self.set_save_dir(self._fs_writer.base_dir)
                     if old_name != "." and os.path.exists(old_name):
                         os.rename(old_name, self.save_dir())
                 else:
                     self._fs_writer.file_name = self._get_id_key()
             self.update_first_and_last_data_timestamps()
-            self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
+            self._timesync_data.arrow_file = f"timesync_{self.start_date_as_str()}"
             self._is_timestamps_updated = False
         return self
```

### Comparing `redvox-3.5.0/redvox/common/station_io.py` & `redvox-3.5.1/redvox/common/station_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/station_model.py` & `redvox-3.5.1/redvox/common/station_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/station_utils.py` & `redvox-3.5.1/redvox/common/station_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,31 +108,34 @@
     def check_key(
         self,
         station_id: Optional[str] = None,
         station_uuid: Optional[str] = None,
         start_timestamp: Optional[float] = None,
     ) -> bool:
         """
-        check if the key has the values specified.  If the parameter is None, any value will match.
+        Check if the key has the values specified.  If the parameter is None, any value will match.
         Note that NAN is a valid value for start_timestamps, but any station with start_timestamp = NAN
         will not match any value, including another NAN.
 
         :param station_id: station id, default None
         :param station_uuid: station uuid, default None
         :param start_timestamp: station start timestamp in microseconds since UTC epoch, default None
         :return: True if all parameters match key values
         """
-        if station_id is not None and station_id != self.id:
-            return False
-        if station_uuid is not None and station_uuid != self.uuid:
-            return False
-        if start_timestamp is not None and (
-            start_timestamp != self.start_timestamp_micros
-            or np.isnan(start_timestamp)
-            or np.isnan(self.start_timestamp_micros)
+        if (
+            (station_id is not None and station_id != self.id)
+            or (station_uuid is not None and station_uuid != self.uuid)
+            or (
+                start_timestamp is not None
+                and (
+                    start_timestamp != self.start_timestamp_micros
+                    or np.isnan(start_timestamp)
+                    or np.isnan(self.start_timestamp_micros)
+                )
+            )
         ):
             return False
         return True
 
     def compare_key(self, other_key: "StationKey") -> bool:
         """
         compare key to another station's key
```

### Comparing `redvox-3.5.0/redvox/common/stats_helper.py` & `redvox-3.5.1/redvox/common/stats_helper.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/timesync.py` & `redvox-3.5.1/redvox/common/timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/timesync_io.py` & `redvox-3.5.1/redvox/common/timesync_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/tri_message_stats.py` & `redvox-3.5.1/redvox/common/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/common/versioning.py` & `redvox-3.5.1/redvox/common/versioning.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox/settings.py` & `redvox-3.5.1/redvox/settings.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.0/redvox.egg-info/PKG-INFO` & `redvox-3.5.1/redvox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.5.0
+Version: 3.5.1
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.5.0/redvox.egg-info/SOURCES.txt` & `redvox-3.5.1/redvox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

