# Comparing `tmp/ni_measurementlink_service-1.1.0.dev2.tar.gz` & `tmp/ni_measurementlink_service-1.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_service-1.1.0.dev2.tar", max compression
+gzip compressed data, was "ni_measurementlink_service-1.2.0.dev0.tar", max compression
```

## Comparing `ni_measurementlink_service-1.1.0.dev2.tar` & `ni_measurementlink_service-1.2.0.dev0.tar`

### file list

```diff
@@ -1,68 +1,75 @@
--rw-r--r--   0        0        0     1071 2023-06-26 21:34:54.060588 ni_measurementlink_service-1.1.0.dev2/LICENSE
--rw-r--r--   0        0        0    16723 2023-06-26 21:34:54.060588 ni_measurementlink_service-1.1.0.dev2/README.md
--rw-r--r--   0        0        0      513 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/__init__.py
--rw-r--r--   0        0        0       62 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/__init__.py
--rw-r--r--   0        0        0    10247 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/discovery_client.py
--rw-r--r--   0        0        0    17484 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/grpc_servicer.py
--rw-r--r--   0        0        0       58 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/__init__.py
--rw-r--r--   0        0        0     5400 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/metadata.py
--rw-r--r--   0        0        0     9237 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
--rw-r--r--   0        0        0     8298 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/serializer.py
--rw-r--r--   0        0        0     3933 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/service_manager.py
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/__init__.py
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/__init__.py
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
--rw-r--r--   0        0        0     4264 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
--rw-r--r--   0        0        0     8921 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
--rw-r--r--   0        0        0    10817 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
--rw-r--r--   0        0        0     6348 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
--rw-r--r--   0        0        0     5345 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
--rw-r--r--   0        0        0    13678 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5546 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0     2362 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
--rw-r--r--   0        0        0     5777 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
--rw-r--r--   0        0        0    15086 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5549 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0     2412 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     1532 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
--rw-r--r--   0        0        0     1314 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
--rw-r--r--   0        0        0     6202 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
--rw-r--r--   0        0        0    18188 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
--rw-r--r--   0        0        0    14078 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
--rw-r--r--   0        0        0     6880 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
--rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
--rw-r--r--   0        0        0     5955 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
--rw-r--r--   0        0        0    13370 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
--rw-r--r--   0        0        0    13882 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     7537 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      709 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/README.md
--rw-r--r--   0        0        0     6052 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
--rw-r--r--   0        0        0     6650 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
--rw-r--r--   0        0        0     7228 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
--rw-r--r--   0        0        0      712 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
--rw-r--r--   0        0        0     9622 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
--rw-r--r--   0        0        0     8468 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
--rw-r--r--   0        0        0     2426 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/session.proto
--rw-r--r--   0        0        0     4196 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2.py
--rw-r--r--   0        0        0     8735 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
--rw-r--r--   0        0        0     8948 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
--rw-r--r--   0        0        0     2873 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi
--rw-r--r--   0        0        0       35 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/utilities/__init__.py
--rw-r--r--   0        0        0       37 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/__init__.py
--rw-r--r--   0        0        0     3520 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/info.py
--rw-r--r--   0        0        0    15001 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/service.py
--rw-r--r--   0        0        0        0 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/py.typed
--rw-r--r--   0        0        0    19771 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/session_management.py
--rw-r--r--   0        0        0     2831 2023-06-26 21:35:52.329345 ni_measurementlink_service-1.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0    19614 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev2/setup.py
--rw-r--r--   0        0        0    17972 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-01 19:42:01.218704 ni_measurementlink_service-1.2.0.dev0/LICENSE
+-rw-r--r--   0        0        0    16811 2023-08-01 19:42:01.218704 ni_measurementlink_service-1.2.0.dev0/README.md
+-rw-r--r--   0        0        0      530 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/__init__.py
+-rw-r--r--   0        0        0       62 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/__init__.py
+-rw-r--r--   0        0        0    13310 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/discovery_client.py
+-rw-r--r--   0        0        0    17561 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/grpc_servicer.py
+-rw-r--r--   0        0        0       58 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/parameter/__init__.py
+-rw-r--r--   0        0        0     5496 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/parameter/metadata.py
+-rw-r--r--   0        0        0     9237 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
+-rw-r--r--   0        0        0     8845 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/parameter/serializer.py
+-rw-r--r--   0        0        0     3933 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/service_manager.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
+-rw-r--r--   0        0        0     4742 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
+-rw-r--r--   0        0        0    10451 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
+-rw-r--r--   0        0        0    10817 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6348 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.266704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
+-rw-r--r--   0        0        0     5345 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
+-rw-r--r--   0        0        0    13678 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5546 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2362 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
+-rw-r--r--   0        0        0     5777 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
+-rw-r--r--   0        0        0    15086 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5549 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2412 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1532 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
+-rw-r--r--   0        0        0     1314 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
+-rw-r--r--   0        0        0     6202 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
+-rw-r--r--   0        0        0    18188 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
+-rw-r--r--   0        0        0    14078 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6880 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
+-rw-r--r--   0        0        0     5955 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
+-rw-r--r--   0        0        0    13370 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13882 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7537 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/__init__.py
+-rw-r--r--   0        0        0     1474 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.py
+-rw-r--r--   0        0        0     1563 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2_grpc.py
+-rw-r--r--   0        0        0      216 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2_grpc.pyi
+-rw-r--r--   0        0        0      709 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/README.md
+-rw-r--r--   0        0        0     6729 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
+-rw-r--r--   0        0        0     6650 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
+-rw-r--r--   0        0        0     7228 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
+-rw-r--r--   0        0        0      712 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
+-rw-r--r--   0        0        0     9622 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
+-rw-r--r--   0        0        0     8468 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
+-rw-r--r--   0        0        0     1109 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/protobuf/types/xydata.proto
+-rw-r--r--   0        0        0     2426 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/session.proto
+-rw-r--r--   0        0        0     4196 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.py
+-rw-r--r--   0        0        0     8735 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
+-rw-r--r--   0        0        0     8948 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
+-rw-r--r--   0        0        0     2873 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi
+-rw-r--r--   0        0        0       35 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/utilities/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/measurement/__init__.py
+-rw-r--r--   0        0        0     3791 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/measurement/info.py
+-rw-r--r--   0        0        0    16931 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/measurement/service.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/py.typed
+-rw-r--r--   0        0        0    19995 2023-08-01 19:42:01.270704 ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/session_management.py
+-rw-r--r--   0        0        0     2727 2023-08-01 19:43:03.131454 ni_measurementlink_service-1.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    19906 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.2.0.dev0/setup.py
+-rw-r--r--   0        0        0    18060 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.2.0.dev0/PKG-INFO
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/LICENSE` & `ni_measurementlink_service-1.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/README.md` & `ni_measurementlink_service-1.2.0.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)
     - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)
 
 ---
 
 ## Introduction
 
