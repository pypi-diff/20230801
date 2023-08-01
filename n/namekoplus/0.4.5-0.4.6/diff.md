# Comparing `tmp/namekoplus-0.4.5.tar.gz` & `tmp/namekoplus-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namekoplus-0.4.5.tar", last modified: Tue Aug  1 06:40:53 2023, max compression
+gzip compressed data, was "namekoplus-0.4.6.tar", last modified: Tue Aug  1 09:17:14 2023, max compression
```

## Comparing `namekoplus-0.4.5.tar` & `namekoplus-0.4.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.315895 namekoplus-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 06:40:41.000000 namekoplus-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 06:40:41.000000 namekoplus-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 06:40:53.315895 namekoplus-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-01 06:40:41.000000 namekoplus-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.307895 namekoplus-0.4.5/namekoplus/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/chassis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis/chassis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/chassis-agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana.json.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.307895 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/config/
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/config/grafana.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.307895 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/all.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/all.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/prometheus_conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/prometheus_conf/prometheus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/statsd_config.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/statsd_mapping.yml.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/chassis-agent/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus/templates/all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/all/all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/all/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.315895 namekoplus-0.4.5/namekoplus/templates/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/demo/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/demo/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.315895 namekoplus-0.4.5/namekoplus/templates/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/event/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/event/events_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.315895 namekoplus-0.4.5/namekoplus/templates/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/http/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/http/http_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.315895 namekoplus-0.4.5/namekoplus/templates/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/rpc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/rpc/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.315895 namekoplus-0.4.5/namekoplus/templates/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/timer/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/templates/timer/timer_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.315895 namekoplus-0.4.5/namekoplus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.315895 namekoplus-0.4.5/namekoplus/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 06:40:41.000000 namekoplus-0.4.5/namekoplus/tests/unit/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:40:53.311895 namekoplus-0.4.5/namekoplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 06:40:53.000000 namekoplus-0.4.5/namekoplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-01 06:40:53.000000 namekoplus-0.4.5/namekoplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:40:53.000000 namekoplus-0.4.5/namekoplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 06:40:53.000000 namekoplus-0.4.5/namekoplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-01 06:40:53.000000 namekoplus-0.4.5/namekoplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 06:40:53.000000 namekoplus-0.4.5/namekoplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 06:40:53.315895 namekoplus-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 06:40:41.000000 namekoplus-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 09:17:01.000000 namekoplus-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 09:17:01.000000 namekoplus-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-01 09:17:14.838031 namekoplus-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 09:17:01.000000 namekoplus-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.834031 namekoplus-0.4.6/namekoplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.834031 namekoplus-0.4.6/namekoplus/chassis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis/chassis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.834031 namekoplus-0.4.6/namekoplus/chassis-agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.834031 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana.json.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.834031 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.834031 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/config/grafana.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.834031 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/all.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/all.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/prometheus_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/prometheus_conf/prometheus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/statsd_config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/statsd_mapping.yml.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/chassis-agent/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/templates/all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/all/all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/all/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/templates/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/demo/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/demo/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/templates/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/event/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/event/events_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/templates/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/http/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/http/http_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/templates/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/rpc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/rpc/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/templates/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/timer/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/templates/timer/timer_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.838031 namekoplus-0.4.6/namekoplus/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 09:17:01.000000 namekoplus-0.4.6/namekoplus/tests/unit/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:14.834031 namekoplus-0.4.6/namekoplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-01 09:17:14.000000 namekoplus-0.4.6/namekoplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-01 09:17:14.000000 namekoplus-0.4.6/namekoplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:17:14.000000 namekoplus-0.4.6/namekoplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 09:17:14.000000 namekoplus-0.4.6/namekoplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-01 09:17:14.000000 namekoplus-0.4.6/namekoplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 09:17:14.000000 namekoplus-0.4.6/namekoplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:17:14.838031 namekoplus-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 09:17:01.000000 namekoplus-0.4.6/setup.py
```

### Comparing `namekoplus-0.4.5/LICENSE` & `namekoplus-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/PKG-INFO` & `namekoplus-0.4.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.4.5
+Version: 0.4.6
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
@@ -56,9 +56,9 @@
 ```
 
 
 ## Detailed Usage
 
 See Documents: 
 
-- [English](https://legendary-sopapillas-e2626d.netlify.app/)
-- [中文](https://doc.bearcatlog.com/)
+- [English](https://murl.vip/TwML)
+- [中文](https://murl.vip/B0O9)
```

### Comparing `namekoplus-0.4.5/README.md` & `namekoplus-0.4.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 ```
 
 
 ## Detailed Usage
 
 See Documents: 
 
-- [English](https://legendary-sopapillas-e2626d.netlify.app/)
-- [中文](https://doc.bearcatlog.com/)
+- [English](https://murl.vip/TwML)
+- [中文](https://murl.vip/B0O9)
```

### Comparing `namekoplus-0.4.5/namekoplus/chassis/chassis.py` & `namekoplus-0.4.6/namekoplus/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana.json.mako` & `namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana.json.mako`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/config/grafana.ini` & `namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/config/grafana.ini`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/all.yaml` & `namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/dashboards/all.yaml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/all.yaml` & `namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/grafana_conf/provisioning/datasources/all.yaml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/prometheus_conf/prometheus.yml` & `namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/prometheus_conf/prometheus.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/chassis-agent/metric-configs/statsd_mapping.yml.mako` & `namekoplus-0.4.6/namekoplus/chassis-agent/metric-configs/statsd_mapping.yml.mako`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml` & `namekoplus-0.4.6/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/command.py` & `namekoplus-0.4.6/namekoplus/command.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/all/all_demo.py` & `namekoplus-0.4.6/namekoplus/templates/all/all_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/all/config.yml` & `namekoplus-0.4.6/namekoplus/templates/all/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/event/config.yml` & `namekoplus-0.4.6/namekoplus/templates/event/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/event/events_demo.py` & `namekoplus-0.4.6/namekoplus/templates/event/events_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/http/config.yml` & `namekoplus-0.4.6/namekoplus/templates/http/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/http/http_demo.py` & `namekoplus-0.4.6/namekoplus/templates/http/http_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/rpc/config.yml` & `namekoplus-0.4.6/namekoplus/templates/rpc/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/rpc/rpc_demo.py` & `namekoplus-0.4.6/namekoplus/templates/rpc/rpc_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/templates/timer/config.yml` & `namekoplus-0.4.6/namekoplus/templates/timer/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus/tests/unit/test_service.py` & `namekoplus-0.4.6/namekoplus/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/namekoplus.egg-info/PKG-INFO` & `namekoplus-0.4.6/namekoplus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.4.5
+Version: 0.4.6
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
@@ -56,9 +56,9 @@
 ```
 
 
 ## Detailed Usage
 
 See Documents: 
 
-- [English](https://legendary-sopapillas-e2626d.netlify.app/)
-- [中文](https://doc.bearcatlog.com/)
+- [English](https://murl.vip/TwML)
+- [中文](https://murl.vip/B0O9)
```

### Comparing `namekoplus-0.4.5/namekoplus.egg-info/SOURCES.txt` & `namekoplus-0.4.6/namekoplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `namekoplus-0.4.5/setup.py` & `namekoplus-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='namekoplus',
-    version='0.4.5',
+    version='0.4.6',
     description='A lightweight Python distributed microservice solution',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     project_urls={
         'Documentation': 'https://doc.bearcatlog.com/',
         'Source Code': 'https://github.com/Bryanthelol/namekoplus',
```

