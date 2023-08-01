# Comparing `tmp/dbm-agent-8.33.9.tar.gz` & `tmp/dbm-agent-8.34.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm-agent-8.33.9.tar", last modified: Sat May 27 07:31:59 2023, max compression
+gzip compressed data, was "dbm-agent-8.34.0.tar", last modified: Tue Aug  1 06:56:43 2023, max compression
```

## Comparing `dbm-agent-8.33.9.tar` & `dbm-agent-8.34.0.tar`

### file list

```diff
@@ -1,113 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.973061 dbm-agent-8.33.9/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-27 07:31:59.972061 dbm-agent-8.33.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4453 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.937062 dbm-agent-8.33.9/bin/
--rw-r--r--   0 root         (0) root         (0)      923 2023-05-27 07:30:06.000000 dbm-agent-8.33.9/bin/dbm-agent
--rw-r--r--   0 root         (0) root         (0)      322 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/bin/dbm-bt-conn-stack
--rw-r--r--   0 root         (0) root         (0)      817 2023-05-27 07:29:36.000000 dbm-agent-8.33.9/bin/dbma-cli-init
--rw-r--r--   0 root         (0) root         (0)     2636 2023-05-27 07:29:33.000000 dbm-agent-8.33.9/bin/dbma-cli-mysql
--rw-r--r--   0 root         (0) root         (0)     2265 2023-05-27 07:29:31.000000 dbm-agent-8.33.9/bin/dbma-cli-redis
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.939062 dbm-agent-8.33.9/dbm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2989 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.939062 dbm-agent-8.33.9/dbma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.941062 dbm-agent-8.33.9/dbma/bil/
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/cmdexecutor.py
--rw-r--r--   0 root         (0) root         (0)     3764 2023-05-27 07:30:34.000000 dbm-agent-8.33.9/dbma/bil/daemon.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/fs.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-05-27 07:30:39.000000 dbm-agent-8.33.9/dbma/bil/fun.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/net.py
--rw-r--r--   0 root         (0) root         (0)     6795 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/osuser.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/sudos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.942062 dbm-agent-8.33.9/dbma/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.944062 dbm-agent-8.33.9/dbma/components/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.944062 dbm-agent-8.33.9/dbma/components/mysql/backups/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/mysql/backups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-27 07:26:51.000000 dbm-agent-8.33.9/dbma/components/mysql/backups/cloneplugin.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-05-27 07:25:58.000000 dbm-agent-8.33.9/dbma/components/mysql/commons.py
--rw-r--r--   0 root         (0) root         (0)    21071 2023-05-27 07:26:05.000000 dbm-agent-8.33.9/dbma/components/mysql/config.py
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-27 07:26:09.000000 dbm-agent-8.33.9/dbma/components/mysql/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15232 2023-05-27 07:26:14.000000 dbm-agent-8.33.9/dbma/components/mysql/install.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-05-27 07:26:20.000000 dbm-agent-8.33.9/dbma/components/mysql/instance.py
--rw-r--r--   0 root         (0) root         (0)     3994 2023-05-27 07:26:23.000000 dbm-agent-8.33.9/dbma/components/mysql/replica.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-05-27 07:26:29.000000 dbm-agent-8.33.9/dbma/components/mysql/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.945062 dbm-agent-8.33.9/dbma/components/mysql/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/mysql/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13668 2023-05-27 07:26:38.000000 dbm-agent-8.33.9/dbma/components/mysql/views/defaultsview.py
--rw-r--r--   0 root         (0) root         (0)     4373 2023-05-27 07:26:44.000000 dbm-agent-8.33.9/dbma/components/mysql/views/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.946062 dbm-agent-8.33.9/dbma/components/orchestrator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/orchestrator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-27 07:26:58.000000 dbm-agent-8.33.9/dbma/components/orchestrator/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-05-27 07:27:01.000000 dbm-agent-8.33.9/dbma/components/orchestrator/install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.948062 dbm-agent-8.33.9/dbma/components/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1623 2023-05-27 07:27:34.000000 dbm-agent-8.33.9/dbma/components/redis/commons.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-05-27 07:27:09.000000 dbm-agent-8.33.9/dbma/components/redis/config.py
--rw-r--r--   0 root         (0) root         (0)      548 2023-05-27 07:27:39.000000 dbm-agent-8.33.9/dbma/components/redis/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7306 2023-05-27 07:27:47.000000 dbm-agent-8.33.9/dbma/components/redis/install.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-05-27 07:27:52.000000 dbm-agent-8.33.9/dbma/components/redis/systemd.py
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-27 07:27:57.000000 dbm-agent-8.33.9/dbma/components/redis/uninstall.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.950062 dbm-agent-8.33.9/dbma/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.951062 dbm-agent-8.33.9/dbma/core/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3460 2023-05-27 07:29:03.000000 dbm-agent-8.33.9/dbma/core/agent/init.py
--rw-r--r--   0 root         (0) root         (0)      115 2023-05-27 07:29:07.000000 dbm-agent-8.33.9/dbma/core/agent/upgrade.py
--rw-r--r--   0 root         (0) root         (0)     3677 2023-05-27 07:28:10.000000 dbm-agent-8.33.9/dbma/core/configs.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-27 07:28:18.000000 dbm-agent-8.33.9/dbma/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     3469 2023-05-27 07:28:26.000000 dbm-agent-8.33.9/dbma/core/httpserver.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-05-27 07:28:34.000000 dbm-agent-8.33.9/dbma/core/messages.py
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-27 07:28:39.000000 dbm-agent-8.33.9/dbma/core/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.951062 dbm-agent-8.33.9/dbma/core/threads/
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/threads/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-05-27 07:28:57.000000 dbm-agent-8.33.9/dbma/core/threads/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.952062 dbm-agent-8.33.9/dbma/core/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/views/dbmagentview.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/views/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.936062 dbm-agent-8.33.9/dbma/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.971062 dbm-agent-8.33.9/dbma/static/cnfs/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/auto-inseption-db.sql
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/create-innodb-cluster.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      514 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/init-5.7.x.sql
--rw-r--r--   0 root         (0) root         (0)     1370 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/init-8.0.x.sql
--rw-r--r--   0 root         (0) root         (0)     6681 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/init-users.sql.jinja
--rw-r--r--   0 root         (0) root         (0)    10688 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-5.7-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    14664 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    17621 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17631 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17687 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17799 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18787 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18776 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18774 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysqld.service.jinja
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/redis.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/redisd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/zabbix-agentd.service
--rw-r--r--   0 root         (0) root         (0)    10464 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/zabbix_agentd.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/zoo.cnf.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.972061 dbm-agent-8.33.9/dbma/static/sql-scripts/
--rw-r--r--   0 root         (0) root         (0)     9468 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/sql-scripts/常用SQL.md
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-27 07:31:24.000000 dbm-agent-8.33.9/dbma/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 07:31:59.973061 dbm-agent-8.33.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.920376 dbm-agent-8.34.0/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-08-01 06:56:43.920376 dbm-agent-8.34.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7740 2023-07-21 12:27:33.000000 dbm-agent-8.34.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.860376 dbm-agent-8.34.0/bin/
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-30 12:35:14.000000 dbm-agent-8.34.0/bin/dbm-agent
+-rw-r--r--   0 root         (0) root         (0)      322 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/bin/dbm-bt-conn-stack
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-30 12:35:07.000000 dbm-agent-8.34.0/bin/dbma-cli-init
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-06-30 12:38:52.000000 dbm-agent-8.34.0/bin/dbma-cli-mysql
+-rw-r--r--   0 root         (0) root         (0)     2321 2023-06-30 12:34:44.000000 dbm-agent-8.34.0/bin/dbma-cli-redis
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.876376 dbm-agent-8.34.0/dbm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-08-01 06:56:43.000000 dbm-agent-8.34.0/dbm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-08-01 06:56:43.000000 dbm-agent-8.34.0/dbm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 06:56:43.000000 dbm-agent-8.34.0/dbm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-08-01 06:56:43.000000 dbm-agent-8.34.0/dbm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      252 2023-08-01 06:56:43.000000 dbm-agent-8.34.0/dbm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.881376 dbm-agent-8.34.0/dbma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.884376 dbm-agent-8.34.0/dbma/bil/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/bil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/bil/cmdexecutor.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-05-27 07:30:34.000000 dbm-agent-8.34.0/dbma/bil/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-06-30 06:41:17.000000 dbm-agent-8.34.0/dbma/bil/fs.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-05-27 07:30:39.000000 dbm-agent-8.34.0/dbma/bil/fun.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/bil/net.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/bil/osuser.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/bil/sudos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.885376 dbm-agent-8.34.0/dbma/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.887376 dbm-agent-8.34.0/dbma/components/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/components/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-05-29 11:59:15.000000 dbm-agent-8.34.0/dbma/components/mysql/asserts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.888376 dbm-agent-8.34.0/dbma/components/mysql/backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-18 14:11:07.000000 dbm-agent-8.34.0/dbma/components/mysql/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7758 2023-07-04 12:23:24.000000 dbm-agent-8.34.0/dbma/components/mysql/backends/clears.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.888376 dbm-agent-8.34.0/dbma/components/mysql/backups/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/components/mysql/backups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-27 07:26:51.000000 dbm-agent-8.34.0/dbma/components/mysql/backups/cloneplugin.py
+-rw-r--r--   0 root         (0) root         (0)     9079 2023-06-17 15:39:10.000000 dbm-agent-8.34.0/dbma/components/mysql/commons.py
+-rw-r--r--   0 root         (0) root         (0)    15768 2023-07-18 06:55:14.000000 dbm-agent-8.34.0/dbma/components/mysql/config.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-21 13:38:17.000000 dbm-agent-8.34.0/dbma/components/mysql/deploy.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-11 09:27:16.000000 dbm-agent-8.34.0/dbma/components/mysql/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14693 2023-07-18 06:49:24.000000 dbm-agent-8.34.0/dbma/components/mysql/install.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-05-27 07:26:20.000000 dbm-agent-8.34.0/dbma/components/mysql/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-05-27 07:26:23.000000 dbm-agent-8.34.0/dbma/components/mysql/replica.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-05-27 07:26:29.000000 dbm-agent-8.34.0/dbma/components/mysql/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.889376 dbm-agent-8.34.0/dbma/components/mysql/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/components/mysql/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13668 2023-07-04 14:24:35.000000 dbm-agent-8.34.0/dbma/components/mysql/views/defaultsview.py
+-rw-r--r--   0 root         (0) root         (0)     4373 2023-05-27 07:26:44.000000 dbm-agent-8.34.0/dbma/components/mysql/views/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.890376 dbm-agent-8.34.0/dbma/components/orchestrator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/components/orchestrator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-27 07:26:58.000000 dbm-agent-8.34.0/dbma/components/orchestrator/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-05-27 07:27:01.000000 dbm-agent-8.34.0/dbma/components/orchestrator/install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.892376 dbm-agent-8.34.0/dbma/components/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/components/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-05-27 07:27:34.000000 dbm-agent-8.34.0/dbma/components/redis/commons.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-05-27 07:27:09.000000 dbm-agent-8.34.0/dbma/components/redis/config.py
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-27 07:27:39.000000 dbm-agent-8.34.0/dbma/components/redis/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2023-07-21 12:27:33.000000 dbm-agent-8.34.0/dbma/components/redis/install.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-27 07:27:52.000000 dbm-agent-8.34.0/dbma/components/redis/systemd.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-27 07:27:57.000000 dbm-agent-8.34.0/dbma/components/redis/uninstall.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.893376 dbm-agent-8.34.0/dbma/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.894376 dbm-agent-8.34.0/dbma/core/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/core/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-05-27 12:44:26.000000 dbm-agent-8.34.0/dbma/core/agent/init.py
+-rw-r--r--   0 root         (0) root         (0)      115 2023-05-27 07:29:07.000000 dbm-agent-8.34.0/dbma/core/agent/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     6064 2023-07-16 14:26:38.000000 dbm-agent-8.34.0/dbma/core/configs.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-27 07:28:18.000000 dbm-agent-8.34.0/dbma/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-06-21 06:55:16.000000 dbm-agent-8.34.0/dbma/core/httpserver.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-27 07:28:34.000000 dbm-agent-8.34.0/dbma/core/messages.py
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-27 07:28:39.000000 dbm-agent-8.34.0/dbma/core/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.894376 dbm-agent-8.34.0/dbma/core/threads/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/core/threads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-05-27 07:28:57.000000 dbm-agent-8.34.0/dbma/core/threads/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.895376 dbm-agent-8.34.0/dbma/core/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/core/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/core/views/dbmagentview.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/core/views/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.798377 dbm-agent-8.34.0/dbma/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.919376 dbm-agent-8.34.0/dbma/static/cnfs/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/auto-inseption-db.sql
+-rw-r--r--   0 root         (0) root         (0)      514 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/init-5.7.x.sql
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/init-8.0.x.sql
+-rw-r--r--   0 root         (0) root         (0)     6681 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/init-users.sql.jinja
+-rw-r--r--   0 root         (0) root         (0)    10688 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysql-5.7-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    14664 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    17799 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18787 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18776 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18775 2023-07-03 13:42:57.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18775 2023-08-01 06:55:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.34.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/mysqld.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/redis.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/cnfs/redisd.service.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:56:43.919376 dbm-agent-8.34.0/dbma/static/sql-scripts/
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-05-20 14:15:43.000000 dbm-agent-8.34.0/dbma/static/sql-scripts/常用SQL.md
+-rw-r--r--   0 root         (0) root         (0)      344 2023-08-01 06:55:56.000000 dbm-agent-8.34.0/dbma/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 06:56:43.920376 dbm-agent-8.34.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-06-21 06:55:16.000000 dbm-agent-8.34.0/setup.py
```

### Comparing `dbm-agent-8.33.9/PKG-INFO` & `dbm-agent-8.34.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.9
+Version: 8.34.0
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.33.9/bin/dbm-agent` & `dbm-agent-8.34.0/bin/dbm-agent`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 import argparse
 from dbma.core.httpserver import start, stop
 from dbma.version import DBM_AGENT_VESION
 
 
 def parser_cmd_args():
-    parser = argparse.ArgumentParser(f"dbma-agent {DBM_AGENT_VESION}")
+    parser = argparse.ArgumentParser(
+        f"dbma-agent {DBM_AGENT_VESION}",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     parser.add_argument(
         "action",
         type=str,
         default="start",
         choices=("start", "stop", "version"),
         help="",
     )
```