-MeasurementLink Support for Python (`ni-measurementlink-service`) is a Python framework that enables measurement developers to quickly create Python measurements and run them as a service (gRPC).
+MeasurementLink Support for Python (`ni-measurementlink-service`) is a Python
+framework that helps you create reusable measurement plug-ins using gRPC
+services. Deploy your measurement plug-ins to perform interactive validation in
+InstrumentStudio and automated testing in TestStand.
 
 ---
 
 ## Dependencies
 
 - Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)
 - [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/discovery_client.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/discovery_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """ Contains API to register and un-register measurement service with discovery service.
 """
 import json
 import logging
 import os
 import pathlib
+import subprocess
 import sys
+import time
 import typing
 from typing import Optional
 
 import grpc
 
 from ni_measurementlink_service._internal.stubs.ni.measurementlink.discovery.v1 import (
     discovery_service_pb2,
@@ -21,14 +23,19 @@
     import msvcrt
 
     import win32con
     import win32file
     import winerror
 
 _logger = logging.getLogger(__name__)
+# Save Popen object to avoid "ResourceWarning: subprocess N is still running"
+_discovery_service_subprocess: Optional[subprocess.Popen] = None
+
+_START_SERVICE_TIMEOUT = 30.0
+_START_SERVICE_POLLING_INTERVAL = 100e-3
 
 
 class ServiceLocation(typing.NamedTuple):
     """Represents the location of a service."""
 
     location: str
     insecure_port: str
@@ -53,15 +60,17 @@
         stub (DiscoveryServiceStub): The gRPC stub used to interact with the discovery
         service.
 
         registration_id(string): The ID from discovery service upon successful registration.
 
     """
 
-    def __init__(self, stub: Optional[discovery_service_pb2_grpc.DiscoveryServiceStub] = None):
+    def __init__(
+        self, stub: Optional[discovery_service_pb2_grpc.DiscoveryServiceStub] = None
+    ) -> None:
         """Initialize the Discovery Client with provided registry service stub.
 
         Args:
             stub (DiscoveryServiceStub, optional): The gRPC stub to interact with discovery
             service. Defaults to None.
 
         """
@@ -102,14 +111,15 @@
             service_location.insecure_port = service_port
             # Service Descriptor
             service_descriptor = discovery_service_pb2.ServiceDescriptor()
             service_descriptor.display_name = measurement_info.display_name
             service_descriptor.service_class = service_info.service_class
             service_descriptor.description_url = service_info.description_url
             service_descriptor.provided_interfaces.extend(service_info.provided_interfaces)
+            service_descriptor.annotations.update(service_info.annotations)
 
             # Registration Request Creation
             request = discovery_service_pb2.RegisterServiceRequest(
                 location=service_location, service_description=service_descriptor
             )
             # Registration RPC Call
             register_response = self.stub.RegisterService(request)
@@ -123,14 +133,15 @@
             else:
                 _logger.exception("Error in registering with discovery service.")
             return False
         except FileNotFoundError:
             _logger.error(
                 "Unable to register with discovery service. Possible reason: discovery service not running."
             )
+            return False
         except Exception:
             _logger.exception("Error in registering with discovery service.")
             return False
         return True
 
     def unregister_service(self) -> bool:
         """Un-registers the measurement service from the discovery service.
@@ -149,26 +160,28 @@
                     registration_id=self.registration_id
                 )
                 # Un-registration RPC Call
                 self.stub.UnregisterService(request)
                 _logger.info("Successfully unregistered with discovery service.")
             else:
                 _logger.info("Not registered with discovery service.")
+                return False
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
                 _logger.error(
                     "Unable to unregister with discovery service. Possible reason: discovery service not available."
                 )
             else:
                 _logger.exception("Error in unregistering with discovery service.")
             return False
         except FileNotFoundError:
             _logger.error(
                 "Unable to unregister with discovery service. Possible reason: discovery service not running."
             )
+            return False
         except Exception:
             _logger.exception("Error in unregistering with discovery service.")
             return False
         return True
 
     def resolve_service(self, provided_interface: str, service_class: str = "") -> ServiceLocation:
         """Resolve the location of a service.
@@ -200,20 +213,92 @@
             insecure_port=response.insecure_port,
             ssl_authenticated_port=response.ssl_authenticated_port,
         )
 
 
 def _get_discovery_service_address() -> str:
     key_file_path = _get_key_file_path()
+    _ensure_discovery_service_started(key_file_path)
     _logger.debug("Discovery service key file path: %s", key_file_path)
     with _open_key_file(str(key_file_path)) as key_file:
         key_json = json.load(key_file)
         return "localhost:" + key_json["InsecurePort"]
 
 
+def _ensure_discovery_service_started(key_file_path: pathlib.Path) -> None:
+    """Check whether discovery service already running, if not start the discovery service."""
+    if _service_already_running(key_file_path):
+        return
+
+    exe_file_path = _get_discovery_service_location()
+    _start_service(exe_file_path, key_file_path)
+
+
+def _get_discovery_service_location() -> pathlib.PurePath:
+    """Gets the location of the discovery service process executable."""
+    registration_json_path = _get_registration_json_file_path()
+    registration_json_obj = json.loads(registration_json_path.read_text())
+    return registration_json_path.parent / registration_json_obj["discovery"]["path"]
+
+
+def _get_registration_json_file_path() -> pathlib.Path:
+    if sys.platform == "win32":
+        return (
+            pathlib.Path(os.environ["ProgramW6432"])
+            / "National Instruments"
+            / "Shared"
+            / "MeasurementLink"
+            / "MeasurementLinkServices.json"
+        )
+    else:
+        raise NotImplementedError("Platform not supported")
+
+
+def _key_file_exists(key_file_path: pathlib.Path) -> bool:
+    return key_file_path.is_file() and key_file_path.stat().st_size > 0
+
+
+def _start_service(exe_file_path: pathlib.PurePath, key_file_path: pathlib.Path) -> None:
+    """Starts the service at the specified path and wait for the service to get up and running."""
+    global _discovery_service_subprocess  # save Popen object to avoid ResourceWarning
+    _discovery_service_subprocess = subprocess.Popen(
+        [exe_file_path],
+        cwd=exe_file_path.parent,
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.DEVNULL,
+    )
+    # After the execution of process, check for key file existence in the path
+    # stop checking after 30 seconds have elapsed and throw error
+    timeout_time = time.time() + _START_SERVICE_TIMEOUT
+    while True:
+        try:
+            with _open_key_file(str(key_file_path)) as _:
+                return
+        except IOError:
+            pass
+        if time.time() >= timeout_time:
+            raise TimeoutError("Timed out waiting for discovery service to start")
+        time.sleep(_START_SERVICE_POLLING_INTERVAL)
+
+
+def _service_already_running(key_file_path: pathlib.Path) -> bool:
+    try:
+        _delete_existing_key_file(key_file_path)
+    except IOError:
+        return True
+    return False
+
+
+def _delete_existing_key_file(key_file_path: pathlib.Path) -> None:
+    if _key_file_exists(key_file_path):
+        with key_file_path.open("w") as _:
+            pass
+        key_file_path.unlink()
+
+
 def _get_key_file_path(cluster_id: Optional[str] = None) -> pathlib.Path:
     if cluster_id is not None:
         return _get_key_file_directory() / f"DiscoveryService_{cluster_id}.json"
     return _get_key_file_directory() / "DiscoveryService.json"
 
 
 def _get_key_file_directory() -> pathlib.Path:
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/grpc_servicer.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/grpc_servicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,16 +330,16 @@
         # measurement details
         measurement_details = v2_measurement_service_pb2.MeasurementDetails()
         measurement_details.display_name = self.measurement_info.display_name
         measurement_details.version = self.measurement_info.version
 
         # Measurement Parameters
         measurement_signature = v2_measurement_service_pb2.MeasurementSignature(
-            configuration_parameters_message_type="ni.measurementlink.measurement.v1.MeasurementConfigurations",
-            outputs_message_type="ni.measurementlink.measurement.v1.MeasurementOutputs",
+            configuration_parameters_message_type="ni.measurementlink.measurement.v2.MeasurementConfigurations",
+            outputs_message_type="ni.measurementlink.measurement.v2.MeasurementOutputs",
         )
 
         # Configurations
         for field_number, configuration_metadata in self.configuration_metadata.items():
             configuration_parameter = v2_measurement_service_pb2.ConfigurationParameter()
             configuration_parameter.field_number = field_number
             configuration_parameter.name = configuration_metadata.display_name
@@ -356,14 +356,15 @@
         # Output Parameters Metadata
         for field_number, output_metadata in self.output_metadata.items():
             output_parameter = v2_measurement_service_pb2.Output()
             output_parameter.field_number = field_number
             output_parameter.name = output_metadata.display_name
             output_parameter.type = output_metadata.type
             output_parameter.repeated = output_metadata.repeated
+            output_parameter.annotations.update(output_metadata.annotations)
             measurement_signature.outputs.append(output_parameter)
 
         # Sending back Response
         metadata_response = v2_measurement_service_pb2.GetMetadataResponse(
             measurement_details=measurement_details,
             measurement_signature=measurement_signature,
             user_interface_details=None,
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/metadata.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/parameter/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,10 +156,13 @@
     ):
         return parameter_metadata.annotations.get("ni/enum.values", "")
     else:
         return ""
 
 
 def _is_valid_enum_value(enum_value: object, user_enum: Dict[str, int]) -> bool:
-    if not isinstance(enum_value, Enum):
+    if isinstance(enum_value, Enum):
+        return enum_value.name in user_enum and user_enum[enum_value.name] == enum_value.value
+    elif isinstance(enum_value, int):
+        return enum_value in user_enum.values()
+    else:
         return False
-    return enum_value.name in user_enum and user_enum[enum_value.name] == enum_value.value
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/serialization_strategy.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/parameter/serialization_strategy.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/serializer.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/parameter/serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Parameter Serializer."""
 
+from enum import Enum
 from io import BytesIO
 from typing import Any, Dict, Sequence
 
 from google.protobuf.internal import encoder
 
 from ni_measurementlink_service._internal.parameter import serialization_strategy
 from ni_measurementlink_service._internal.parameter.metadata import (
@@ -71,23 +72,20 @@
             parameter_metadata.type,
             parameter_metadata.repeated,
         )
         type_default_value = serialization_strategy.Context.get_type_default(
             parameter_metadata.type,
             parameter_metadata.repeated,
         )
-        # Convert enum parameters to their underlying value.
+        # Convert enum parameters to their underlying value if necessary.
         if (
             parameter_metadata.annotations.get("ni/type_specialization")
             == TypeSpecialization.Enum.value
         ):
-            if parameter_metadata.repeated:
-                parameter = [x.value for x in parameter]
-            else:
-                parameter = parameter.value
+            parameter = _get_enum_value(parameter, parameter_metadata.repeated)
         # Skipping serialization if the value is None or if its a type default value.
         if parameter is not None and parameter != type_default_value:
             inner_encoder = encoder(i + 1)
             inner_encoder(serialize_buffer.write, parameter, None)
     return serialize_buffer.getvalue()
 
 
@@ -220,19 +218,36 @@
         None: No return value.
 
     """
     for id, value in parameter_by_id.items():
         parameter_metadata = parameter_metadata_dict[id]
         if get_enum_values_annotation(parameter_metadata):
             enum_type = _get_enum_type(parameter_metadata)
+            is_protobuf_enum = enum_type is int
             if parameter_metadata.repeated:
                 for index, member_value in enumerate(value):
-                    parameter_by_id[id][index] = enum_type(member_value)
+                    if is_protobuf_enum:
+                        parameter_by_id[id][index] = member_value
+                    else:
+                        parameter_by_id[id][index] = enum_type(member_value)
             else:
-                parameter_by_id[id] = enum_type(value)
+                if is_protobuf_enum:
+                    parameter_by_id[id] = value
+                else:
+                    parameter_by_id[id] = enum_type(value)
+
+
+def _get_enum_value(parameter: Any, repeated: bool) -> Any:
+    if repeated:
+        if len(parameter) > 0 and isinstance(parameter[0], Enum):
+            return [x.value for x in parameter]
+    else:
+        if isinstance(parameter, Enum):
+            return parameter.value
+    return parameter
 
 
 def _get_enum_type(parameter_metadata: ParameterMetadata) -> type:
     if parameter_metadata.repeated and len(parameter_metadata.default_value) > 0:
         return type(parameter_metadata.default_value[0])
     else:
         return type(parameter_metadata.default_value)
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/service_manager.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/service_manager.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,36 +9,40 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7ni/measurementlink/discovery/v1/discovery_service.proto\x12\x1fni.measurementlink.discovery.v1\"v\n\x11ServiceDescriptor\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x65scription_url\x18\x02 \x01(\t\x12\x1b\n\x13provided_interfaces\x18\x03 \x03(\t\x12\x15\n\rservice_class\x18\x04 \x01(\t\"Z\n\x0fServiceLocation\x12\x10\n\x08location\x18\x01 \x01(\t\x12\x15\n\rinsecure_port\x18\x02 \x01(\t\x12\x1e\n\x16ssl_authenticated_port\x18\x03 \x01(\t\"\xad\x01\n\x16RegisterServiceRequest\x12O\n\x13service_description\x18\x01 \x01(\x0b\x32\x32.ni.measurementlink.discovery.v1.ServiceDescriptor\x12\x42\n\x08location\x18\x02 \x01(\x0b\x32\x30.ni.measurementlink.discovery.v1.ServiceLocation\"2\n\x17RegisterServiceResponse\x12\x17\n\x0fregistration_id\x18\x01 \x01(\t\"3\n\x18UnregisterServiceRequest\x12\x17\n\x0fregistration_id\x18\x01 \x01(\t\"\x1b\n\x19UnregisterServiceResponse\"6\n\x18\x45numerateServicesRequest\x12\x1a\n\x12provided_interface\x18\x01 \x01(\t\"k\n\x19\x45numerateServicesResponse\x12N\n\x12\x61vailable_services\x18\x01 \x03(\x0b\x32\x32.ni.measurementlink.discovery.v1.ServiceDescriptor\"J\n\x15ResolveServiceRequest\x12\x1a\n\x12provided_interface\x18\x01 \x01(\t\x12\x15\n\rservice_class\x18\x02 \x01(\t2\xaf\x04\n\x10\x44iscoveryService\x12\x84\x01\n\x0fRegisterService\x12\x37.ni.measurementlink.discovery.v1.RegisterServiceRequest\x1a\x38.ni.measurementlink.discovery.v1.RegisterServiceResponse\x12\x8a\x01\n\x11UnregisterService\x12\x39.ni.measurementlink.discovery.v1.UnregisterServiceRequest\x1a:.ni.measurementlink.discovery.v1.UnregisterServiceResponse\x12\x8a\x01\n\x11\x45numerateServices\x12\x39.ni.measurementlink.discovery.v1.EnumerateServicesRequest\x1a:.ni.measurementlink.discovery.v1.EnumerateServicesResponse\x12z\n\x0eResolveService\x12\x36.ni.measurementlink.discovery.v1.ResolveServiceRequest\x1a\x30.ni.measurementlink.discovery.v1.ServiceLocationB\xcc\x01\n#com.ni.measurementlink.discovery.v1B\x15\x44iscoveryServiceProtoP\x01Z\x0b\x64iscoveryv1\xa2\x02\x04NIMD\xaa\x02\x30NationalInstruments.MeasurementLink.Discovery.V1\xca\x02\x1fNI\\MeasurementLink\\Discovery\\V1\xea\x02\"NI::MeasurementLink::Discovery::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7ni/measurementlink/discovery/v1/discovery_service.proto\x12\x1fni.measurementlink.discovery.v1\"\x84\x02\n\x11ServiceDescriptor\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x65scription_url\x18\x02 \x01(\t\x12\x1b\n\x13provided_interfaces\x18\x03 \x03(\t\x12\x15\n\rservice_class\x18\x04 \x01(\t\x12X\n\x0b\x61nnotations\x18\x05 \x03(\x0b\x32\x43.ni.measurementlink.discovery.v1.ServiceDescriptor.AnnotationsEntry\x1a\x32\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"Z\n\x0fServiceLocation\x12\x10\n\x08location\x18\x01 \x01(\t\x12\x15\n\rinsecure_port\x18\x02 \x01(\t\x12\x1e\n\x16ssl_authenticated_port\x18\x03 \x01(\t\"\xad\x01\n\x16RegisterServiceRequest\x12O\n\x13service_description\x18\x01 \x01(\x0b\x32\x32.ni.measurementlink.discovery.v1.ServiceDescriptor\x12\x42\n\x08location\x18\x02 \x01(\x0b\x32\x30.ni.measurementlink.discovery.v1.ServiceLocation\"2\n\x17RegisterServiceResponse\x12\x17\n\x0fregistration_id\x18\x01 \x01(\t\"3\n\x18UnregisterServiceRequest\x12\x17\n\x0fregistration_id\x18\x01 \x01(\t\"\x1b\n\x19UnregisterServiceResponse\"6\n\x18\x45numerateServicesRequest\x12\x1a\n\x12provided_interface\x18\x01 \x01(\t\"k\n\x19\x45numerateServicesResponse\x12N\n\x12\x61vailable_services\x18\x01 \x03(\x0b\x32\x32.ni.measurementlink.discovery.v1.ServiceDescriptor\"J\n\x15ResolveServiceRequest\x12\x1a\n\x12provided_interface\x18\x01 \x01(\t\x12\x15\n\rservice_class\x18\x02 \x01(\t2\xaf\x04\n\x10\x44iscoveryService\x12\x84\x01\n\x0fRegisterService\x12\x37.ni.measurementlink.discovery.v1.RegisterServiceRequest\x1a\x38.ni.measurementlink.discovery.v1.RegisterServiceResponse\x12\x8a\x01\n\x11UnregisterService\x12\x39.ni.measurementlink.discovery.v1.UnregisterServiceRequest\x1a:.ni.measurementlink.discovery.v1.UnregisterServiceResponse\x12\x8a\x01\n\x11\x45numerateServices\x12\x39.ni.measurementlink.discovery.v1.EnumerateServicesRequest\x1a:.ni.measurementlink.discovery.v1.EnumerateServicesResponse\x12z\n\x0eResolveService\x12\x36.ni.measurementlink.discovery.v1.ResolveServiceRequest\x1a\x30.ni.measurementlink.discovery.v1.ServiceLocationB\xcc\x01\n#com.ni.measurementlink.discovery.v1B\x15\x44iscoveryServiceProtoP\x01Z\x0b\x64iscoveryv1\xa2\x02\x04NIMD\xaa\x02\x30NationalInstruments.MeasurementLink.Discovery.V1\xca\x02\x1fNI\\MeasurementLink\\Discovery\\V1\xea\x02\"NI::MeasurementLink::Discovery::V1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ni.measurementlink.discovery.v1.discovery_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n#com.ni.measurementlink.discovery.v1B\025DiscoveryServiceProtoP\001Z\013discoveryv1\242\002\004NIMD\252\0020NationalInstruments.MeasurementLink.Discovery.V1\312\002\037NI\\MeasurementLink\\Discovery\\V1\352\002\"NI::MeasurementLink::Discovery::V1'
-  _SERVICEDESCRIPTOR._serialized_start=92
-  _SERVICEDESCRIPTOR._serialized_end=210
-  _SERVICELOCATION._serialized_start=212
-  _SERVICELOCATION._serialized_end=302
-  _REGISTERSERVICEREQUEST._serialized_start=305
-  _REGISTERSERVICEREQUEST._serialized_end=478
-  _REGISTERSERVICERESPONSE._serialized_start=480
-  _REGISTERSERVICERESPONSE._serialized_end=530
-  _UNREGISTERSERVICEREQUEST._serialized_start=532
-  _UNREGISTERSERVICEREQUEST._serialized_end=583
-  _UNREGISTERSERVICERESPONSE._serialized_start=585
-  _UNREGISTERSERVICERESPONSE._serialized_end=612
-  _ENUMERATESERVICESREQUEST._serialized_start=614
-  _ENUMERATESERVICESREQUEST._serialized_end=668
-  _ENUMERATESERVICESRESPONSE._serialized_start=670
-  _ENUMERATESERVICESRESPONSE._serialized_end=777
-  _RESOLVESERVICEREQUEST._serialized_start=779
-  _RESOLVESERVICEREQUEST._serialized_end=853
-  _DISCOVERYSERVICE._serialized_start=856
-  _DISCOVERYSERVICE._serialized_end=1415
+  _SERVICEDESCRIPTOR_ANNOTATIONSENTRY._options = None
+  _SERVICEDESCRIPTOR_ANNOTATIONSENTRY._serialized_options = b'8\001'
+  _SERVICEDESCRIPTOR._serialized_start=93
+  _SERVICEDESCRIPTOR._serialized_end=353
+  _SERVICEDESCRIPTOR_ANNOTATIONSENTRY._serialized_start=303
+  _SERVICEDESCRIPTOR_ANNOTATIONSENTRY._serialized_end=353
+  _SERVICELOCATION._serialized_start=355
+  _SERVICELOCATION._serialized_end=445
+  _REGISTERSERVICEREQUEST._serialized_start=448
+  _REGISTERSERVICEREQUEST._serialized_end=621
+  _REGISTERSERVICERESPONSE._serialized_start=623
+  _REGISTERSERVICERESPONSE._serialized_end=673
+  _UNREGISTERSERVICEREQUEST._serialized_start=675
+  _UNREGISTERSERVICEREQUEST._serialized_end=726
+  _UNREGISTERSERVICERESPONSE._serialized_start=728
+  _UNREGISTERSERVICERESPONSE._serialized_end=755
+  _ENUMERATESERVICESREQUEST._serialized_start=757
+  _ENUMERATESERVICESREQUEST._serialized_end=811
+  _ENUMERATESERVICESRESPONSE._serialized_start=813
+  _ENUMERATESERVICESRESPONSE._serialized_end=920
+  _RESOLVESERVICEREQUEST._serialized_start=922
+  _RESOLVESERVICEREQUEST._serialized_end=996
+  _DISCOVERYSERVICE._serialized_start=999
+  _DISCOVERYSERVICE._serialized_end=1558
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -22,40 +22,75 @@
 class ServiceDescriptor(google.protobuf.message.Message):
     """Description of a registered service. This information can be used to display information to the user
     about the service when services are being developed for a plugin architecture
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
+    class AnnotationsEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     DESCRIPTION_URL_FIELD_NUMBER: builtins.int
     PROVIDED_INTERFACES_FIELD_NUMBER: builtins.int
     SERVICE_CLASS_FIELD_NUMBER: builtins.int
+    ANNOTATIONS_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Required. The user visible name of the service."""
     description_url: builtins.str
     """Optional. Url which provides descriptive information about the service"""
     @property
     def provided_interfaces(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Required. The service interfaces provided by the service. This is the gRPC Full Name of the service.
         Registration can use the gRPC metadata to provide these names.
         """
     service_class: builtins.str
     """Required. The "class" of a service. The value of this field should be unique for a given interface in provided_interfaces.
     In effect, the .proto service declaration defines the interface, and this field defines a class or concrete type of the interface.
     """
+    @property
+    def annotations(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
+        """Optional. Represents a set of annotations on the service.
+        Well-known annotations:
+        - Description
+          - Key: "ni/service.description"
+          - Expected format: string
+          - Example: "Measure inrush current with a shorted load and validate results against configured limits."
+        - Collection
+          - Key: "ni/service.collection"
+          - Expected format: "." delimited namespace/hierarchy case-insensitive string
+          - Example: "CurrentTests.Inrush"
+        - Tags
+          - Key: "ni/service.tags"
+          - Expected format: serialized JSON string of an array of strings
+          - Example: "[\\"powerup\\", \\"current\\"]"
+        """
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         description_url: builtins.str = ...,
         provided_interfaces: collections.abc.Iterable[builtins.str] | None = ...,
         service_class: builtins.str = ...,
+        annotations: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description_url", b"description_url", "display_name", b"display_name", "provided_interfaces", b"provided_interfaces", "service_class", b"service_class"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["annotations", b"annotations", "description_url", b"description_url", "display_name", b"display_name", "provided_interfaces", b"provided_interfaces", "service_class", b"service_class"]) -> None: ...
 
 global___ServiceDescriptor = ServiceDescriptor
 
 @typing_extensions.final
 class ServiceLocation(google.protobuf.message.Message):
     """Represents the location of a service. The location generally includes the IP address and port number for the service
     which can be used to establish communication with the service.
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/README.md` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto`

 * *Files 19% similar despite different names*

```diff
@@ -63,14 +63,30 @@
   // Required. The service interfaces provided by the service. This is the gRPC Full Name of the service.
   // Registration can use the gRPC metadata to provide these names.
   repeated string provided_interfaces = 3;
 
   // Required. The "class" of a service. The value of this field should be unique for a given interface in provided_interfaces.
   // In effect, the .proto service declaration defines the interface, and this field defines a class or concrete type of the interface.
   string service_class = 4;
+
+  // Optional. Represents a set of annotations on the service.
+  // Well-known annotations:
+  // - Description
+  //   - Key: "ni/service.description"
+  //   - Expected format: string
+  //   - Example: "Measure inrush current with a shorted load and validate results against configured limits."
+  // - Collection
+  //   - Key: "ni/service.collection"
+  //   - Expected format: "." delimited namespace/hierarchy case-insensitive string
+  //   - Example: "CurrentTests.Inrush"
+  // - Tags
+  //   - Key: "ni/service.tags"
+  //   - Expected format: serialized JSON string of an array of strings
+  //   - Example: "[\"powerup\", \"current\"]"
+  map<string, string> annotations = 5;
 }
 
 // Represents the location of a service. The location generally includes the IP address and port number for the service
 // which can be used to establish communication with the service.
 message ServiceLocation {
   // Required: The location of the service. This is typically an IP address or DNS name.
   string location = 1;
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/session.proto` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/proto/session.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/info.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/measurement/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Contains classes and enums to represent measurement metadata."""
 from __future__ import annotations
 
 import enum
-import typing
 from pathlib import Path
-from typing import NamedTuple
+from typing import Dict, List, NamedTuple
 
 from google.protobuf import type_pb2
 
 
 class MeasurementInfo(NamedTuple):
     """Class that represents the measurement information.
 
@@ -21,15 +20,15 @@
 
         ui_file_paths (list): Absolute paths of the UI file(s) linked to the measurement.
 
     """
 
     display_name: str
     version: str
-    ui_file_paths: typing.List[Path]
+    ui_file_paths: List[Path]
 
 
 class ServiceInfo(NamedTuple):
     """Class the represents the service information.
 
     Attributes
     ----------
@@ -40,19 +39,24 @@
 
         description_url (str): Description URL of the measurement.
 
         provided_interfaces (List[str]): List of interfaces the service provides.
         For e.g., ni.measurementlink.measurement.v2.MeasurementService.
         Defaults to ["ni.measurementlink.measurement.v1.MeasurementService"].
 
+        annotations (Dict[str,str]): Dict that contains extra information of the measurement.
+        As default we added a (str) description, (str) collection and a (List[str]) list of tags.
+        Feel free to add your own Annotations as needed.
+
     """
 
     service_class: str
     description_url: str
-    provided_interfaces: typing.List[str] = ["ni.measurementlink.measurement.v1.MeasurementService"]
+    provided_interfaces: List[str] = ["ni.measurementlink.measurement.v1.MeasurementService"]
+    annotations: Dict[str, str] = {}
 
 
 class TypeSpecialization(enum.Enum):
     """Enum that represents the type specializations for measurement parameters."""
 
     NoType = ""
     Pin = "pin"
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/service.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/measurement/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,31 @@
 from __future__ import annotations
 
 import json
 from enum import Enum
 from os import path
 from pathlib import Path
 from threading import Lock
-from typing import Any, Callable, Dict, List, Optional, Type, TypeVar
+from types import TracebackType
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import grpc
+from google.protobuf.descriptor import EnumDescriptor
 
 from ni_measurementlink_service._internal import grpc_servicer
 from ni_measurementlink_service._internal.discovery_client import DiscoveryClient
 from ni_measurementlink_service._internal.parameter import (
     metadata as parameter_metadata,
 )
 from ni_measurementlink_service._internal.service_manager import GrpcService
@@ -21,14 +35,22 @@
     DataType,
     MeasurementInfo,
     ServiceInfo,
     TypeSpecialization,
 )
 from ni_measurementlink_service.session_management import PinMapContext
 
+if TYPE_CHECKING:
+    from google.protobuf.internal.enum_type_wrapper import (
+        EnumTypeWrapper,
+        _EnumTypeWrapper,
+    )
+
+    SupportedEnumType = Union[Type[Enum], _EnumTypeWrapper]
+
 
 class MeasurementContext:
     """Proxy for the Measurement Service's context-local state."""
 
     @property
     def grpc_context(self) -> grpc.ServicerContext:
         """Get the context for the RPC."""
@@ -61,26 +83,32 @@
 _TGrpcChannelPool = TypeVar("_TGrpcChannelPool", bound="GrpcChannelPool")
 _TMeasurementService = TypeVar("_TMeasurementService", bound="MeasurementService")
 
 
 class GrpcChannelPool(object):
     """Class that manages gRPC channel lifetimes."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize the GrpcChannelPool object."""
         self._lock: Lock = Lock()
         self._channel_cache: Dict[str, grpc.Channel] = {}
 
     def __enter__(self: _TGrpcChannelPool) -> _TGrpcChannelPool:
         """Enter the runtime context of the GrpcChannelPool."""
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> Literal[False]:
         """Exit the runtime context of the GrpcChannelPool."""
         self.close()
+        return False
 
     def get_channel(self, target: str) -> grpc.Channel:
         """Return a gRPC channel.
 
         Args:
             target (str): The server address
 
@@ -177,22 +205,33 @@
 
         self.measurement_info = MeasurementInfo(
             display_name=service["displayName"],
             version=version,
             ui_file_paths=ui_file_paths,
         )
 
+        def convert_value_to_str(value: object) -> str:
+            if isinstance(value, str):
+                return value
+            return json.dumps(value, separators=(",", ":"))
+
+        service_annotations_string = {
+            key: convert_value_to_str(value)
+            for key, value in service.get("annotations", {}).items()
+        }
+
         self.service_info = ServiceInfo(
             service_class=service["serviceClass"],
             description_url=service["descriptionUrl"],
             provided_interfaces=service["providedInterfaces"],
+            annotations=service_annotations_string,
         )
 
-        self.configuration_parameter_list: list = []
-        self.output_parameter_list: list = []
+        self.configuration_parameter_list: List[Any] = []
+        self.output_parameter_list: List[Any] = []
         self.grpc_service = GrpcService()
         self.context: MeasurementContext = MeasurementContext()
         self.discovery_client: DiscoveryClient = self.grpc_service.discovery_client
         self.channel_pool: GrpcChannelPool = GrpcChannelPool()
 
     def register_measurement(self, measurement_function: Callable) -> Callable:
         """Register a function as the measurement function for a measurement service.
@@ -218,15 +257,15 @@
     def configuration(
         self,
         display_name: str,
         type: DataType,
         default_value: Any,
         *,
         instrument_type: str = "",
-        enum_type: Optional[Type[Enum]] = None,
+        enum_type: Optional[SupportedEnumType] = None,
     ) -> Callable:
         """Add a configuration parameter to a measurement function.
 
         This decorator maps the measurement service's configuration parameters
         to Python positional parameters. To add multiple configuration parameters
         to the same measurement function, use this decorator multiple times.
         The order of decorator calls must match the order of positional parameters.
@@ -246,15 +285,15 @@
             is DataType.Pin. Pin maps have built in instrument definitions using the
             NI driver based instrument type ids. These can be found as constants
             in `nims.session_management`. For example, for an NI DCPower instrument
             the instrument type is `nims.session_management.INSTRUMENT_TYPE_NI_DCPOWER`.
             For custom instruments the user defined instrument type id is defined in the
             pin map file.
 
-            enum_type (Optional[Type[Enum]]):
+            enum_type (Optional[SupportedEnumType]):
             Defines the enum type associated with this configuration parameter. This is only
             supported when configuration type is DataType.Enum or DataType.EnumArray1D.
 
         Returns
         -------
             Callable: Callable that takes in Any Python Function
             and returns the same python function.
@@ -272,15 +311,19 @@
 
         def _configuration(func):
             return func
 
         return _configuration
 
     def output(
-        self, display_name: str, type: DataType, *, enum_type: Optional[Type[Enum]] = None
+        self,
+        display_name: str,
+        type: DataType,
+        *,
+        enum_type: Optional[SupportedEnumType] = None,
     ) -> Callable:
         """Add an output parameter to a measurement function.
 
         This decorator maps the measurement service's output parameters to
         the elements of the tuple returned by the measurement function.
         To add multiple output parameters to the same measurement function,
         use this decorator multiple times.
@@ -291,15 +334,15 @@
 
         Args
         ----
             display_name (str): Display name of the output.
 
             type (DataType): Data type of the output.
 
-            enum_type (Optional[Type[Enum]]):
+            enum_type (Optional[SupportedEnumType]:
             Defines the enum type associated with this configuration parameter. This is only
             supported when configuration type is DataType.Enum or DataType.EnumArray1D.
 
         Returns
         -------
             Callable: Callable that takes in Any Python Function and
             returns the same python function.
@@ -342,15 +385,15 @@
         return self
 
     def _make_annotations_dict(
         self,
         type_specialization: TypeSpecialization,
         *,
         instrument_type: str = "",
-        enum_type: Optional[Type[Enum]] = None,
+        enum_type: Optional[SupportedEnumType] = None,
     ) -> Dict[str, str]:
         annotations: Dict[str, str] = {}
         if type_specialization == TypeSpecialization.NoType:
             return annotations
 
         annotations["ni/type_specialization"] = type_specialization.value
         if type_specialization == TypeSpecialization.Pin:
@@ -360,34 +403,53 @@
             if enum_type is not None:
                 annotations["ni/enum.values"] = self._enum_to_annotations_value(enum_type)
             else:
                 raise ValueError("enum_type is required for enum parameters.")
 
         return annotations
 
-    def _enum_to_annotations_value(self, enum_type: Type[Enum]) -> str:
-        if not any(member.value == 0 for member in enum_type):
-            raise ValueError("The enum does not have a value for 0.")
+    def _enum_to_annotations_value(self, enum_type: SupportedEnumType) -> str:
         enum_values = {}
-        for member in enum_type:
-            enum_values[member.name] = member.value
+        # Note that the type of protobuf enums are an instance of EnumTypeWrapper.
+        # Additionally, issubclass excludes instances as valid parameters so
+        # we use isinstance here.
+        if self._is_protobuf_enum(enum_type):
+            enum_type = cast("EnumTypeWrapper", enum_type)
+            if 0 not in enum_type.values():
+                raise ValueError("The enum does not have a value for 0.")
+            for name, value in enum_type.items():
+                enum_values[name] = value
+        elif isinstance(enum_type, type) and issubclass(enum_type, Enum):
+            if not any(member.value == 0 for member in enum_type):
+                raise ValueError("The enum does not have a value for 0.")
+            for member in enum_type:
+                enum_values[member.name] = member.value
         return json.dumps(enum_values)
 
+    def _is_protobuf_enum(self, enum_type: SupportedEnumType) -> bool:
+        return isinstance(getattr(enum_type, "DESCRIPTOR", None), EnumDescriptor)
+
     def close_service(self) -> None:
         """Close the Service after un-registering with discovery service and cleanups."""
         self.grpc_service.stop()
         self.channel_pool.close()
 
     def __enter__(self: _TMeasurementService) -> _TMeasurementService:
         """Enter the runtime context related to the measurement service."""
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> Literal[False]:
         """Exit the runtime context related to the measurement service."""
         self.close_service()
+        return False
 
     def get_channel(self, provided_interface: str, service_class: str = "") -> grpc.Channel:
         """Return gRPC channel to specified service.
 
         Args
         ----
             provided_interface (str): The gRPC Full Name of the service.
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/session_management.py` & `ni_measurementlink_service-1.2.0.dev0/ni_measurementlink_service/session_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 """Contains methods related to managing driver sessions."""
 from __future__ import annotations
 
 import abc
 import warnings
 from functools import cached_property
-from typing import (
-    Any,
-    Iterable,
-    List,
-    NamedTuple,
-    Optional,
-    Sequence,
-    TypeVar,
-)
+from types import TracebackType
+from typing import Any, Iterable, List, Literal, NamedTuple, Optional, Sequence, Type, TypeVar
 
 import grpc
 from deprecation import DeprecatedWarning
 
 from ni_measurementlink_service._internal.stubs import session_pb2
 from ni_measurementlink_service._internal.stubs.ni.measurementlink import (
     pin_map_context_pb2,
@@ -179,29 +172,34 @@
 class BaseReservation(abc.ABC):
     """Manages session reservation."""
 
     def __init__(
         self,
         session_manager: Client,
         session_info: Sequence[session_management_service_pb2.SessionInformation],
-    ):
+    ) -> None:
         """Initialize reservation object."""
         self._session_manager = session_manager
         self._session_info = session_info
 
     def __enter__(self: _TReservation) -> _TReservation:
         """Context management protocol. Returns self."""
         return self
 
-    def __exit__(self, *exc):
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> Literal[False]:
         """Context management protocol. Calls unreserve()."""
         self.unreserve()
         return False
 
-    def unreserve(self):
+    def unreserve(self) -> None:
         """Unreserve sessions."""
         self._session_manager._unreserve_sessions(self._session_info)
 
 
 class SingleSessionReservation(BaseReservation):
     """Manages reservation for a single session."""
 
@@ -236,15 +234,15 @@
     else:
         raise AttributeError(f"module {__name__} has no attribute {name}")
 
 
 class Client(object):
     """Class that manages driver sessions."""
 
-    def __init__(self, *, grpc_channel: grpc.Channel):
+    def __init__(self, *, grpc_channel: grpc.Channel) -> None:
         """Initialize session manangement client."""
         self._client: session_management_service_pb2_grpc.SessionManagementServiceStub = (
             session_management_service_pb2_grpc.SessionManagementServiceStub(grpc_channel)
         )
 
     def reserve_session(
         self,
@@ -384,20 +382,20 @@
             self._client.ReserveSessions(request)
         )
 
         return response.sessions
 
     def _unreserve_sessions(
         self, session_info: Iterable[session_management_service_pb2.SessionInformation]
-    ):
+    ) -> None:
         """Unreserves sessions so they can be accessed by other clients."""
         request = session_management_service_pb2.UnreserveSessionsRequest(sessions=session_info)
         self._client.UnreserveSessions(request)
 
-    def register_sessions(self, session_info: Iterable[SessionInformation]):
+    def register_sessions(self, session_info: Iterable[SessionInformation]) -> None:
         """Register the sessions with the Session Manager.
 
         Indicates that the sessions are open and will need to be closed later.
 
         Args:
         ----
             session_info (Iterable[SessionInformation]): Sessions to register with the session
@@ -426,15 +424,15 @@
                     ],
                 )
                 for info in session_info
             )
         )
         self._client.RegisterSessions(request)
 
