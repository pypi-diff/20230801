# Comparing `tmp/namekoplus-0.4.1.tar.gz` & `tmp/namekoplus-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namekoplus-0.4.1.tar", last modified: Fri Jul 28 09:54:20 2023, max compression
+gzip compressed data, was "namekoplus-0.4.4.tar", last modified: Tue Aug  1 06:10:40 2023, max compression
```

## Comparing `namekoplus-0.4.1.tar` & `namekoplus-0.4.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.054284 namekoplus-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 09:54:10.000000 namekoplus-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-28 09:54:10.000000 namekoplus-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-28 09:54:20.054284 namekoplus-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 09:54:10.000000 namekoplus-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/chassis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis/chassis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/chassis-agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana.json.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.046284 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/config/
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/config/grafana.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.046284 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/all.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/all.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/prometheus_conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/prometheus_conf/prometheus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/statsd_config.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/statsd_mapping.yml.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/chassis-agent/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/templates/all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/all/all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/all/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/templates/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/demo/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/demo/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus/templates/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/event/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/event/events_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.054284 namekoplus-0.4.1/namekoplus/templates/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/http/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/http/http_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.054284 namekoplus-0.4.1/namekoplus/templates/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/rpc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/rpc/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.054284 namekoplus-0.4.1/namekoplus/templates/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/timer/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/templates/timer/timer_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.054284 namekoplus-0.4.1/namekoplus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.054284 namekoplus-0.4.1/namekoplus/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-28 09:54:10.000000 namekoplus-0.4.1/namekoplus/tests/unit/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:54:20.050284 namekoplus-0.4.1/namekoplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-28 09:54:20.000000 namekoplus-0.4.1/namekoplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-28 09:54:20.000000 namekoplus-0.4.1/namekoplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:54:20.000000 namekoplus-0.4.1/namekoplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-28 09:54:20.000000 namekoplus-0.4.1/namekoplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-28 09:54:20.000000 namekoplus-0.4.1/namekoplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 09:54:20.000000 namekoplus-0.4.1/namekoplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:54:20.054284 namekoplus-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-28 09:54:10.000000 namekoplus-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.561273 namekoplus-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 06:10:27.000000 namekoplus-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 06:10:27.000000 namekoplus-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 06:10:40.561273 namekoplus-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-01 06:10:27.000000 namekoplus-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.553272 namekoplus-0.4.4/namekoplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.553272 namekoplus-0.4.4/namekoplus/chassis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis/chassis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.553272 namekoplus-0.4.4/namekoplus/chassis-agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana.json.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.553272 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/config/grafana.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.553272 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/all.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/all.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/prometheus_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/prometheus_conf/prometheus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/statsd_config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/statsd_mapping.yml.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/chassis-agent/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/templates/all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/all/all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/all/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/templates/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/demo/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/demo/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/templates/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/event/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/event/events_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/templates/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/http/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/http/http_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/templates/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/rpc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/rpc/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/templates/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/timer/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/templates/timer/timer_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.557273 namekoplus-0.4.4/namekoplus/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 06:10:27.000000 namekoplus-0.4.4/namekoplus/tests/unit/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:10:40.553272 namekoplus-0.4.4/namekoplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 06:10:40.000000 namekoplus-0.4.4/namekoplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-01 06:10:40.000000 namekoplus-0.4.4/namekoplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:10:40.000000 namekoplus-0.4.4/namekoplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 06:10:40.000000 namekoplus-0.4.4/namekoplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-01 06:10:40.000000 namekoplus-0.4.4/namekoplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 06:10:40.000000 namekoplus-0.4.4/namekoplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 06:10:40.561273 namekoplus-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 06:10:27.000000 namekoplus-0.4.4/setup.py
```

### Comparing `namekoplus-0.4.1/LICENSE` & `namekoplus-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/PKG-INFO` & `namekoplus-0.4.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.4.1
+Version: 0.4.4
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
@@ -27,17 +27,19 @@
 Provides-Extra: mysql
 Provides-Extra: security
 Provides-Extra: dev
 License-File: LICENSE
 
 # namekoplus
 