### Comparing `dbm-agent-8.33.9/bin/dbma-cli-init` & `dbm-agent-8.34.0/bin/dbma-cli-init`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import argparse
 from dbma.bil.net import get_ip_by_card_name
 from dbma.core.agent.init import init
 
 
 def parser_cmd_args():
     """ """
-    parser = argparse.ArgumentParser("dbma-cli-init")
+    parser = argparse.ArgumentParser(
+        "dbma-cli-init", formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
     parser.add_argument("--net-card", default="eth0")
     parser.add_argument("--dbm-center-url-prefix", default="http://127.0.0.1:8080")
     return parser.parse_args()
 
 
 def main():
     args = parser_cmd_args()
```

### Comparing `dbm-agent-8.33.9/bin/dbma-cli-mysql` & `dbm-agent-8.34.0/bin/dbma-cli-mysql`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 from dbma.components.mysql.commons import make_mysql_writable
 
 
 def parser_cmd_args():
     """
     实现命令行参数的处理
     """
-    parser = argparse.ArgumentParser(__name__)
+    parser = argparse.ArgumentParser(
+        __name__, formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
     parser.add_argument("--port", type=int, default=3306, help="instance port")
     parser.add_argument(
         "--pkg-name",
         type=str,
         default=default_pkg.name,
-        help="mysql install package name default {}".format(default_pkg.name),
+        help="mysql install package name ",
     )
     parser.add_argument(
         "--ibps",
         type=str,
         default="128M",
         help="innodb-buffer-pool-size  et: 128M , 512M, 1G, 2G",
     )
```

### Comparing `dbm-agent-8.33.9/bin/dbma-cli-redis` & `dbm-agent-8.34.0/bin/dbma-cli-redis`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from dbma.components.redis.commons import default_redis_pkg, default_redis_port
 
 
 def parser_cmd_args():
     """
     实现命令行参数的处理
     """
-    parser = argparse.ArgumentParser(__name__)
+    parser = argparse.ArgumentParser(__name__, formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument(
         "--pkg", default=default_redis_pkg, help="redis install pkg", type=str
     )
     parser.add_argument(
         "--port", default=default_redis_port, help="redis default port", type=int
     )
     parser.add_argument(
```

### Comparing `dbm-agent-8.33.9/dbm_agent.egg-info/PKG-INFO` & `dbm-agent-8.34.0/dbm_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.9
+Version: 8.34.0
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.33.9/dbm_agent.egg-info/SOURCES.txt` & `dbm-agent-8.34.0/dbm_agent.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,21 +18,25 @@
 dbma/bil/fs.py
 dbma/bil/fun.py
 dbma/bil/net.py
 dbma/bil/osuser.py
 dbma/bil/sudos.py
 dbma/components/__init__.py
 dbma/components/mysql/__init__.py
+dbma/components/mysql/asserts.py
 dbma/components/mysql/commons.py
 dbma/components/mysql/config.py
+dbma/components/mysql/deploy.py
 dbma/components/mysql/exceptions.py
 dbma/components/mysql/install.py
 dbma/components/mysql/instance.py
 dbma/components/mysql/replica.py
 dbma/components/mysql/source.py
+dbma/components/mysql/backends/__init__.py
+dbma/components/mysql/backends/clears.py
 dbma/components/mysql/backups/__init__.py
 dbma/components/mysql/backups/cloneplugin.py
 dbma/components/mysql/views/__init__.py
 dbma/components/mysql/views/defaultsview.py
 dbma/components/mysql/views/handlers.py
 dbma/components/orchestrator/__init__.py
 dbma/components/orchestrator/exceptions.py
@@ -55,39 +59,22 @@
 dbma/core/agent/upgrade.py
 dbma/core/threads/__init__.py
 dbma/core/threads/backends.py
 dbma/core/views/__init__.py
 dbma/core/views/dbmagentview.py
 dbma/core/views/response.py
 dbma/static/cnfs/auto-inseption-db.sql
-dbma/static/cnfs/create-innodb-cluster.js
-dbma/static/cnfs/dbm-backup-proxyd.service.jinja
-dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
 dbma/static/cnfs/init-5.7.x.sql
 dbma/static/cnfs/init-8.0.x.sql
 dbma/static/cnfs/init-users.sql.jinja
 dbma/static/cnfs/mysql-5.7-init-only.jinja
 dbma/static/cnfs/mysql-5.7.25.cnf.jinja
 dbma/static/cnfs/mysql-8.0-init-only.jinja
-dbma/static/cnfs/mysql-8.0.17.cnf.jinja
-dbma/static/cnfs/mysql-8.0.18.cnf.jinja
-dbma/static/cnfs/mysql-8.0.19.cnf.jinja
-dbma/static/cnfs/mysql-8.0.20.cnf.jinja
-dbma/static/cnfs/mysql-8.0.21.cnf.jinja
-dbma/static/cnfs/mysql-8.0.22.cnf.jinja
-dbma/static/cnfs/mysql-8.0.23.cnf.jinja
-dbma/static/cnfs/mysql-8.0.25.cnf.jinja
-dbma/static/cnfs/mysql-8.0.26.cnf.jinja
-dbma/static/cnfs/mysql-8.0.27.cnf.jinja
-dbma/static/cnfs/mysql-8.0.28.cnf.jinja
-dbma/static/cnfs/mysql-8.0.29.cnf.jinja
 dbma/static/cnfs/mysql-8.0.30.cnf.jinja
 dbma/static/cnfs/mysql-8.0.31.cnf.jinja
 dbma/static/cnfs/mysql-8.0.32.cnf.jinja
 dbma/static/cnfs/mysql-8.0.33.cnf.jinja
+dbma/static/cnfs/mysql-8.0.34.cnf.jinja
 dbma/static/cnfs/mysqld.service.jinja
 dbma/static/cnfs/redis.conf.jinja
 dbma/static/cnfs/redisd.service.jinja
-dbma/static/cnfs/zabbix-agentd.service
-dbma/static/cnfs/zabbix_agentd.conf.jinja
-dbma/static/cnfs/zoo.cnf.jinja
 dbma/static/sql-scripts/常用SQL.md
```

### Comparing `dbm-agent-8.33.9/dbma/bil/daemon.py` & `dbm-agent-8.34.0/dbma/bil/daemon.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/bil/fs.py` & `dbm-agent-8.34.0/dbma/bil/fs.py`

 * *Files 20% similar despite different names*

```diff
@@ -136,14 +136,76 @@
         None
     """
     with open("/etc/profile", "a") as f:
         f.write(line)
         f.write("\n")
 
 
+def get_file_size(file_path: Path):
+    """返回给定文件的大小(字节)
+
+    Parameters:
+    -----------
+    file_path: Path
+        文件路径
+    """
+    # 如果参数是 str 给它转换成 Path
+    if isinstance(file_path, str):
+        file_path = Path(file_path)
+
+    res = os.lstat(file_path)
+    return res.st_size
+
+
+def is_file_greater_then(file_path: Path = None, size: int = None):
+    """
+    检查 file_path 对应文件大小是不是大于 size, 如果是返回 True, 不是返回 False。
+
+    Parameters:
+    -----------
+    file_path: Path
+        文件路径
+
+    size: int
+        大小
+
+    Return:
+    -------
+    bool
+    """
+    return get_file_size(file_path) > size
+
+
+def truncate_or_delete_file(file_path: Path = None, chunk_size: int = 16 * 1024 * 1024):
+    """
+    如果 file_path 的大小大于 chunk_size 就截断 chunk_size 大小的段，不然就删除文件
+
+    Parameters:
+    -----------
+    file_path: Path
+        要执行删除|截断的文件
+
+    chunk_size: int
+        单次截断的大小
+
+    """
+    if isinstance(file_path, str):
+        file_path = Path(file_path)
+
+    # 如果已经不足 chunk_size 大，就删除掉；然后就 truncate 指定大小
+    file_size = get_file_size(file_path)
+    if file_size <= chunk_size:
+        os.remove(file_path)
+        return 0
+
+    chunk = file_size - chunk_size
+    os.truncate(file_path, chunk)
+    return chunk
+
+
 join = os.path.join
 
 readlink = os.readlink
 
 listdir = os.listdir
 
 mkdir = os.mkdir
```

### Comparing `dbm-agent-8.33.9/dbma/bil/net.py` & `dbm-agent-8.34.0/dbma/bil/net.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/bil/osuser.py` & `dbm-agent-8.34.0/dbma/bil/osuser.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/bil/sudos.py` & `dbm-agent-8.34.0/dbma/bil/sudos.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/mysql/backups/cloneplugin.py` & `dbm-agent-8.34.0/dbma/components/mysql/backups/cloneplugin.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/mysql/exceptions.py` & `dbm-agent-8.34.0/dbma/components/redis/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # -*- coding: utf-8 -*-
 
-"""异常树"""
+"""Resdis 相关的异常"""
 
-from dbma.core.exception import DBMAgentException
+from dbma.core.exception import (
+    FileExistsException,
+    FileNotExistsException,
+    DirectoryExistsException,
+)
 
 
-class MySQLTemplateFileNotExistsException(DBMAgentException):
-    """MySQL 配置文件模板不存在"""
+class RedisConfigTemplateFileNotExistsException(FileNotExistsException):
+    """Redis 配置文件模板不存在"""
 
     pass
 
 
-class MySQLPkgFileNotExistsException(DBMAgentException):
-    """MySQL 安装包文件模板不存在"""
+class RedisPkgFileNotExistsException(FileNotExistsException):
+    """Redis 的安装包文件不存在"""
 
     pass
 
 
-class InstanceHasBeenInstalledException(DBMAgentException):
-    """给定实例已经安装过了"""
-
-    pass
-
-
-class MySQLSystemdFileNotExists(DBMAgentException):
-    """ """
+class RedisDatabaseDirectoryExistsException(DirectoryExistsException):
+    """Redis 的数据目录已经存在"""
 
     pass
```

### Comparing `dbm-agent-8.33.9/dbma/components/mysql/install.py` & `dbm-agent-8.34.0/dbma/components/mysql/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,35 @@
 import shutil
 import tarfile
 import logging
 from pathlib import Path
 from datetime import datetime
 from dbma.bil.fun import fname
 from dbma.core import messages
-from dbma.bil.osuser import MySQLUser
 from dbma.bil.cmdexecutor import exe_shell_cmd
 from dbma.core.configs import dbm_agent_config
-from dbma.components.mysql.config import MySQLConfig
+from dbma.components.mysql.config import MySQLSRConfig, MySQLSystemdConfig
 from dbma.components.mysql.commons import get_mysql_version
 from dbma.components.mysql.commons import export_cmds_to_path
 from dbma.components.mysql.commons import pkg_to_basedir, default_pkg
-from dbma.components.mysql.commons import export_header_files, export_so_files
+from dbma.components.mysql.commons import (
+    export_header_files,
+    export_so_files,
+    create_os_user_for_mysql,
+    create_mysql_dirs,
+)
 from dbma.components.mysql.exceptions import MySQLSystemdFileNotExists
 from dbma.components.mysql.exceptions import MySQLPkgFileNotExistsException
 from dbma.components.mysql.exceptions import InstanceHasBeenInstalledException
+from dbma.components.mysql.asserts import (
+    assert_mysql_install_pkg_exists,
+    assert_mysql_datadir_not_exists,
+    assert_mysql_systemd_file_exists,
+    assert_mysql_systemd_file_not_exists,
+)
 
 
 def create_init_sql_file(version: str = None):
     """生成 init-sql 文件给 init 的时候用
 
     Parameters:
     -----------
@@ -94,29 +104,23 @@
     Return:
     -------
     None
 
     Exceptions:
     ----------
     MySQLPkgFileNotExistsException
-
-    InstanceHasBeenInstalledException
-
+    MySQLDataDirectoryExists
     """
-    # 检查安装包是否存在
     logging.info(messages.FUN_STARTS.format(fname()))
-    if not pkg.exists():
-        logging.warn(messages.FILE_NOT_EXISTS.format(pkg))
-        raise MySQLPkgFileNotExistsException(messages.FILE_NOT_EXISTS.format(pkg))
+
+    # 检查安装包是否存在
+    assert_mysql_install_pkg_exists(pkg)
 
     # 检查给定的实例是不是已经安装过了
-    datadir = Path(dbm_agent_config.mysql_datadir_parent) / "{}".format(port)
-    if datadir.exists():
-        logging.warn(messages.MYSQL_INSTANCE_HAS_EXISTS.format(port))
-        raise InstanceHasBeenInstalledException(str(port))
+    assert_mysql_datadir_not_exists(port)
 
     logging.info(messages.FUN_ENDS.format(fname()))
 
 
 def check_mysql_systemd_exists(port: int = 3306):
     """检查 mysql 的 systemd 配置文件是否存在
 
@@ -159,15 +163,16 @@
     -----------
     MySQLSystemdFileNotExists
     """
     # 如果 systemd 配置文件不存在就报异常
     logging.info(messages.FUN_STARTS.format(fname()))
 
     try:
-        check_mysql_systemd_exists(port)
+        # check_mysql_systemd_exists(port)
+        assert_mysql_systemd_file_exists(port)
         # 没有报异常，说明 systemd 配置存在, 准备执行 enable 操作
         enable_cmd = "systemctl enable mysqld-{}".format(port)
         logging.info(messages.EXECUTE_CMD.format(enable_cmd))
         exe_shell_cmd(enable_cmd)
     except MySQLSystemdFileNotExists as err:
         raise err
 
@@ -190,15 +195,16 @@
     -----------
     MySQLSystemdFileNotExists
     """
     # 如果 systemd 配置文件不存在就报异常
     logging.info(messages.FUN_STARTS.format(fname()))
 
     try:
-        check_mysql_systemd_exists(port)
+        # check_mysql_systemd_exists(port)
+        assert_mysql_systemd_file_exists(port)
         # 没有报异常，说明 systemd 配置存在
         # 执行 enable 操作
         disable_cmd = "systemctl disable mysqld-{}".format(port)
         logging.info(messages.EXECUTE_CMD.format(disable_cmd))
         exe_shell_cmd(disable_cmd)
     except MySQLSystemdFileNotExists as err:
         logging.info(err)
@@ -223,15 +229,16 @@
     -----------
     MySQLSystemdFileNotExists
     """
     # 如果 systemd 配置文件不存在就报异常
     logging.info(messages.FUN_STARTS.format(fname()))
 
     try:
-        check_mysql_systemd_exists(port)
+        # check_mysql_systemd_exists(port)
+        assert_mysql_systemd_file_exists(port)
         # 没有报异常，说明 systemd 配置存在
         # 执行 start 操作
         start_cmd = "systemctl start mysqld-{}".format(port)
         logging.info(messages.EXECUTE_CMD.format(start_cmd))
         exe_shell_cmd(start_cmd)
     except MySQLSystemdFileNotExists as err:
         raise err
@@ -255,15 +262,16 @@
     -----------
     MySQLSystemdFileNotExists
     """
     # 如果 systemd 配置文件不存在就报异常
     logging.info(messages.FUN_STARTS.format(fname()))
 
     try:
-        check_mysql_systemd_exists(port)
+        # check_mysql_systemd_exists(port)
+        assert_mysql_systemd_file_exists(port)
         # 没有报异常，说明 systemd 配置存在
         # 执行 stop 操作
         stop_cmd = "systemctl stop mysqld-{}".format(port)
         logging.info(messages.EXECUTE_CMD.format(stop_cmd))
         exe_shell_cmd(stop_cmd)
     except MySQLSystemdFileNotExists as err:
         raise err
@@ -281,36 +289,16 @@
 
     Return:
     -------
         None
     """
     logging.info(messages.FUN_STARTS.format(fname()))
 
-    # 创建用户
-    user = MySQLUser(port)
-    user.create()
-
-    # 创建 datadir & binlogdir
-    datadir = Path(dbm_agent_config.mysql_datadir_parent) / str(port)
-    binlogdir = Path(dbm_agent_config.mysql_binlogdir_parent) / str(port)
-
-    if not datadir.exists():
-        logging.info(messages.CREATE_DIR.format(datadir))
-        os.mkdir(datadir)
-    else:
-        logging.warning(messages.DIR_EXISTS.format(datadir))
-
-    if not binlogdir.exists():
-        logging.info(messages.CREATE_DIR.format(binlogdir))
-        os.mkdir(binlogdir)
-    else:
-        logging.warning(messages.DIR_EXISTS.format(binlogdir))
-
-    user.chown(datadir)
-    user.chown(binlogdir)
+    user = create_os_user_for_mysql(port)
+    create_mysql_dirs(port, user)
 
     logging.info(messages.FUN_ENDS.format(fname()))
 
 
 def backup_dirs(port: int = 3306, suffix=None):
     """备份数据目录和 binlog 目录，如果 suffix 为 None 就用当前时间值
 
@@ -363,15 +351,15 @@
     logging.info(messages.FUN_STARTS.format(fname()))
 
     # 计算 suffix
     if suffix is None:
         suffix = datetime.now().isoformat().replace(":", "-").replace(".", "-")
     datadir = Path(dbm_agent_config.mysql_datadir_parent) / str(port)
     if not datadir.exists():
-        logging.warn(messages.DIR_NOT_EXISTS.format(datadir))
+        logging.warning(messages.DIR_NOT_EXISTS.format(datadir))
         return
 
     config_file = "/etc/my-{}.cnf".format(port)
     config_backup_file = datadir / "my-{}.cnf-backup-{}".format(port, suffix)
     logging.info(messages.MOVE_FILE_TO.format(config_file, config_backup_file))
 
     # 备份文件
@@ -399,14 +387,17 @@
     """
     logging.info(messages.FUN_STARTS.format(fname()))
 
     if not pkg.exists():
         logging.error(messages.FILE_NOT_EXISTS.format(pkg))
         raise MySQLPkgFileNotExistsException(messages.FILE_NOT_EXISTS.format(pkg))
 
+    # TODO
+    # / 运行加大了测试用例的编写难度
+    # 这个后面改掉
     basedir = pkg_to_basedir(pkg)
     flag_file = basedir / ".dbm-agent-decompression.txt"
     if flag_file.exists():
         logging.info("ends decompression pkg .")
         return
 
     # 准备解压
@@ -444,22 +435,22 @@
     logging.info(messages.FUN_STARTS.format(fname()))
     logging.info(
         "basedir = '{}', port = '{}', innodb_buffer_pool_size = '{}' .".format(
             basedir, port, innodb_buffer_pool_size
         )
     )
 
-    config = MySQLConfig(
-        basedir=str(basedir), port=port, innodb_buffer_pool_size=innodb_buffer_pool_size
+    config = MySQLSRConfig(
+        port=port, basedir=basedir, innodb_buffer_pool_size=innodb_buffer_pool_size
     )
+    config.save()
+    config.save_init_cnf()
 
-    config.calcu_second_attrs()
-    config.generate_cnf_config_file()
-    config.generate_init_cnf_config_file()
-    config.generate_systemd_cnf_config()
+    sysconfig = MySQLSystemdConfig(config.port, config.basedir, config.user)
+    sysconfig.save()
 
     logging.info(messages.FUN_ENDS.format(fname()))
 
 
 def init_mysql(port: int = 3306, basedir: Path = None):
     """初始化 MySQL
 
@@ -526,34 +517,29 @@
         logging.error("instance has been installed {} .".format(err))
         raise err
     except Exception as err:
         logging.info("unknown Exception {}".format(err))
         raise err
 
     version = get_mysql_version(pkg.name)
-    basedir = pkg_to_basedir(pkg)
 
     # 第一步 创建用户和目录
     create_user_and_dirs(port)
 
     # 第二步 解压安装包
     decompression_pkg(pkg)
 
     # 第三步 计算 basedir
     basedir = pkg_to_basedir(pkg)
 
-    # TODO 清理掉 read_only 参数
     # 第四步 创建配置文件
     create_mysql_config_file(
         port=port, basedir=basedir, innodb_buffer_pool_size=innodb_buffer_pool_size
     )
 
-    # 第五步 复制 init 文件
-    create_init_sql_file(version)
-
     # 第五步 初始化 mysql 实例
     init_mysql(port=port, basedir=basedir)
 
     # 第六步 启用 mysqld 服务
     enable_systemd_for_mysql(port)
 
     # 第七步 启动 mysql 实例
@@ -565,15 +551,15 @@
     # 第九步 导出头文件
     export_header_files(pkg)
 
     # 第十步 导出 so 文件
     export_so_files(pkg)
 
     # 清理 init-sql
-    remove_init_sql_file()
+    # remove_init_sql_file()
 
     logging.info(messages.FUN_ENDS.format(fname()))
 
 
 def uninstall_mysql(port: int = 3306):
     """卸载 mysql 数据库
```

### Comparing `dbm-agent-8.33.9/dbma/components/mysql/instance.py` & `dbm-agent-8.34.0/dbma/components/mysql/instance.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/mysql/replica.py` & `dbm-agent-8.34.0/dbma/components/mysql/replica.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/mysql/source.py` & `dbm-agent-8.34.0/dbma/components/mysql/source.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/mysql/views/defaultsview.py` & `dbm-agent-8.34.0/dbma/components/mysql/views/defaultsview.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/mysql/views/handlers.py` & `dbm-agent-8.34.0/dbma/components/mysql/views/handlers.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/orchestrator/install.py` & `dbm-agent-8.34.0/dbma/components/orchestrator/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/redis/commons.py` & `dbm-agent-8.34.0/dbma/components/redis/commons.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/redis/config.py` & `dbm-agent-8.34.0/dbma/components/redis/config.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/components/redis/install.py` & `dbm-agent-8.34.0/dbma/components/redis/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 from dbma.core import messages
 from dbma.bil.fun import fname
 from dbma.bil.osuser import RedisUser
 from dbma.components.redis.exceptions import (
     RedisDatabaseDirectoryExistsException,
     RedisPkgFileNotExistsException,
 )
-from dbma.components.redis.commons import (
-    default_redis_pkg,
-    redis_pkg_re_pattern,
-    default_redis_port,
-)
+from dbma.components.redis.commons import default_redis_pkg, redis_pkg_re_pattern
 from dbma.bil.cmdexecutor import exe_shell_cmd
 from dbma.components.redis.config import RedisConfig, RedisReplicaConfig
 from dbma.components.redis.systemd import RedisSystemdConfig
 
 
 def create_redis_user(port: int = 6379):
     """创建 redis 用户"""
```

### Comparing `dbm-agent-8.33.9/dbma/components/redis/systemd.py` & `dbm-agent-8.34.0/dbma/components/redis/systemd.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/core/agent/init.py` & `dbm-agent-8.34.0/dbma/core/agent/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
         item = DBM_AGENT_BASE_DIR / subdir
         if not item.exists():
             logging.info("go to create dir {} .".format(item))
             item.mkdir()
 
     # 创建 MySQL+Redis 会用的的一些公共目录
     DATABASE_DIR = Path("/database")
+    if not DATABASE_DIR.exists():
+        DATABASE_DIR.mkdir()
+
     for subdir in ("mysql", "mysql/data", "mysql/binlog", "redis"):
         item = DATABASE_DIR / subdir
         if not item.exists():
             logging.info("go to create dir {} .".format(item))
             item.mkdir()
 
     logging.info("create directions done .")
```

### Comparing `dbm-agent-8.33.9/dbma/core/exception.py` & `dbm-agent-8.34.0/dbma/core/exception.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/core/httpserver.py` & `dbm-agent-8.34.0/dbma/core/httpserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from logging.handlers import RotatingFileHandler
 from dbma.bil.daemon import start_daemon, stop_daemon
 from dbma.bil.osuser import get_uid_gid, is_root, DBMAUser
 from dbma.core.router import routes
 from dbma.core.threads import backends
 from dbma.core.configs import DBMAgentConfig
 from dbma.core.views import dbmagentview as _
+from dbma.components.mysql.backends.clears import start_clear_tasks
 from dbma.components.mysql.views import defaultsview as _
 
 dbm_agent_config = DBMAgentConfig()
 dbm_center_host = urlparse(dbm_agent_config.dbmcenter_url_prefix).hostname
 
 
 # 是否启动 dbmacenter 安全增强
@@ -91,14 +92,15 @@
     logging.info("| start dbm-agent . |")
     logging.info("-" * 21)
     logging.info("logging-level {}".format(dbm_agent_config.log_level))
 
     # 启动后台线程
     logging.info("start backends threads .")
     backends.start_cycle_tasks()
+    start_clear_tasks()
 
     # 启动 http 服务
     logging.info("going to start dbm-agent http-server bind on 0.0.0.0:8086 .")
 
     app = web.Application(middlewares=[enforce_token])
     app.add_routes(routes)
     web.run_app(app, host="0.0.0.0", port=8086, access_log=None)
```

### Comparing `dbm-agent-8.33.9/dbma/core/messages.py` & `dbm-agent-8.34.0/dbma/core/messages.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/core/threads/backends.py` & `dbm-agent-8.34.0/dbma/core/threads/backends.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/auto-inseption-db.sql` & `dbm-agent-8.34.0/dbma/static/cnfs/auto-inseption-db.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/init-5.7.x.sql` & `dbm-agent-8.34.0/dbma/static/cnfs/init-5.7.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/init-8.0.x.sql` & `dbm-agent-8.34.0/dbma/static/cnfs/init-8.0.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/init-users.sql.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/init-users.sql.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/mysql-5.7-init-only.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/mysql-5.7-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/mysql-5.7.25.cnf.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/mysql-5.7.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0-init-only.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.17.cnf.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.30.cnf.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [mysqld]
-# basic
+#### for basic
 user                                     = {{user}}
 basedir                                  = {{basedir}}
 datadir                                  = {{datadir}}
 server_id                                = {{server_id}}
 port                                     = {{port}}
 bind_address                             = {{bind_address}}
 admin_address                            = {{admin_address}}
 mysqlx_port                              = {{mysqlx_port}}
 admin_port                               = {{admin_port}}
 socket                                   = {{socket}}
 mysqlx_socket                            = {{mysqlx_socket}}
 pid_file                                 = {{pid_file}}  
-character_set_server                     = {{character_set_server}}
+character_set_server                     = utf8mb4
 open_files_limit                         = {{open_files_limit}}
 max_prepared_stmt_count                  = {{max_prepared_stmt_count}}  
 skip_name_resolve                        = {{skip_name_resolve}}     
 super_read_only                          = {{super_read_only}}
 log_timestamps                           = {{log_timestamps}}
 event_scheduler                          = {{event_scheduler}}
 auto_generate_certs                      = {{auto_generate_certs}}
@@ -24,49 +24,60 @@
 end_markers_in_json                      = {{end_markers_in_json}}
 tmpdir                                   = {{tmpdir}}
 max_connections                          = {{max_connections}}
 autocommit                               = {{autocommit}}
 sort_buffer_size                         = {{sort_buffer_size}}
 join_buffer_size                         = {{join_buffer_size}}
 eq_range_index_dive_limit                = {{eq_range_index_dive_limit}}
+authentication_policy                    = '*,*,*'
+show_gipk_in_create_table_and_information_schema = {{show_gipk_in_create_table_and_information_schema}}
 
-## table 
+
+#### for table 
 big_tables                               = {{big_tables}}
 sql_require_primary_key                  = {{sql_require_primary_key}}
 lower_case_table_names                   = {{lower_case_table_names}}
 auto_increment_increment                 = {{auto_increment_increment}}
 auto_increment_offset                    = {{auto_increment_offset}}
 table_open_cache                         = {{table_open_cache}}
 table_definition_cache                   = {{table_definition_cache}}
 table_open_cache_instances               = {{table_open_cache_instances}}
 
-## net 
+
+#### for net 
 max_allowed_packet                       = {{max_allowed_packet}}
 connect_timeout                          = {{connect_timeout}}
 interactive_timeout                      = {{interactive_timeout}}
 net_read_timeout                         = {{net_read_timeout}}
 net_retry_count                          = {{net_retry_count}}
 net_write_timeout                        = {{net_write_timeout}}
 net_buffer_length                        = {{net_buffer_length}}
 
-## logs 
+
+#### for logs 
 log_output                               = {{log_output}}
 general_log                              = {{general_log}}
 general_log_file                         = {{general_log_file}}
-# error
+
+
+## error
 log_error                                = {{log_error}}
 log_statements_unsafe_for_binlog         = {{log_statements_unsafe_for_binlog}}
-# slow
+
+
+## for slow
 slow_query_log                           = {{slow_query_log}}
 slow_query_log_file                      = {{slow_query_log_file}}
 long_query_time                          = {{long_query_time}}
 log_queries_not_using_indexes            = {{log_queries_not_using_indexes}}
 log_slow_admin_statements                = {{log_slow_admin_statements}}
-log_slow_slave_statements                = {{log_slow_slave_statements}}
-# binlog
+log_slow_replica_statements              = ON
+
+
+## for binlog
 log_bin                                  = {{log_bin }}
 binlog_checksum                          = {{binlog_checksum}}
 log_bin_trust_function_creators          = {{log_bin_trust_function_creators}}
 binlog_direct_non_transactional_updates  = {{binlog_direct_non_transactional_updates}}
 binlog_expire_logs_seconds               = {{binlog_expire_logs_seconds}}
 binlog_error_action                      = {{binlog_error_action}}
 binlog_format                            = {{binlog_format}}
@@ -74,62 +85,64 @@
 max_binlog_cache_size                    = {{max_binlog_cache_size}}
 max_binlog_size                          = {{max_binlog_size}}
 binlog_order_commits                     = {{binlog_order_commits}}
 binlog_row_image                         = {{binlog_row_image}}
 binlog_row_metadata                      = {{binlog_row_metadata}}
 binlog_rows_query_log_events             = {{binlog_rows_query_log_events}}
 binlog_stmt_cache_size                   = {{binlog_stmt_cache_size}}
-log_slave_updates                        = {{log_slave_updates}}
+log_replica_updates                      = ON
+binlog_transaction_compression           = {{binlog_transaction_compression}}
 binlog_transaction_dependency_history_size ={{binlog_transaction_dependency_history_size}}
 binlog_transaction_dependency_tracking   = {{binlog_transaction_dependency_tracking}}
 sync_binlog                              = {{sync_binlog}}
 binlog_cache_size                        = {{binlog_cache_size}}
 binlog_group_commit_sync_delay           = {{binlog_group_commit_sync_delay}}
 binlog_group_commit_sync_no_delay_count  = {{binlog_group_commit_sync_no_delay_count}}
 
-## replication
+
+#### for replication
 rpl_semi_sync_master_enabled             = {{rpl_semi_sync_master_enabled}}
 rpl_semi_sync_slave_enabled              = {{rpl_semi_sync_slave_enabled}}
 rpl_semi_sync_master_timeout             = {{rpl_semi_sync_master_timeout}}
 rpl_semi_sync_master_wait_point          = {{rpl_semi_sync_master_wait_point}}
 rpl_semi_sync_master_wait_no_slave       = {{rpl_semi_sync_master_wait_no_slave}}
 rpl_semi_sync_master_wait_for_slave_count = {{rpl_semi_sync_master_wait_for_slave_count}}
-master_info_repository                   = {{master_info_repository}}
-sync_master_info                         = {{sync_master_info}}
-skip_slave_start                         = {{skip_slave_start}}
-slave_load_tmpdir                        = {{slave_load_tmpdir}}
+sync_source_info                         = 1000
+skip_replica_start                       = ON
+replica_load_tmpdir                      = /tmp/
 plugin_load_add                          = semisync_master.so
 plugin_load_add                          = semisync_slave.so
 relay_log                                = {{relay_log}}
 sync_relay_log                           = {{sync_relay_log}}
 sync_relay_log_info                      = {{sync_relay_log_info}}
-relay_log_info_repository                = {{relay_log_info_repository}}
-slave_preserve_commit_order              = {{slave_preserve_commit_order}}
-slave_parallel_type                      = {{slave_parallel_type}}
-slave_parallel_workers                   = {{slave_parallel_workers}}
-slave_max_allowed_packet                 = {{slave_max_allowed_packet}}
-
+slave_preserve_commit_order              = ON
+replica_parallel_type                    = LOGICAL_CLOCK
+replica_parallel_workers                  = {{replica_parallel_workers}}
+replica_max_allowed_packet               = {{replica_max_allowed_packet}}
 
 
-## gtid
+#### for gtid
 gtid_mode                                = {{gtid_mode}}
 binlog_gtid_simple_recovery              = {{binlog_gtid_simple_recovery}}
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
-## clone 
+
+#### for clone 
 plugin-load-add                          = mysql_clone.so
-clone                                    = FORCE_PLUS_PERMANEN
+clone                                    = FORCE_PLUS_PERMANENT
+
 
-# engines 
+#### for engines 
 default_storage_engine                   = {{default_storage_engine}}
 default_tmp_storage_engine               = {{default_tmp_storage_engine}}
 internal_tmp_mem_storage_engine          = {{internal_tmp_mem_storage_engine}}
 
-## innodb
+
+#### for innodb
 innodb_data_home_dir                     = {{innodb_data_home_dir}}
 innodb_data_file_path                    = {{innodb_data_file_path}}
 innodb_page_size                         = {{innodb_page_size}}
 innodb_default_row_format                = {{innodb_default_row_format}}
 innodb_log_group_home_dir                = {{innodb_log_group_home_dir}}
 innodb_redo_log_encrypt                  = {{innodb_redo_log_encrypt}}
 innodb_online_alter_log_max_size         = {{innodb_online_alter_log_max_size}}
@@ -206,33 +219,35 @@
 innodb_page_cleaners                     = {{innodb_page_cleaners}}
 innodb_adaptive_hash_index               = {{innodb_adaptive_hash_index}}
 innodb_adaptive_hash_index_parts         = {{innodb_adaptive_hash_index_parts}}
 innodb_flush_log_at_timeout              = {{innodb_flush_log_at_timeout}}
 innodb_fsync_threshold                   = {{innodb_fsync_threshold}}
 innodb_fill_factor                       = {{innodb_fill_factor}}
 innodb_file_per_table                    = {{innodb_file_per_table}}
+sql_generate_invisible_primary_key       = {{sql_generate_invisible_primary_key}} 
 innodb_autoextend_increment              = {{innodb_autoextend_increment}}
 innodb_open_files                        = {{innodb_open_files}}
 innodb_buffer_pool_chunk_size            = {{innodb_buffer_pool_chunk_size}}
 innodb_buffer_pool_instances             = {{innodb_buffer_pool_instances}}
 innodb_log_files_in_group                = {{innodb_log_files_in_group}}
 innodb_log_file_size                     = {{innodb_log_file_size}}
+innodb_redo_log_capacity                 = {{innodb_redo_log_capacity}}
 innodb_flush_neighbors                   = {{innodb_flush_neighbors}}
 innodb_io_capacity                       = {{innodb_io_capacity}}
 innodb_io_capacity_max                   = {{innodb_io_capacity_max}}
 innodb_autoinc_lock_mode                 = {{innodb_autoinc_lock_mode}}
 innodb_change_buffer_max_size            = {{innodb_change_buffer_max_size}}
 innodb_flush_method                      = {{innodb_flush_method}}
 innodb_log_buffer_size                   = {{innodb_log_buffer_size}}
 innodb_flush_log_at_trx_commit           = {{innodb_flush_log_at_trx_commit}}
 innodb_buffer_pool_size                  = {{innodb_buffer_pool_size}}
 
 
 {% if is_mgr %}
-## group replication
+#### for group replication
 plugin_load_add                                    = group_replication.so
 group_replication_recovery_use_ssl                 = {{group_replication_recovery_use_ssl}}
 group_replication_ssl_mode                         = {{group_replication_ssl_mode}}
 group_replication_single_primary_mode              = {{group_replication_single_primary_mode}}
 group_replication_group_name                       = {{group_replication_group_name}}
 group_replication_start_on_boot                    = {{group_replication_start_on_boot}}
 group_replication_bootstrap_group                  = {{group_replication_bootstrap_group}}
@@ -265,21 +280,13 @@
 performance_schema_consumer_events_statements_history_long              =OFF 
 performance_schema_consumer_events_waits_current                        =ON  
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
-
-
-
-
-
-
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
-# base on mysql-8.0.17 
-# generated by https://www.sqlpy.com 2019年09月12日 10:29
+# base on mysql-8.0.30
+# generated by https://www.sqlpy.com 2022年09月16日 23:45
 # wechat: jianglegege
 # email: 1721900707@qq.com
-# -- ~ _ ~ --
-
-
+# -- ~ _ ~ --
```

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.18.cnf.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.31.cnf.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [mysqld]
-# basic
+#### for basic
 user                                     = {{user}}
 basedir                                  = {{basedir}}
 datadir                                  = {{datadir}}
 server_id                                = {{server_id}}
 port                                     = {{port}}
 bind_address                             = {{bind_address}}
 admin_address                            = {{admin_address}}
 mysqlx_port                              = {{mysqlx_port}}
 admin_port                               = {{admin_port}}
 socket                                   = {{socket}}
 mysqlx_socket                            = {{mysqlx_socket}}
 pid_file                                 = {{pid_file}}  
-character_set_server                     = {{character_set_server}}
+character_set_server                     = utf8mb4
 open_files_limit                         = {{open_files_limit}}
 max_prepared_stmt_count                  = {{max_prepared_stmt_count}}  
 skip_name_resolve                        = {{skip_name_resolve}}     
 super_read_only                          = {{super_read_only}}
 log_timestamps                           = {{log_timestamps}}
 event_scheduler                          = {{event_scheduler}}
 auto_generate_certs                      = {{auto_generate_certs}}
@@ -24,120 +24,145 @@
 end_markers_in_json                      = {{end_markers_in_json}}
 tmpdir                                   = {{tmpdir}}
 max_connections                          = {{max_connections}}
 autocommit                               = {{autocommit}}
 sort_buffer_size                         = {{sort_buffer_size}}
 join_buffer_size                         = {{join_buffer_size}}
 eq_range_index_dive_limit                = {{eq_range_index_dive_limit}}
+authentication_policy                    = '*,*,*'
+show_gipk_in_create_table_and_information_schema = {{show_gipk_in_create_table_and_information_schema}}
 
-## table 
+
+#### for table 
 big_tables                               = {{big_tables}}
 sql_require_primary_key                  = {{sql_require_primary_key}}
 lower_case_table_names                   = {{lower_case_table_names}}
 auto_increment_increment                 = {{auto_increment_increment}}
 auto_increment_offset                    = {{auto_increment_offset}}
 table_open_cache                         = {{table_open_cache}}
 table_definition_cache                   = {{table_definition_cache}}
 table_open_cache_instances               = {{table_open_cache_instances}}
 
-## net 
+
+#### for net 
 max_allowed_packet                       = {{max_allowed_packet}}
 connect_timeout                          = {{connect_timeout}}
 interactive_timeout                      = {{interactive_timeout}}
 net_read_timeout                         = {{net_read_timeout}}
 net_retry_count                          = {{net_retry_count}}
 net_write_timeout                        = {{net_write_timeout}}
 net_buffer_length                        = {{net_buffer_length}}
 
-## logs 
+
+#### for logs 
 log_output                               = {{log_output}}
 general_log                              = {{general_log}}
 general_log_file                         = {{general_log_file}}
-# error
+
+
+## error
 log_error                                = {{log_error}}
 log_statements_unsafe_for_binlog         = {{log_statements_unsafe_for_binlog}}
-# slow
+
+
+## for slow
 slow_query_log                           = {{slow_query_log}}
 slow_query_log_file                      = {{slow_query_log_file}}
 long_query_time                          = {{long_query_time}}
 log_queries_not_using_indexes            = {{log_queries_not_using_indexes}}
 log_slow_admin_statements                = {{log_slow_admin_statements}}
-log_slow_slave_statements                = {{log_slow_slave_statements}}
-# binlog
-log_bin                                  = {{log_bin }}
-binlog_checksum                          = {{binlog_checksum}}
-log_bin_trust_function_creators          = {{log_bin_trust_function_creators}}
-binlog_direct_non_transactional_updates  = {{binlog_direct_non_transactional_updates}}
-binlog_expire_logs_seconds               = {{binlog_expire_logs_seconds}}
-binlog_error_action                      = {{binlog_error_action}}
-binlog_format                            = {{binlog_format}}
-max_binlog_stmt_cache_size               = {{max_binlog_stmt_cache_size}}
-max_binlog_cache_size                    = {{max_binlog_cache_size}}
-max_binlog_size                          = {{max_binlog_size}}
-binlog_order_commits                     = {{binlog_order_commits}}
-binlog_row_image                         = {{binlog_row_image}}
-binlog_row_metadata                      = {{binlog_row_metadata}}
-binlog_rows_query_log_events             = {{binlog_rows_query_log_events}}
-binlog_stmt_cache_size                   = {{binlog_stmt_cache_size}}
-log_slave_updates                        = {{log_slave_updates}}
-binlog_transaction_dependency_history_size ={{binlog_transaction_dependency_history_size}}
-binlog_transaction_dependency_tracking   = {{binlog_transaction_dependency_tracking}}
-sync_binlog                              = {{sync_binlog}}
-binlog_cache_size                        = {{binlog_cache_size}}
-binlog_group_commit_sync_delay           = {{binlog_group_commit_sync_delay}}
-binlog_group_commit_sync_no_delay_count  = {{binlog_group_commit_sync_no_delay_count}}
-
-## replication
-rpl_semi_sync_master_enabled             = {{rpl_semi_sync_master_enabled}}
-rpl_semi_sync_slave_enabled              = {{rpl_semi_sync_slave_enabled}}
-rpl_semi_sync_master_timeout             = {{rpl_semi_sync_master_timeout}}
-rpl_semi_sync_master_wait_point          = {{rpl_semi_sync_master_wait_point}}
-rpl_semi_sync_master_wait_no_slave       = {{rpl_semi_sync_master_wait_no_slave}}
-rpl_semi_sync_master_wait_for_slave_count = {{rpl_semi_sync_master_wait_for_slave_count}}
-master_info_repository                   = {{master_info_repository}}
-sync_master_info                         = {{sync_master_info}}
-skip_slave_start                         = {{skip_slave_start}}
-slave_load_tmpdir                        = {{slave_load_tmpdir}}
-plugin_load_add                          = semisync_master.so
-plugin_load_add                          = semisync_slave.so
-relay_log                                = {{relay_log}}
-sync_relay_log                           = {{sync_relay_log}}
-sync_relay_log_info                      = {{sync_relay_log_info}}
-relay_log_info_repository                = {{relay_log_info_repository}}
-slave_preserve_commit_order              = {{slave_preserve_commit_order}}
-slave_parallel_type                      = {{slave_parallel_type}}
-slave_parallel_workers                   = {{slave_parallel_workers}}
-slave_max_allowed_packet                 = {{slave_max_allowed_packet}}
+log_slow_replica_statements              = ON
 
 
+## for binlog
+log_bin                                    = {{log_bin }}
+binlog_checksum                            = {{binlog_checksum}}
+log_bin_trust_function_creators            = {{log_bin_trust_function_creators}}
+binlog_direct_non_transactional_updates    = {{binlog_direct_non_transactional_updates}}
+binlog_expire_logs_seconds                 = {{binlog_expire_logs_seconds}}
+binlog_error_action                        = {{binlog_error_action}}
+binlog_format                              = {{binlog_format}}
+max_binlog_stmt_cache_size                 = {{max_binlog_stmt_cache_size}}
+max_binlog_cache_size                      = {{max_binlog_cache_size}}
+max_binlog_size                            = {{max_binlog_size}}
+binlog_order_commits                       = {{binlog_order_commits}}
+binlog_row_image                           = {{binlog_row_image}}
+binlog_row_metadata                        = {{binlog_row_metadata}}
+binlog_rows_query_log_events               = {{binlog_rows_query_log_events}}
+binlog_stmt_cache_size                     = {{binlog_stmt_cache_size}}
+log_replica_updates                        = ON
+binlog_transaction_compression             = {{binlog_transaction_compression}}
+binlog_transaction_dependency_history_size = {{binlog_transaction_dependency_history_size}}
+binlog_transaction_dependency_tracking     = {{binlog_transaction_dependency_tracking}}
+transaction_write_set_extraction           = {{transaction_write_set_extraction}}
+sync_binlog                                = {{sync_binlog}}
+binlog_cache_size                          = {{binlog_cache_size}}
+binlog_group_commit_sync_delay             = {{binlog_group_commit_sync_delay}}
+binlog_group_commit_sync_no_delay_count    = {{binlog_group_commit_sync_no_delay_count}}
+
+
+#### for replication
+rpl_semi_sync_master_enabled              = {{rpl_semi_sync_master_enabled}}
+rpl_semi_sync_slave_enabled               = {{rpl_semi_sync_slave_enabled}}
+rpl_semi_sync_master_timeout              = {{rpl_semi_sync_master_timeout}}
+rpl_semi_sync_master_wait_point           = {{rpl_semi_sync_master_wait_point}}
+rpl_semi_sync_master_wait_no_slave        = {{rpl_semi_sync_master_wait_no_slave}}
+rpl_semi_sync_master_wait_for_slave_count = {{rpl_semi_sync_master_wait_for_slave_count}}
+sync_source_info                          = 1000
+skip_replica_start                        = ON
+replica_load_tmpdir                       = /tmp/
+plugin_load_add                           = semisync_master.so
+plugin_load_add                           = semisync_slave.so
+relay_log                                 = {{relay_log}}
+sync_relay_log                            = {{sync_relay_log}}
+sync_relay_log_info                       = {{sync_relay_log_info}}
+replica_preserve_commit_order             = ON
+#replica_parallel_type                    = LOGICAL_CLOCK          # deprecated from 8.0.29
+replica_parallel_workers                  = {{replica_parallel_workers}}
+replica_max_allowed_packet                = {{replica_max_allowed_packet}}
 
-## gtid
+
+#### for gtid
 gtid_mode                                = {{gtid_mode}}
 binlog_gtid_simple_recovery              = {{binlog_gtid_simple_recovery}}
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
-## clone 
+
+#### for clone 
 plugin-load-add                          = mysql_clone.so
-clone                                    = FORCE_PLUS_PERMANEN
+clone                                    = FORCE_PLUS_PERMANENT
+clone_autotune_concurrency                = {{ clone_autotune_concurrency}}
+clone_buffer_size                         = {{ clone_buffer_size}}
+clone_block_ddl                           = {{ clone_block_ddl}}
+clone_delay_after_data_drop               = {{ clone_delay_after_data_drop}}
+clone_ddl_timeout                         = {{ clone_ddl_timeout}}
+clone_donor_timeout_after_network_failure = {{ clone_donor_timeout_after_network_failure}}
+clone_enable_compression                  = {{ clone_enable_compression}}
+clone_max_concurrency                     = {{ clone_max_concurrency}}
+clone_max_data_bandwidth                  = {{ clone_max_data_bandwidth}}
+clone_max_network_bandwidth               = {{ clone_max_network_bandwidth}}
+clone_valid_donor_list                    = {{ clone_valid_donor_list}}
 
-# engines 
+
+#### for engines 
 default_storage_engine                   = {{default_storage_engine}}
 default_tmp_storage_engine               = {{default_tmp_storage_engine}}
 internal_tmp_mem_storage_engine          = {{internal_tmp_mem_storage_engine}}
 
-## innodb
+
+#### for innodb
 innodb_data_home_dir                     = {{innodb_data_home_dir}}
 innodb_data_file_path                    = {{innodb_data_file_path}}
 innodb_page_size                         = {{innodb_page_size}}
 innodb_default_row_format                = {{innodb_default_row_format}}
-innodb_log_group_home_dir                = {{innodb_log_group_home_dir}}
 innodb_redo_log_encrypt                  = {{innodb_redo_log_encrypt}}
 innodb_online_alter_log_max_size         = {{innodb_online_alter_log_max_size}}
-innodb_undo_directory                    = {{innodb_undo_directory}}
+#innodb_log_group_home_dir               = {{innodb_log_group_home_dir}}
+#innodb_undo_directory                   = {{innodb_undo_directory}}
 innodb_undo_log_encrypt                  = {{innodb_undo_log_encrypt}}
 innodb_undo_log_truncate                 = {{innodb_undo_log_truncate}}
 innodb_max_undo_log_size                 = {{innodb_max_undo_log_size}}
 innodb_rollback_on_timeout               = {{innodb_rollback_on_timeout}}
 innodb_rollback_segments                 = {{innodb_rollback_segments}}
 innodb_log_checksums                     = {{innodb_log_checksums}}
 innodb_checksum_algorithm                = {{innodb_checksum_algorithm}}
@@ -196,43 +221,45 @@
 innodb_disable_sort_file_cache           = {{innodb_disable_sort_file_cache}}
 innodb_numa_interleave                   = {{innodb_numa_interleave}}
 innodb_strict_mode                       = {{innodb_strict_mode}}
 innodb_sort_buffer_size                  = {{innodb_sort_buffer_size}}
 innodb_fast_shutdown                     = {{innodb_fast_shutdown}}
 innodb_force_load_corrupted              = {{innodb_force_load_corrupted}}
 innodb_force_recovery                    = {{innodb_force_recovery}}
-innodb_temp_tablespaces_dir              = {{innodb_temp_tablespaces_dir}}
+#innodb_temp_tablespaces_dir              = {{innodb_temp_tablespaces_dir}}
 innodb_tmpdir                            = {{innodb_tmpdir}}
 innodb_temp_data_file_path               = {{innodb_temp_data_file_path}}
 innodb_page_cleaners                     = {{innodb_page_cleaners}}
 innodb_adaptive_hash_index               = {{innodb_adaptive_hash_index}}
 innodb_adaptive_hash_index_parts         = {{innodb_adaptive_hash_index_parts}}
 innodb_flush_log_at_timeout              = {{innodb_flush_log_at_timeout}}
 innodb_fsync_threshold                   = {{innodb_fsync_threshold}}
 innodb_fill_factor                       = {{innodb_fill_factor}}
 innodb_file_per_table                    = {{innodb_file_per_table}}
+sql_generate_invisible_primary_key       = {{sql_generate_invisible_primary_key}} 
 innodb_autoextend_increment              = {{innodb_autoextend_increment}}
 innodb_open_files                        = {{innodb_open_files}}
 innodb_buffer_pool_chunk_size            = {{innodb_buffer_pool_chunk_size}}
 innodb_buffer_pool_instances             = {{innodb_buffer_pool_instances}}
-innodb_log_files_in_group                = {{innodb_log_files_in_group}}
-innodb_log_file_size                     = {{innodb_log_file_size}}
+#innodb_log_files_in_group               = {{innodb_log_files_in_group}}
+#innodb_log_file_size                    = {{innodb_log_file_size}}
+innodb_redo_log_capacity                 = {{innodb_redo_log_capacity}}
 innodb_flush_neighbors                   = {{innodb_flush_neighbors}}
 innodb_io_capacity                       = {{innodb_io_capacity}}
 innodb_io_capacity_max                   = {{innodb_io_capacity_max}}
 innodb_autoinc_lock_mode                 = {{innodb_autoinc_lock_mode}}
 innodb_change_buffer_max_size            = {{innodb_change_buffer_max_size}}
 innodb_flush_method                      = {{innodb_flush_method}}
 innodb_log_buffer_size                   = {{innodb_log_buffer_size}}
 innodb_flush_log_at_trx_commit           = {{innodb_flush_log_at_trx_commit}}
 innodb_buffer_pool_size                  = {{innodb_buffer_pool_size}}
 
 
 {% if is_mgr %}
-## group replication
+#### for group replication
 plugin_load_add                                    = group_replication.so
 group_replication_recovery_use_ssl                 = {{group_replication_recovery_use_ssl}}
 group_replication_ssl_mode                         = {{group_replication_ssl_mode}}
 group_replication_single_primary_mode              = {{group_replication_single_primary_mode}}
 group_replication_group_name                       = {{group_replication_group_name}}
 group_replication_start_on_boot                    = {{group_replication_start_on_boot}}
 group_replication_bootstrap_group                  = {{group_replication_bootstrap_group}}
@@ -265,21 +292,14 @@
 performance_schema_consumer_events_statements_history_long              =OFF 
 performance_schema_consumer_events_waits_current                        =ON  
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
-
-
-
-
-
-
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
-# base on mysql-8.0.18 
-# generated by https://www.sqlpy.com 2019年10月14日 21时47分11秒
+# base on mysql-8.0.31
+# generated by https://www.sqlpy.com 2022年11月11日 23:45
 # wechat: jianglegege
 # email: 1721900707@qq.com
 # -- ~ _ ~ --
-
-
+
```

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.19.cnf.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.32.cnf.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 bind_address                             = {{bind_address}}
 admin_address                            = {{admin_address}}
 mysqlx_port                              = {{mysqlx_port}}
 admin_port                               = {{admin_port}}
 socket                                   = {{socket}}
 mysqlx_socket                            = {{mysqlx_socket}}
 pid_file                                 = {{pid_file}}  
-character_set_server                     = {{character_set_server}}
+character_set_server                     = utf8mb4
 open_files_limit                         = {{open_files_limit}}
 max_prepared_stmt_count                  = {{max_prepared_stmt_count}}  
 skip_name_resolve                        = {{skip_name_resolve}}     
 super_read_only                          = {{super_read_only}}
 log_timestamps                           = {{log_timestamps}}
 event_scheduler                          = {{event_scheduler}}
 auto_generate_certs                      = {{auto_generate_certs}}
@@ -24,120 +24,145 @@
 end_markers_in_json                      = {{end_markers_in_json}}
 tmpdir                                   = {{tmpdir}}
 max_connections                          = {{max_connections}}
 autocommit                               = {{autocommit}}
 sort_buffer_size                         = {{sort_buffer_size}}
 join_buffer_size                         = {{join_buffer_size}}
 eq_range_index_dive_limit                = {{eq_range_index_dive_limit}}
+authentication_policy                    = '*,*,*'
+show_gipk_in_create_table_and_information_schema = {{show_gipk_in_create_table_and_information_schema}}
+
 
 #### for table 
 big_tables                               = {{big_tables}}
 sql_require_primary_key                  = {{sql_require_primary_key}}
 lower_case_table_names                   = {{lower_case_table_names}}
 auto_increment_increment                 = {{auto_increment_increment}}
 auto_increment_offset                    = {{auto_increment_offset}}
 table_open_cache                         = {{table_open_cache}}
 table_definition_cache                   = {{table_definition_cache}}
 table_open_cache_instances               = {{table_open_cache_instances}}
 
+
 #### for net 
 max_allowed_packet                       = {{max_allowed_packet}}
 connect_timeout                          = {{connect_timeout}}
 interactive_timeout                      = {{interactive_timeout}}
 net_read_timeout                         = {{net_read_timeout}}
 net_retry_count                          = {{net_retry_count}}
 net_write_timeout                        = {{net_write_timeout}}
 net_buffer_length                        = {{net_buffer_length}}
 
+
 #### for logs 
 log_output                               = {{log_output}}
 general_log                              = {{general_log}}
 general_log_file                         = {{general_log_file}}
+
+
 ## error
 log_error                                = {{log_error}}
 log_statements_unsafe_for_binlog         = {{log_statements_unsafe_for_binlog}}
-## slow
+
+
+## for slow
 slow_query_log                           = {{slow_query_log}}
 slow_query_log_file                      = {{slow_query_log_file}}
 long_query_time                          = {{long_query_time}}
 log_queries_not_using_indexes            = {{log_queries_not_using_indexes}}
 log_slow_admin_statements                = {{log_slow_admin_statements}}
-log_slow_slave_statements                = {{log_slow_slave_statements}}
-## binlog
-log_bin                                  = {{log_bin }}
-binlog_checksum                          = {{binlog_checksum}}
-log_bin_trust_function_creators          = {{log_bin_trust_function_creators}}
-binlog_direct_non_transactional_updates  = {{binlog_direct_non_transactional_updates}}
-binlog_expire_logs_seconds               = {{binlog_expire_logs_seconds}}
-binlog_error_action                      = {{binlog_error_action}}
-binlog_format                            = {{binlog_format}}
-max_binlog_stmt_cache_size               = {{max_binlog_stmt_cache_size}}
-max_binlog_cache_size                    = {{max_binlog_cache_size}}
-max_binlog_size                          = {{max_binlog_size}}
-binlog_order_commits                     = {{binlog_order_commits}}
-binlog_row_image                         = {{binlog_row_image}}
-binlog_row_metadata                      = {{binlog_row_metadata}}
-binlog_rows_query_log_events             = {{binlog_rows_query_log_events}}
-binlog_stmt_cache_size                   = {{binlog_stmt_cache_size}}
-log_slave_updates                        = {{log_slave_updates}}
-binlog_transaction_dependency_history_size ={{binlog_transaction_dependency_history_size}}
-binlog_transaction_dependency_tracking   = {{binlog_transaction_dependency_tracking}}
-sync_binlog                              = {{sync_binlog}}
-binlog_cache_size                        = {{binlog_cache_size}}
-binlog_group_commit_sync_delay           = {{binlog_group_commit_sync_delay}}
-binlog_group_commit_sync_no_delay_count  = {{binlog_group_commit_sync_no_delay_count}}
+log_slow_replica_statements              = ON
+
+
+## for binlog
+log_bin                                    = {{log_bin }}
+binlog_checksum                            = {{binlog_checksum}}
+log_bin_trust_function_creators            = {{log_bin_trust_function_creators}}
+binlog_direct_non_transactional_updates    = {{binlog_direct_non_transactional_updates}}
+binlog_expire_logs_seconds                 = {{binlog_expire_logs_seconds}}
+binlog_error_action                        = {{binlog_error_action}}
+binlog_format                              = {{binlog_format}}
+max_binlog_stmt_cache_size                 = {{max_binlog_stmt_cache_size}}
+max_binlog_cache_size                      = {{max_binlog_cache_size}}
+max_binlog_size                            = {{max_binlog_size}}
+binlog_order_commits                       = {{binlog_order_commits}}
+binlog_row_image                           = {{binlog_row_image}}
+binlog_row_metadata                        = {{binlog_row_metadata}}
+binlog_rows_query_log_events               = {{binlog_rows_query_log_events}}
+binlog_stmt_cache_size                     = {{binlog_stmt_cache_size}}
+log_replica_updates                        = ON
+binlog_transaction_compression             = {{binlog_transaction_compression}}
+binlog_transaction_dependency_history_size = {{binlog_transaction_dependency_history_size}}
+binlog_transaction_dependency_tracking     = {{binlog_transaction_dependency_tracking}}
+transaction_write_set_extraction           = {{transaction_write_set_extraction}}
+sync_binlog                                = {{sync_binlog}}
+binlog_cache_size                          = {{binlog_cache_size}}
+binlog_group_commit_sync_delay             = {{binlog_group_commit_sync_delay}}
+binlog_group_commit_sync_no_delay_count    = {{binlog_group_commit_sync_no_delay_count}}
+
 
 #### for replication
-rpl_semi_sync_master_enabled             = {{rpl_semi_sync_master_enabled}}
-rpl_semi_sync_slave_enabled              = {{rpl_semi_sync_slave_enabled}}
-rpl_semi_sync_master_timeout             = {{rpl_semi_sync_master_timeout}}
-rpl_semi_sync_master_wait_point          = {{rpl_semi_sync_master_wait_point}}
-rpl_semi_sync_master_wait_no_slave       = {{rpl_semi_sync_master_wait_no_slave}}
+rpl_semi_sync_master_enabled              = {{rpl_semi_sync_master_enabled}}
+rpl_semi_sync_slave_enabled               = {{rpl_semi_sync_slave_enabled}}
+rpl_semi_sync_master_timeout              = {{rpl_semi_sync_master_timeout}}
+rpl_semi_sync_master_wait_point           = {{rpl_semi_sync_master_wait_point}}
+rpl_semi_sync_master_wait_no_slave        = {{rpl_semi_sync_master_wait_no_slave}}
 rpl_semi_sync_master_wait_for_slave_count = {{rpl_semi_sync_master_wait_for_slave_count}}
-master_info_repository                   = {{master_info_repository}}
-sync_master_info                         = {{sync_master_info}}
-skip_slave_start                         = {{skip_slave_start}}
-slave_load_tmpdir                        = {{slave_load_tmpdir}}
-plugin_load_add                          = semisync_master.so
-plugin_load_add                          = semisync_slave.so
-relay_log                                = {{relay_log}}
-sync_relay_log                           = {{sync_relay_log}}
-sync_relay_log_info                      = {{sync_relay_log_info}}
-relay_log_info_repository                = {{relay_log_info_repository}}
-slave_preserve_commit_order              = {{slave_preserve_commit_order}}
-slave_parallel_type                      = {{slave_parallel_type}}
-slave_parallel_workers                   = {{slave_parallel_workers}}
-slave_max_allowed_packet                 = {{slave_max_allowed_packet}}
-
+sync_source_info                          = 1000
+skip_replica_start                        = ON
+replica_load_tmpdir                       = /tmp/
+plugin_load_add                           = semisync_master.so
+plugin_load_add                           = semisync_slave.so
+relay_log                                 = {{relay_log}}
+sync_relay_log                            = {{sync_relay_log}}
+sync_relay_log_info                       = {{sync_relay_log_info}}
+replica_preserve_commit_order             = ON
+#replica_parallel_type                    = LOGICAL_CLOCK          # deprecated from 8.0.29
+replica_parallel_workers                  = {{replica_parallel_workers}}
+replica_max_allowed_packet                = {{replica_max_allowed_packet}}
 
 
 #### for gtid
 gtid_mode                                = {{gtid_mode}}
 binlog_gtid_simple_recovery              = {{binlog_gtid_simple_recovery}}
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
+
 #### for clone 
-plugin-load-add                          = mysql_clone.so
-clone                                    = FORCE_PLUS_PERMANEN
+plugin-load-add                           = mysql_clone.so
+clone                                     = FORCE_PLUS_PERMANENT
+clone_autotune_concurrency                = {{ clone_autotune_concurrency}}
+clone_buffer_size                         = {{ clone_buffer_size}}
+clone_block_ddl                           = {{ clone_block_ddl}}
+clone_delay_after_data_drop               = {{ clone_delay_after_data_drop}}
+clone_ddl_timeout                         = {{ clone_ddl_timeout}}
+clone_donor_timeout_after_network_failure = {{ clone_donor_timeout_after_network_failure}}
+clone_enable_compression                  = {{ clone_enable_compression}}
+clone_max_concurrency                     = {{ clone_max_concurrency}}
+clone_max_data_bandwidth                  = {{ clone_max_data_bandwidth}}
+clone_max_network_bandwidth               = {{ clone_max_network_bandwidth}}
+clone_valid_donor_list                    = {{ clone_valid_donor_list}}
+
 
 #### for engines 
 default_storage_engine                   = {{default_storage_engine}}
 default_tmp_storage_engine               = {{default_tmp_storage_engine}}
 internal_tmp_mem_storage_engine          = {{internal_tmp_mem_storage_engine}}
 
+
 #### for innodb
 innodb_data_home_dir                     = {{innodb_data_home_dir}}
 innodb_data_file_path                    = {{innodb_data_file_path}}
 innodb_page_size                         = {{innodb_page_size}}
 innodb_default_row_format                = {{innodb_default_row_format}}
-innodb_log_group_home_dir                = {{innodb_log_group_home_dir}}
 innodb_redo_log_encrypt                  = {{innodb_redo_log_encrypt}}
 innodb_online_alter_log_max_size         = {{innodb_online_alter_log_max_size}}
-innodb_undo_directory                    = {{innodb_undo_directory}}
+#innodb_log_group_home_dir               = {{innodb_log_group_home_dir}}
+#innodb_undo_directory                   = {{innodb_undo_directory}}
 innodb_undo_log_encrypt                  = {{innodb_undo_log_encrypt}}
 innodb_undo_log_truncate                 = {{innodb_undo_log_truncate}}
 innodb_max_undo_log_size                 = {{innodb_max_undo_log_size}}
 innodb_rollback_on_timeout               = {{innodb_rollback_on_timeout}}
 innodb_rollback_segments                 = {{innodb_rollback_segments}}
 innodb_log_checksums                     = {{innodb_log_checksums}}
 innodb_checksum_algorithm                = {{innodb_checksum_algorithm}}
@@ -196,30 +221,32 @@
 innodb_disable_sort_file_cache           = {{innodb_disable_sort_file_cache}}
 innodb_numa_interleave                   = {{innodb_numa_interleave}}
 innodb_strict_mode                       = {{innodb_strict_mode}}
 innodb_sort_buffer_size                  = {{innodb_sort_buffer_size}}
 innodb_fast_shutdown                     = {{innodb_fast_shutdown}}
 innodb_force_load_corrupted              = {{innodb_force_load_corrupted}}
 innodb_force_recovery                    = {{innodb_force_recovery}}
-innodb_temp_tablespaces_dir              = {{innodb_temp_tablespaces_dir}}
+#innodb_temp_tablespaces_dir              = {{innodb_temp_tablespaces_dir}}
 innodb_tmpdir                            = {{innodb_tmpdir}}
 innodb_temp_data_file_path               = {{innodb_temp_data_file_path}}
 innodb_page_cleaners                     = {{innodb_page_cleaners}}
 innodb_adaptive_hash_index               = {{innodb_adaptive_hash_index}}
 innodb_adaptive_hash_index_parts         = {{innodb_adaptive_hash_index_parts}}
 innodb_flush_log_at_timeout              = {{innodb_flush_log_at_timeout}}
 innodb_fsync_threshold                   = {{innodb_fsync_threshold}}
 innodb_fill_factor                       = {{innodb_fill_factor}}
 innodb_file_per_table                    = {{innodb_file_per_table}}
+sql_generate_invisible_primary_key       = {{sql_generate_invisible_primary_key}} 
 innodb_autoextend_increment              = {{innodb_autoextend_increment}}
 innodb_open_files                        = {{innodb_open_files}}
 innodb_buffer_pool_chunk_size            = {{innodb_buffer_pool_chunk_size}}
 innodb_buffer_pool_instances             = {{innodb_buffer_pool_instances}}
-innodb_log_files_in_group                = {{innodb_log_files_in_group}}
-innodb_log_file_size                     = {{innodb_log_file_size}}
+#innodb_log_files_in_group               = {{innodb_log_files_in_group}}
+#innodb_log_file_size                    = {{innodb_log_file_size}}
+innodb_redo_log_capacity                 = {{innodb_redo_log_capacity}}
 innodb_flush_neighbors                   = {{innodb_flush_neighbors}}
 innodb_io_capacity                       = {{innodb_io_capacity}}
 innodb_io_capacity_max                   = {{innodb_io_capacity_max}}
 innodb_autoinc_lock_mode                 = {{innodb_autoinc_lock_mode}}
 innodb_change_buffer_max_size            = {{innodb_change_buffer_max_size}}
 innodb_flush_method                      = {{innodb_flush_method}}
 innodb_log_buffer_size                   = {{innodb_log_buffer_size}}
@@ -265,21 +292,14 @@
 performance_schema_consumer_events_statements_history_long              =OFF 
 performance_schema_consumer_events_waits_current                        =ON  
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
-
-
-
-
-
-
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
-# base on mysql-8.0.19
-# generated by https://www.sqlpy.com 2020年1月15日 10:32
+# base on mysql-8.0.32
+# generated by https://www.sqlpy.com at {{now}}
 # wechat: jianglegege
 # email: 1721900707@qq.com
-# -- ~ _ ~ --   
-
-
+# -- ~ _ ~ --
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.20.cnf.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.33.cnf.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 bind_address                             = {{bind_address}}
 admin_address                            = {{admin_address}}
 mysqlx_port                              = {{mysqlx_port}}
 admin_port                               = {{admin_port}}
 socket                                   = {{socket}}
 mysqlx_socket                            = {{mysqlx_socket}}
 pid_file                                 = {{pid_file}}  
-character_set_server                     = {{character_set_server}}
+character_set_server                     = utf8mb4
 open_files_limit                         = {{open_files_limit}}
 max_prepared_stmt_count                  = {{max_prepared_stmt_count}}  
 skip_name_resolve                        = {{skip_name_resolve}}     
 super_read_only                          = {{super_read_only}}
 log_timestamps                           = {{log_timestamps}}
 event_scheduler                          = {{event_scheduler}}
 auto_generate_certs                      = {{auto_generate_certs}}
@@ -24,121 +24,145 @@
 end_markers_in_json                      = {{end_markers_in_json}}
 tmpdir                                   = {{tmpdir}}
 max_connections                          = {{max_connections}}
 autocommit                               = {{autocommit}}
 sort_buffer_size                         = {{sort_buffer_size}}
 join_buffer_size                         = {{join_buffer_size}}
 eq_range_index_dive_limit                = {{eq_range_index_dive_limit}}
+authentication_policy                    = '*,*,*'
+show_gipk_in_create_table_and_information_schema = {{show_gipk_in_create_table_and_information_schema}}
+
 
 #### for table 
 big_tables                               = {{big_tables}}
 sql_require_primary_key                  = {{sql_require_primary_key}}
 lower_case_table_names                   = {{lower_case_table_names}}
 auto_increment_increment                 = {{auto_increment_increment}}
 auto_increment_offset                    = {{auto_increment_offset}}
 table_open_cache                         = {{table_open_cache}}
 table_definition_cache                   = {{table_definition_cache}}
 table_open_cache_instances               = {{table_open_cache_instances}}
 
+
 #### for net 
 max_allowed_packet                       = {{max_allowed_packet}}
 connect_timeout                          = {{connect_timeout}}
 interactive_timeout                      = {{interactive_timeout}}
 net_read_timeout                         = {{net_read_timeout}}
 net_retry_count                          = {{net_retry_count}}
 net_write_timeout                        = {{net_write_timeout}}
 net_buffer_length                        = {{net_buffer_length}}
 
+
 #### for logs 
 log_output                               = {{log_output}}
 general_log                              = {{general_log}}
 general_log_file                         = {{general_log_file}}
+
+
 ## error
 log_error                                = {{log_error}}
 log_statements_unsafe_for_binlog         = {{log_statements_unsafe_for_binlog}}
-## slow
+
+
+## for slow
 slow_query_log                           = {{slow_query_log}}
 slow_query_log_file                      = {{slow_query_log_file}}
 long_query_time                          = {{long_query_time}}
 log_queries_not_using_indexes            = {{log_queries_not_using_indexes}}
 log_slow_admin_statements                = {{log_slow_admin_statements}}
-log_slow_slave_statements                = {{log_slow_slave_statements}}
-## binlog
-log_bin                                  = {{log_bin }}
-binlog_checksum                          = {{binlog_checksum}}
-log_bin_trust_function_creators          = {{log_bin_trust_function_creators}}
-binlog_direct_non_transactional_updates  = {{binlog_direct_non_transactional_updates}}
-binlog_expire_logs_seconds               = {{binlog_expire_logs_seconds}}
-binlog_error_action                      = {{binlog_error_action}}
-binlog_format                            = {{binlog_format}}
-max_binlog_stmt_cache_size               = {{max_binlog_stmt_cache_size}}
-max_binlog_cache_size                    = {{max_binlog_cache_size}}
-max_binlog_size                          = {{max_binlog_size}}
-binlog_order_commits                     = {{binlog_order_commits}}
-binlog_row_image                         = {{binlog_row_image}}
-binlog_row_metadata                      = {{binlog_row_metadata}}
-binlog_rows_query_log_events             = {{binlog_rows_query_log_events}}
-binlog_stmt_cache_size                   = {{binlog_stmt_cache_size}}
-log_slave_updates                        = {{log_slave_updates}}
-binlog_transaction_compression           = {{binlog_transaction_compression}}
-binlog_transaction_dependency_history_size ={{binlog_transaction_dependency_history_size}}
-binlog_transaction_dependency_tracking   = {{binlog_transaction_dependency_tracking}}
-sync_binlog                              = {{sync_binlog}}
-binlog_cache_size                        = {{binlog_cache_size}}
-binlog_group_commit_sync_delay           = {{binlog_group_commit_sync_delay}}
-binlog_group_commit_sync_no_delay_count  = {{binlog_group_commit_sync_no_delay_count}}
+log_slow_replica_statements              = ON
+
+
+## for binlog
+log_bin                                    = {{log_bin }}
+binlog_checksum                            = {{binlog_checksum}}
+log_bin_trust_function_creators            = {{log_bin_trust_function_creators}}
+binlog_direct_non_transactional_updates    = {{binlog_direct_non_transactional_updates}}
+binlog_expire_logs_seconds                 = {{binlog_expire_logs_seconds}}
+binlog_error_action                        = {{binlog_error_action}}
+binlog_format                              = {{binlog_format}}
+max_binlog_stmt_cache_size                 = {{max_binlog_stmt_cache_size}}
+max_binlog_cache_size                      = {{max_binlog_cache_size}}
+max_binlog_size                            = {{max_binlog_size}}
+binlog_order_commits                       = {{binlog_order_commits}}
+binlog_row_image                           = {{binlog_row_image}}
+binlog_row_metadata                        = {{binlog_row_metadata}}
+binlog_rows_query_log_events               = {{binlog_rows_query_log_events}}
+binlog_stmt_cache_size                     = {{binlog_stmt_cache_size}}
+log_replica_updates                        = ON
+binlog_transaction_compression             = {{binlog_transaction_compression}}
+binlog_transaction_dependency_history_size = {{binlog_transaction_dependency_history_size}}
+binlog_transaction_dependency_tracking     = {{binlog_transaction_dependency_tracking}}
+#transaction_write_set_extraction           = {{transaction_write_set_extraction}}
+sync_binlog                                = {{sync_binlog}}
+binlog_cache_size                          = {{binlog_cache_size}}
+binlog_group_commit_sync_delay             = {{binlog_group_commit_sync_delay}}
+binlog_group_commit_sync_no_delay_count    = {{binlog_group_commit_sync_no_delay_count}}
+
 
 #### for replication
-rpl_semi_sync_master_enabled             = {{rpl_semi_sync_master_enabled}}
-rpl_semi_sync_slave_enabled              = {{rpl_semi_sync_slave_enabled}}
-rpl_semi_sync_master_timeout             = {{rpl_semi_sync_master_timeout}}
-rpl_semi_sync_master_wait_point          = {{rpl_semi_sync_master_wait_point}}
-rpl_semi_sync_master_wait_no_slave       = {{rpl_semi_sync_master_wait_no_slave}}
+rpl_semi_sync_master_enabled              = {{rpl_semi_sync_master_enabled}}
+rpl_semi_sync_slave_enabled               = {{rpl_semi_sync_slave_enabled}}
+rpl_semi_sync_master_timeout              = {{rpl_semi_sync_master_timeout}}
+rpl_semi_sync_master_wait_point           = {{rpl_semi_sync_master_wait_point}}
+rpl_semi_sync_master_wait_no_slave        = {{rpl_semi_sync_master_wait_no_slave}}
 rpl_semi_sync_master_wait_for_slave_count = {{rpl_semi_sync_master_wait_for_slave_count}}
-master_info_repository                   = {{master_info_repository}}
-sync_master_info                         = {{sync_master_info}}
-skip_slave_start                         = {{skip_slave_start}}
-slave_load_tmpdir                        = {{slave_load_tmpdir}}
-plugin_load_add                          = semisync_master.so
-plugin_load_add                          = semisync_slave.so
-relay_log                                = {{relay_log}}
-sync_relay_log                           = {{sync_relay_log}}
-sync_relay_log_info                      = {{sync_relay_log_info}}
-relay_log_info_repository                = {{relay_log_info_repository}}
-slave_preserve_commit_order              = {{slave_preserve_commit_order}}
-slave_parallel_type                      = {{slave_parallel_type}}
-slave_parallel_workers                   = {{slave_parallel_workers}}
-slave_max_allowed_packet                 = {{slave_max_allowed_packet}}
-
+sync_source_info                          = 1000
+skip_replica_start                        = ON
+replica_load_tmpdir                       = /tmp/
+plugin_load_add                           = semisync_master.so
+plugin_load_add                           = semisync_slave.so
+relay_log                                 = {{relay_log}}
+sync_relay_log                            = {{sync_relay_log}}
+sync_relay_log_info                       = {{sync_relay_log_info}}
+replica_preserve_commit_order             = ON
+#replica_parallel_type                    = LOGICAL_CLOCK          # deprecated from 8.0.29
+replica_parallel_workers                  = {{replica_parallel_workers}}
+replica_max_allowed_packet                = {{replica_max_allowed_packet}}
 
 
 #### for gtid
 gtid_mode                                = {{gtid_mode}}
 binlog_gtid_simple_recovery              = {{binlog_gtid_simple_recovery}}
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
+
 #### for clone 
-plugin-load-add                          = mysql_clone.so
-clone                                    = FORCE_PLUS_PERMANENT
+plugin-load-add                           = mysql_clone.so
+clone                                     = FORCE_PLUS_PERMANENT
+clone_autotune_concurrency                = {{ clone_autotune_concurrency}}
+clone_buffer_size                         = {{ clone_buffer_size}}
+clone_block_ddl                           = {{ clone_block_ddl}}
+clone_delay_after_data_drop               = {{ clone_delay_after_data_drop}}
+clone_ddl_timeout                         = {{ clone_ddl_timeout}}
+clone_donor_timeout_after_network_failure = {{ clone_donor_timeout_after_network_failure}}
+clone_enable_compression                  = {{ clone_enable_compression}}
+clone_max_concurrency                     = {{ clone_max_concurrency}}
+clone_max_data_bandwidth                  = {{ clone_max_data_bandwidth}}
+clone_max_network_bandwidth               = {{ clone_max_network_bandwidth}}
+clone_valid_donor_list                    = {{ clone_valid_donor_list}}
+
 
 #### for engines 
 default_storage_engine                   = {{default_storage_engine}}
 default_tmp_storage_engine               = {{default_tmp_storage_engine}}
 internal_tmp_mem_storage_engine          = {{internal_tmp_mem_storage_engine}}
 
+
 #### for innodb
 innodb_data_home_dir                     = {{innodb_data_home_dir}}
 innodb_data_file_path                    = {{innodb_data_file_path}}
 innodb_page_size                         = {{innodb_page_size}}
 innodb_default_row_format                = {{innodb_default_row_format}}
-innodb_log_group_home_dir                = {{innodb_log_group_home_dir}}
 innodb_redo_log_encrypt                  = {{innodb_redo_log_encrypt}}
 innodb_online_alter_log_max_size         = {{innodb_online_alter_log_max_size}}
-innodb_undo_directory                    = {{innodb_undo_directory}}
+#innodb_log_group_home_dir               = {{innodb_log_group_home_dir}}
+#innodb_undo_directory                   = {{innodb_undo_directory}}
 innodb_undo_log_encrypt                  = {{innodb_undo_log_encrypt}}
 innodb_undo_log_truncate                 = {{innodb_undo_log_truncate}}
 innodb_max_undo_log_size                 = {{innodb_max_undo_log_size}}
 innodb_rollback_on_timeout               = {{innodb_rollback_on_timeout}}
 innodb_rollback_segments                 = {{innodb_rollback_segments}}
 innodb_log_checksums                     = {{innodb_log_checksums}}
 innodb_checksum_algorithm                = {{innodb_checksum_algorithm}}
@@ -197,30 +221,32 @@
 innodb_disable_sort_file_cache           = {{innodb_disable_sort_file_cache}}
 innodb_numa_interleave                   = {{innodb_numa_interleave}}
 innodb_strict_mode                       = {{innodb_strict_mode}}
 innodb_sort_buffer_size                  = {{innodb_sort_buffer_size}}
 innodb_fast_shutdown                     = {{innodb_fast_shutdown}}
 innodb_force_load_corrupted              = {{innodb_force_load_corrupted}}
 innodb_force_recovery                    = {{innodb_force_recovery}}
-innodb_temp_tablespaces_dir              = {{innodb_temp_tablespaces_dir}}
+#innodb_temp_tablespaces_dir              = {{innodb_temp_tablespaces_dir}}
 innodb_tmpdir                            = {{innodb_tmpdir}}
 innodb_temp_data_file_path               = {{innodb_temp_data_file_path}}
 innodb_page_cleaners                     = {{innodb_page_cleaners}}
 innodb_adaptive_hash_index               = {{innodb_adaptive_hash_index}}
 innodb_adaptive_hash_index_parts         = {{innodb_adaptive_hash_index_parts}}
 innodb_flush_log_at_timeout              = {{innodb_flush_log_at_timeout}}
 innodb_fsync_threshold                   = {{innodb_fsync_threshold}}
 innodb_fill_factor                       = {{innodb_fill_factor}}
 innodb_file_per_table                    = {{innodb_file_per_table}}
+sql_generate_invisible_primary_key       = {{sql_generate_invisible_primary_key}} 
 innodb_autoextend_increment              = {{innodb_autoextend_increment}}
 innodb_open_files                        = {{innodb_open_files}}
 innodb_buffer_pool_chunk_size            = {{innodb_buffer_pool_chunk_size}}
 innodb_buffer_pool_instances             = {{innodb_buffer_pool_instances}}
-innodb_log_files_in_group                = {{innodb_log_files_in_group}}
-innodb_log_file_size                     = {{innodb_log_file_size}}
+#innodb_log_files_in_group               = {{innodb_log_files_in_group}}
+#innodb_log_file_size                    = {{innodb_log_file_size}}
+innodb_redo_log_capacity                 = {{innodb_redo_log_capacity}}
 innodb_flush_neighbors                   = {{innodb_flush_neighbors}}
 innodb_io_capacity                       = {{innodb_io_capacity}}
 innodb_io_capacity_max                   = {{innodb_io_capacity_max}}
 innodb_autoinc_lock_mode                 = {{innodb_autoinc_lock_mode}}
 innodb_change_buffer_max_size            = {{innodb_change_buffer_max_size}}
 innodb_flush_method                      = {{innodb_flush_method}}
 innodb_log_buffer_size                   = {{innodb_log_buffer_size}}
@@ -266,21 +292,13 @@
 performance_schema_consumer_events_statements_history_long              =OFF 
 performance_schema_consumer_events_waits_current                        =ON  
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
-
-
-
-
-
-
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
-# base on mysql-8.0.19
-# generated by https://www.sqlpy.com 2020年1月15日 10:32
+# base on mysql-8.0.33
+# generated by https://www.sqlpy.com at {{now}}
 # wechat: jianglegege
 # email: 1721900707@qq.com
-# -- ~ _ ~ --   
-
-
+# -- ~ _ ~ --
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.21.cnf.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/mysql-8.0.34.cnf.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 bind_address                             = {{bind_address}}
 admin_address                            = {{admin_address}}
 mysqlx_port                              = {{mysqlx_port}}
 admin_port                               = {{admin_port}}
 socket                                   = {{socket}}
 mysqlx_socket                            = {{mysqlx_socket}}
 pid_file                                 = {{pid_file}}  
-character_set_server                     = {{character_set_server}}
+character_set_server                     = utf8mb4
 open_files_limit                         = {{open_files_limit}}
 max_prepared_stmt_count                  = {{max_prepared_stmt_count}}  
 skip_name_resolve                        = {{skip_name_resolve}}     
 super_read_only                          = {{super_read_only}}
 log_timestamps                           = {{log_timestamps}}
 event_scheduler                          = {{event_scheduler}}
 auto_generate_certs                      = {{auto_generate_certs}}
@@ -24,121 +24,145 @@
 end_markers_in_json                      = {{end_markers_in_json}}
 tmpdir                                   = {{tmpdir}}
 max_connections                          = {{max_connections}}
 autocommit                               = {{autocommit}}
 sort_buffer_size                         = {{sort_buffer_size}}
 join_buffer_size                         = {{join_buffer_size}}
 eq_range_index_dive_limit                = {{eq_range_index_dive_limit}}
+authentication_policy                    = '*,*,*'
+show_gipk_in_create_table_and_information_schema = {{show_gipk_in_create_table_and_information_schema}}
+
 
 #### for table 
 big_tables                               = {{big_tables}}
 sql_require_primary_key                  = {{sql_require_primary_key}}
 lower_case_table_names                   = {{lower_case_table_names}}
 auto_increment_increment                 = {{auto_increment_increment}}
 auto_increment_offset                    = {{auto_increment_offset}}
 table_open_cache                         = {{table_open_cache}}
 table_definition_cache                   = {{table_definition_cache}}
 table_open_cache_instances               = {{table_open_cache_instances}}
 
+
 #### for net 
 max_allowed_packet                       = {{max_allowed_packet}}
 connect_timeout                          = {{connect_timeout}}
 interactive_timeout                      = {{interactive_timeout}}
 net_read_timeout                         = {{net_read_timeout}}
 net_retry_count                          = {{net_retry_count}}
 net_write_timeout                        = {{net_write_timeout}}
 net_buffer_length                        = {{net_buffer_length}}
 
+
 #### for logs 
 log_output                               = {{log_output}}
 general_log                              = {{general_log}}
 general_log_file                         = {{general_log_file}}
+
+
 ## error
 log_error                                = {{log_error}}
 log_statements_unsafe_for_binlog         = {{log_statements_unsafe_for_binlog}}
-## slow
+
+
+## for slow
 slow_query_log                           = {{slow_query_log}}
 slow_query_log_file                      = {{slow_query_log_file}}
 long_query_time                          = {{long_query_time}}
 log_queries_not_using_indexes            = {{log_queries_not_using_indexes}}
 log_slow_admin_statements                = {{log_slow_admin_statements}}
-log_slow_slave_statements                = {{log_slow_slave_statements}}
-## binlog
-log_bin                                  = {{log_bin }}
-binlog_checksum                          = {{binlog_checksum}}
-log_bin_trust_function_creators          = {{log_bin_trust_function_creators}}
-binlog_direct_non_transactional_updates  = {{binlog_direct_non_transactional_updates}}
-binlog_expire_logs_seconds               = {{binlog_expire_logs_seconds}}
-binlog_error_action                      = {{binlog_error_action}}
-binlog_format                            = {{binlog_format}}
-max_binlog_stmt_cache_size               = {{max_binlog_stmt_cache_size}}
-max_binlog_cache_size                    = {{max_binlog_cache_size}}
-max_binlog_size                          = {{max_binlog_size}}
-binlog_order_commits                     = {{binlog_order_commits}}
-binlog_row_image                         = {{binlog_row_image}}
-binlog_row_metadata                      = {{binlog_row_metadata}}
-binlog_rows_query_log_events             = {{binlog_rows_query_log_events}}
-binlog_stmt_cache_size                   = {{binlog_stmt_cache_size}}
-log_slave_updates                        = {{log_slave_updates}}
-binlog_transaction_compression           = {{binlog_transaction_compression}}
-binlog_transaction_dependency_history_size ={{binlog_transaction_dependency_history_size}}
-binlog_transaction_dependency_tracking   = {{binlog_transaction_dependency_tracking}}
-sync_binlog                              = {{sync_binlog}}
-binlog_cache_size                        = {{binlog_cache_size}}
-binlog_group_commit_sync_delay           = {{binlog_group_commit_sync_delay}}
-binlog_group_commit_sync_no_delay_count  = {{binlog_group_commit_sync_no_delay_count}}
+log_slow_replica_statements              = ON
+
+
+## for binlog
+log_bin                                    = {{log_bin }}
+binlog_checksum                            = {{binlog_checksum}}
+log_bin_trust_function_creators            = {{log_bin_trust_function_creators}}
+binlog_direct_non_transactional_updates    = {{binlog_direct_non_transactional_updates}}
+binlog_expire_logs_seconds                 = {{binlog_expire_logs_seconds}}
+binlog_error_action                        = {{binlog_error_action}}
+binlog_format                              = {{binlog_format}}
+max_binlog_stmt_cache_size                 = {{max_binlog_stmt_cache_size}}
+max_binlog_cache_size                      = {{max_binlog_cache_size}}
+max_binlog_size                            = {{max_binlog_size}}
+binlog_order_commits                       = {{binlog_order_commits}}
+binlog_row_image                           = {{binlog_row_image}}
+binlog_row_metadata                        = {{binlog_row_metadata}}
+binlog_rows_query_log_events               = {{binlog_rows_query_log_events}}
+binlog_stmt_cache_size                     = {{binlog_stmt_cache_size}}
+log_replica_updates                        = ON
+binlog_transaction_compression             = {{binlog_transaction_compression}}
+binlog_transaction_dependency_history_size = {{binlog_transaction_dependency_history_size}}
+binlog_transaction_dependency_tracking     = {{binlog_transaction_dependency_tracking}}
+#transaction_write_set_extraction           = {{transaction_write_set_extraction}}
+sync_binlog                                = {{sync_binlog}}
+binlog_cache_size                          = {{binlog_cache_size}}
+binlog_group_commit_sync_delay             = {{binlog_group_commit_sync_delay}}
+binlog_group_commit_sync_no_delay_count    = {{binlog_group_commit_sync_no_delay_count}}
+
 
 #### for replication
-rpl_semi_sync_master_enabled             = {{rpl_semi_sync_master_enabled}}
-rpl_semi_sync_slave_enabled              = {{rpl_semi_sync_slave_enabled}}
-rpl_semi_sync_master_timeout             = {{rpl_semi_sync_master_timeout}}
-rpl_semi_sync_master_wait_point          = {{rpl_semi_sync_master_wait_point}}
-rpl_semi_sync_master_wait_no_slave       = {{rpl_semi_sync_master_wait_no_slave}}
+rpl_semi_sync_master_enabled              = {{rpl_semi_sync_master_enabled}}
+rpl_semi_sync_slave_enabled               = {{rpl_semi_sync_slave_enabled}}
+rpl_semi_sync_master_timeout              = {{rpl_semi_sync_master_timeout}}
+rpl_semi_sync_master_wait_point           = {{rpl_semi_sync_master_wait_point}}
+rpl_semi_sync_master_wait_no_slave        = {{rpl_semi_sync_master_wait_no_slave}}
 rpl_semi_sync_master_wait_for_slave_count = {{rpl_semi_sync_master_wait_for_slave_count}}
-master_info_repository                   = {{master_info_repository}}
-sync_master_info                         = {{sync_master_info}}
-skip_slave_start                         = {{skip_slave_start}}
-slave_load_tmpdir                        = {{slave_load_tmpdir}}
-plugin_load_add                          = semisync_master.so
-plugin_load_add                          = semisync_slave.so
-relay_log                                = {{relay_log}}
-sync_relay_log                           = {{sync_relay_log}}
-sync_relay_log_info                      = {{sync_relay_log_info}}
-relay_log_info_repository                = {{relay_log_info_repository}}
-slave_preserve_commit_order              = {{slave_preserve_commit_order}}
-slave_parallel_type                      = {{slave_parallel_type}}
-slave_parallel_workers                   = {{slave_parallel_workers}}
-slave_max_allowed_packet                 = {{slave_max_allowed_packet}}
-
+sync_source_info                          = 1000
+skip_replica_start                        = ON
+replica_load_tmpdir                       = /tmp/
+plugin_load_add                           = semisync_master.so
+plugin_load_add                           = semisync_slave.so
+relay_log                                 = {{relay_log}}
+sync_relay_log                            = {{sync_relay_log}}
+sync_relay_log_info                       = {{sync_relay_log_info}}
+replica_preserve_commit_order             = ON
+#replica_parallel_type                    = LOGICAL_CLOCK          # deprecated from 8.0.29
+replica_parallel_workers                  = {{replica_parallel_workers}}
+replica_max_allowed_packet                = {{replica_max_allowed_packet}}
 
 
 #### for gtid
 gtid_mode                                = {{gtid_mode}}
 binlog_gtid_simple_recovery              = {{binlog_gtid_simple_recovery}}
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
+
 #### for clone 
-plugin-load-add                          = mysql_clone.so
-clone                                    = FORCE_PLUS_PERMANENT
+plugin-load-add                           = mysql_clone.so
+clone                                     = FORCE_PLUS_PERMANENT
+clone_autotune_concurrency                = {{ clone_autotune_concurrency}}
+clone_buffer_size                         = {{ clone_buffer_size}}
+clone_block_ddl                           = {{ clone_block_ddl}}
+clone_delay_after_data_drop               = {{ clone_delay_after_data_drop}}
+clone_ddl_timeout                         = {{ clone_ddl_timeout}}
+clone_donor_timeout_after_network_failure = {{ clone_donor_timeout_after_network_failure}}
+clone_enable_compression                  = {{ clone_enable_compression}}
+clone_max_concurrency                     = {{ clone_max_concurrency}}
+clone_max_data_bandwidth                  = {{ clone_max_data_bandwidth}}
+clone_max_network_bandwidth               = {{ clone_max_network_bandwidth}}
+clone_valid_donor_list                    = {{ clone_valid_donor_list}}
+
 
 #### for engines 
 default_storage_engine                   = {{default_storage_engine}}
 default_tmp_storage_engine               = {{default_tmp_storage_engine}}
 internal_tmp_mem_storage_engine          = {{internal_tmp_mem_storage_engine}}
 
+
 #### for innodb
 innodb_data_home_dir                     = {{innodb_data_home_dir}}
 innodb_data_file_path                    = {{innodb_data_file_path}}
 innodb_page_size                         = {{innodb_page_size}}
 innodb_default_row_format                = {{innodb_default_row_format}}
-innodb_log_group_home_dir                = {{innodb_log_group_home_dir}}
 innodb_redo_log_encrypt                  = {{innodb_redo_log_encrypt}}
 innodb_online_alter_log_max_size         = {{innodb_online_alter_log_max_size}}
-innodb_undo_directory                    = {{innodb_undo_directory}}
+#innodb_log_group_home_dir               = {{innodb_log_group_home_dir}}
+#innodb_undo_directory                   = {{innodb_undo_directory}}
 innodb_undo_log_encrypt                  = {{innodb_undo_log_encrypt}}
 innodb_undo_log_truncate                 = {{innodb_undo_log_truncate}}
 innodb_max_undo_log_size                 = {{innodb_max_undo_log_size}}
 innodb_rollback_on_timeout               = {{innodb_rollback_on_timeout}}
 innodb_rollback_segments                 = {{innodb_rollback_segments}}
 innodb_log_checksums                     = {{innodb_log_checksums}}
 innodb_checksum_algorithm                = {{innodb_checksum_algorithm}}
@@ -197,30 +221,32 @@
 innodb_disable_sort_file_cache           = {{innodb_disable_sort_file_cache}}
 innodb_numa_interleave                   = {{innodb_numa_interleave}}
 innodb_strict_mode                       = {{innodb_strict_mode}}
 innodb_sort_buffer_size                  = {{innodb_sort_buffer_size}}
 innodb_fast_shutdown                     = {{innodb_fast_shutdown}}
 innodb_force_load_corrupted              = {{innodb_force_load_corrupted}}
 innodb_force_recovery                    = {{innodb_force_recovery}}
-innodb_temp_tablespaces_dir              = {{innodb_temp_tablespaces_dir}}
+#innodb_temp_tablespaces_dir              = {{innodb_temp_tablespaces_dir}}
 innodb_tmpdir                            = {{innodb_tmpdir}}
 innodb_temp_data_file_path               = {{innodb_temp_data_file_path}}
 innodb_page_cleaners                     = {{innodb_page_cleaners}}
 innodb_adaptive_hash_index               = {{innodb_adaptive_hash_index}}
 innodb_adaptive_hash_index_parts         = {{innodb_adaptive_hash_index_parts}}
 innodb_flush_log_at_timeout              = {{innodb_flush_log_at_timeout}}
 innodb_fsync_threshold                   = {{innodb_fsync_threshold}}
 innodb_fill_factor                       = {{innodb_fill_factor}}
 innodb_file_per_table                    = {{innodb_file_per_table}}
+sql_generate_invisible_primary_key       = {{sql_generate_invisible_primary_key}} 
 innodb_autoextend_increment              = {{innodb_autoextend_increment}}
 innodb_open_files                        = {{innodb_open_files}}
 innodb_buffer_pool_chunk_size            = {{innodb_buffer_pool_chunk_size}}
 innodb_buffer_pool_instances             = {{innodb_buffer_pool_instances}}
-innodb_log_files_in_group                = {{innodb_log_files_in_group}}
-innodb_log_file_size                     = {{innodb_log_file_size}}
+#innodb_log_files_in_group               = {{innodb_log_files_in_group}}
+#innodb_log_file_size                    = {{innodb_log_file_size}}
+innodb_redo_log_capacity                 = {{innodb_redo_log_capacity}}
 innodb_flush_neighbors                   = {{innodb_flush_neighbors}}
 innodb_io_capacity                       = {{innodb_io_capacity}}
 innodb_io_capacity_max                   = {{innodb_io_capacity_max}}
 innodb_autoinc_lock_mode                 = {{innodb_autoinc_lock_mode}}
 innodb_change_buffer_max_size            = {{innodb_change_buffer_max_size}}
 innodb_flush_method                      = {{innodb_flush_method}}
 innodb_log_buffer_size                   = {{innodb_log_buffer_size}}
@@ -266,21 +292,13 @@
 performance_schema_consumer_events_statements_history_long              =OFF 
 performance_schema_consumer_events_waits_current                        =ON  
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
-
-
-
-
-
-
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
-# base on mysql-8.0.21
-# generated by https://www.sqlpy.com 2020年1月15日 10:32
+# base on mysql-8.0.34
+# generated by https://www.sqlpy.com at {{now}}
 # wechat: jianglegege
 # email: 1721900707@qq.com
-# -- ~ _ ~ --   
-
-
+# -- ~ _ ~ --
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/redis.conf.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/redis.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/cnfs/redisd.service.jinja` & `dbm-agent-8.34.0/dbma/static/cnfs/redisd.service.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/dbma/static/sql-scripts/常用SQL.md` & `dbm-agent-8.34.0/dbma/static/sql-scripts/常用SQL.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.9/setup.py` & `dbm-agent-8.34.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         "dbma/core/agent",
         "dbma/core/threads",
         "dbma/bil",
         "dbma/components",
         "dbma/components/mysql",
         "dbma/components/mysql/views",
         "dbma/components/mysql/backups",
+        "dbma/components/mysql/backends",
         "dbma/components/redis",
         "dbma/components/orchestrator",
     ],
     package_data={"dbma": ["static/cnfs/*", "static/sql-scripts/*"]},
     url="https://github.com/Neeky/dbm-agent",
     install_requires=[
         "mysql-connector-python>=8.0.31",
```