-    def unregister_sessions(self, session_info: Iterable[SessionInformation]):
+    def unregister_sessions(self, session_info: Iterable[SessionInformation]) -> None:
         """Unregisters the sessions from the Session Manager.
 
         Indicates that the sessions have been closed and will need to be reopened before they can be
         used again.
 
         Args:
             session_info (Iterable[SessionInformation]): Sessions to be registered.
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/pyproject.toml` & `ni_measurementlink_service-1.2.0.dev0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 [tool.black]
-extend-exclude ='((.+_pb2_grpc)|(.+_pb2))+(.py)$' # Regex to files with _pb2_grpc.py and _pb2.py Auto Generated Code are excluded
+extend_exclude = '_pb2(_grpc)?\.(py|pyi)$|ni_measurementlink_generator/'
 line-length = 100
-exclude = '''
-(
-\.git # root of the project
-| \.venv
-| venv
-)
-'''
+
+[tool.ni-python-styleguide]
+extend_exclude = '*_pb2_grpc.py,*_pb2_grpc.pyi,*_pb2.py,*_pb2.pyi,ni_measurementlink_generator/'
 
 [tool.poetry]
 name = "ni_measurementlink_service"
-version = "1.1.0-dev2"
+version = "1.2.0-dev0"
 description = "MeasurementLink Support for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md" # apply the repo readme to the package as well
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -66,17 +62,14 @@
 tomlkit = "^0.11.0"
 sphinx-click = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.ni-python-styleguide]
-extend_exclude = "*_pb2_grpc.py,*_pb2.py,venv,ni_measurementlink_generator/*"
-
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --strict-markers"
 filterwarnings = ["always::ImportWarning", "always::ResourceWarning"]
 testpaths = ["tests"]
 
 [tool.mypy]
 warn_unused_configs = true
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/setup.py` & `ni_measurementlink_service-1.2.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,38 +13,41 @@
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v1',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v2',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap.v1',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1',
+ 'ni_measurementlink_service._internal.stubs.ni.protobuf',
+ 'ni_measurementlink_service._internal.stubs.ni.protobuf.types',
  'ni_measurementlink_service._internal.utilities',
  'ni_measurementlink_service.measurement']
 
 package_data = \
 {'': ['*'],
  'ni_measurementlink_service._internal.stubs': ['proto/*',
                                                 'proto/ni/measurementlink/*',
                                                 'proto/ni/measurementlink/discovery/v1/*',
                                                 'proto/ni/measurementlink/measurement/v1/*',
                                                 'proto/ni/measurementlink/measurement/v2/*',
                                                 'proto/ni/measurementlink/pinmap/v1/*',
-                                                'proto/ni/measurementlink/sessionmanagement/v1/*']}
+                                                'proto/ni/measurementlink/sessionmanagement/v1/*',
+                                                'proto/ni/protobuf/types/*']}
 
 install_requires = \
 ['deprecation>=2.1', 'grpcio>=1.49.1,<2.0.0', 'protobuf>=4.21,<5.0']
 
 extras_require = \
 {':sys_platform == "win32"': ['pywin32>=303']}
 
 setup_kwargs = {
     'name': 'ni-measurementlink-service',
-    'version': '1.1.0.dev2',
+    'version': '1.2.0.dev0',
     'description': 'MeasurementLink Support for Python',
-    'long_description': '# MeasurementLink™ Support for Python\n\n- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)\n  - [Introduction](#introduction)\n  - [Dependencies](#dependencies)\n  - [Documentation](#documentation)\n  - [Examples](#examples)\n  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)\n    - [Installation](#installation)\n    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)\n  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)\n  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)\n    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)\n    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)\n  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)\n    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)\n    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)\n    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)\n\n---\n\n## Introduction\n\nMeasurementLink Support for Python (`ni-measurementlink-service`) is a Python framework that enables measurement developers to quickly create Python measurements and run them as a service (gRPC).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)\n- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)\n- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)\n\n---\n\n## Documentation\n\n- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)\n- [API Reference](https://ni.github.io/measurementlink-python/)\n\n---\n\n## System Configuration\n\n### Enable Win32 Long Paths\n\nBy default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. \n\nThere are three ways to do this:\n- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.\n- Set the `Enable Win32 long paths` group policy:\n  - Run `gpedit.msc`.\n  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.\n  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.\n- In the Windows registry, set `HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\FileSystem\\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).\n\n---\n\n## Examples\n\nThe `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If\nyou are using a previous version of MeasurementLink, download the appropriate examples:\n\n- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q3: [measurementlink-python-examples-1.1.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.1.0/measurementlink-python-examples-1.1.0.zip)\n\nFor more information on setting up and running the example measurements, see the included `README.md` file.\n\nFor best results, use the example measurements corresponding to the version of MeasurementLink\nthat you are using. Newer examples may demonstrate features that are not available in older\nversions of MeasurementLink.\n\n---\n\n## Developing Measurements: Quick Start\n\nThis section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.\n\n### Installation\n\nMake sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-service\n```\n\nCheck if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:\n\n```cmd\npip show ni-measurementlink-service\n```\n\n### Developing a minimal Python measurement\n\n1. Install the `ni-measurementlink-generator` package.\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-generator\n```\n\n2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.\n\n    1. Running `ni-measurementlink-generator` without optional arguments:\n\n    `ni-measurementlink-generator SampleMeasurement`\n\n    \'SampleMeasurement\' is the display name of your measurement service. Without the optional arguments,\n    the other arguments are generated for you based on the display name.\n\n    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,\n    `service-class`, and `description-url`:\n\n    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`\n\n    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`\n\n    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`\n\n    If no output directory is specified, the files will\n    be placed in a new folder under the current directory\n    named after the display name without spaces.\n\n3. To customize the created measurement, provide metadata of the measurement\'s configuration (input parameters) and outputs (output parameters) in `measurement.py`.\n    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        #Display Names can not contains backslash or front slash.\n        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")\n        def measure(input_1, input_2):\n            \'\'\' A simple Measurement method\'\'\'\n            return ["foo", "bar"]\n        ```\n\n    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")\n        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)\n        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)\n        def measure(input_1, input_2):\n            return ["foo", "bar"]\n        ```\n\n4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)\n\n---\n\n## Steps to run/debug the measurement service\n\n1. Start the discovery service if not already started.\n\n2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    .venv\\scripts\\activate\n    ```\n\n    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.\n    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:\n\n        ```cmd\n        Set-ExecutionPolicy RemoteSigned \n        ```\n\n3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.\n\n4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.\n\n5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    deactivate\n    ```\n\n---\n\n## Static Registration of Python Measurements\n\nThe MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.\n\nTo statically register a measurement service with the MeasurementLink discovery service, do the following:\n\n1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.\n\n2. Edit the measurement service\'s `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.\n\n3. Copy the measurement service\'s directory (including the `.serviceconfig` file and startup batch file) to a subdirectory of `C:\\ProgramData\\National Instruments\\MeasurementLink\\Services`.\n> **Note**\n> If you are using a virtual environment, do not copy the `.venv` subdirectory&mdash;the virtual environment must be re-created in the new location.\n\nOnce your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.\n\n### Create a batch file that runs a Python measurement\n\nThe batch file used for static registration is responsible for starting the Python Scripts.\n\nTypical Batch File:\n\n``` cmd\n"<path_to_python_exe>" "<path_to_measurement_file>"\n```\n\nExamples to start the fictitious file named `foo_measurement.py`:\n\n1. Using the Python system distribution\n\n    ```cmd\n    python foo_measurement.py\n    ```\n\n2. Using the virtual environment\n\n    ```cmd\n    REM Windows\n    .\\.venv\\Scripts\\python.exe foo_measurement.py\n\n    REM Linux \n    .venv/bin/python foo_measurement.py\n    ```\n\n### Create Executable for Python Scripts\n\nTo create an executable from a measurement, measurement authors can use the [pyinstaller](https://www.pyinstaller.org/) tooling. During the executable creation, the user can also embed the User Interface file using the `--add-data "<path_of_the_UI_File>;."`.\n\nTypical Pyinstaller command to build executable.\n\n```cmd\npyinstaller --onefile --console --add-data "<path_of_the_UI_File>;." --paths .venv\\Lib\\site-packages\\ <path_of_the_measurement_script>\n```\n\n## Troubleshooting\n\n### "File not found" or "No such file or directory" errors when copying or running a measurement service\n\nIf copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.\n\n## Appendix: Managing Measurement as Python Package (Project)\n\nMeasurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:\n\n1. Measurement Python module (`.py` file)\n    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.\n    - This file is run to start the measurement as a service.\n\n2. UI File\n    - UI file for the measurement. Types of supported UI files are:\n        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.\n        - LabVIEW UI (`.vi`)\n    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).\n\nPython communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.\n\n### Create and Manage Python Measurement Package using Poetry\n\n1. Install `poetry` (one-time setup)\n\n    1. Make sure the system has the recommended Python version installed.\n\n    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.\n\n2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.\n\n    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.\n\n        ``` cmd\n        cd <path_of_directory_of_your_choice>\n        ```\n\n    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.\n\n        ``` cmd\n        poetry new <name_of_the_project>\n        ```\n\n    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.\n\n        ``` cmd\n        cd <name_of_the_project>\n        poetry add ni-measurementlink-service\n        ```\n\n    4. The virtual environment will be auto-created by poetry.\n\n    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).\n\n            ``` cmd\n            poetry add <dependency_package_name>\n            ```\n\nFor detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).\n\n### Create and Manage Python Measurement Package using `venv`\n\n1. Make sure the system has the recommended Python version installed.\n\n2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.\n\n    ``` cmd\n    cd <path_of_directory_of_your_choice>\n    ```\n\n3. Create a virtual environment.\n\n    ``` cmd\n    REM This creates a virtual environment named .venv\n    python -m venv .venv\n    ```\n\n4. Activate the virtual environment. After successful activation\n\n    ``` cmd\n    .venv\\scripts\\activate\n    REM Optionally upgrade the pip within the venv by executing the command\n    python -m pip install -U pip\n    ```\n\n5. Install the `ni-measurementlink-service` package into the virtual environment.\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n    - Any additional dependencies required by measurement can be added pip install.\n\n        ``` cmd\n        pip install <dependency_package_name>\n        ```\n\nFor detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).\n\n### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package\n\nMeasurement developers can also install `ni-measurementlink-service` as a system package if necessary.\n\n1. Install the `ni-measurementlink-service` package from the command prompt\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n\n---\n',
+    'long_description': '# MeasurementLink™ Support for Python\n\n- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)\n  - [Introduction](#introduction)\n  - [Dependencies](#dependencies)\n  - [Documentation](#documentation)\n  - [Examples](#examples)\n  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)\n    - [Installation](#installation)\n    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)\n  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)\n  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)\n    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)\n    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)\n  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)\n    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)\n    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)\n    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)\n\n---\n\n## Introduction\n\nMeasurementLink Support for Python (`ni-measurementlink-service`) is a Python\nframework that helps you create reusable measurement plug-ins using gRPC\nservices. Deploy your measurement plug-ins to perform interactive validation in\nInstrumentStudio and automated testing in TestStand.\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)\n- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)\n- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)\n\n---\n\n## Documentation\n\n- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)\n- [API Reference](https://ni.github.io/measurementlink-python/)\n\n---\n\n## System Configuration\n\n### Enable Win32 Long Paths\n\nBy default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. \n\nThere are three ways to do this:\n- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.\n- Set the `Enable Win32 long paths` group policy:\n  - Run `gpedit.msc`.\n  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.\n  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.\n- In the Windows registry, set `HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\FileSystem\\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).\n\n---\n\n## Examples\n\nThe `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If\nyou are using a previous version of MeasurementLink, download the appropriate examples:\n\n- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q3: [measurementlink-python-examples-1.1.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.1.0/measurementlink-python-examples-1.1.0.zip)\n\nFor more information on setting up and running the example measurements, see the included `README.md` file.\n\nFor best results, use the example measurements corresponding to the version of MeasurementLink\nthat you are using. Newer examples may demonstrate features that are not available in older\nversions of MeasurementLink.\n\n---\n\n## Developing Measurements: Quick Start\n\nThis section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.\n\n### Installation\n\nMake sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-service\n```\n\nCheck if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:\n\n```cmd\npip show ni-measurementlink-service\n```\n\n### Developing a minimal Python measurement\n\n1. Install the `ni-measurementlink-generator` package.\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-generator\n```\n\n2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.\n\n    1. Running `ni-measurementlink-generator` without optional arguments:\n\n    `ni-measurementlink-generator SampleMeasurement`\n\n    \'SampleMeasurement\' is the display name of your measurement service. Without the optional arguments,\n    the other arguments are generated for you based on the display name.\n\n    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,\n    `service-class`, and `description-url`:\n\n    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`\n\n    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`\n\n    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`\n\n    If no output directory is specified, the files will\n    be placed in a new folder under the current directory\n    named after the display name without spaces.\n\n3. To customize the created measurement, provide metadata of the measurement\'s configuration (input parameters) and outputs (output parameters) in `measurement.py`.\n    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        #Display Names can not contains backslash or front slash.\n        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")\n        def measure(input_1, input_2):\n            \'\'\' A simple Measurement method\'\'\'\n            return ["foo", "bar"]\n        ```\n\n    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")\n        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)\n        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)\n        def measure(input_1, input_2):\n            return ["foo", "bar"]\n        ```\n\n4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)\n\n---\n\n## Steps to run/debug the measurement service\n\n1. Start the discovery service if not already started.\n\n2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    .venv\\scripts\\activate\n    ```\n\n    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.\n    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:\n\n        ```cmd\n        Set-ExecutionPolicy RemoteSigned \n        ```\n\n3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.\n\n4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.\n\n5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    deactivate\n    ```\n\n---\n\n## Static Registration of Python Measurements\n\nThe MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.\n\nTo statically register a measurement service with the MeasurementLink discovery service, do the following:\n\n1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.\n\n2. Edit the measurement service\'s `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.\n\n3. Copy the measurement service\'s directory (including the `.serviceconfig` file and startup batch file) to a subdirectory of `C:\\ProgramData\\National Instruments\\MeasurementLink\\Services`.\n> **Note**\n> If you are using a virtual environment, do not copy the `.venv` subdirectory&mdash;the virtual environment must be re-created in the new location.\n\nOnce your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.\n\n### Create a batch file that runs a Python measurement\n\nThe batch file used for static registration is responsible for starting the Python Scripts.\n\nTypical Batch File:\n\n``` cmd\n"<path_to_python_exe>" "<path_to_measurement_file>"\n```\n\nExamples to start the fictitious file named `foo_measurement.py`:\n\n1. Using the Python system distribution\n\n    ```cmd\n    python foo_measurement.py\n    ```\n\n2. Using the virtual environment\n\n    ```cmd\n    REM Windows\n    .\\.venv\\Scripts\\python.exe foo_measurement.py\n\n    REM Linux \n    .venv/bin/python foo_measurement.py\n    ```\n\n### Create Executable for Python Scripts\n\nTo create an executable from a measurement, measurement authors can use the [pyinstaller](https://www.pyinstaller.org/) tooling. During the executable creation, the user can also embed the User Interface file using the `--add-data "<path_of_the_UI_File>;."`.\n\nTypical Pyinstaller command to build executable.\n\n```cmd\npyinstaller --onefile --console --add-data "<path_of_the_UI_File>;." --paths .venv\\Lib\\site-packages\\ <path_of_the_measurement_script>\n```\n\n## Troubleshooting\n\n### "File not found" or "No such file or directory" errors when copying or running a measurement service\n\nIf copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.\n\n## Appendix: Managing Measurement as Python Package (Project)\n\nMeasurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:\n\n1. Measurement Python module (`.py` file)\n    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.\n    - This file is run to start the measurement as a service.\n\n2. UI File\n    - UI file for the measurement. Types of supported UI files are:\n        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.\n        - LabVIEW UI (`.vi`)\n    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).\n\nPython communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.\n\n### Create and Manage Python Measurement Package using Poetry\n\n1. Install `poetry` (one-time setup)\n\n    1. Make sure the system has the recommended Python version installed.\n\n    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.\n\n2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.\n\n    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.\n\n        ``` cmd\n        cd <path_of_directory_of_your_choice>\n        ```\n\n    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.\n\n        ``` cmd\n        poetry new <name_of_the_project>\n        ```\n\n    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.\n\n        ``` cmd\n        cd <name_of_the_project>\n        poetry add ni-measurementlink-service\n        ```\n\n    4. The virtual environment will be auto-created by poetry.\n\n    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).\n\n            ``` cmd\n            poetry add <dependency_package_name>\n            ```\n\nFor detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).\n\n### Create and Manage Python Measurement Package using `venv`\n\n1. Make sure the system has the recommended Python version installed.\n\n2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.\n\n    ``` cmd\n    cd <path_of_directory_of_your_choice>\n    ```\n\n3. Create a virtual environment.\n\n    ``` cmd\n    REM This creates a virtual environment named .venv\n    python -m venv .venv\n    ```\n\n4. Activate the virtual environment. After successful activation\n\n    ``` cmd\n    .venv\\scripts\\activate\n    REM Optionally upgrade the pip within the venv by executing the command\n    python -m pip install -U pip\n    ```\n\n5. Install the `ni-measurementlink-service` package into the virtual environment.\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n    - Any additional dependencies required by measurement can be added pip install.\n\n        ``` cmd\n        pip install <dependency_package_name>\n        ```\n\nFor detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).\n\n### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package\n\nMeasurement developers can also install `ni-measurementlink-service` as a system package if necessary.\n\n1. Install the `ni-measurementlink-service` package from the command prompt\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n\n---\n',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/measurementlink-python/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ni_measurementlink_service-1.1.0.dev2/PKG-INFO` & `ni_measurementlink_service-1.2.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ni-measurementlink-service
-Version: 1.1.0.dev2
+Version: 1.2.0.dev0
 Summary: MeasurementLink Support for Python
 Home-page: https://github.com/ni/measurementlink-python/
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,15 +47,18 @@
     - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)
     - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)
 
 ---
 
 ## Introduction
 
-MeasurementLink Support for Python (`ni-measurementlink-service`) is a Python framework that enables measurement developers to quickly create Python measurements and run them as a service (gRPC).
+MeasurementLink Support for Python (`ni-measurementlink-service`) is a Python
+framework that helps you create reusable measurement plug-ins using gRPC
+services. Deploy your measurement plug-ins to perform interactive validation in
+InstrumentStudio and automated testing in TestStand.
 
 ---
 
 ## Dependencies
 
 - Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)
 - [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)
```