+[![Upload Python Package](https://github.com/Bryanthelol/namekoplus/actions/workflows/python-publish.yml/badge.svg?event=release)](https://github.com/Bryanthelol/namekoplus/actions/workflows/python-publish.yml)
+
 A lightweight Python distributed microservice solution
 
-## Command Line Tool Usage
+## CLI Usage
 
 ### Checkout Command
 
 ```shell
 namekoplus --help
 ```
 
@@ -54,9 +56,9 @@
 ```
 
 
 ## Detailed Usage
 
 See Documents: 
 
-- [中文](https://doc.bearcatlog.com/)
 - [English](https://legendary-sopapillas-e2626d.netlify.app/)
+- [中文](https://doc.bearcatlog.com/)
```

### Comparing `namekoplus-0.4.1/namekoplus/chassis/chassis.py` & `namekoplus-0.4.4/namekoplus/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana.json.mako` & `namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana.json.mako`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/config/grafana.ini` & `namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/config/grafana.ini`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/all.yaml` & `namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/all.yaml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/all.yaml` & `namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/all.yaml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/prometheus_conf/prometheus.yml` & `namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/prometheus_conf/prometheus.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/chassis-agent/metric-configs/statsd_mapping.yml.mako` & `namekoplus-0.4.4/namekoplus/chassis-agent/metric-configs/statsd_mapping.yml.mako`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml` & `namekoplus-0.4.4/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/command.py` & `namekoplus-0.4.4/namekoplus/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import importlib
 import inspect
 import os
 import shutil
 from contextlib import contextmanager
 from time import sleep
 
 import click
 import shortuuid
 from python_on_whales import DockerException, ClientNotFoundError, DockerClient, docker
 from mako.template import Template
 
-
 INIT_TYPE_CHOICES = ['all', 'rpc', 'event', 'http', 'timer', 'demo']
 MIDDLEWARE_CHOICES = ['rabbitmq', 'metrics']
 TEST_TYPE_CHOICES = ['unit']
 
 
 def check_docker():
     """
@@ -155,14 +153,15 @@
 
 def stop_network(network_name):
     with status(f'Stopping network {network_name}'):
         docker.network.remove(network_name)
 
 
 def start_metric_servers():
+    # TODO 检查相应容器是否已启动，如果启动，则先删除
     start_network('metric_servers')
     sleep(0.5)
     start_prometheus()
     sleep(0.5)
     start_statsd_exporter()
     sleep(0.5)
     start_statsd_agent()
@@ -320,18 +319,17 @@
               help='The class name of the nameko service')
 def metric_config_gen(module, class_name_str):
     """
     Generate metric config for nameko services.
     """
     import sys
     from statsd.client.timer import Timer
-    sys.path.append(os.getcwd()) 
+    sys.path.append(os.getcwd())
 
     # Extract information of statsd config from the class of nameko service
-    dest_dir = module.split('.')[0]
     file_name = module.split('.')[-1]
     _module = __import__(module)
 
     config_list = []
     for class_name in class_name_str.split(','):
         members = inspect.getmembers(getattr(getattr(_module, file_name), class_name), predicate=inspect.isfunction)
         for member_tuple in members:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `namekoplus-0.4.1/namekoplus/templates/all/all_demo.py` & `namekoplus-0.4.4/namekoplus/templates/all/all_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/templates/all/config.yml` & `namekoplus-0.4.4/namekoplus/templates/all/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/templates/event/config.yml` & `namekoplus-0.4.4/namekoplus/templates/event/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/templates/event/events_demo.py` & `namekoplus-0.4.4/namekoplus/templates/event/events_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/templates/http/config.yml` & `namekoplus-0.4.4/namekoplus/templates/http/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/templates/http/http_demo.py` & `namekoplus-0.4.4/namekoplus/templates/http/http_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/templates/rpc/config.yml` & `namekoplus-0.4.4/namekoplus/templates/rpc/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/templates/rpc/rpc_demo.py` & `namekoplus-0.4.4/namekoplus/templates/rpc/rpc_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/templates/timer/config.yml` & `namekoplus-0.4.4/namekoplus/templates/timer/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus/tests/unit/test_service.py` & `namekoplus-0.4.4/namekoplus/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/namekoplus.egg-info/PKG-INFO` & `namekoplus-0.4.4/namekoplus.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.4.1
+Version: 0.4.4
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
@@ -27,17 +27,19 @@
 Provides-Extra: mysql
 Provides-Extra: security
 Provides-Extra: dev
 License-File: LICENSE
 
 # namekoplus
 
+[![Upload Python Package](https://github.com/Bryanthelol/namekoplus/actions/workflows/python-publish.yml/badge.svg?event=release)](https://github.com/Bryanthelol/namekoplus/actions/workflows/python-publish.yml)
+
 A lightweight Python distributed microservice solution
 
-## Command Line Tool Usage
+## CLI Usage
 
 ### Checkout Command
 
 ```shell
 namekoplus --help
 ```
 
@@ -54,9 +56,9 @@
 ```
 
 
 ## Detailed Usage
 
 See Documents: 
 
-- [中文](https://doc.bearcatlog.com/)
 - [English](https://legendary-sopapillas-e2626d.netlify.app/)
+- [中文](https://doc.bearcatlog.com/)
```

### Comparing `namekoplus-0.4.1/namekoplus.egg-info/SOURCES.txt` & `namekoplus-0.4.4/namekoplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.1/setup.py` & `namekoplus-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='namekoplus',
-    version='0.4.1',
+    version='0.4.4',
     description='A lightweight Python distributed microservice solution',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     project_urls={
         'Documentation': 'https://doc.bearcatlog.com/',
         'Source Code': 'https://github.com/Bryanthelol/namekoplus',
```

