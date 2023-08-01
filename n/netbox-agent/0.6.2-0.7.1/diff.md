# Comparing `tmp/netbox_agent-0.6.2.tar.gz` & `tmp/netbox_agent-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netbox_agent-0.6.2.tar", last modified: Mon Aug 24 11:48:30 2020, max compression
+gzip compressed data, was "netbox_agent-0.7.1.tar", last modified: Tue Aug  1 08:08:49 2023, max compression
```

## Comparing `netbox_agent-0.6.2.tar` & `netbox_agent-0.7.1.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-08-24 11:48:30.928936 netbox_agent-0.6.2/
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)    10361 2020-08-24 11:48:30.929274 netbox_agent-0.6.2/PKG-INFO
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     7803 2020-08-24 11:45:01.000000 netbox_agent-0.6.2/README.md
-drwxr-xr-x   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-08-24 11:48:30.915656 netbox_agent-0.6.2/netbox_agent/
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)      162 2020-02-02 22:10:00.000000 netbox_agent-0.6.2/netbox_agent/__init__.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     1480 2020-07-11 13:25:59.000000 netbox_agent-0.6.2/netbox_agent/cli.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     4625 2020-07-11 13:33:34.000000 netbox_agent-0.6.2/netbox_agent/config.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     6479 2020-02-02 22:10:10.000000 netbox_agent-0.6.2/netbox_agent/dmidecode.py
-drwxr-xr-x   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-08-24 11:48:30.920292 netbox_agent-0.6.2/netbox_agent/drivers/
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-02-02 22:10:00.000000 netbox_agent-0.6.2/netbox_agent/drivers/__init__.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)      206 2020-02-02 22:10:00.000000 netbox_agent-0.6.2/netbox_agent/drivers/cmd.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)      191 2020-02-02 22:10:00.000000 netbox_agent-0.6.2/netbox_agent/drivers/file.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     2303 2020-05-04 11:23:11.000000 netbox_agent-0.6.2/netbox_agent/ethtool.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)    15449 2020-06-14 16:46:02.000000 netbox_agent-0.6.2/netbox_agent/inventory.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     2240 2020-05-04 11:23:11.000000 netbox_agent-0.6.2/netbox_agent/ipmi.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     2376 2020-02-02 22:10:10.000000 netbox_agent-0.6.2/netbox_agent/lldp.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     3669 2020-07-01 17:52:12.000000 netbox_agent-0.6.2/netbox_agent/location.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)      200 2020-05-04 11:23:11.000000 netbox_agent-0.6.2/netbox_agent/logging.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     4715 2020-07-01 17:52:12.000000 netbox_agent-0.6.2/netbox_agent/lshw.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     1703 2020-07-01 17:52:12.000000 netbox_agent-0.6.2/netbox_agent/misc.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)    24186 2020-07-01 17:52:12.000000 netbox_agent-0.6.2/netbox_agent/network.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     4310 2020-06-15 13:48:39.000000 netbox_agent-0.6.2/netbox_agent/power.py
-drwxr-xr-x   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-08-24 11:48:30.924436 netbox_agent-0.6.2/netbox_agent/raid/
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-02-02 22:10:00.000000 netbox_agent-0.6.2/netbox_agent/raid/__init__.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)      447 2020-02-02 22:10:00.000000 netbox_agent-0.6.2/netbox_agent/raid/base.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     5745 2020-06-14 16:46:02.000000 netbox_agent-0.6.2/netbox_agent/raid/hp.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     2519 2020-02-02 22:10:10.000000 netbox_agent-0.6.2/netbox_agent/raid/omreport.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     2521 2020-02-02 22:10:10.000000 netbox_agent-0.6.2/netbox_agent/raid/storcli.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)    11709 2020-08-24 11:45:01.000000 netbox_agent-0.6.2/netbox_agent/server.py
-drwxr-xr-x   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-08-24 11:48:30.928583 netbox_agent-0.6.2/netbox_agent/vendors/
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-02-02 22:10:00.000000 netbox_agent-0.6.2/netbox_agent/vendors/__init__.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     1930 2020-03-22 17:33:54.000000 netbox_agent-0.6.2/netbox_agent/vendors/dell.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)      609 2020-03-22 17:33:54.000000 netbox_agent-0.6.2/netbox_agent/vendors/generic.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     2644 2020-08-24 11:45:01.000000 netbox_agent-0.6.2/netbox_agent/vendors/hp.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)      954 2020-03-22 17:33:54.000000 netbox_agent-0.6.2/netbox_agent/vendors/qct.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     2019 2020-08-24 11:45:01.000000 netbox_agent-0.6.2/netbox_agent/vendors/supermicro.py
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     3542 2020-07-11 13:33:34.000000 netbox_agent-0.6.2/netbox_agent/virtualmachine.py
-drwxr-xr-x   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        0 2020-08-24 11:48:30.918927 netbox_agent-0.6.2/netbox_agent.egg-info/
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)    10361 2020-08-24 11:48:30.000000 netbox_agent-0.6.2/netbox_agent.egg-info/PKG-INFO
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     1071 2020-08-24 11:48:30.000000 netbox_agent-0.6.2/netbox_agent.egg-info/SOURCES.txt
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        1 2020-08-24 11:48:30.000000 netbox_agent-0.6.2/netbox_agent.egg-info/dependency_links.txt
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)       56 2020-08-24 11:48:30.000000 netbox_agent-0.6.2/netbox_agent.egg-info/entry_points.txt
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)        1 2020-03-22 16:52:59.000000 netbox_agent-0.6.2/netbox_agent.egg-info/not-zip-safe
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)       84 2020-08-24 11:48:30.000000 netbox_agent-0.6.2/netbox_agent.egg-info/requires.txt
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)       13 2020-08-24 11:48:30.000000 netbox_agent-0.6.2/netbox_agent.egg-info/top_level.txt
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)      443 2020-08-24 11:48:30.929998 netbox_agent-0.6.2/setup.cfg
--rw-r--r--   0 sobl     (259783395) MILLEMERCIS\Domain Users (2131105609)     1059 2020-08-24 11:45:14.000000 netbox_agent-0.6.2/setup.py
+drwxr-xr-x   0 solvik     (501) staff       (20)        0 2023-08-01 08:08:49.299893 netbox_agent-0.7.1/
+-rw-r--r--   0 solvik     (501) staff       (20)    11357 2020-02-02 22:10:00.000000 netbox_agent-0.7.1/LICENSE
+-rw-r--r--   0 solvik     (501) staff       (20)       25 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/MANIFEST.in
+-rw-r--r--   0 solvik     (501) staff       (20)    10989 2023-08-01 08:08:49.300001 netbox_agent-0.7.1/PKG-INFO
+-rw-r--r--   0 solvik     (501) staff       (20)    10504 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/README.md
+drwxr-xr-x   0 solvik     (501) staff       (20)        0 2023-08-01 08:08:49.289773 netbox_agent-0.7.1/netbox_agent/
+-rw-r--r--   0 solvik     (501) staff       (20)      162 2020-02-02 22:10:00.000000 netbox_agent-0.7.1/netbox_agent/__init__.py
+-rw-r--r--   0 solvik     (501) staff       (20)     1724 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/cli.py
+-rw-r--r--   0 solvik     (501) staff       (20)     6107 2023-08-01 08:07:49.000000 netbox_agent-0.7.1/netbox_agent/config.py
+-rw-r--r--   0 solvik     (501) staff       (20)     6479 2020-02-02 22:10:10.000000 netbox_agent-0.7.1/netbox_agent/dmidecode.py
+drwxr-xr-x   0 solvik     (501) staff       (20)        0 2023-08-01 08:08:49.297781 netbox_agent-0.7.1/netbox_agent/drivers/
+-rw-r--r--   0 solvik     (501) staff       (20)        0 2020-02-02 22:10:00.000000 netbox_agent-0.7.1/netbox_agent/drivers/__init__.py
+-rw-r--r--   0 solvik     (501) staff       (20)      206 2020-02-02 22:10:00.000000 netbox_agent-0.7.1/netbox_agent/drivers/cmd.py
+-rw-r--r--   0 solvik     (501) staff       (20)      191 2020-02-02 22:10:00.000000 netbox_agent-0.7.1/netbox_agent/drivers/file.py
+-rw-r--r--   0 solvik     (501) staff       (20)     2303 2020-05-04 11:23:11.000000 netbox_agent-0.7.1/netbox_agent/ethtool.py
+-rw-r--r--   0 solvik     (501) staff       (20)    19333 2023-08-01 08:07:49.000000 netbox_agent-0.7.1/netbox_agent/inventory.py
+-rw-r--r--   0 solvik     (501) staff       (20)     2266 2023-08-01 08:07:49.000000 netbox_agent-0.7.1/netbox_agent/ipmi.py
+-rw-r--r--   0 solvik     (501) staff       (20)     2662 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/lldp.py
+-rw-r--r--   0 solvik     (501) staff       (20)     3669 2020-07-01 17:52:12.000000 netbox_agent-0.7.1/netbox_agent/location.py
+-rw-r--r--   0 solvik     (501) staff       (20)      200 2020-05-04 11:23:11.000000 netbox_agent-0.7.1/netbox_agent/logging.py
+-rw-r--r--   0 solvik     (501) staff       (20)     6749 2023-08-01 08:07:49.000000 netbox_agent-0.7.1/netbox_agent/lshw.py
+-rw-r--r--   0 solvik     (501) staff       (20)     3089 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/misc.py
+-rw-r--r--   0 solvik     (501) staff       (20)    26650 2023-08-01 08:07:49.000000 netbox_agent-0.7.1/netbox_agent/network.py
+-rw-r--r--   0 solvik     (501) staff       (20)     4500 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/power.py
+drwxr-xr-x   0 solvik     (501) staff       (20)        0 2023-08-01 08:08:49.298567 netbox_agent-0.7.1/netbox_agent/raid/
+-rw-r--r--   0 solvik     (501) staff       (20)        0 2020-02-02 22:10:00.000000 netbox_agent-0.7.1/netbox_agent/raid/__init__.py
+-rw-r--r--   0 solvik     (501) staff       (20)      496 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/raid/base.py
+-rw-r--r--   0 solvik     (501) staff       (20)     7479 2023-08-01 08:07:49.000000 netbox_agent-0.7.1/netbox_agent/raid/hp.py
+-rw-r--r--   0 solvik     (501) staff       (20)     4466 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/raid/omreport.py
+-rw-r--r--   0 solvik     (501) staff       (20)     5517 2022-12-12 16:15:10.000000 netbox_agent-0.7.1/netbox_agent/raid/storcli.py
+-rw-r--r--   0 solvik     (501) staff       (20)    18986 2022-12-12 16:15:10.000000 netbox_agent-0.7.1/netbox_agent/server.py
+drwxr-xr-x   0 solvik     (501) staff       (20)        0 2023-08-01 08:08:49.299713 netbox_agent-0.7.1/netbox_agent/vendors/
+-rw-r--r--   0 solvik     (501) staff       (20)        0 2020-02-02 22:10:00.000000 netbox_agent-0.7.1/netbox_agent/vendors/__init__.py
+-rw-r--r--   0 solvik     (501) staff       (20)     2455 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/vendors/dell.py
+-rw-r--r--   0 solvik     (501) staff       (20)      610 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/vendors/generic.py
+-rw-r--r--   0 solvik     (501) staff       (20)     4465 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/vendors/hp.py
+-rw-r--r--   0 solvik     (501) staff       (20)      954 2020-03-22 17:33:54.000000 netbox_agent-0.7.1/netbox_agent/vendors/qct.py
+-rw-r--r--   0 solvik     (501) staff       (20)     2550 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/netbox_agent/vendors/supermicro.py
+-rw-r--r--   0 solvik     (501) staff       (20)     4049 2023-08-01 08:07:49.000000 netbox_agent-0.7.1/netbox_agent/virtualmachine.py
+drwxr-xr-x   0 solvik     (501) staff       (20)        0 2023-08-01 08:08:49.297222 netbox_agent-0.7.1/netbox_agent.egg-info/
+-rw-r--r--   0 solvik     (501) staff       (20)    10989 2023-08-01 08:08:49.000000 netbox_agent-0.7.1/netbox_agent.egg-info/PKG-INFO
+-rw-r--r--   0 solvik     (501) staff       (20)     1108 2023-08-01 08:08:49.000000 netbox_agent-0.7.1/netbox_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 solvik     (501) staff       (20)        1 2023-08-01 08:08:49.000000 netbox_agent-0.7.1/netbox_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 solvik     (501) staff       (20)       55 2023-08-01 08:08:49.000000 netbox_agent-0.7.1/netbox_agent.egg-info/entry_points.txt
+-rw-r--r--   0 solvik     (501) staff       (20)        1 2020-03-22 16:52:59.000000 netbox_agent-0.7.1/netbox_agent.egg-info/not-zip-safe
+-rw-r--r--   0 solvik     (501) staff       (20)      136 2023-08-01 08:08:49.000000 netbox_agent-0.7.1/netbox_agent.egg-info/requires.txt
+-rw-r--r--   0 solvik     (501) staff       (20)       13 2023-08-01 08:08:49.000000 netbox_agent-0.7.1/netbox_agent.egg-info/top_level.txt
+-rw-r--r--   0 solvik     (501) staff       (20)      136 2022-09-14 16:57:21.000000 netbox_agent-0.7.1/requirements.txt
+-rw-r--r--   0 solvik     (501) staff       (20)      443 2023-08-01 08:08:49.300599 netbox_agent-0.7.1/setup.cfg
+-rw-r--r--   0 solvik     (501) staff       (20)     1202 2022-08-08 13:26:07.000000 netbox_agent-0.7.1/setup.py
```

### Comparing `netbox_agent-0.6.2/PKG-INFO` & `netbox_agent-0.7.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,274 +1,292 @@
-Metadata-Version: 2.1
-Name: netbox_agent
-Version: 0.6.2
-Summary: NetBox agent for server
-Home-page: https://github.com/solvik/netbox_agent
-Author: Solvik Blum
-Author-email: solvik@solvik.fr
-License: Apache2
-Description: # Netbox agent [![Build Status](https://travis-ci.com/Solvik/netbox-agent.svg?branch=master)](https://travis-ci.com/Solvik/netbox-agent)
-        
-        This project aims to create hardware automatically into [Netbox](https://github.com/netbox-community/netbox) based on standard tools (dmidecode, lldpd, parsing /sys/, etc).
-        
-        The goal is to generate an existing infrastructure on Netbox and have the ability to update it regularly by executing the agent.
-        
-        # Features
-        
-        * Create virtual machines, servers, chassis and blade through standard tools (`dmidecode`)
-        * Create physical, bonding and vlan network interfaces with IPs (IPv4 & IPv6)
-        * Create IPMI interface if found
-        * Create or get existing VLAN and associate it to interfaces
-        * Generic ability to guess datacenters and rack location through drivers (`cmd` and `file` and custom ones)
-        * Update existing `Device` and `Interface`
-        * Handle blade moving (new slot, new chassis)
-        * Automatic cabling (server's interface to switch's interface) using lldp
-        * Local inventory using `Inventory Item` for CPU, RAM, RAID cards, physical disks (behind raid cards)
-        * PSUs creation and power consumption reporting (based on vendor's tools)
-        
-        # Requirements
-        
-        - Netbox >= 2.6
-        - Python >= 3.4
-        - [pynetbox](https://github.com/digitalocean/pynetbox/)
-        - [python3-netaddr](https://github.com/drkjam/netaddr)
-        - [python3-netifaces](https://github.com/al45tair/netifaces)
-        - [jsonargparse](https://github.com/omni-us/jsonargparse/)
-        
-        - ethtool
-        - dmidecode
-        - ipmitool
-        - lldpd
-        - lshw
-        
-        ## Inventory requirement
-        - hpassacli
-        - storcli
-        - omreport
-        
-        # Installation
-        
-        ```
-        # pip3 install netbox-agent
-        ```
-        
-        # Usage
-        
-        The agent can be run from a shell and get its configuration from either the configuration file or environment variables.
-        
-        Configuration values are overridden based on the following precedence: command line arguments (might include config file) > environment variables > default config file > defaults.
-        
-        ```
-        # netbox_agent -c /etc/netbox_agent.yml --register
-        INFO:root:Creating chassis blade (serial: QTFCQ574502EF)
-        INFO:root:Creating blade (serial: QTFCQ574502D2) myserver on chassis QTFCQ574502EF
-        INFO:root:Setting device (QTFCQ574502D2) new slot on Slot 9 (Chassis QTFCQ574502EF)..
-        INFO:root:Interface a8:1e:84:f2:9e:6a not found, creating..
-        INFO:root:Creating NIC enp1s0f1 (a8:1e:84:f2:9e:6a) on myserver
-        INFO:root:Interface 02:42:7a:89:cf:a4 not found, creating..
-        INFO:root:Creating NIC br-07ea1e4a2f0e (02:42:7a:89:cf:a4) on myserver
-        INFO:root:Create new IP 172.19.0.1/16 on br-07ea1e4a2f0e
-        INFO:root:Interface a8:1e:84:f2:9e:69 not found, creating..
-        INFO:root:Creating NIC enp1s0f0 (a8:1e:84:f2:9e:69) on myserver
-        INFO:root:Create new IP 42.42.42.42/24 on enp1s0f0
-        INFO:root:Create new IP fe80::aa1e:84ff:fef2:9e69/64 on enp1s0f0
-        INFO:root:Interface a8:1e:84:cd:9d:d6 not found, creating..
-        INFO:root:Creating NIC IPMI (a8:1e:84:cd:9d:d6) on myserver
-        INFO:root:Create new IP 10.191.122.10/24 on IPMI
-        ```
-        
-        If you need, you can update only specific informations like:
-        * Network
-        * Inventory
-        * Location
-        * PSUs
-        
-        ```
-        # ip a add 42.42.42.43/24 dev enp1s0f1
-        # netbox_agent -c /etc/netbox_agent.yaml --update-network
-        INFO:root:Create new IP 42.42.42.43/24 on enp1s0f1
-        # netbox_agent --update-inventory
-        INFO:root:Creating Disk Samsung SSD 850 S2RBNX0K101698D
-        ```
-        
-        # Configuration
-        
-        ```
-        # Netbox configuration
-        netbox:
-         url: 'http://netbox.internal.company.com'
-         token: supersecrettoken
-         # uncomment to disable ssl verification
-         # ssl_verify: false
-        
-        # Network configuration
-        network:
-          # Regex to ignore interfaces 
-          ignore_interfaces: "(dummy.*|docker.*)"
-          # Regex to ignore IP addresses
-          ignore_ips: (127\.0\.0\..*)
-          # enable auto-cabling by parsing LLDP answers
-          lldp: true
-        
-        #
-        # You can use these to change the Netbox roles.
-        # These are the defaults.
-        #
-        #device:
-        # chassis_role: "Server Chassis"
-        # blade_role: "Blade"
-        # server_role: "Server"
-        # tags: server, blade, ,just a comma,delimited,list
-        #￼
-        #
-        # Can use this to set the tenant
-        #
-        #tenant:
-        # driver: "file:/tmp/tenant"
-        # regex: "(.*)"
-        ￼
-        ## Enable virtual machine support 
-        # virtual:
-        #   # not mandatory, can be guessed
-        #   enabled: True
-        #   # see https://netbox.company.com/virtualization/clusters/
-        #   cluster_name: my_vm_cluster
-        
-        # Enable datacenter location feature in Netbox
-        datacenter_location:
-         driver: "cmd:cat /etc/qualification | tr [A-Z] [a-z]"
-         regex: "datacenter: (?P<datacenter>[A-Za-z0-9]+)"
-        # driver: 'cmd:lldpctl'
-        # regex: 'SysName: .*\.([A-Za-z0-9]+)'
-        #
-        # driver: "file:/tmp/datacenter"
-        # regex: "(.*)"
-        
-        # Enable rack location feature in Netbox
-        rack_location:
-        # driver: 'cmd:lldpctl'
-        # match SysName: sw-dist-a1.dc42
-        # regex: 'SysName:[ ]+[A-Za-z]+-[A-Za-z]+-([A-Za-z0-9]+)'
-        #
-        # driver: "file:/tmp/datacenter"
-        # regex: "(.*)"
-        
-        # Enable local inventory reporting 
-        inventory: true
-        ```
-        
-        # Specific workflow
-        
-        ## Blades
-        
-        Each vendor class has a `is_blade` method which is later used for `Device` creation using the Netbox [parent/child feature](https://netbox.readthedocs.io/en/stable/core-functionality/devices/).
-        
-        The `get_blade_slot` method return the name of the `Device Bay`.
-        
-        
-        Certain vendors don't report the blade slot in `dmidecode`, so we can use the `slot_location` regex feature of the configuration file.
-        
-        ## Anycast IP
-        
-        The default behavior of the agent is to assign an interface to an IP.
-        So two servers with anycasted IPs, running update mode, would only trigger IP's interface assignement in a loop.
-        
-        In order to handle this case, user need to set Netbox IP's mode to `Anycast` so that the agent will create another one if it's present on another server.
-        
-        # Hardware
-        
-        Tested on:
-        
-        ## Virtual Machines
-        
-        * Hyper-V
-        * VMWare
-        * VirtualBox
-        * AWS
-        * GCP
-        
-        ## [Dell Inc.](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/dell.py)
-        
-        ### Blades
-        
-        * PowerEdge MX7000
-        * PowerEdge M1000e (your `DeviceType` should have slots named `Slot 01` and so on)
-        * PowerEdge MX740c
-        * PowerEdge M640
-        * PowerEdge M630
-        * PowerEdge M620
-        * PowerEdge M610
-        
-        ### Pizzas
-        
-        * DSS7500
-        
-        ## [HP / HPE](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/hp.py)
-        
-        ### Blades
-        
-        * HP BladeSystem c7000 Enclosure G2 / G3 (your `DeviceType` should have slots named `Bay 1` and so on)
-        * HP ProLiant BL460c Gen8
-        * HP ProLiant BL460c Gen9
-        * HP ProLiant BL460c Gen10
-        * HP Moonshot 1500 Enclosure (your `DeviceType` should have slots batch create with `Bay c[1-45n1]`) with HP ProLiant m750, m710x, m510 Server Cartridge
-        
-        ### Pizzas
-        
-        * ProLiant DL380p Gen8
-        * ProLiant SL4540 Gen8
-        * ProLiant SL4540 Gen9
-        * ProLiant XL450 Gen10
-        
-        ## [Supermicro](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/supermicro.py)
-        
-        ### Blades
-        
-        * SBI-* and SBA-* should be supported, but I need dmidecode output example to support automatic blade location
-        
-        ### Pizzas
-        
-        * SSG-6028R
-        * SYS-6018R
-        
-        ## [QCT](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/qct.py)
-        
-        ### Blades
-        
-        * QuantaMicro X10E-9N
-        
-        ### Pizzas
-        
-        * Nothing ATM, feel free to send me a dmidecode or make a PR!
-        
-        # Known limitations
-        
-        * The project is only compatible with Linux.
-        Since it uses `ethtool` and parses `/sys/` directory, it's not compatible with *BSD distributions.
-        * Netbox `>=2.6.0,<=2.6.2` has a caching problem ; if the cache lifetime is too high, the script can get stale data after modification.
-        We advise to set `CACHE_TIME` to `0`.
-        
-        # Developing
-        
-        If you want to run the agent while adding features or just for debugging purposes
-        
-        ```
-        # git clone https://github.com/Solvik/netbox-agent.git
-        # cd netbox-agent
-        # python3 -m netbox_agent.cli --register
-        ```
-        
-        On a personal note, I use the docker image from [netbox-community/netbox-docker](https://github.com/netbox-community/netbox-docker)
-        ```
-        # git clone https://github.com/netbox-community/netbox-docker
-        # cd netbox-docker
-        # docker-compose pull
-        # docker-compose up 
-        ```
-        
-Keywords: netbox
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
+# Netbox agent [![Build Status](https://travis-ci.com/Solvik/netbox-agent.svg?branch=master)](https://travis-ci.com/Solvik/netbox-agent)
+
+This project aims to create hardware automatically into [Netbox](https://github.com/netbox-community/netbox) based on standard tools (dmidecode, lldpd, parsing /sys/, etc).
+
+The goal is to generate an existing infrastructure on Netbox and have the ability to update it regularly by executing the agent.
+
+# Features
+
+* Create virtual machines, servers, chassis and blade through standard tools (`dmidecode`)
+* Create physical, bonding and vlan network interfaces with IPs (IPv4 & IPv6)
+* Create IPMI interface if found
+* Create or get existing VLAN and associate it to interfaces
+* Generic ability to guess datacenters and rack location through drivers (`cmd` and `file` and custom ones)
+* Update existing `Device` and `Interface`
+* Handle blade moving (new slot, new chassis)
+* Handle blade GPU expansions
+* Automatic cabling (server's interface to switch's interface) using lldp
+* Local inventory using `Inventory Item` for CPU, GPU, RAM, RAID cards, physical disks (behind raid cards)
+* PSUs creation and power consumption reporting (based on vendor's tools)
+
+# Requirements
+
+- Netbox >= 2.6
+- Python >= 3.4
+- [pynetbox](https://github.com/digitalocean/pynetbox/)
+- [python3-netaddr](https://github.com/drkjam/netaddr)
+- [python3-netifaces](https://github.com/al45tair/netifaces)
+- [jsonargparse](https://github.com/omni-us/jsonargparse/)
+
+- ethtool
+- dmidecode
+- ipmitool
+- lldpd
+- lshw
+
+## Inventory requirement
+- hpassacli
+- storcli
+- omreport
+
+# Installation
+
+```
+# pip3 install netbox-agent
+```
+
+# Usage
+
+The agent can be run from a shell and get its configuration from either the configuration file or environment variables.
+
+Configuration values are overridden based on the following precedence: command line arguments (might include config file) > environment variables > default config file > defaults.
+
+```
+# netbox_agent -c /etc/netbox_agent.yaml --register
+INFO:root:Creating chassis blade (serial: QTFCQ574502EF)
+INFO:root:Creating blade (serial: QTFCQ574502D2) myserver on chassis QTFCQ574502EF
+INFO:root:Setting device (QTFCQ574502D2) new slot on Slot 9 (Chassis QTFCQ574502EF)..
+INFO:root:Interface a8:1e:84:f2:9e:6a not found, creating..
+INFO:root:Creating NIC enp1s0f1 (a8:1e:84:f2:9e:6a) on myserver
+INFO:root:Interface 02:42:7a:89:cf:a4 not found, creating..
+INFO:root:Creating NIC br-07ea1e4a2f0e (02:42:7a:89:cf:a4) on myserver
+INFO:root:Create new IP 172.19.0.1/16 on br-07ea1e4a2f0e
+INFO:root:Interface a8:1e:84:f2:9e:69 not found, creating..
+INFO:root:Creating NIC enp1s0f0 (a8:1e:84:f2:9e:69) on myserver
+INFO:root:Create new IP 42.42.42.42/24 on enp1s0f0
+INFO:root:Create new IP fe80::aa1e:84ff:fef2:9e69/64 on enp1s0f0
+INFO:root:Interface a8:1e:84:cd:9d:d6 not found, creating..
+INFO:root:Creating NIC IPMI (a8:1e:84:cd:9d:d6) on myserver
+INFO:root:Create new IP 10.191.122.10/24 on IPMI
+```
+
+If you need, you can update only specific informations like:
+* Network
+* Inventory
+* Location
+* PSUs
+
+```
+# ip a add 42.42.42.43/24 dev enp1s0f1
+# netbox_agent -c /etc/netbox_agent.yaml --update-network
+INFO:root:Create new IP 42.42.42.43/24 on enp1s0f1
+# netbox_agent --update-inventory
+INFO:root:Creating Disk Samsung SSD 850 S2RBNX0K101698D
+```
+
+# Configuration
+
+```
+# Netbox configuration
+netbox:
+ url: 'http://netbox.internal.company.com'
+ token: supersecrettoken
+ # uncomment to disable ssl verification
+ # ssl_verify: false
+ # uncomment to use the system's CA certificates
+ # ssl_ca_certs_file: /etc/ssl/certs/ca-certificates.crt
+
+# Network configuration
+network:
+  # Regex to ignore interfaces
+  ignore_interfaces: "(dummy.*|docker.*)"
+  # Regex to ignore IP addresses
+  ignore_ips: (127\.0\.0\..*)
+  # enable auto-cabling by parsing LLDP answers
+  lldp: true
+
+#
+# You can use these to change the Netbox roles.
+# These are the defaults.
+#
+#device:
+# chassis_role: "Server Chassis"
+# blade_role: "Blade"
+# server_role: "Server"
+# tags: server, blade, ,just a comma,delimited,list
+# custom_fields: field1=value1,field2=value2#
+#
+# Can use this to set the tenant
+#
+#tenant:
+# driver: "file:/tmp/tenant"
+# regex: "(.*)"
+
+## Enable virtual machine support
+# virtual:
+#   # not mandatory, can be guessed
+#   enabled: True
+#   # see https://netbox.company.com/virtualization/clusters/
+#   cluster_name: my_vm_cluster
+
+# Enable datacenter location feature in Netbox
+datacenter_location:
+ driver: "cmd:cat /etc/qualification | tr [A-Z] [a-z]"
+ regex: "datacenter: (?P<datacenter>[A-Za-z0-9]+)"
+# driver: 'cmd:lldpctl'
+# regex: 'SysName: .*\.([A-Za-z0-9]+)'
+#
+# driver: "file:/tmp/datacenter"
+# regex: "(.*)"
+
+# Enable rack location feature in Netbox
+rack_location:
+# driver: 'cmd:lldpctl'
+# match SysName: sw-dist-a1.dc42
+# regex: 'SysName:[ ]+[A-Za-z]+-[A-Za-z]+-([A-Za-z0-9]+)'
+#
+# driver: "file:/tmp/datacenter"
+# regex: "(.*)"
+
+# Enable local inventory reporting
+inventory: true
+```
+
+# Specific workflow
+
+## Blades
+
+Each vendor class has a `is_blade` method which is later used for `Device` creation using the Netbox [parent/child feature](https://netbox.readthedocs.io/en/stable/core-functionality/devices/).
+
+The `get_blade_slot` method return the name of the `Device Bay`.
+
+
+Certain vendors don't report the blade slot in `dmidecode`, so we can use the `slot_location` regex feature of the configuration file.
+
+Some blade servers can be equipped with additional hardware using expansion blades, next to the processing blade, such as GPU expansion, or drives bay expansion. By default, the hardware from the expnasion is associated with the blade server itself, but it's possible to register the expansion as its own device using the `--expansion-as-device` command line parameter, or by setting `expansion_as_device` to `true` in the configuration file.
+
+## Drives attributes processing
+
+It is possible to process drives extended attributes such as the drive's physical or logical identifier, logical drive RAID type, size, consistency and so on.
+
+Those attributes as set as `custom_fields` in Netbox, and need to be registered properly before being able to specify them during the inventory phase.
+
+As the custom fields have to be created prior being able to register the disks extended attributes, this feature is only activated using the `--process-virtual-drives` command line parameter, or by setting `process_virtual_drives` to `true` in the configuration file.
+
+The custom fields to create as `DCIM > inventory item` `Text` are described below.
+
+```
+NAME            LABEL                      DESCRIPTION
+mount_point     Mount point                Device mount point(s)
+pd_identifier   Physical disk identifier   Physical disk identifier in the RAID controller
+vd_array        Virtual drive array        Virtual drive array the disk is member of
+vd_consistency  Virtual drive consistency  Virtual disk array consistency
+vd_device       Virtual drive device       Virtual drive system device
+vd_raid_type    Virtual drive RAID         Virtual drive array RAID type
+vd_size         Virtual drive size         Virtual drive array size
+```
+
+In the current implementation, the disks attributes ore not updated: if a disk with the correct serial number is found, it's sufficient to consider it as up to date.
+
+To force the reprocessing of the disks extended attributes, the `--force-disk-refresh` command line option can be used: it removes all existing disks to before populating them with the correct parsing. Unless this option is specified, the extended attributes won't be modified unless a disk is replaced.
+
+It is possible to dump the physical/virtual disks map on the filesystem under the JSON notation to ease or automate disks management. The file path has to be provided using the `--dump-disks-map` command line parameter.
+
+
+## Anycast IP
+
+The default behavior of the agent is to assign an interface to an IP.
+So two servers with anycasted IPs, running update mode, would only trigger IP's interface assignement in a loop.
+
+In order to handle this case, user need to set Netbox IP's mode to `Anycast` so that the agent will create another one if it's present on another server.
+
+# Hardware
+
+Tested on:
+
+## Virtual Machines
+
+* Hyper-V
+* VMWare
+* VirtualBox
+* AWS
+* GCP
+
+## [Dell Inc.](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/dell.py)
+
+### Blades
+
+* PowerEdge MX7000
+* PowerEdge M1000e (your `DeviceType` should have slots named `Slot 01` and so on)
+* PowerEdge MX740c
+* PowerEdge M640
+* PowerEdge M630
+* PowerEdge M620
+* PowerEdge M610
+
+### Pizzas
+
+* DSS7500
+
+## [HP / HPE](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/hp.py)
+
+### Blades
+
+* HP BladeSystem c7000 Enclosure G2 / G3 (your `DeviceType` should have slots named `Bay 1` and so on)
+* HP ProLiant BL460c Gen8
+* HP ProLiant BL460c Gen9
+* HP ProLiant BL460c Gen10
+* HP ProLiant BL460c Gen10 Graphics Exp its expansion HP ProLiant BL460c Graphics Expansion Blade
+* HP Moonshot 1500 Enclosure (your `DeviceType` should have slots batch create with `Bay c[1-45n1]`) with HP ProLiant m750, m710x, m510 Server Cartridge
+
+### Pizzas
+
+* ProLiant DL380p Gen8
+* ProLiant SL4540 Gen8
+* ProLiant SL4540 Gen9
+* ProLiant XL450 Gen10
+
+## [Supermicro](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/supermicro.py)
+
+### Blades
+
+* SBI-* and SBA-* should be supported, but I need dmidecode output example to support automatic blade location
+
+### Pizzas
+
+* SSG-6028R
+* SYS-6018R
+
+## [QCT](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/qct.py)
+
+### Blades
+
+* QuantaMicro X10E-9N
+
+### Pizzas
+
+* Nothing ATM, feel free to send me a dmidecode or make a PR!
+
+# Known limitations
+
+* The project is only compatible with Linux.
+Since it uses `ethtool` and parses `/sys/` directory, it's not compatible with *BSD distributions.
+* Netbox `>=2.6.0,<=2.6.2` has a caching problem ; if the cache lifetime is too high, the script can get stale data after modification.
+We advise to set `CACHE_TIME` to `0`.
+
+# Developing
+
+If you want to run the agent while adding features or just for debugging purposes
+
+```
+# git clone https://github.com/Solvik/netbox-agent.git
+# cd netbox-agent
+# python3 -m netbox_agent.cli --register
+```
+
+On a personal note, I use the docker image from [netbox-community/netbox-docker](https://github.com/netbox-community/netbox-docker)
+```
+# git clone https://github.com/netbox-community/netbox-docker
+# cd netbox-docker
+# docker-compose pull
+# docker-compose up
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `netbox_agent-0.6.2/README.md` & `netbox_agent-0.7.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: netbox_agent
+Version: 0.7.1
+Summary: NetBox agent for server
+Home-page: https://github.com/solvik/netbox_agent
+Author: Solvik Blum
+Author-email: solvik@solvik.fr
+License: Apache2
+Keywords: netbox
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Netbox agent [![Build Status](https://travis-ci.com/Solvik/netbox-agent.svg?branch=master)](https://travis-ci.com/Solvik/netbox-agent)
 
 This project aims to create hardware automatically into [Netbox](https://github.com/netbox-community/netbox) based on standard tools (dmidecode, lldpd, parsing /sys/, etc).
 
 The goal is to generate an existing infrastructure on Netbox and have the ability to update it regularly by executing the agent.
 
 # Features
@@ -9,16 +25,17 @@
 * Create virtual machines, servers, chassis and blade through standard tools (`dmidecode`)
 * Create physical, bonding and vlan network interfaces with IPs (IPv4 & IPv6)
 * Create IPMI interface if found
 * Create or get existing VLAN and associate it to interfaces
 * Generic ability to guess datacenters and rack location through drivers (`cmd` and `file` and custom ones)
 * Update existing `Device` and `Interface`
 * Handle blade moving (new slot, new chassis)
+* Handle blade GPU expansions
 * Automatic cabling (server's interface to switch's interface) using lldp
-* Local inventory using `Inventory Item` for CPU, RAM, RAID cards, physical disks (behind raid cards)
+* Local inventory using `Inventory Item` for CPU, GPU, RAM, RAID cards, physical disks (behind raid cards)
 * PSUs creation and power consumption reporting (based on vendor's tools)
 
 # Requirements
 
 - Netbox >= 2.6
 - Python >= 3.4
 - [pynetbox](https://github.com/digitalocean/pynetbox/)
@@ -46,15 +63,15 @@
 # Usage
 
 The agent can be run from a shell and get its configuration from either the configuration file or environment variables.
 
 Configuration values are overridden based on the following precedence: command line arguments (might include config file) > environment variables > default config file > defaults.
 
 ```
-# netbox_agent -c /etc/netbox_agent.yml --register
+# netbox_agent -c /etc/netbox_agent.yaml --register
 INFO:root:Creating chassis blade (serial: QTFCQ574502EF)
 INFO:root:Creating blade (serial: QTFCQ574502D2) myserver on chassis QTFCQ574502EF
 INFO:root:Setting device (QTFCQ574502D2) new slot on Slot 9 (Chassis QTFCQ574502EF)..
 INFO:root:Interface a8:1e:84:f2:9e:6a not found, creating..
 INFO:root:Creating NIC enp1s0f1 (a8:1e:84:f2:9e:6a) on myserver
 INFO:root:Interface 02:42:7a:89:cf:a4 not found, creating..
 INFO:root:Creating NIC br-07ea1e4a2f0e (02:42:7a:89:cf:a4) on myserver
@@ -87,18 +104,20 @@
 ```
 # Netbox configuration
 netbox:
  url: 'http://netbox.internal.company.com'
  token: supersecrettoken
  # uncomment to disable ssl verification
  # ssl_verify: false
+ # uncomment to use the system's CA certificates
+ # ssl_ca_certs_file: /etc/ssl/certs/ca-certificates.crt
 
 # Network configuration
 network:
-  # Regex to ignore interfaces 
+  # Regex to ignore interfaces
   ignore_interfaces: "(dummy.*|docker.*)"
   # Regex to ignore IP addresses
   ignore_ips: (127\.0\.0\..*)
   # enable auto-cabling by parsing LLDP answers
   lldp: true
 
 #
@@ -106,23 +125,23 @@
 # These are the defaults.
 #
 #device:
 # chassis_role: "Server Chassis"
 # blade_role: "Blade"
 # server_role: "Server"
 # tags: server, blade, ,just a comma,delimited,list
-#￼
+# custom_fields: field1=value1,field2=value2#
 #
 # Can use this to set the tenant
 #
 #tenant:
 # driver: "file:/tmp/tenant"
 # regex: "(.*)"
-￼
-## Enable virtual machine support 
+
+## Enable virtual machine support
 # virtual:
 #   # not mandatory, can be guessed
 #   enabled: True
 #   # see https://netbox.company.com/virtualization/clusters/
 #   cluster_name: my_vm_cluster
 
 # Enable datacenter location feature in Netbox
@@ -140,29 +159,59 @@
 # driver: 'cmd:lldpctl'
 # match SysName: sw-dist-a1.dc42
 # regex: 'SysName:[ ]+[A-Za-z]+-[A-Za-z]+-([A-Za-z0-9]+)'
 #
 # driver: "file:/tmp/datacenter"
 # regex: "(.*)"
 
-# Enable local inventory reporting 
+# Enable local inventory reporting
 inventory: true
 ```
 
 # Specific workflow
 
 ## Blades
 
 Each vendor class has a `is_blade` method which is later used for `Device` creation using the Netbox [parent/child feature](https://netbox.readthedocs.io/en/stable/core-functionality/devices/).
 
 The `get_blade_slot` method return the name of the `Device Bay`.
 
 
 Certain vendors don't report the blade slot in `dmidecode`, so we can use the `slot_location` regex feature of the configuration file.
 
+Some blade servers can be equipped with additional hardware using expansion blades, next to the processing blade, such as GPU expansion, or drives bay expansion. By default, the hardware from the expnasion is associated with the blade server itself, but it's possible to register the expansion as its own device using the `--expansion-as-device` command line parameter, or by setting `expansion_as_device` to `true` in the configuration file.
+
+## Drives attributes processing
+
+It is possible to process drives extended attributes such as the drive's physical or logical identifier, logical drive RAID type, size, consistency and so on.
+
+Those attributes as set as `custom_fields` in Netbox, and need to be registered properly before being able to specify them during the inventory phase.
+
+As the custom fields have to be created prior being able to register the disks extended attributes, this feature is only activated using the `--process-virtual-drives` command line parameter, or by setting `process_virtual_drives` to `true` in the configuration file.
+
+The custom fields to create as `DCIM > inventory item` `Text` are described below.
+
+```
+NAME            LABEL                      DESCRIPTION
+mount_point     Mount point                Device mount point(s)
+pd_identifier   Physical disk identifier   Physical disk identifier in the RAID controller
+vd_array        Virtual drive array        Virtual drive array the disk is member of
+vd_consistency  Virtual drive consistency  Virtual disk array consistency
+vd_device       Virtual drive device       Virtual drive system device
+vd_raid_type    Virtual drive RAID         Virtual drive array RAID type
+vd_size         Virtual drive size         Virtual drive array size
+```
+
+In the current implementation, the disks attributes ore not updated: if a disk with the correct serial number is found, it's sufficient to consider it as up to date.
+
+To force the reprocessing of the disks extended attributes, the `--force-disk-refresh` command line option can be used: it removes all existing disks to before populating them with the correct parsing. Unless this option is specified, the extended attributes won't be modified unless a disk is replaced.
+
+It is possible to dump the physical/virtual disks map on the filesystem under the JSON notation to ease or automate disks management. The file path has to be provided using the `--dump-disks-map` command line parameter.
+
+
 ## Anycast IP
 
 The default behavior of the agent is to assign an interface to an IP.
 So two servers with anycasted IPs, running update mode, would only trigger IP's interface assignement in a loop.
 
 In order to handle this case, user need to set Netbox IP's mode to `Anycast` so that the agent will create another one if it's present on another server.
 
@@ -198,14 +247,15 @@
 
 ### Blades
 
 * HP BladeSystem c7000 Enclosure G2 / G3 (your `DeviceType` should have slots named `Bay 1` and so on)
 * HP ProLiant BL460c Gen8
 * HP ProLiant BL460c Gen9
 * HP ProLiant BL460c Gen10
+* HP ProLiant BL460c Gen10 Graphics Exp its expansion HP ProLiant BL460c Graphics Expansion Blade
 * HP Moonshot 1500 Enclosure (your `DeviceType` should have slots batch create with `Bay c[1-45n1]`) with HP ProLiant m750, m710x, m510 Server Cartridge
 
 ### Pizzas
 
 * ProLiant DL380p Gen8
 * ProLiant SL4540 Gen8
 * ProLiant SL4540 Gen9
@@ -250,9 +300,9 @@
 ```
 
 On a personal note, I use the docker image from [netbox-community/netbox-docker](https://github.com/netbox-community/netbox-docker)
 ```
 # git clone https://github.com/netbox-community/netbox-docker
 # cd netbox-docker
 # docker-compose pull
-# docker-compose up 
+# docker-compose up
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `netbox_agent-0.6.2/netbox_agent/cli.py` & `netbox_agent-0.7.1/netbox_agent/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from packaging import version
 import netbox_agent.dmidecode as dmidecode
 from netbox_agent.config import config
+from netbox_agent.config import netbox_instance as nb
 from netbox_agent.logging import logging  # NOQA
 from netbox_agent.vendors.dell import DellHost
 from netbox_agent.vendors.generic import GenericHost
 from netbox_agent.vendors.hp import HPHost
 from netbox_agent.vendors.qct import QCTHost
 from netbox_agent.vendors.supermicro import SupermicroHost
 from netbox_agent.virtualmachine import VirtualMachine, is_vm
@@ -28,19 +30,23 @@
     else:
         manufacturer = dmidecode.get_by_type(dmi, 'Chassis')[0].get('Manufacturer')
         try:
             server = MANUFACTURERS[manufacturer](dmi=dmi)
         except KeyError:
             server = GenericHost(dmi=dmi)
 
+    if version.parse(nb.version) < version.parse('2.9'):
+        print('netbox-agent is not compatible with Netbox prior to verison 2.9')
+        return False
+
+    if config.register or config.update_all or config.update_network or \
+       config.update_location or config.update_inventory or config.update_psu:
+        server.netbox_create_or_update(config)
     if config.debug:
         server.print_debug()
-    if config.register or config.update_all or config.update_network or config.update_location or \
-       config.update_inventory or config.update_psu:
-        server.netbox_create_or_update(config)
     return True
 
 
 def main():
     return run(config)
```

### Comparing `netbox_agent-0.6.2/netbox_agent/config.py` & `netbox_agent-0.7.1/netbox_agent/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,26 +24,36 @@
     p.add_argument('-r', '--register', action='store_true', help='Register server to Netbox')
     p.add_argument('-u', '--update-all', action='store_true', help='Update all infos in Netbox')
     p.add_argument('-d', '--debug', action='store_true', help='Print debug infos')
     p.add_argument('--update-network', action='store_true', help='Update network')
     p.add_argument('--update-inventory', action='store_true', help='Update inventory')
     p.add_argument('--update-location', action='store_true', help='Update location')
     p.add_argument('--update-psu', action='store_true', help='Update PSU')
+    p.add_argument('--purge-old-devices', action='store_true',
+                   help='Purge existing (old ?) devices having same name but different serial')
+    p.add_argument('--expansion-as-device', action='store_true',
+                   help='Manage blade expansions as external devices')
 
     p.add_argument('--log_level', default='debug')
+    p.add_argument('--netbox.ssl_ca_certs_file', help='SSL CA certificates file')
     p.add_argument('--netbox.url', help='Netbox URL')
     p.add_argument('--netbox.token', help='Netbox API Token')
     p.add_argument('--netbox.ssl_verify', default=True, action='store_true',
                    help='Disable SSL verification')
     p.add_argument('--virtual.enabled', action='store_true', help='Is a virtual machine or not')
     p.add_argument('--virtual.cluster_name', help='Cluster name of VM')
     p.add_argument('--hostname_cmd', default=None,
                    help="Command to output hostname, used as Device's name in netbox")
+    p.add_argument('--device.platform', default=None,
+                   help='Override device platform. Here we use OS distribution.')
     p.add_argument('--device.tags', default=r'',
                    help='tags to use for a host')
+    p.add_argument('--preserve-tags', action='store_true', help='Append new unique tags, preserve those already present')
+    p.add_argument('--device.custom_fields', default=r'',
+                   help='custom_fields to use for a host, eg: field1=v1,field2=v2')
     p.add_argument('--device.blade_role', default=r'Blade',
                    help='role to use for a blade server')
     p.add_argument('--device.chassis_role', default=r'Server Chassis',
                    help='role to use for a chassis')
     p.add_argument('--device.server_role', default=r'Server',
                    help='role to use for a server')
     p.add_argument('--tenant.driver',
@@ -64,36 +74,50 @@
     p.add_argument('--slot_location.driver', help='Slot location driver, ie: cmd, file')
     p.add_argument('--slot_location.driver_file', help='Slot location custom driver file path')
     p.add_argument('--slot_location.regex', help='Slot location regex to extract slot name')
     p.add_argument('--network.ignore_interfaces', default=r'(dummy.*|docker.*)',
                    help='Regex to ignore interfaces')
     p.add_argument('--network.ignore_ips', default=r'^(127\.0\.0\..*|fe80.*|::1.*)',
                    help='Regex to ignore IPs')
+    p.add_argument('--network.ipmi', default=True, help='Enable gathering IPMI information')
     p.add_argument('--network.lldp', help='Enable auto-cabling feature through LLDP infos')
     p.add_argument('--inventory', action='store_true',
                    help='Enable HW inventory (CPU, Memory, RAID Cards, Disks) feature')
+    p.add_argument('--process-virtual-drives', action='store_true',
+                   help='Process virtual drives information from RAID '
+                        'controllers to fill disk custom_fields')
+    p.add_argument('--force-disk-refresh', action='store_true',
+                   help='Forces disks detection reprocessing')
+    p.add_argument('--dump-disks-map',
+                   help='File path to dump physical/virtual disks map')
 
     options = p.parse_args()
     return options
 
 
+config = get_config()
+
+
 def get_netbox_instance():
-    config = get_config()
     if config.netbox.url is None or config.netbox.token is None:
         logging.error('Netbox URL and token are mandatory')
         sys.exit(1)
 
     nb = pynetbox.api(
         url=get_config().netbox.url,
         token=get_config().netbox.token,
     )
-    if get_config().netbox.ssl_verify is False:
+    ca_certs_file = config.netbox.ssl_ca_certs_file
+    if ca_certs_file is not None:
+        session = requests.Session()
+        session.verify = ca_certs_file
+        nb.http_session = session
+    elif config.netbox.ssl_verify is False:
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         session = requests.Session()
         session.verify = False
         nb.http_session = session
 
     return nb
 
 
-config = get_config()
 netbox_instance = get_netbox_instance()
```

### Comparing `netbox_agent-0.6.2/netbox_agent/dmidecode.py` & `netbox_agent-0.7.1/netbox_agent/dmidecode.py`

 * *Files identical despite different names*

### Comparing `netbox_agent-0.6.2/netbox_agent/ethtool.py` & `netbox_agent-0.7.1/netbox_agent/ethtool.py`

 * *Files identical despite different names*

### Comparing `netbox_agent-0.6.2/netbox_agent/inventory.py` & `netbox_agent-0.7.1/netbox_agent/inventory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import logging
-import re
-
-import pynetbox
-
 from netbox_agent.config import config
 from netbox_agent.config import netbox_instance as nb
 from netbox_agent.lshw import LSHW
 from netbox_agent.misc import get_vendor, is_tool
 from netbox_agent.raid.hp import HPRaid
 from netbox_agent.raid.omreport import OmreportRaid
 from netbox_agent.raid.storcli import StorcliRaid
+import traceback
+import pynetbox
+import logging
+import json
+import re
+
 
 INVENTORY_TAG = {
     'cpu': {'name': 'hw:cpu', 'slug': 'hw-cpu'},
+    'gpu': {'name': 'hw:gpu', 'slug': 'hw-gpu'},
     'disk': {'name': 'hw:disk', 'slug': 'hw-disk'},
     'interface': {'name': 'hw:interface', 'slug': 'hw-interface'},
     'memory': {'name': 'hw:memory', 'slug': 'hw-memory'},
     'motherboard': {'name': 'hw:motherboard', 'slug': 'hw-motherboard'},
     'raid_card': {'name': 'hw:raid_card', 'slug': 'hw-raid-card'},
 }
 
@@ -28,48 +30,53 @@
     - https://github.com/netbox-community/netbox/issues/3333
 
     This class implements for:
     * memory
     * cpu
     * raid cards
     * disks
+    * gpus
 
     methods that:
     * get local item
     * get netbox item
     * create netbox item
     * update netbox item
 
     Known issues:
     - no scan of non-raid devices
     - no scan of NVMe devices
     """
 
-    def __init__(self, server):
+    def __init__(self, server, update_expansion=False):
         self.create_netbox_tags()
         self.server = server
-        netbox_server = self.server.get_netbox_server()
+        self.update_expansion = update_expansion
+        netbox_server = self.server.get_netbox_server(update_expansion)
 
         self.device_id = netbox_server.id if netbox_server else None
         self.raid = None
         self.disks = []
 
         self.lshw = LSHW()
 
     def create_netbox_tags(self):
+        ret = []
         for key, tag in INVENTORY_TAG.items():
             nb_tag = nb.extras.tags.get(
                 name=tag['name']
             )
             if not nb_tag:
                 nb_tag = nb.extras.tags.create(
                     name=tag['name'],
                     slug=tag['slug'],
                     comments=tag['name'],
                 )
+            ret.append(nb_tag)
+        return ret
 
     def find_or_create_manufacturer(self, name):
         if name is None:
             return None
 
         manufacturer = nb.dcim.manufacturers.get(
             name=name,
@@ -91,15 +98,15 @@
                 device_id=device_id,
                 tag=tag
             )
         except pynetbox.core.query.RequestError:
             logging.info('Tag {tag} is missing, returning empty array.'.format(tag=tag))
             items = []
 
-        return items
+        return list(items)
 
     def create_netbox_inventory_item(self, device_id, tags, vendor, name, serial, description):
         manufacturer = self.find_or_create_manufacturer(vendor)
 
         _ = nb.dcim.inventory_items.create(
             device=device_id,
             manufacturer=manufacturer.id,
@@ -146,28 +153,28 @@
                 nb_motherboard.delete()
 
         # create interfaces that are not in netbox
         for motherboard in motherboards:
             if motherboard.get('serial') not in [x.serial for x in nb_motherboards]:
                 self.create_netbox_inventory_item(
                     device_id=self.device_id,
-                    tags=[INVENTORY_TAG['motherboard']['name']],
+                    tags=[{'name': INVENTORY_TAG['motherboard']['name']}],
                     vendor='{}'.format(motherboard.get('vendor', 'N/A')),
                     serial='{}'.format(motherboard.get('serial', 'No SN')),
                     name='{}'.format(motherboard.get('name')),
                     description='{}'.format(motherboard.get('description'))
                 )
 
     def create_netbox_interface(self, iface):
         manufacturer = self.find_or_create_manufacturer(iface["vendor"])
         _ = nb.dcim.inventory_items.create(
             device=self.device_id,
             manufacturer=manufacturer.id,
             discovered=True,
-            tags=[INVENTORY_TAG['interface']['name']],
+            tags=[{'name': INVENTORY_TAG['interface']['name']}],
             name="{}".format(iface['product']),
             serial='{}'.format(iface['serial']),
             description='{} {}'.format(iface['description'], iface['name'])
         )
 
     def do_netbox_interfaces(self):
         nb_interfaces = self.get_netbox_inventory(
@@ -192,15 +199,15 @@
     def create_netbox_cpus(self):
         for cpu in self.lshw.get_hw_linux('cpu'):
             manufacturer = self.find_or_create_manufacturer(cpu["vendor"])
             _ = nb.dcim.inventory_items.create(
                 device=self.device_id,
                 manufacturer=manufacturer.id,
                 discovered=True,
-                tags=[INVENTORY_TAG['cpu']['name']],
+                tags=[{'name': INVENTORY_TAG['cpu']['name']}],
                 name=cpu['product'],
                 description='CPU {}'.format(cpu['location']),
                 # asset_tag=cpu['location']
             )
 
             logging.info('Creating CPU model {}'.format(cpu['product']))
 
@@ -214,45 +221,51 @@
         if not len(nb_cpus) or \
            len(nb_cpus) and len(cpus) != len(nb_cpus):
             for x in nb_cpus:
                 x.delete()
 
             self.create_netbox_cpus()
 
-    def get_raid_cards(self):
+    def get_raid_cards(self, filter_cards=False):
         raid_class = None
-        if self.server.manufacturer == 'Dell':
+        if self.server.manufacturer in ('Dell', 'Huawei'):
             if is_tool('omreport'):
                 raid_class = OmreportRaid
             if is_tool('storcli'):
                 raid_class = StorcliRaid
-        elif self.server.manufacturer == 'HP':
+        elif self.server.manufacturer in ('HP', 'HPE'):
             if is_tool('ssacli'):
                 raid_class = HPRaid
 
         if not raid_class:
             return []
 
         self.raid = raid_class()
-        controllers = self.raid.get_controllers()
-        if len(self.raid.get_controllers()):
-            return controllers
+
+        if filter_cards and config.expansion_as_device \
+                and self.server.own_expansion_slot():
+            return [
+                c for c in self.raid.get_controllers()
+                if c.is_external() is self.update_expansion
+            ]
+        else:
+            return self.raid.get_controllers()
 
     def create_netbox_raid_card(self, raid_card):
         manufacturer = self.find_or_create_manufacturer(
             raid_card.get_manufacturer()
         )
 
         name = raid_card.get_product_name()
         serial = raid_card.get_serial_number()
         nb_raid_card = nb.dcim.inventory_items.create(
             device=self.device_id,
             discovered=True,
             manufacturer=manufacturer.id if manufacturer else None,
-            tags=[INVENTORY_TAG['raid_card']['name']],
+            tags=[{'name': INVENTORY_TAG['raid_card']['name']}],
             name='{}'.format(name),
             serial='{}'.format(serial),
             description='RAID Card',
         )
         logging.info('Creating RAID Card {name} (SN: {serial})'.format(
             name=name,
             serial=serial,
@@ -270,15 +283,15 @@
         We only need to handle destroy and new cards
         """
 
         nb_raid_cards = self.get_netbox_inventory(
             device_id=self.device_id,
             tag=[INVENTORY_TAG['raid_card']['slug']]
         )
-        raid_cards = self.get_raid_cards()
+        raid_cards = self.get_raid_cards(filter_cards=True)
 
         # delete cards that are in netbox but not locally
         # use the serial_number has the comparison element
         for nb_raid_card in nb_raid_cards:
             if nb_raid_card.serial not in [x.get_serial_number() for x in raid_cards]:
                 logging.info('Deleting unknown locally RAID Card {serial}'.format(
                     serial=nb_raid_card.serial,
@@ -286,130 +299,164 @@
                 nb_raid_card.delete()
 
         # create card that are not in netbox
         for raid_card in raid_cards:
             if raid_card.get_serial_number() not in [x.serial for x in nb_raid_cards]:
                 self.create_netbox_raid_card(raid_card)
 
-    def is_virtual_disk(self, disk):
+    def is_virtual_disk(self, disk, raid_devices):
+        disk_type = disk.get('type')
         logicalname = disk.get('logicalname')
         description = disk.get('description')
         size = disk.get('size')
         product = disk.get('product')
-
+        if logicalname in raid_devices or disk_type is None or product is None or description is None:
+            return True
         non_raid_disks = [
             'MR9361-8i',
         ]
 
-        if size is None and logicalname is None or \
-           'virtual' in product.lower() or 'logical' in product.lower() or \
+        if logicalname in raid_devices or \
            product in non_raid_disks or \
+           'virtual' in product.lower() or \
+           'logical' in product.lower() or \
+           'volume' in description.lower() or \
+           'dvd-ram' in description.lower() or \
            description == 'SCSI Enclosure' or \
-           'volume' in description.lower():
+           (size is None and logicalname is None):
             return True
         return False
 
     def get_hw_disks(self):
         disks = []
 
+        for raid_card in self.get_raid_cards(filter_cards=True):
+            disks.extend(raid_card.get_physical_disks())
+
+        raid_devices = [
+            d.get('custom_fields', {}).get('vd_device')
+            for d in disks
+            if d.get('custom_fields', {}).get('vd_device')
+        ]
+
         for disk in self.lshw.get_hw_linux("storage"):
-            if self.is_virtual_disk(disk):
+            if self.is_virtual_disk(disk, raid_devices):
                 continue
-
-            logicalname = disk.get('logicalname')
-            description = disk.get('description')
-            size = disk.get('size', 0)
-            product = disk.get('product')
-            serial = disk.get('serial')
-
-            d = {}
-            d["name"] = ""
-            d['Size'] = '{} GB'.format(int(size / 1024 / 1024 / 1024))
-            d['logicalname'] = logicalname
-            d['description'] = description
-            d['SN'] = serial
-            d['Model'] = product
+            size = int(getattr(disk, "size", 0)) / 1073741824
+            d = {
+                "name": "",
+                'Size': '{} GB'.format(size),
+                'logicalname': disk.get('logicalname'),
+                'description': disk.get('description'),
+                'SN': disk.get('serial'),
+                'Model': disk.get('product'),
+                'Type': disk.get('type'),
+            }
             if disk.get('vendor'):
                 d['Vendor'] = disk['vendor']
             else:
                 d['Vendor'] = get_vendor(disk['product'])
             disks.append(d)
 
-        for raid_card in self.get_raid_cards():
-            disks += raid_card.get_physical_disks()
-
         # remove duplicate serials
         seen = set()
         uniq = [x for x in disks if x['SN'] not in seen and not seen.add(x['SN'])]
         return uniq
 
     def create_netbox_disk(self, disk):
         manufacturer = None
         if "Vendor" in disk:
             manufacturer = self.find_or_create_manufacturer(disk["Vendor"])
 
         logicalname = disk.get('logicalname')
         desc = disk.get('description')
-        # nonraid disk
-        if logicalname and desc:
-            if type(logicalname) is list:
-                logicalname = logicalname[0]
-            name = '{} - {} ({})'.format(
-                desc,
-                logicalname,
-                disk.get('Size', 0))
-            description = 'Device {}'.format(disk.get('logicalname', 'Unknown'))
-        else:
-            name = '{} ({})'.format(disk['Model'], disk['Size'])
-            description = '{}'.format(disk['Type'])
+        name = '{} ({})'.format(disk['Model'], disk['Size'])
+        description = disk['Type']
+        sn = disk.get('SN', 'unknown')
+
+        parms = {
+            'device': self.device_id,
+            'discovered': True,
+            'tags': [{'name': INVENTORY_TAG['disk']['name']}],
+            'name': name,
+            'serial': sn,
+            'part_id': disk['Model'],
+            'description': description,
+            'manufacturer': getattr(manufacturer, "id", None),
+        }
+        if config.process_virtual_drives:
+            parms['custom_fields'] = disk.get("custom_fields", {})
 
-        _ = nb.dcim.inventory_items.create(
-            device=self.device_id,
-            discovered=True,
-            tags=[INVENTORY_TAG['disk']['name']],
-            name=name,
-            serial=disk['SN'],
-            part_id=disk['Model'],
-            description=description,
-            manufacturer=manufacturer.id if manufacturer else None
-        )
+        _ = nb.dcim.inventory_items.create(**parms)
 
         logging.info('Creating Disk {model} {serial}'.format(
             model=disk['Model'],
-            serial=disk['SN'],
+            serial=sn,
         ))
 
+    def dump_disks_map(self, disks):
+        disk_map = [d['custom_fields'] for d in disks if 'custom_fields' in d]
+        if config.dump_disks_map == "-":
+            f = sys.stdout
+        else:
+            f = open(config.dump_disks_map, "w")
+        f.write(
+            json.dumps(
+                disk_map,
+                separators=(',', ':'),
+                indent=4,
+                sort_keys=True
+            )
+        )
+        if config.dump_disks_map != "-":
+            f.close()
+
     def do_netbox_disks(self):
         nb_disks = self.get_netbox_inventory(
             device_id=self.device_id,
-            tag=INVENTORY_TAG['disk']['slug'])
+            tag=INVENTORY_TAG['disk']['slug']
+        )
         disks = self.get_hw_disks()
+        if config.dump_disks_map:
+            try:
+                self.dump_disks_map(disks)
+            except Exception as e:
+                logging.error("Failed to dump disks map: {}".format(e))
+                logging.debug(traceback.format_exc())
+        disk_serials = [d['SN'] for d in disks if 'SN' in d]
 
         # delete disks that are in netbox but not locally
         # use the serial_number has the comparison element
         for nb_disk in nb_disks:
-            if nb_disk.serial not in [x['SN'] for x in disks if x.get('SN')]:
+            if nb_disk.serial not in disk_serials or \
+                    config.force_disk_refresh:
                 logging.info('Deleting unknown locally Disk {serial}'.format(
                     serial=nb_disk.serial,
                 ))
                 nb_disk.delete()
 
+        if config.force_disk_refresh:
+            nb_disks = self.get_netbox_inventory(
+                device_id=self.device_id,
+                tag=INVENTORY_TAG['disk']['slug']
+            )
+
         # create disks that are not in netbox
         for disk in disks:
-            if disk.get('SN') not in [x.serial for x in nb_disks]:
+            if disk.get('SN') not in [d.serial for d in nb_disks]:
                 self.create_netbox_disk(disk)
 
     def create_netbox_memory(self, memory):
         manufacturer = self.find_or_create_manufacturer(memory['vendor'])
         name = 'Slot {} ({}GB)'.format(memory['slot'], memory['size'])
         nb_memory = nb.dcim.inventory_items.create(
             device=self.device_id,
             discovered=True,
             manufacturer=manufacturer.id,
-            tags=[INVENTORY_TAG['memory']['name']],
+            tags=[{'name': INVENTORY_TAG['memory']['name']}],
             name=name,
             part_id=memory['product'],
             serial=memory['serial'],
             description=memory['description'],
         )
 
         logging.info('Creating Memory {location} {type} {size}GB'.format(
@@ -434,17 +481,70 @@
                 ))
                 nb_memory.delete()
 
         for memory in memories:
             if memory.get('serial') not in [x.serial for x in nb_memories]:
                 self.create_netbox_memory(memory)
 
+    def create_netbox_gpus(self, gpus):
+        for gpu in gpus:
+            if 'product' in gpu and len(gpu['product']) > 50:
+                gpu['product'] = (gpu['product'][:48] + '..')
+
+            manufacturer = self.find_or_create_manufacturer(gpu["vendor"])
+            _ = nb.dcim.inventory_items.create(
+                device=self.device_id,
+                manufacturer=manufacturer.id,
+                discovered=True,
+                tags=[{'name': INVENTORY_TAG['gpu']['name']}],
+                name=gpu['product'],
+                description=gpu['description'],
+            )
+
+            logging.info('Creating GPU model {}'.format(gpu['product']))
+
+    def is_external_gpu(self, gpu):
+        is_3d_gpu = gpu['description'].startswith('3D')
+        return self.server.is_blade() and \
+            self.server.own_gpu_expansion_slot() and is_3d_gpu
+
+    def do_netbox_gpus(self):
+        gpus = []
+        gpu_models = {}
+        for gpu in  self.lshw.get_hw_linux('gpu'):
+            # Filters GPU if an expansion bay is detected:
+            # The internal (VGA) GPU only goes into the blade inventory,
+            # the external (3D) GPU goes into the expansion blade.
+            if config.expansion_as_device and \
+                    self.update_expansion ^ self.is_external_gpu(gpu):
+                continue
+            gpus.append(gpu)
+            gpu_models.setdefault(gpu["product"], 0)
+            gpu_models[gpu["product"]] += 1
+
+        nb_gpus = self.get_netbox_inventory(
+            device_id=self.device_id,
+            tag=INVENTORY_TAG['gpu']['slug'],
+        )
+        nb_gpu_models = {}
+        for gpu in nb_gpus:
+            nb_gpu_models.setdefault(str(gpu), 0)
+            nb_gpu_models[str(gpu)] += 1
+        up_to_date = set(gpu_models) == set(nb_gpu_models)
+        if not gpus or not up_to_date:
+            for x in nb_gpus:
+                x.delete()
+        if gpus and not up_to_date:
+            self.create_netbox_gpus(gpus)
+
     def create_or_update(self):
         if config.inventory is None or config.update_inventory is None:
             return False
-        self.do_netbox_cpus()
-        self.do_netbox_memories()
-        self.do_netbox_raid_cards()
+        if self.update_expansion is False:
+            self.do_netbox_cpus()
+            self.do_netbox_memories()
+            self.do_netbox_interfaces()
+            self.do_netbox_motherboard()
+        self.do_netbox_gpus()
         self.do_netbox_disks()
-        self.do_netbox_interfaces()
-        self.do_netbox_motherboard()
+        self.do_netbox_raid_cards()
         return True
```

### Comparing `netbox_agent-0.6.2/netbox_agent/ipmi.py` & `netbox_agent-0.7.1/netbox_agent/ipmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             if key not in ['802.1q VLAN ID', 'IP Address', 'Subnet Mask', 'MAC Address']:
                 continue
             value = ':'.join(line.split(':')[1:]).strip()
             _ipmi[key] = value
 
         ret = {}
         ret['name'] = 'IPMI'
+        ret["mtu"] = 1500
         ret['bonding'] = False
         ret['mac'] = _ipmi['MAC Address']
         ret['vlan'] = int(_ipmi['802.1q VLAN ID']) \
             if _ipmi['802.1q VLAN ID'] != 'Disabled' else None
         ip = _ipmi['IP Address']
         netmask = _ipmi['Subnet Mask']
         address = str(IPNetwork('{}/{}'.format(ip, netmask)))
```

### Comparing `netbox_agent-0.6.2/netbox_agent/lldp.py` & `netbox_agent-0.7.1/netbox_agent/lldp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import logging
 import subprocess
 
+from netbox_agent.misc import is_tool
+
 
 class LLDP():
     def __init__(self, output=None):
+        if not is_tool('lldpctl'):
+            logging.debug('lldpd package seems to be missing or daemon not running.')
         if output:
             self.output = output
         else:
             self.output = subprocess.getoutput('lldpctl -f keyvalue')
         self.data = self.parse()
 
     def parse(self):
@@ -36,21 +41,23 @@
                     vlans[interface][vid] = vlans[interface].get(vid, {})
                 elif 'pvid' in path:
                     vlans[interface][vid]['pvid'] = True
             if 'vlan' not in path:
                 current_dict[final] = value
         for interface, vlan in vlans.items():
             output_dict['lldp'][interface]['vlan'] = vlan
+        if not output_dict:
+            logging.debug('No LLDP output, please check your network config.')
         return output_dict
 
     def get_switch_ip(self, interface):
         # lldp.eth0.chassis.mgmt-ip=100.66.7.222
         if self.data['lldp'].get(interface) is None:
             return None
-        return self.data['lldp'][interface]['chassis']['mgmt-ip']
+        return self.data['lldp'][interface]['chassis'].get('mgmt-ip')
 
     def get_switch_port(self, interface):
         # lldp.eth0.port.descr=GigabitEthernet1/0/1
         if self.data['lldp'].get(interface) is None:
             return None
         if self.data['lldp'][interface]['port'].get('ifname'):
             return self.data['lldp'][interface]['port']['ifname']
```

### Comparing `netbox_agent-0.6.2/netbox_agent/location.py` & `netbox_agent-0.7.1/netbox_agent/location.py`

 * *Files identical despite different names*

### Comparing `netbox_agent-0.6.2/netbox_agent/network.py` & `netbox_agent-0.7.1/netbox_agent/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,21 @@
             if config.network.ignore_interfaces and \
                re.match(config.network.ignore_interfaces, interface):
                 logging.debug('Ignore interface {interface}'.format(interface=interface))
                 continue
 
             ip_addr = netifaces.ifaddresses(interface).get(netifaces.AF_INET, [])
             ip6_addr = netifaces.ifaddresses(interface).get(netifaces.AF_INET6, [])
+            if config.network.ignore_ips:
+                for i, ip in enumerate(ip_addr):
+                    if re.match(config.network.ignore_ips, ip['addr']):
+                        ip_addr.pop(i)
+                for i, ip in enumerate(ip6_addr):
+                    if re.match(config.network.ignore_ips, ip['addr']):
+                        ip6_addr.pop(i)
 
             # netifaces returns a ipv6 netmask that netaddr does not understand.
             # this strips the netmask down to the correct format for netaddr,
             # and remove the interface.
             # ie, this:
             #   {
             #      'addr': 'fe80::ec4:7aff:fe59:ec4a%eno1.50',
@@ -73,23 +80,20 @@
             #   }
             #
             for addr in ip6_addr:
                 addr["addr"] = addr["addr"].replace('%{}'.format(interface), '')
                 addr["netmask"] = addr["netmask"].split('/')[0]
                 ip_addr.append(addr)
 
-            if config.network.ignore_ips and ip_addr:
-                for i, ip in enumerate(ip_addr):
-                    if re.match(config.network.ignore_ips, ip['addr']):
-                        ip_addr.pop(i)
-
             mac = open('/sys/class/net/{}/address'.format(interface), 'r').read().strip()
+            mtu = int(open('/sys/class/net/{}/mtu'.format(interface), 'r').read().strip())
             vlan = None
             if len(interface.split('.')) > 1:
                 vlan = int(interface.split('.')[1])
+
             bonding = False
             bonding_slaves = []
             if os.path.isdir('/sys/class/net/{}/bonding'.format(interface)):
                 bonding = True
                 bonding_slaves = open(
                     '/sys/class/net/{}/bonding/slaves'.format(interface)
                 ).read().split()
@@ -107,14 +111,15 @@
                         x['addr'],
                         IPAddress(x['netmask']).netmask_bits()
                     ) for x in ip_addr
                 ] if ip_addr else None,  # FIXME: handle IPv6 addresses
                 'ethtool': Ethtool(interface).parse(),
                 'virtual': virtual,
                 'vlan': vlan,
+                'mtu': mtu,
                 'bonding': bonding,
                 'bonding_slaves': bonding_slaves,
             }
             nics.append(nic)
         return nics
 
     def _set_bonding_interfaces(self):
@@ -141,27 +146,27 @@
     def get_network_cards(self):
         return self.nics
 
     def get_netbox_network_card(self, nic):
         if nic['mac'] is None:
             interface = self.nb_net.interfaces.get(
                 name=nic['name'],
-                **self.custom_arg_id,
+                **self.custom_arg_id
             )
         else:
             interface = self.nb_net.interfaces.get(
                 mac_address=nic['mac'],
                 name=nic['name'],
-                **self.custom_arg_id,
+                **self.custom_arg_id
             )
         return interface
 
     def get_netbox_network_cards(self):
         return self.nb_net.interfaces.filter(
-            **self.custom_arg_id,
+            **self.custom_arg_id
         )
 
     def get_netbox_type_for_nic(self, nic):
         if self.get_network_type() == 'virtual':
             return self.dcim_choices['interface:type']['Virtual']
 
         if nic.get('bonding'):
@@ -173,22 +178,27 @@
         if nic.get('virtual'):
             return self.dcim_choices['interface:type']['Virtual']
 
         if nic.get('ethtool') is None:
             return self.dcim_choices['interface:type']['Other']
 
         if nic['ethtool']['speed'] == '10000Mb/s':
-            if nic['ethtool']['port'] == 'FIBRE':
+            if nic['ethtool']['port'] in ('FIBRE', 'Direct Attach Copper'):
                 return self.dcim_choices['interface:type']['SFP+ (10GE)']
             return self.dcim_choices['interface:type']['10GBASE-T (10GE)']
 
+        elif nic['ethtool']['speed'] == '25000Mb/s':
+            if nic['ethtool']['port'] in ('FIBRE', 'Direct Attach Copper'):
+                return self.dcim_choices['interface:type']['SFP28 (25GE)']
+
         elif nic['ethtool']['speed'] == '1000Mb/s':
-            if nic['ethtool']['port'] == 'FIBRE':
+            if nic['ethtool']['port'] in ('FIBRE', 'Direct Attach Copper'):
                 return self.dcim_choices['interface:type']['SFP (1GE)']
             return self.dcim_choices['interface:type']['1000BASE-T (1GE)']
+
         return self.dcim_choices['interface:type']['Other']
 
     def get_or_create_vlan(self, vlan_id):
         # FIXME: we may need to specify the datacenter
         # since users may have same vlan id in multiple dc
         vlan = nb.ipam.vlans.get(
             vid=vlan_id,
@@ -200,39 +210,46 @@
             )
         return vlan
 
     def reset_vlan_on_interface(self, nic, interface):
         update = False
         vlan_id = nic['vlan']
         lldp_vlan = self.lldp.get_switch_vlan(nic['name']) if config.network.lldp else None
+        # For strange reason, we need to get the object from scratch
+        # The object returned by pynetbox's save isn't always working (since pynetbox 6)
+        interface = self.nb_net.interfaces.get(id=interface.id)
 
-        # if local interface isn't a interface vlan or lldp doesn't report a vlan-id
+        # Handle the case were the local interface isn't an interface vlan as reported by Netbox
+        # and that LLDP doesn't report a vlan-id
         if vlan_id is None and lldp_vlan is None and \
            (interface.mode is not None or len(interface.tagged_vlans) > 0):
             logging.info('Interface {interface} is not tagged, reseting mode'.format(
                 interface=interface))
             update = True
             interface.mode = None
             interface.tagged_vlans = []
             interface.untagged_vlan = None
-        # if it's a vlan interface
+        # if the local interface is configured with a vlan, it's supposed to be taggued
+        # if mode is either not set or not correctly configured or vlan are not
+        # correctly configured, we reset the vlan
         elif vlan_id and (
                 interface.mode is None or
                 type(interface.mode) is not int and (
+                    hasattr(interface.mode, 'value') and
                     interface.mode.value == self.dcim_choices['interface:mode']['Access'] or
                     len(interface.tagged_vlans) != 1 or
-                    interface.tagged_vlans[0].vid != vlan_id)):
+                    int(interface.tagged_vlans[0].vid) != int(vlan_id))):
             logging.info('Resetting tagged VLAN(s) on interface {interface}'.format(
                 interface=interface))
             update = True
             nb_vlan = self.get_or_create_vlan(vlan_id)
             interface.mode = self.dcim_choices['interface:mode']['Tagged']
             interface.tagged_vlans = [nb_vlan] if nb_vlan else []
             interface.untagged_vlan = None
-        # if lldp reports a vlan-id with pvid
+        # Finally if LLDP reports a vlan-id with the pvid attribute
         elif lldp_vlan:
             pvid_vlan = [key for (key, value) in lldp_vlan.items() if value['pvid']]
             if len(pvid_vlan) > 0 and (
                     interface.mode is None or
                     interface.mode.value != self.dcim_choices['interface:mode']['Access'] or
                     interface.untagged_vlan is None or
                     interface.untagged_vlan.vid != int(pvid_vlan[0])):
@@ -242,35 +259,37 @@
                 nb_vlan = self.get_or_create_vlan(pvid_vlan[0])
                 interface.mode = self.dcim_choices['interface:mode']['Access']
                 interface.untagged_vlan = nb_vlan.id
         return update, interface
 
     def create_netbox_nic(self, nic, mgmt=False):
         # TODO: add Optic Vendor, PN and Serial
-        type = self.get_netbox_type_for_nic(nic)
+        nic_type = self.get_netbox_type_for_nic(nic)
         logging.info('Creating NIC {name} ({mac}) on {device}'.format(
             name=nic['name'], mac=nic['mac'], device=self.device.name))
 
         nb_vlan = None
 
-        params = {
+        params = dict(self.custom_arg)
+        params.update({
             'name': nic['name'],
-            'type': type,
+            'type': nic_type,
             'mgmt_only': mgmt,
-            **self.custom_arg,
-        }
-
-        if not nic.get('virtual', False):
+        })
+        if nic['mac']:
             params['mac_address'] = nic['mac']
 
+        if nic['mtu']:
+            params['mtu'] = nic['mtu']
+
         interface = self.nb_net.interfaces.create(**params)
 
         if nic['vlan']:
             nb_vlan = self.get_or_create_vlan(nic['vlan'])
-            interface.mode = 200
+            interface.mode = self.dcim_choices['interface:mode']['Tagged']
             interface.tagged_vlans = [nb_vlan.id]
             interface.save()
         elif config.network.lldp and self.lldp.get_switch_vlan(nic['name']) is not None:
             # if lldp reports a vlan on an interface, tag the interface in access and set the vlan
             # report only the interface which has `pvid=yes` (ie: lldp.eth3.vlan.pvid=yes)
             # if pvid is not present, it'll be processed as a vlan tagged interface
             vlans = self.lldp.get_switch_vlan(nic['name'])
@@ -306,95 +325,112 @@
         * If IP doesn't exist, create it
         * If IP exists and isn't assigned, take it
         * If IP exists and interface is wrong, change interface
         '''
         netbox_ips = nb.ipam.ip_addresses.filter(
             address=ip,
         )
-        if not len(netbox_ips):
+        if not netbox_ips:
             logging.info('Create new IP {ip} on {interface}'.format(
                 ip=ip, interface=interface))
+            query_params = {
+                'address': ip,
+                'status': "active",
+                'assigned_object_type': self.assigned_object_type,
+                'assigned_object_id': interface.id
+            }
+
             netbox_ip = nb.ipam.ip_addresses.create(
-                address=ip,
-                interface=interface.id,
-                status=1,
+                **query_params
             )
-        else:
-            netbox_ip = netbox_ips[0]
-            # If IP exists in anycast
-            if netbox_ip.role and netbox_ip.role.label == 'Anycast':
-                logging.debug('IP {} is Anycast..'.format(ip))
-                unassigned_anycast_ip = [x for x in netbox_ips if x.interface is None]
-                assigned_anycast_ip = [x for x in netbox_ips if
-                                       x.interface and x.interface.id == interface.id]
-                # use the first available anycast ip
-                if len(unassigned_anycast_ip):
-                    logging.info('Assigning existing Anycast IP {} to interface'.format(ip))
-                    netbox_ip = unassigned_anycast_ip[0]
-                    netbox_ip.interface = interface
-                    netbox_ip.save()
-                # or if everything is assigned to other servers
-                elif not len(assigned_anycast_ip):
-                    logging.info('Creating Anycast IP {} and assigning it to interface'.format(ip))
-                    netbox_ip = nb.ipam.ip_addresses.create(
-                        address=ip,
-                        interface=interface.id,
-                        status=1,
-                        role=self.ipam_choices['ip-address:role']['Anycast'],
-                        tenant=self.tenant.id if self.tenant else None,
-                    )
-                return netbox_ip
-            else:
-                if netbox_ip.interface is None:
-                    logging.info('Assigning existing IP {ip} to {interface}'.format(
-                        ip=ip, interface=interface))
-                elif netbox_ip.interface.id != interface.id:
-                    logging.info(
-                        'Detected interface change for ip {ip}: old interface is '
-                        '{old_interface} (id: {old_id}), new interface is {new_interface} '
-                        ' (id: {new_id})'
-                        .format(
-                            old_interface=netbox_ip.interface, new_interface=interface,
-                            old_id=netbox_ip.id, new_id=interface.id, ip=netbox_ip.address
-                        ))
-                else:
-                    return netbox_ip
+            return netbox_ip
+
+        netbox_ip = list(netbox_ips)[0]
+        # If IP exists in anycast
+        if netbox_ip.role and netbox_ip.role.label == 'Anycast':
+            logging.debug('IP {} is Anycast..'.format(ip))
+            unassigned_anycast_ip = [x for x in netbox_ips if x.interface is None]
+            assigned_anycast_ip = [x for x in netbox_ips if
+                                   x.interface and x.interface.id == interface.id]
+            # use the first available anycast ip
+            if len(unassigned_anycast_ip):
+                logging.info('Assigning existing Anycast IP {} to interface'.format(ip))
+                netbox_ip = unassigned_anycast_ip[0]
                 netbox_ip.interface = interface
                 netbox_ip.save()
-        return netbox_ip
+            # or if everything is assigned to other servers
+            elif not len(assigned_anycast_ip):
+                logging.info('Creating Anycast IP {} and assigning it to interface'.format(ip))
+                query_params = {
+                    "address": ip,
+                    "status": "active",
+                    "role": self.ipam_choices['ip-address:role']['Anycast'],
+                    "tenant": self.tenant.id if self.tenant else None,
+                    "assigned_object_type": self.assigned_object_type,
+                    "assigned_object_id": interface.id
+                }
+                netbox_ip = nb.ipam.ip_addresses.create(**query_params)
+            return netbox_ip
+        else:
+            ip_interface = getattr(netbox_ip, 'interface', None)
+            assigned_object = getattr(netbox_ip, 'assigned_object', None)
+            if not ip_interface or not assigned_object:
+                logging.info('Assigning existing IP {ip} to {interface}'.format(
+                    ip=ip, interface=interface))
+            elif (ip_interface and ip_interface.id != interface.id) or \
+                 (assigned_object and assigned_object_id != interface.id):
+
+                old_interface = getattr(netbox_ip, "assigned_object", "n/a")
+                logging.info(
+                    'Detected interface change for ip {ip}: old interface is '
+                    '{old_interface} (id: {old_id}), new interface is {new_interface} '
+                    ' (id: {new_id})'
+                    .format(
+                        old_interface=old_interface, new_interface=interface,
+                        old_id=netbox_ip.id, new_id=interface.id, ip=netbox_ip.address
+                    ))
+            else:
+                return netbox_ip
+
+            netbox_ip.assigned_object_type = self.assigned_object_type
+            netbox_ip.assigned_object_id = interface.id
+            netbox_ip.save()
 
     def create_or_update_netbox_network_cards(self):
         if config.update_all is None or config.update_network is None:
             return None
         logging.debug('Creating/Updating NIC...')
 
         # delete unknown interface
-        nb_nics = self.get_netbox_network_cards()
+        nb_nics = list(self.get_netbox_network_cards())
         local_nics = [x['name'] for x in self.nics]
-        for nic in nb_nics[:]:
+        for nic in nb_nics:
             if nic.name not in local_nics:
                 logging.info('Deleting netbox interface {name} because not present locally'.format(
                     name=nic.name
                 ))
                 nb_nics.remove(nic)
                 nic.delete()
 
         # delete IP on netbox that are not known on this server
         if len(nb_nics):
             netbox_ips = nb.ipam.ip_addresses.filter(
-                interface_id=[x.id for x in nb_nics],
+                **{self.intf_type: [x.id for x in nb_nics]}
             )
+
+            netbox_ips = list(netbox_ips)
             all_local_ips = list(chain.from_iterable([
                 x['ip'] for x in self.nics if x['ip'] is not None
             ]))
             for netbox_ip in netbox_ips:
                 if netbox_ip.address not in all_local_ips:
                     logging.info('Unassigning IP {ip} from {interface}'.format(
-                        ip=netbox_ip.address, interface=netbox_ip.interface))
-                    netbox_ip.interface = None
+                        ip=netbox_ip.address, interface=netbox_ip.assigned_object))
+                    netbox_ip.assigned_object_type = None
+                    netbox_ip.assigned_object_id = None
                     netbox_ip.save()
 
         # update each nic
         for nic in self.nics:
             interface = self.get_netbox_network_card(nic)
             if not interface:
                 logging.info('Interface {mac_address} not found, creating..'.format(
@@ -408,20 +444,28 @@
                     interface=interface, name=nic['name']))
                 interface.name = nic['name']
                 nic_update += 1
 
             ret, interface = self.reset_vlan_on_interface(nic, interface)
             nic_update += ret
 
-            _type = self.get_netbox_type_for_nic(nic)
-            if not interface.type or \
-               _type != interface.type.value:
-                logging.info('Interface type is wrong, resetting')
-                interface.type = _type
-                nic_update += 1
+            if hasattr(interface, 'mtu'):
+                if nic['mtu'] != interface.mtu:
+                    logging.info('Interface mtu is wrong, updating to: {mtu}'.format(
+                        mtu=nic['mtu']))
+                    interface.mtu = nic['mtu']
+                    nic_update += 1
+
+            if hasattr(interface, 'type'):
+                _type = self.get_netbox_type_for_nic(nic)
+                if not interface.type or \
+                   _type != interface.type.value:
+                    logging.info('Interface type is wrong, resetting')
+                    interface.type = _type
+                    nic_update += 1
 
             if hasattr(interface, 'lag') and interface.lag is not None:
                 local_lag_int = next(
                     item for item in self.nics if item['name'] == interface.lag.name
                 )
                 if nic['name'] not in local_lag_int['bonding_slaves']:
                     logging.info('Interface has no LAG, resetting')
@@ -448,22 +492,27 @@
         self._set_bonding_interfaces()
         logging.debug('Finished updating NIC!')
 
 
 class ServerNetwork(Network):
     def __init__(self, server, *args, **kwargs):
         super(ServerNetwork, self).__init__(server, args, kwargs)
-        self.ipmi = self.get_ipmi()
+
+        if config.network.ipmi:
+            self.ipmi = self.get_ipmi()
         if self.ipmi:
             self.nics.append(self.ipmi)
+
         self.server = server
         self.device = self.server.get_netbox_server()
         self.nb_net = nb.dcim
         self.custom_arg = {'device': getattr(self.device, "id", None)}
         self.custom_arg_id = {'device_id': getattr(self.device, "id", None)}
+        self.intf_type = "interface_id"
+        self.assigned_object_type = "dcim.interface"
 
     def get_network_type(self):
         return 'server'
 
     def get_ipmi(self):
         ipmi = IPMI().parse()
         return ipmi
@@ -476,15 +525,15 @@
             address=switch_ip,
         )
         if not nb_mgmt_ip:
             logging.error('Switch IP {} cannot be found in Netbox'.format(switch_ip))
             return nb_server_interface
 
         try:
-            nb_switch = nb_mgmt_ip.interface.device
+            nb_switch = nb_mgmt_ip.assigned_object.device
             logging.info('Found a switch in Netbox based on LLDP infos: {} (id: {})'.format(
                 switch_ip,
                 nb_switch.id
             ))
         except KeyError:
             logging.error(
                 'Switch IP {} is found but not associated to a Netbox Switch Device'.format(
@@ -576,14 +625,16 @@
     def __init__(self, server, *args, **kwargs):
         super(VirtualNetwork, self).__init__(server, args, kwargs)
         self.server = server
         self.device = self.server.get_netbox_vm()
         self.nb_net = nb.virtualization
         self.custom_arg = {'virtual_machine': getattr(self.device, "id", None)}
         self.custom_arg_id = {'virtual_machine_id': getattr(self.device, "id", None)}
+        self.intf_type = "vminterface_id"
+        self.assigned_object_type = "virtualization.vminterface"
 
         dcim_c = nb.virtualization.interfaces.choices()
         for _choice_type in dcim_c:
             key = 'interface:{}'.format(_choice_type)
             self.dcim_choices[key] = {}
             for choice in dcim_c[_choice_type]:
                 self.dcim_choices[key][choice['display_name']] = choice['value']
```

### Comparing `netbox_agent-0.6.2/netbox_agent/power.py` & `netbox_agent-0.7.1/netbox_agent/power.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def get_netbox_power_supply(self):
         return nb.dcim.power_ports.filter(
             device_id=self.device_id
         )
 
     def create_or_update_power_supply(self):
-        nb_psus = self.get_netbox_power_supply()
+        nb_psus = list(self.get_netbox_power_supply())
         psus = self.get_power_supply()
 
         # Delete unknown PSU
         delete = False
         for nb_psu in nb_psus:
             if nb_psu.name not in [x['name'] for x in psus]:
                 logging.info('Deleting unknown locally PSU {name}'.format(
@@ -101,26 +101,31 @@
             return False
         nb_psus = self.get_netbox_power_supply()
 
         if not len(nb_psus) or not len(psu_cons):
             return False
 
         # find power feeds for rack or dc
-        voltage = None
         pwr_feeds = None
         if self.netbox_server.rack:
             pwr_feeds = nb.dcim.power_feeds.filter(
                 rack=self.netbox_server.rack.id
             )
-        if pwr_feeds is None or not len(pwr_feeds):
+
+        if pwr_feeds:
+            voltage = [p['voltage'] for p in pwr_feeds]
+        else:
             logging.info('Could not find power feeds for Rack, defaulting value to 230')
-            voltage = 230
+            voltage = [230 for _ in nb_psus]
 
         for i, nb_psu in enumerate(nb_psus):
-            nb_psu.allocated_draw = float(psu_cons[i]) * voltage
+            nb_psu.allocated_draw = int(float(psu_cons[i]) * voltage[i])
+            if nb_psu.allocated_draw < 1:
+                logging.info('PSU is not connected or in standby mode')
+                continue
             nb_psu.save()
             logging.info('Updated power consumption for PSU {}: {}W'.format(
                 nb_psu.name,
                 nb_psu.allocated_draw,
             ))
 
         return True
```

### Comparing `netbox_agent-0.6.2/netbox_agent/vendors/dell.py` & `netbox_agent-0.7.1/netbox_agent/vendors/dell.py`

 * *Files 21% similar despite different names*

```diff
@@ -63,7 +63,26 @@
                 if line.startswith('PS'):
                     amp_value = line.split(':')[1].split()[0]
                     value.append(amp_value)
                 else:
                     break
 
         return value
+
+    def get_expansion_product(self):
+        """
+        Get the extension slot that is on a pair slot number
+        next to the compute slot that is on an odd slot number
+        """
+        raise NotImplementedError
+
+    def is_expansion_slot(self, server):
+        """
+        Return True if its an extension slot
+        """
+        raise NotImplementedError
+
+    def get_blade_expansion_slot(self):
+        """
+        Expansion slot are always the compute bay number + 1
+        """
+        raise NotImplementedError
```

### Comparing `netbox_agent-0.6.2/netbox_agent/vendors/generic.py` & `netbox_agent-0.7.1/netbox_agent/vendors/generic.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class GenericHost(ServerBase):
     def __init__(self, *args, **kwargs):
         super(GenericHost, self).__init__(*args, **kwargs)
         self.manufacturer = dmidecode.get_by_type(self.dmi, 'Baseboard')[0].get('Manufacturer')
 
     def is_blade(self):
-        return None
+        return False
 
     def get_blade_slot(self):
         return None
 
     def get_chassis_name(self):
         return None
```

### Comparing `netbox_agent-0.6.2/netbox_agent/vendors/hp.py` & `netbox_agent-0.7.1/netbox_agent/vendors/supermicro.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,79 @@
-import netbox_agent.dmidecode as dmidecode
+from netbox_agent.location import Slot
 from netbox_agent.server import ServerBase
 
 
-class HPHost(ServerBase):
+class SupermicroHost(ServerBase):
+    """
+     Supermicro DMI can be messed up.  They depend on the vendor
+     to set the correct values.  The endusers cannot
+     change them without buying a license from Supermicro.
+
+     There are 3 serial numbers in the system
+
+       1) System - this is used for the chassis information.
+       2) Baseboard - this is used for the blade.
+       3) Chassis - this is ignored.
+
+    """
+
     def __init__(self, *args, **kwargs):
-        super(HPHost, self).__init__(*args, **kwargs)
-        self.manufacturer = "HP"
-        self.product = self.get_product_name()
-        if self.is_blade():
-            self.hp_rack_locator = self._find_rack_locator()
+        super(SupermicroHost, self).__init__(*args, **kwargs)
+        self.manufacturer = 'Supermicro'
 
     def is_blade(self):
-        if self.product.startswith("ProLiant BL"):
-            return True
-        elif self.product.startswith("ProLiant m") and self.product.endswith("Server Cartridge"):
-            return True
-        else:
-            return False
+        product_name = self.system[0]['Product Name'].strip()
+        # Blades
+        blade = product_name.startswith('SBI')
+        blade |= product_name.startswith('SBA')
+        # Twin
+        blade |= 'TR-' in product_name
+        # TwinPro
+        blade |= 'TP-' in product_name
+        # BigTwin
+        blade |= 'BT-' in product_name
+        # Microcloud
+        blade |= product_name.startswith('SYS-5039')
+        blade |= product_name.startswith('SYS-5038')
+        return blade
 
-    def _find_rack_locator(self):
-        """
-        Depending on the server, the type of the `HP ProLiant System/Rack Locator`
-        can change.
-        So we need to find it every time
-        """
-        # FIXME: make a dmidecode function get_by_dminame() ?
+    def get_blade_slot(self):
         if self.is_blade():
-            locator = dmidecode.get_by_type(self.dmi, 204)
-            if self.product == "ProLiant BL460c Gen10":
-                locator = locator[0]["Strings"]
-                return {
-                    "Enclosure Model": locator[2].strip(),
-                    "Enclosure Name": locator[0].strip(),
-                    "Server Bay": locator[3].strip(),
-                    "Enclosure Serial": locator[4].strip(),
-                }
-
-            # HP ProLiant m750, m710x, m510 Server Cartridge
-            if self.product.startswith("ProLiant m") and self.product.endswith("Server Cartridge"):
-                locator = dmidecode.get_by_type(self.dmi, 2)
-                chassis = dmidecode.get_by_type(self.dmi, 3)
-                return {
-                    "Enclosure Model": "Moonshot 1500 Chassis",
-                    "Enclosure Name": "Unknown",
-                    "Server Bay": locator[0]["Location In Chassis"].strip(),
-                    "Enclosure Serial": chassis[0]["Serial Number"].strip(),
-                }
+            # Some Supermicro servers don't report the slot in dmidecode
+            # let's use a regex
+            slot = Slot()
+            return slot.get()
+        # No supermicro on hands
+        return None
 
-            return locator[0]
+    def get_service_tag(self):
+        if self.is_blade():
+            return self.baseboard[0]['Serial Number'].strip()
+        return self.system[0]['Serial Number'].strip()
 
-    def get_blade_slot(self):
+    def get_product_name(self):
         if self.is_blade():
-            return "Bay {}".format(str(self.hp_rack_locator["Server Bay"].strip()))
-        return None
+            return self.baseboard[0]['Product Name'].strip()
+        return self.system[0]['Product Name'].strip()
 
     def get_chassis(self):
         if self.is_blade():
-            return self.hp_rack_locator["Enclosure Model"].strip()
+            return self.system[0]['Product Name'].strip()
         return self.get_product_name()
 
+    def get_chassis_service_tag(self):
+        if self.is_blade():
+            return self.system[0]['Serial Number'].strip()
+        return self.get_service_tag()
+
     def get_chassis_name(self):
         if not self.is_blade():
             return None
-        return self.hp_rack_locator["Enclosure Name"].strip()
+        return 'Chassis {}'.format(self.get_chassis_service_tag())
 
-    def get_chassis_service_tag(self):
-        if self.is_blade():
-            return self.hp_rack_locator["Enclosure Serial"].strip()
-        return self.get_service_tag()
+    def get_expansion_product(self):
+        """
+        Get the extension slot that is on a pair slot number
+        next to the compute slot that is on an odd slot number
+        I only know on model of slot GPU extension card that.
+        """
+        raise NotImplementedError
```

### Comparing `netbox_agent-0.6.2/netbox_agent/vendors/qct.py` & `netbox_agent-0.7.1/netbox_agent/vendors/qct.py`

 * *Files identical despite different names*

### Comparing `netbox_agent-0.6.2/netbox_agent/virtualmachine.py` & `netbox_agent-0.7.1/netbox_agent/virtualmachine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import os
 
 import netbox_agent.dmidecode as dmidecode
 from netbox_agent.config import config
 from netbox_agent.config import netbox_instance as nb
 from netbox_agent.location import Tenant
 from netbox_agent.logging import logging  # NOQA
-from netbox_agent.misc import create_netbox_tags, get_hostname
+from netbox_agent.misc import create_netbox_tags, get_hostname, get_device_platform
 from netbox_agent.network import VirtualNetwork
 
 
 def is_vm(dmi):
-    bios = dmidecode.get_by_type(dmi, 'BIOS')
-    system = dmidecode.get_by_type(dmi, 'System')
+    bios = dmidecode.get_by_type(dmi, 'BIOS')[0]
+    system = dmidecode.get_by_type(dmi, 'System')[0]
 
-    if 'Hyper-V' in bios[0]['Version'] or \
-       'Xen' in bios[0]['Version'] or \
-       'Google Compute Engine' in system[0]['Product Name'] or \
-       'RHEV Hypervisor' in system[0]['Product Name'] or \
-       'VirtualBox' in bios[0]['Version'] or \
-       'VMware' in system[0]['Manufacturer']:
-        return True
-    return False
+    return (
+        (
+            'Hyper-V' in bios['Version'] or
+            'Xen' in bios['Version'] or
+            'Google Compute Engine' in system['Product Name']
+        ) or
+        (
+            (
+                'Amazon EC2' in system['Manufacturer'] and
+                not system['Product Name'].endswith('.metal')
+            ) or
+            'RHEV Hypervisor' in system['Product Name'] or
+            'QEMU' in system['Manufacturer'] or
+            'VirtualBox' in bios['Version'] or
+            'VMware' in system['Manufacturer']
+        )
+    )
 
 
 class VirtualMachine(object):
     def __init__(self, dmi=None):
         if dmi:
             self.dmi = dmi
         else:
             self.dmi = dmidecode.parse()
         self.network = None
+        self.device_platform = get_device_platform(config.device.platform)
 
         self.tags = list(set(config.device.tags.split(','))) if config.device.tags else []
         if self.tags and len(self.tags):
             create_netbox_tags(self.tags)
 
     def get_memory(self):
         mem_bytes = os.sysconf('SC_PAGE_SIZE') * os.sysconf('SC_PHYS_PAGES')  # e.g. 4015976448
@@ -89,14 +99,15 @@
         if not vm:
             logging.debug('Creating Virtual machine..')
             cluster = self.get_netbox_cluster(config.virtual.cluster_name)
 
             vm = nb.virtualization.virtual_machines.create(
                 name=hostname,
                 cluster=cluster.id,
+                platform=self.device_platform.id,
                 vcpus=vcpus,
                 memory=memory,
                 tenant=tenant.id if tenant else None,
                 tags=self.tags,
             )
             created = True
 
@@ -109,10 +120,13 @@
                 updated += 1
             if vm.memory != memory:
                 vm.memory = memory
                 updated += 1
             if sorted(set(vm.tags)) != sorted(set(self.tags)):
                 vm.tags = self.tags
                 updated += 1
+            if vm.platform != self.device_platform:
+                vm.platform = self.device_platform
+                updated += 1
 
         if updated:
             vm.save()
```

### Comparing `netbox_agent-0.6.2/netbox_agent.egg-info/PKG-INFO` & `netbox_agent-0.7.1/netbox_agent.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,274 +1,308 @@
 Metadata-Version: 2.1
 Name: netbox-agent
-Version: 0.6.2
+Version: 0.7.1
 Summary: NetBox agent for server
 Home-page: https://github.com/solvik/netbox_agent
 Author: Solvik Blum
 Author-email: solvik@solvik.fr
 License: Apache2
-Description: # Netbox agent [![Build Status](https://travis-ci.com/Solvik/netbox-agent.svg?branch=master)](https://travis-ci.com/Solvik/netbox-agent)
-        
-        This project aims to create hardware automatically into [Netbox](https://github.com/netbox-community/netbox) based on standard tools (dmidecode, lldpd, parsing /sys/, etc).
-        
-        The goal is to generate an existing infrastructure on Netbox and have the ability to update it regularly by executing the agent.
-        
-        # Features
-        
-        * Create virtual machines, servers, chassis and blade through standard tools (`dmidecode`)
-        * Create physical, bonding and vlan network interfaces with IPs (IPv4 & IPv6)
-        * Create IPMI interface if found
-        * Create or get existing VLAN and associate it to interfaces
-        * Generic ability to guess datacenters and rack location through drivers (`cmd` and `file` and custom ones)
-        * Update existing `Device` and `Interface`
-        * Handle blade moving (new slot, new chassis)
-        * Automatic cabling (server's interface to switch's interface) using lldp
-        * Local inventory using `Inventory Item` for CPU, RAM, RAID cards, physical disks (behind raid cards)
-        * PSUs creation and power consumption reporting (based on vendor's tools)
-        
-        # Requirements
-        
-        - Netbox >= 2.6
-        - Python >= 3.4
-        - [pynetbox](https://github.com/digitalocean/pynetbox/)
-        - [python3-netaddr](https://github.com/drkjam/netaddr)
-        - [python3-netifaces](https://github.com/al45tair/netifaces)
-        - [jsonargparse](https://github.com/omni-us/jsonargparse/)
-        
-        - ethtool
-        - dmidecode
-        - ipmitool
-        - lldpd
-        - lshw
-        
-        ## Inventory requirement
-        - hpassacli
-        - storcli
-        - omreport
-        
-        # Installation
-        
-        ```
-        # pip3 install netbox-agent
-        ```
-        
-        # Usage
-        
-        The agent can be run from a shell and get its configuration from either the configuration file or environment variables.
-        
-        Configuration values are overridden based on the following precedence: command line arguments (might include config file) > environment variables > default config file > defaults.
-        
-        ```
-        # netbox_agent -c /etc/netbox_agent.yml --register
-        INFO:root:Creating chassis blade (serial: QTFCQ574502EF)
-        INFO:root:Creating blade (serial: QTFCQ574502D2) myserver on chassis QTFCQ574502EF
-        INFO:root:Setting device (QTFCQ574502D2) new slot on Slot 9 (Chassis QTFCQ574502EF)..
-        INFO:root:Interface a8:1e:84:f2:9e:6a not found, creating..
-        INFO:root:Creating NIC enp1s0f1 (a8:1e:84:f2:9e:6a) on myserver
-        INFO:root:Interface 02:42:7a:89:cf:a4 not found, creating..
-        INFO:root:Creating NIC br-07ea1e4a2f0e (02:42:7a:89:cf:a4) on myserver
-        INFO:root:Create new IP 172.19.0.1/16 on br-07ea1e4a2f0e
-        INFO:root:Interface a8:1e:84:f2:9e:69 not found, creating..
-        INFO:root:Creating NIC enp1s0f0 (a8:1e:84:f2:9e:69) on myserver
-        INFO:root:Create new IP 42.42.42.42/24 on enp1s0f0
-        INFO:root:Create new IP fe80::aa1e:84ff:fef2:9e69/64 on enp1s0f0
-        INFO:root:Interface a8:1e:84:cd:9d:d6 not found, creating..
-        INFO:root:Creating NIC IPMI (a8:1e:84:cd:9d:d6) on myserver
-        INFO:root:Create new IP 10.191.122.10/24 on IPMI
-        ```
-        
-        If you need, you can update only specific informations like:
-        * Network
-        * Inventory
-        * Location
-        * PSUs
-        
-        ```
-        # ip a add 42.42.42.43/24 dev enp1s0f1
-        # netbox_agent -c /etc/netbox_agent.yaml --update-network
-        INFO:root:Create new IP 42.42.42.43/24 on enp1s0f1
-        # netbox_agent --update-inventory
-        INFO:root:Creating Disk Samsung SSD 850 S2RBNX0K101698D
-        ```
-        
-        # Configuration
-        
-        ```
-        # Netbox configuration
-        netbox:
-         url: 'http://netbox.internal.company.com'
-         token: supersecrettoken
-         # uncomment to disable ssl verification
-         # ssl_verify: false
-        
-        # Network configuration
-        network:
-          # Regex to ignore interfaces 
-          ignore_interfaces: "(dummy.*|docker.*)"
-          # Regex to ignore IP addresses
-          ignore_ips: (127\.0\.0\..*)
-          # enable auto-cabling by parsing LLDP answers
-          lldp: true
-        
-        #
-        # You can use these to change the Netbox roles.
-        # These are the defaults.
-        #
-        #device:
-        # chassis_role: "Server Chassis"
-        # blade_role: "Blade"
-        # server_role: "Server"
-        # tags: server, blade, ,just a comma,delimited,list
-        #￼
-        #
-        # Can use this to set the tenant
-        #
-        #tenant:
-        # driver: "file:/tmp/tenant"
-        # regex: "(.*)"
-        ￼
-        ## Enable virtual machine support 
-        # virtual:
-        #   # not mandatory, can be guessed
-        #   enabled: True
-        #   # see https://netbox.company.com/virtualization/clusters/
-        #   cluster_name: my_vm_cluster
-        
-        # Enable datacenter location feature in Netbox
-        datacenter_location:
-         driver: "cmd:cat /etc/qualification | tr [A-Z] [a-z]"
-         regex: "datacenter: (?P<datacenter>[A-Za-z0-9]+)"
-        # driver: 'cmd:lldpctl'
-        # regex: 'SysName: .*\.([A-Za-z0-9]+)'
-        #
-        # driver: "file:/tmp/datacenter"
-        # regex: "(.*)"
-        
-        # Enable rack location feature in Netbox
-        rack_location:
-        # driver: 'cmd:lldpctl'
-        # match SysName: sw-dist-a1.dc42
-        # regex: 'SysName:[ ]+[A-Za-z]+-[A-Za-z]+-([A-Za-z0-9]+)'
-        #
-        # driver: "file:/tmp/datacenter"
-        # regex: "(.*)"
-        
-        # Enable local inventory reporting 
-        inventory: true
-        ```
-        
-        # Specific workflow
-        
-        ## Blades
-        
-        Each vendor class has a `is_blade` method which is later used for `Device` creation using the Netbox [parent/child feature](https://netbox.readthedocs.io/en/stable/core-functionality/devices/).
-        
-        The `get_blade_slot` method return the name of the `Device Bay`.
-        
-        
-        Certain vendors don't report the blade slot in `dmidecode`, so we can use the `slot_location` regex feature of the configuration file.
-        
-        ## Anycast IP
-        
-        The default behavior of the agent is to assign an interface to an IP.
-        So two servers with anycasted IPs, running update mode, would only trigger IP's interface assignement in a loop.
-        
-        In order to handle this case, user need to set Netbox IP's mode to `Anycast` so that the agent will create another one if it's present on another server.
-        
-        # Hardware
-        
-        Tested on:
-        
-        ## Virtual Machines
-        
-        * Hyper-V
-        * VMWare
-        * VirtualBox
-        * AWS
-        * GCP
-        
-        ## [Dell Inc.](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/dell.py)
-        
-        ### Blades
-        
-        * PowerEdge MX7000
-        * PowerEdge M1000e (your `DeviceType` should have slots named `Slot 01` and so on)
-        * PowerEdge MX740c
-        * PowerEdge M640
-        * PowerEdge M630
-        * PowerEdge M620
-        * PowerEdge M610
-        
-        ### Pizzas
-        
-        * DSS7500
-        
-        ## [HP / HPE](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/hp.py)
-        
-        ### Blades
-        
-        * HP BladeSystem c7000 Enclosure G2 / G3 (your `DeviceType` should have slots named `Bay 1` and so on)
-        * HP ProLiant BL460c Gen8
-        * HP ProLiant BL460c Gen9
-        * HP ProLiant BL460c Gen10
-        * HP Moonshot 1500 Enclosure (your `DeviceType` should have slots batch create with `Bay c[1-45n1]`) with HP ProLiant m750, m710x, m510 Server Cartridge
-        
-        ### Pizzas
-        
-        * ProLiant DL380p Gen8
-        * ProLiant SL4540 Gen8
-        * ProLiant SL4540 Gen9
-        * ProLiant XL450 Gen10
-        
-        ## [Supermicro](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/supermicro.py)
-        
-        ### Blades
-        
-        * SBI-* and SBA-* should be supported, but I need dmidecode output example to support automatic blade location
-        
-        ### Pizzas
-        
-        * SSG-6028R
-        * SYS-6018R
-        
-        ## [QCT](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/qct.py)
-        
-        ### Blades
-        
-        * QuantaMicro X10E-9N
-        
-        ### Pizzas
-        
-        * Nothing ATM, feel free to send me a dmidecode or make a PR!
-        
-        # Known limitations
-        
-        * The project is only compatible with Linux.
-        Since it uses `ethtool` and parses `/sys/` directory, it's not compatible with *BSD distributions.
-        * Netbox `>=2.6.0,<=2.6.2` has a caching problem ; if the cache lifetime is too high, the script can get stale data after modification.
-        We advise to set `CACHE_TIME` to `0`.
-        
-        # Developing
-        
-        If you want to run the agent while adding features or just for debugging purposes
-        
-        ```
-        # git clone https://github.com/Solvik/netbox-agent.git
-        # cd netbox-agent
-        # python3 -m netbox_agent.cli --register
-        ```
-        
-        On a personal note, I use the docker image from [netbox-community/netbox-docker](https://github.com/netbox-community/netbox-docker)
-        ```
-        # git clone https://github.com/netbox-community/netbox-docker
-        # cd netbox-docker
-        # docker-compose pull
-        # docker-compose up 
-        ```
-        
 Keywords: netbox
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Netbox agent [![Build Status](https://travis-ci.com/Solvik/netbox-agent.svg?branch=master)](https://travis-ci.com/Solvik/netbox-agent)
+
+This project aims to create hardware automatically into [Netbox](https://github.com/netbox-community/netbox) based on standard tools (dmidecode, lldpd, parsing /sys/, etc).
+
+The goal is to generate an existing infrastructure on Netbox and have the ability to update it regularly by executing the agent.
+
+# Features
+
+* Create virtual machines, servers, chassis and blade through standard tools (`dmidecode`)
+* Create physical, bonding and vlan network interfaces with IPs (IPv4 & IPv6)
+* Create IPMI interface if found
+* Create or get existing VLAN and associate it to interfaces
+* Generic ability to guess datacenters and rack location through drivers (`cmd` and `file` and custom ones)
+* Update existing `Device` and `Interface`
+* Handle blade moving (new slot, new chassis)
+* Handle blade GPU expansions
+* Automatic cabling (server's interface to switch's interface) using lldp
+* Local inventory using `Inventory Item` for CPU, GPU, RAM, RAID cards, physical disks (behind raid cards)
+* PSUs creation and power consumption reporting (based on vendor's tools)
+
+# Requirements
+
+- Netbox >= 2.6
+- Python >= 3.4
+- [pynetbox](https://github.com/digitalocean/pynetbox/)
+- [python3-netaddr](https://github.com/drkjam/netaddr)
+- [python3-netifaces](https://github.com/al45tair/netifaces)
+- [jsonargparse](https://github.com/omni-us/jsonargparse/)
+
+- ethtool
+- dmidecode
+- ipmitool
+- lldpd
+- lshw
+
+## Inventory requirement
+- hpassacli
+- storcli
+- omreport
+
+# Installation
+
+```
+# pip3 install netbox-agent
+```
+
+# Usage
+
+The agent can be run from a shell and get its configuration from either the configuration file or environment variables.
+
+Configuration values are overridden based on the following precedence: command line arguments (might include config file) > environment variables > default config file > defaults.
+
+```
+# netbox_agent -c /etc/netbox_agent.yaml --register
+INFO:root:Creating chassis blade (serial: QTFCQ574502EF)
+INFO:root:Creating blade (serial: QTFCQ574502D2) myserver on chassis QTFCQ574502EF
+INFO:root:Setting device (QTFCQ574502D2) new slot on Slot 9 (Chassis QTFCQ574502EF)..
+INFO:root:Interface a8:1e:84:f2:9e:6a not found, creating..
+INFO:root:Creating NIC enp1s0f1 (a8:1e:84:f2:9e:6a) on myserver
+INFO:root:Interface 02:42:7a:89:cf:a4 not found, creating..
+INFO:root:Creating NIC br-07ea1e4a2f0e (02:42:7a:89:cf:a4) on myserver
+INFO:root:Create new IP 172.19.0.1/16 on br-07ea1e4a2f0e
+INFO:root:Interface a8:1e:84:f2:9e:69 not found, creating..
+INFO:root:Creating NIC enp1s0f0 (a8:1e:84:f2:9e:69) on myserver
+INFO:root:Create new IP 42.42.42.42/24 on enp1s0f0
+INFO:root:Create new IP fe80::aa1e:84ff:fef2:9e69/64 on enp1s0f0
+INFO:root:Interface a8:1e:84:cd:9d:d6 not found, creating..
+INFO:root:Creating NIC IPMI (a8:1e:84:cd:9d:d6) on myserver
+INFO:root:Create new IP 10.191.122.10/24 on IPMI
+```
+
+If you need, you can update only specific informations like:
+* Network
+* Inventory
+* Location
+* PSUs
+
+```
+# ip a add 42.42.42.43/24 dev enp1s0f1
+# netbox_agent -c /etc/netbox_agent.yaml --update-network
+INFO:root:Create new IP 42.42.42.43/24 on enp1s0f1
+# netbox_agent --update-inventory
+INFO:root:Creating Disk Samsung SSD 850 S2RBNX0K101698D
+```
+
+# Configuration
+
+```
+# Netbox configuration
+netbox:
+ url: 'http://netbox.internal.company.com'
+ token: supersecrettoken
+ # uncomment to disable ssl verification
+ # ssl_verify: false
+ # uncomment to use the system's CA certificates
+ # ssl_ca_certs_file: /etc/ssl/certs/ca-certificates.crt
+
+# Network configuration
+network:
+  # Regex to ignore interfaces
+  ignore_interfaces: "(dummy.*|docker.*)"
+  # Regex to ignore IP addresses
+  ignore_ips: (127\.0\.0\..*)
+  # enable auto-cabling by parsing LLDP answers
+  lldp: true
+
+#
+# You can use these to change the Netbox roles.
+# These are the defaults.
+#
+#device:
+# chassis_role: "Server Chassis"
+# blade_role: "Blade"
+# server_role: "Server"
+# tags: server, blade, ,just a comma,delimited,list
+# custom_fields: field1=value1,field2=value2#
+#
+# Can use this to set the tenant
+#
+#tenant:
+# driver: "file:/tmp/tenant"
+# regex: "(.*)"
+
+## Enable virtual machine support
+# virtual:
+#   # not mandatory, can be guessed
+#   enabled: True
+#   # see https://netbox.company.com/virtualization/clusters/
+#   cluster_name: my_vm_cluster
+
+# Enable datacenter location feature in Netbox
+datacenter_location:
+ driver: "cmd:cat /etc/qualification | tr [A-Z] [a-z]"
+ regex: "datacenter: (?P<datacenter>[A-Za-z0-9]+)"
+# driver: 'cmd:lldpctl'
+# regex: 'SysName: .*\.([A-Za-z0-9]+)'
+#
+# driver: "file:/tmp/datacenter"
+# regex: "(.*)"
+
+# Enable rack location feature in Netbox
+rack_location:
+# driver: 'cmd:lldpctl'
+# match SysName: sw-dist-a1.dc42
+# regex: 'SysName:[ ]+[A-Za-z]+-[A-Za-z]+-([A-Za-z0-9]+)'
+#
+# driver: "file:/tmp/datacenter"
+# regex: "(.*)"
+
+# Enable local inventory reporting
+inventory: true
+```
+
+# Specific workflow
+
+## Blades
+
+Each vendor class has a `is_blade` method which is later used for `Device` creation using the Netbox [parent/child feature](https://netbox.readthedocs.io/en/stable/core-functionality/devices/).
+
+The `get_blade_slot` method return the name of the `Device Bay`.
+
+
+Certain vendors don't report the blade slot in `dmidecode`, so we can use the `slot_location` regex feature of the configuration file.
+
+Some blade servers can be equipped with additional hardware using expansion blades, next to the processing blade, such as GPU expansion, or drives bay expansion. By default, the hardware from the expnasion is associated with the blade server itself, but it's possible to register the expansion as its own device using the `--expansion-as-device` command line parameter, or by setting `expansion_as_device` to `true` in the configuration file.
+
+## Drives attributes processing
+
+It is possible to process drives extended attributes such as the drive's physical or logical identifier, logical drive RAID type, size, consistency and so on.
+
+Those attributes as set as `custom_fields` in Netbox, and need to be registered properly before being able to specify them during the inventory phase.
+
+As the custom fields have to be created prior being able to register the disks extended attributes, this feature is only activated using the `--process-virtual-drives` command line parameter, or by setting `process_virtual_drives` to `true` in the configuration file.
+
+The custom fields to create as `DCIM > inventory item` `Text` are described below.
+
+```
+NAME            LABEL                      DESCRIPTION
+mount_point     Mount point                Device mount point(s)
+pd_identifier   Physical disk identifier   Physical disk identifier in the RAID controller
+vd_array        Virtual drive array        Virtual drive array the disk is member of
+vd_consistency  Virtual drive consistency  Virtual disk array consistency
+vd_device       Virtual drive device       Virtual drive system device
+vd_raid_type    Virtual drive RAID         Virtual drive array RAID type
+vd_size         Virtual drive size         Virtual drive array size
+```
+
+In the current implementation, the disks attributes ore not updated: if a disk with the correct serial number is found, it's sufficient to consider it as up to date.
+
+To force the reprocessing of the disks extended attributes, the `--force-disk-refresh` command line option can be used: it removes all existing disks to before populating them with the correct parsing. Unless this option is specified, the extended attributes won't be modified unless a disk is replaced.
+
+It is possible to dump the physical/virtual disks map on the filesystem under the JSON notation to ease or automate disks management. The file path has to be provided using the `--dump-disks-map` command line parameter.
+
+
+## Anycast IP
+
+The default behavior of the agent is to assign an interface to an IP.
+So two servers with anycasted IPs, running update mode, would only trigger IP's interface assignement in a loop.
+
+In order to handle this case, user need to set Netbox IP's mode to `Anycast` so that the agent will create another one if it's present on another server.
+
+# Hardware
+
+Tested on:
+
+## Virtual Machines
+
+* Hyper-V
+* VMWare
+* VirtualBox
+* AWS
+* GCP
+
+## [Dell Inc.](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/dell.py)
+
+### Blades
+
+* PowerEdge MX7000
+* PowerEdge M1000e (your `DeviceType` should have slots named `Slot 01` and so on)
+* PowerEdge MX740c
+* PowerEdge M640
+* PowerEdge M630
+* PowerEdge M620
+* PowerEdge M610
+
+### Pizzas
+
+* DSS7500
+
+## [HP / HPE](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/hp.py)
+
+### Blades
+
+* HP BladeSystem c7000 Enclosure G2 / G3 (your `DeviceType` should have slots named `Bay 1` and so on)
+* HP ProLiant BL460c Gen8
+* HP ProLiant BL460c Gen9
+* HP ProLiant BL460c Gen10
+* HP ProLiant BL460c Gen10 Graphics Exp its expansion HP ProLiant BL460c Graphics Expansion Blade
+* HP Moonshot 1500 Enclosure (your `DeviceType` should have slots batch create with `Bay c[1-45n1]`) with HP ProLiant m750, m710x, m510 Server Cartridge
+
+### Pizzas
+
+* ProLiant DL380p Gen8
+* ProLiant SL4540 Gen8
+* ProLiant SL4540 Gen9
+* ProLiant XL450 Gen10
+
+## [Supermicro](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/supermicro.py)
+
+### Blades
+
+* SBI-* and SBA-* should be supported, but I need dmidecode output example to support automatic blade location
+
+### Pizzas
+
+* SSG-6028R
+* SYS-6018R
+
+## [QCT](https://github.com/Solvik/netbox-agent/blob/master/netbox_agent/vendors/qct.py)
+
+### Blades
+
+* QuantaMicro X10E-9N
+
+### Pizzas
+
+* Nothing ATM, feel free to send me a dmidecode or make a PR!
+
+# Known limitations
+
+* The project is only compatible with Linux.
+Since it uses `ethtool` and parses `/sys/` directory, it's not compatible with *BSD distributions.
+* Netbox `>=2.6.0,<=2.6.2` has a caching problem ; if the cache lifetime is too high, the script can get stale data after modification.
+We advise to set `CACHE_TIME` to `0`.
+
+# Developing
+
+If you want to run the agent while adding features or just for debugging purposes
+
+```
+# git clone https://github.com/Solvik/netbox-agent.git
+# cd netbox-agent
+# python3 -m netbox_agent.cli --register
+```
+
+On a personal note, I use the docker image from [netbox-community/netbox-docker](https://github.com/netbox-community/netbox-docker)
+```
+# git clone https://github.com/netbox-community/netbox-docker
+# cd netbox-docker
+# docker-compose pull
+# docker-compose up
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `netbox_agent-0.6.2/netbox_agent.egg-info/SOURCES.txt` & `netbox_agent-0.7.1/netbox_agent.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.cfg
 setup.py
 netbox_agent/__init__.py
 netbox_agent/cli.py
 netbox_agent/config.py
 netbox_agent/dmidecode.py
 netbox_agent/ethtool.py
```

