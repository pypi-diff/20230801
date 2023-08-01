# Comparing `tmp/networklab-1.5.5.dev3.tar.gz` & `tmp/networklab-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.5.5.dev3.tar", last modified: Sat Jul 29 06:48:57 2023, max compression
+gzip compressed data, was "networklab-1.6.0.tar", last modified: Tue Aug  1 15:06:45 2023, max compression
```

## Comparing `networklab-1.5.5.dev3.tar` & `networklab-1.6.0.tar`

### file list

```diff
@@ -1,644 +1,642 @@
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.099838 networklab-1.5.5.dev3/
--rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/LICENSE.md
--rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/MANIFEST.in
--rw-r--r--   0 pipi       (501) staff       (20)     3744 2023-07-29 06:48:57.099691 networklab-1.5.5.dev3/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)     3030 2023-07-11 15:49:20.000000 networklab-1.5.5.dev3/README.md
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.899815 networklab-1.5.5.dev3/netsim/
--rwxr-xr-x   0 pipi       (501) staff       (20)       51 2023-07-29 06:48:30.000000 networklab-1.5.5.dev3/netsim/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)    13301 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/addressing.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.901251 networklab-1.5.5.dev3/netsim/ansible/
--rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     2899 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/config.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/create-config.ansible
--rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.5.dev3/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     3460 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/initial-config.ansible
--rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.5.dev3/netsim/ansible/missing.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.901965 networklab-1.5.5.dev3/netsim/ansible/tasks/
--rw-r--r--   0 pipi       (501) staff       (20)      720 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/create-config.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.906272 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      592 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      555 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      593 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     4846 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3196 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2250 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.912504 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.912962 networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.913316 networklab-1.5.5.dev3/netsim/ansible/tasks/frr/
--rw-r--r--   0 pipi       (501) staff       (20)      555 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 pipi       (501) staff       (20)      243 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/frr/mpls-clab.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.913556 networklab-1.5.5.dev3/netsim/ansible/tasks/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/iosxr/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.913782 networklab-1.5.5.dev3/netsim/ansible/tasks/linux/
--rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.913987 networklab-1.5.5.dev3/netsim/ansible/tasks/nxos/
--rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.914703 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)      502 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/vsrx.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.914974 networklab-1.5.5.dev3/netsim/ansible/tasks/vmx/
--rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/vmx/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.915213 networklab-1.5.5.dev3/netsim/ansible/templates/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.920670 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/
--rw-r--r--   0 pipi       (501) staff       (20)      618 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1267 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.927242 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/
--rw-r--r--   0 pipi       (501) staff       (20)     1363 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/frr.bgp-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     8056 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3504 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.927577 networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/
--rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.929749 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/
--rw-r--r--   0 pipi       (501) staff       (20)      903 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1631 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1853 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1239 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.931944 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/
--rw-r--r--   0 pipi       (501) staff       (20)     1346 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.948049 networklab-1.5.5.dev3/netsim/ansible/templates/initial/
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1200 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      480 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      466 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     5288 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3945 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1706 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.948907 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      923 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3481 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2026 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3479 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4863 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.952394 networklab-1.5.5.dev3/netsim/ansible/templates/isis/
--rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.5.dev3/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.961886 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/
--rw-r--r--   0 pipi       (501) staff       (20)      149 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      203 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      333 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      562 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1159 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      342 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.982613 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/
--rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1040 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1061 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1801 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1964 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.984503 networklab-1.5.5.dev3/netsim/ansible/templates/sr/
--rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.984794 networklab-1.5.5.dev3/netsim/ansible/templates/srv6/
--rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.990761 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/
--rw-r--r--   0 pipi       (501) staff       (20)      561 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1029 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vptx.j2
--rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.019325 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/
--rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      920 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      180 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1068 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1336 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1272 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.026113 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/
--rw-r--r--   0 pipi       (501) staff       (20)      423 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1929 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2234 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/api.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.028975 networklab-1.5.5.dev3/netsim/augment/
--rw-r--r--   0 pipi       (501) staff       (20)      230 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/augment/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6449 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/augment/components.py
--rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/augment/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     6452 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/augment/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)    18000 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/augment/groups.py
--rw-r--r--   0 pipi       (501) staff       (20)    40803 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/augment/links.py
--rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/augment/main.py
--rw-r--r--   0 pipi       (501) staff       (20)    12868 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/augment/nodes.py
--rw-r--r--   0 pipi       (501) staff       (20)     2810 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/augment/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     7621 2023-07-13 14:26:22.000000 networklab-1.5.5.dev3/netsim/augment/topology.py
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/callback.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.035974 networklab-1.5.5.dev3/netsim/cli/
--rwxr-xr-x   0 pipi       (501) staff       (20)     9773 2023-07-27 05:51:10.000000 networklab-1.5.5.dev3/netsim/cli/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.5.dev3/netsim/cli/alias.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1716 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     4169 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.5.dev3/netsim/cli/collect.py
--rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.5.dev3/netsim/cli/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     5545 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/connect.py
--rw-r--r--   0 pipi       (501) staff       (20)     2974 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/cli/create.py
--rw-r--r--   0 pipi       (501) staff       (20)     7029 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/cli/down.py
--rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.5.dev3/netsim/cli/empty.yml
--rw-r--r--   0 pipi       (501) staff       (20)     6323 2023-07-27 06:04:59.000000 networklab-1.5.5.dev3/netsim/cli/external_commands.py
--rw-r--r--   0 pipi       (501) staff       (20)     1583 2023-07-13 14:12:56.000000 networklab-1.5.5.dev3/netsim/cli/graph.py
--rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/cli/initial.py
--rw-r--r--   0 pipi       (501) staff       (20)     2043 2023-07-13 14:28:37.000000 networklab-1.5.5.dev3/netsim/cli/inspect.py
--rw-r--r--   0 pipi       (501) staff       (20)     2027 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/install.py
--rw-r--r--   0 pipi       (501) staff       (20)     9994 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-04-10 10:10:02.000000 networklab-1.5.5.dev3/netsim/cli/read.py
--rw-r--r--   0 pipi       (501) staff       (20)     1424 2023-07-13 14:13:04.000000 networklab-1.5.5.dev3/netsim/cli/report.py
--rw-r--r--   0 pipi       (501) staff       (20)     1354 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/cli/restart.py
--rw-r--r--   0 pipi       (501) staff       (20)     9161 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/show.py
--rw-r--r--   0 pipi       (501) staff       (20)     4774 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     3431 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/test.py
--rw-r--r--   0 pipi       (501) staff       (20)    10868 2023-07-27 10:32:32.000000 networklab-1.5.5.dev3/netsim/cli/up.py
--rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.5.dev3/netsim/cli/usage.py
--rw-r--r--   0 pipi       (501) staff       (20)     2287 2023-07-13 14:38:47.000000 networklab-1.5.5.dev3/netsim/cli/usage.txt
--rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/cli/version.py
--rw-r--r--   0 pipi       (501) staff       (20)      752 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/common.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.037158 networklab-1.5.5.dev3/netsim/data/
--rw-r--r--   0 pipi       (501) staff       (20)     4332 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/data/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3076 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/data/filemaps.py
--rw-r--r--   0 pipi       (501) staff       (20)     1329 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/data/global_vars.py
--rw-r--r--   0 pipi       (501) staff       (20)    20638 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/data/types.py
--rw-r--r--   0 pipi       (501) staff       (20)    19573 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/data/validate.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.038754 networklab-1.5.5.dev3/netsim/defaults/
--rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/defaults/addressing.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2557 2023-07-29 06:38:12.000000 networklab-1.5.5.dev3/netsim/defaults/attributes.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/defaults/automation.yml
--rw-r--r--   0 pipi       (501) staff       (20)      610 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/defaults/hints.yml
--rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/defaults/multilab.yml
--rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/defaults/ports.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.051513 networklab-1.5.5.dev3/netsim/devices/
--rw-r--r--   0 pipi       (501) staff       (20)     1812 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      854 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/arubacx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1128 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/arubacx.yml
--rw-r--r--   0 pipi       (501) staff       (20)      950 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/asav.py
--rw-r--r--   0 pipi       (501) staff       (20)      798 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/devices/asav.yml
--rw-r--r--   0 pipi       (501) staff       (20)      740 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/csr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2241 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/eos.py
--rw-r--r--   0 pipi       (501) staff       (20)     1642 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1210 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      822 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/iosv.py
--rw-r--r--   0 pipi       (501) staff       (20)     1449 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/iosv.yml
--rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/junos.py
--rw-r--r--   0 pipi       (501) staff       (20)      757 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/devices/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1148 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      923 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1355 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/devices/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1671 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      932 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/devices/unknown.py
--rw-r--r--   0 pipi       (501) staff       (20)      115 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/devices/unknown.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/vmx.py
--rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/vmx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/vptx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1638 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/devices/vptx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/vsrx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1275 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/devices/vsrx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.895416 networklab-1.5.5.dev3/netsim/extra/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.051789 networklab-1.5.5.dev3/netsim/extra/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.5.dev3/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.056629 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.057173 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     4976 2023-04-15 13:39:23.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/default-originate.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2162 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4470 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/topology.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.057453 networklab-1.5.5.dev3/netsim/extra/multilab/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.057979 networklab-1.5.5.dev3/netsim/extra/multilab/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.5.dev3/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3509 2023-04-15 10:43:11.000000 networklab-1.5.5.dev3/netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.5.dev3/netsim/extra/multilab/plugin.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.058248 networklab-1.5.5.dev3/netsim/extra/none/
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/extra/none/none.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.059147 networklab-1.5.5.dev3/netsim/extra/proxy-arp/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.059969 networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     1772 2023-04-15 10:43:07.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.061263 networklab-1.5.5.dev3/netsim/install/
--rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.5.dev3/netsim/install/ansible.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     3619 2023-07-27 16:30:58.000000 networklab-1.5.5.dev3/netsim/install/containerlab.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.5.dev3/netsim/install/grpc.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.064869 networklab-1.5.5.dev3/netsim/install/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)     1183 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.065165 networklab-1.5.5.dev3/netsim/install/libvirt/asav/
--rw-r--r--   0 pipi       (501) staff       (20)      972 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 pipi       (501) staff       (20)      369 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/install/libvirt/asav.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.5.dev3/netsim/install/libvirt/csr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.5.dev3/netsim/install/libvirt/eos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/install/libvirt/iosv.xml.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.065390 networklab-1.5.5.dev3/netsim/install/libvirt/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.5.dev3/netsim/install/libvirt/iosxr/iosxr_config.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.5.dev3/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.5.dev3/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.066251 networklab-1.5.5.dev3/netsim/install/libvirt/vptx/
--rw-r--r--   0 pipi       (501) staff       (20)     1994 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx/juniper.conf
--rwxr-xr-x   0 pipi       (501) staff       (20)     1089 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx/make-config.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)      654 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx/run.sh
--rw-r--r--   0 pipi       (501) staff       (20)     1653 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2552 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx.xml.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.066427 networklab-1.5.5.dev3/netsim/install/libvirt/vsrx/
--rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 pipi       (501) staff       (20)     3185 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/install/ubuntu.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.074822 networklab-1.5.5.dev3/netsim/modules/
--rw-r--r--   0 pipi       (501) staff       (20)    23644 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6155 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/_dataplane.py
--rw-r--r--   0 pipi       (501) staff       (20)    10721 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/_routing.py
--rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.5.dev3/netsim/modules/bfd.py
--rw-r--r--   0 pipi       (501) staff       (20)      724 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/bfd.yml
--rw-r--r--   0 pipi       (501) staff       (20)    21025 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/modules/bgp.py
--rw-r--r--   0 pipi       (501) staff       (20)     1843 2023-07-13 14:46:51.000000 networklab-1.5.5.dev3/netsim/modules/bgp.yml
--rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.5.dev3/netsim/modules/eigrp.py
--rw-r--r--   0 pipi       (501) staff       (20)      318 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/eigrp.yml
--rw-r--r--   0 pipi       (501) staff       (20)    17695 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/evpn.py
--rw-r--r--   0 pipi       (501) staff       (20)     1119 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/evpn.yml
--rw-r--r--   0 pipi       (501) staff       (20)     6763 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/gateway.py
--rw-r--r--   0 pipi       (501) staff       (20)     1029 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/gateway.yml
--rw-r--r--   0 pipi       (501) staff       (20)      141 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/initial.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/modules/isis.py
--rw-r--r--   0 pipi       (501) staff       (20)     1074 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/isis.yml
--rw-r--r--   0 pipi       (501) staff       (20)     7051 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/mpls.py
--rw-r--r--   0 pipi       (501) staff       (20)     1060 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/mpls.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3764 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/ospf.py
--rw-r--r--   0 pipi       (501) staff       (20)     1389 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/ospf.yml
--rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/modules/sr.py
--rw-r--r--   0 pipi       (501) staff       (20)      417 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/sr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.5.dev3/netsim/modules/srv6.py
--rw-r--r--   0 pipi       (501) staff       (20)      518 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/srv6.yml
--rw-r--r--   0 pipi       (501) staff       (20)    58909 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/modules/vlan.py
--rw-r--r--   0 pipi       (501) staff       (20)     1246 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/vlan.yml
--rw-r--r--   0 pipi       (501) staff       (20)    22607 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/modules/vrf.py
--rw-r--r--   0 pipi       (501) staff       (20)      458 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/vrf.yml
--rw-r--r--   0 pipi       (501) staff       (20)     9043 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/vxlan.py
--rw-r--r--   0 pipi       (501) staff       (20)      591 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/vxlan.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.078291 networklab-1.5.5.dev3/netsim/outputs/
--rw-r--r--   0 pipi       (501) staff       (20)     2233 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/outputs/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     7386 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     1786 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/outputs/common.py
--rw-r--r--   0 pipi       (501) staff       (20)    10023 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/d2.py
--rw-r--r--   0 pipi       (501) staff       (20)      545 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/outputs/d2.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2805 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)      255 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/format.py
--rw-r--r--   0 pipi       (501) staff       (20)     7556 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/graph.py
--rw-r--r--   0 pipi       (501) staff       (20)      218 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/outputs/graph.yml
--rw-r--r--   0 pipi       (501) staff       (20)      641 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/outputs/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.5.dev3/netsim/outputs/json.py
--rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.5.dev3/netsim/outputs/none.py
--rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/outputs/provider.py
--rw-r--r--   0 pipi       (501) staff       (20)     2235 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/report.py
--rw-r--r--   0 pipi       (501) staff       (20)     2893 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/tools.py
--rw-r--r--   0 pipi       (501) staff       (20)     1678 2023-07-13 14:21:52.000000 networklab-1.5.5.dev3/netsim/outputs/yaml.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.080599 networklab-1.5.5.dev3/netsim/providers/
--rw-r--r--   0 pipi       (501) staff       (20)     9311 2023-07-27 16:25:46.000000 networklab-1.5.5.dev3/netsim/providers/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3873 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/providers/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)      989 2023-07-27 16:25:46.000000 networklab-1.5.5.dev3/netsim/providers/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.5.dev3/netsim/providers/external.py
--rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/providers/external.yml
--rw-r--r--   0 pipi       (501) staff       (20)    13611 2023-07-27 16:28:14.000000 networklab-1.5.5.dev3/netsim/providers/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)     1157 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/providers/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.5.dev3/netsim/providers/virtualbox.py
--rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/providers/virtualbox.yml
--rw-r--r--   0 pipi       (501) staff       (20)     8373 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/read_topology.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.080876 networklab-1.5.5.dev3/netsim/templates/
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.5.dev3/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.896657 networklab-1.5.5.dev3/netsim/templates/provider/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.081132 networklab-1.5.5.dev3/netsim/templates/provider/clab/
--rw-r--r--   0 pipi       (501) staff       (20)     3857 2023-07-27 16:25:46.000000 networklab-1.5.5.dev3/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.081366 networklab-1.5.5.dev3/netsim/templates/provider/clab/frr/
--rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/templates/provider/clab/frr/daemons.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.081573 networklab-1.5.5.dev3/netsim/templates/provider/clab/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.5.dev3/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.081809 networklab-1.5.5.dev3/netsim/templates/provider/external/
--rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.5.dev3/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.092400 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)      683 2023-07-27 10:09:42.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/frr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      952 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2023-06-25 15:22:47.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 pipi       (501) staff       (20)     2728 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vptx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.094733 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/
--rw-r--r--   0 pipi       (501) staff       (20)      818 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      192 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/frr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/virtualbox-ports.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.095517 networklab-1.5.5.dev3/netsim/templates/tests/
--rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.5.dev3/netsim/templates/tests/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.5.dev3/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.5.dev3/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.096596 networklab-1.5.5.dev3/netsim/tools/
--rw-r--r--   0 pipi       (501) staff       (20)      764 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/tools/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     5106 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/tools/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      614 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/tools/graphite.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.096769 networklab-1.5.5.dev3/netsim/tools/suzieq/
--rw-r--r--   0 pipi       (501) staff       (20)      304 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 pipi       (501) staff       (20)      643 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/tools/suzieq.yml
--rw-r--r--   0 pipi       (501) staff       (20)      542 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/topology-defaults.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.098310 networklab-1.5.5.dev3/netsim/utils/
--rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/utils/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     2216 2023-07-27 05:43:15.000000 networklab-1.5.5.dev3/netsim/utils/files.py
--rw-r--r--   0 pipi       (501) staff       (20)     4079 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/utils/log.py
--rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/utils/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     1784 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/utils/strings.py
--rw-r--r--   0 pipi       (501) staff       (20)     5411 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/utils/templates.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.099220 networklab-1.5.5.dev3/networklab.egg-info/
--rw-r--r--   0 pipi       (501) staff       (20)     3744 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)    21652 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 pipi       (501) staff       (20)       51 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/entry_points.txt
--rw-r--r--   0 pipi       (501) staff       (20)      120 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/requires.txt
--rw-r--r--   0 pipi       (501) staff       (20)        7 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/top_level.txt
--rw-r--r--   0 pipi       (501) staff       (20)      181 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/requirements.txt
--rw-r--r--   0 pipi       (501) staff       (20)       38 2023-07-29 06:48:57.099878 networklab-1.5.5.dev3/setup.cfg
--rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.5.dev3/setup.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.099383 networklab-1.5.5.dev3/tests/
--rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/tests/test_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.943418 networklab-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-01 15:06:33.000000 networklab-1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 15:06:33.000000 networklab-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-08-01 15:06:45.943418 networklab-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-01 15:06:33.000000 networklab-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.811417 networklab-1.6.0/netsim/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/addressing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.811417 networklab-1.6.0/netsim/ansible/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2899 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1269 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/create-config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/missing.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.815417 networklab-1.6.0/netsim/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/create-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.819417 networklab-1.6.0/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.819417 networklab-1.6.0/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.819417 networklab-1.6.0/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.819417 networklab-1.6.0/netsim/ansible/tasks/frr/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/frr/mpls-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.823417 networklab-1.6.0/netsim/ansible/tasks/iosxr/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/iosxr/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.823417 networklab-1.6.0/netsim/ansible/tasks/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.823417 networklab-1.6.0/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.823417 networklab-1.6.0/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.823417 networklab-1.6.0/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/tasks/vmx/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.823417 networklab-1.6.0/netsim/ansible/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.827417 networklab-1.6.0/netsim/ansible/templates/bfd/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.835417 networklab-1.6.0/netsim/ansible/templates/bgp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/frr.bgp-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.835417 networklab-1.6.0/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.835417 networklab-1.6.0/netsim/ansible/templates/evpn/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.839417 networklab-1.6.0/netsim/ansible/templates/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.847417 networklab-1.6.0/netsim/ansible/templates/initial/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.847417 networklab-1.6.0/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.851417 networklab-1.6.0/netsim/ansible/templates/isis/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.855417 networklab-1.6.0/netsim/ansible/templates/mpls/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.863417 networklab-1.6.0/netsim/ansible/templates/ospf/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/junos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/junos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.867417 networklab-1.6.0/netsim/ansible/templates/sr/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.867417 networklab-1.6.0/netsim/ansible/templates/srv6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.871418 networklab-1.6.0/netsim/ansible/templates/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.879418 networklab-1.6.0/netsim/ansible/templates/vrf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.879418 networklab-1.6.0/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/ansible/templates/vxlan/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.883418 networklab-1.6.0/netsim/augment/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40803 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/augment/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.887418 networklab-1.6.0/netsim/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9623 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/alias.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/clab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/down.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/external_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.887418 networklab-1.6.0/netsim/cli/show_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show_commands/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show_commands/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show_commands/module_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show_commands/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show_commands/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show_commands/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/show_commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/usage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/cli/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.891418 networklab-1.6.0/netsim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/data/filemaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/data/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/data/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.891418 networklab-1.6.0/netsim/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/defaults/addressing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/defaults/attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/defaults/automation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/defaults/hints.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/defaults/multilab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/defaults/ports.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.899418 networklab-1.6.0/netsim/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/arubacx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/asav.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/asav.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/csr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/iosv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/iosv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/junos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/none.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/unknown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/vmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/vmx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/vptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/vsrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/vsrx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/devices/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.807417 networklab-1.6.0/netsim/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.903418 networklab-1.6.0/netsim/extra/ebgp.utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/default-originate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/topology.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/ebgp.utils/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.903418 networklab-1.6.0/netsim/extra/multilab/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/multilab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.903418 networklab-1.6.0/netsim/extra/none/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/none/none.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.903418 networklab-1.6.0/netsim/extra/proxy-arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.903418 networklab-1.6.0/netsim/install/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/ansible.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3619 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/containerlab.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/grpc.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.907418 networklab-1.6.0/netsim/install/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.907418 networklab-1.6.0/netsim/install/libvirt/asav/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/iosv.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.911418 networklab-1.6.0/netsim/install/libvirt/vptx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1089 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.911418 networklab-1.6.0/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3185 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/libvirt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/install/ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.919418 networklab-1.6.0/netsim/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    23644 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/_dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/bfd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/bfd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/bgp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/eigrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/eigrp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/evpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/evpn.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/gateway.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/isis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/isis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/mpls.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/ospf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/sr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/sr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/srv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/srv6.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    58909 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/vlan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22607 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/vrf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/vxlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/modules/vxlan.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.923418 networklab-1.6.0/netsim/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/d2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/d2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/graph.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.927418 networklab-1.6.0/netsim/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/clab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/external.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/virtualbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/providers/virtualbox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/read_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.927418 networklab-1.6.0/netsim/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.807417 networklab-1.6.0/netsim/templates/provider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.927418 networklab-1.6.0/netsim/templates/provider/clab/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.927418 networklab-1.6.0/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/clab/frr/daemons.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.927418 networklab-1.6.0/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.927418 networklab-1.6.0/netsim/templates/provider/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.935418 networklab-1.6.0/netsim/templates/provider/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/forwarded-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.935418 networklab-1.6.0/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/provider/virtualbox/vsrx-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.939418 networklab-1.6.0/netsim/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/tests/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.939418 networklab-1.6.0/netsim/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/tools/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/tools/graphite.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.939418 networklab-1.6.0/netsim/tools/suzieq/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/tools/suzieq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/topology-defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.939418 networklab-1.6.0/netsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-08-01 15:06:33.000000 networklab-1.6.0/netsim/utils/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.943418 networklab-1.6.0/networklab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-08-01 15:06:45.000000 networklab-1.6.0/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21574 2023-08-01 15:06:45.000000 networklab-1.6.0/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:06:45.000000 networklab-1.6.0/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 15:06:45.000000 networklab-1.6.0/networklab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 15:06:45.000000 networklab-1.6.0/networklab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 15:06:45.000000 networklab-1.6.0/networklab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 15:06:33.000000 networklab-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:06:45.943418 networklab-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-01 15:06:33.000000 networklab-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:45.943418 networklab-1.6.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-08-01 15:06:33.000000 networklab-1.6.0/tests/test_transformation.py
```

### Comparing `networklab-1.5.5.dev3/LICENSE.md` & `networklab-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/PKG-INFO` & `networklab-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.5.dev3
+Version: 1.6.0
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,19 +30,17 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
+The latest release is [release 1.6.0](https://github.com/ipspace/netlab/releases/tag/release_1.6.0). It contains [numerous new features](https://netlab.tools/release/1.6/) that might have a few bugs attached to them. Should you encounter one of those creatures, please open a Github issue and use release 1.5.4. You might also want to [read the release notes](https://netlab.tools/release/).
 
-The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
-
-## An overview of tools:
+## An Overview of CLI Commands
 
 **netlab up**
 : Uses **[netlab create](https://netlab.tools/netlab/create/)** to create configuration files, starts the virtual lab, and uses **[netlab initial](https://netlab.tools/netlab/initial/)** to deploy device configurations, including IP addressing, LLDP, OSPF, BGP, IS-IS, EIGRP, VRRP, VLANs, VRFs, MPLS, SR-MPLS, VXLAN, EVPN and SRv6. [More details](https://netlab.tools/netlab/up/)
 
 **netlab down**
 : Destroys the virtual lab. [More details](https://netlab.tools/netlab/down/)
```

### Comparing `networklab-1.5.5.dev3/README.md` & `networklab-1.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
+The latest release is [release 1.6.0](https://github.com/ipspace/netlab/releases/tag/release_1.6.0). It contains [numerous new features](https://netlab.tools/release/1.6/) that might have a few bugs attached to them. Should you encounter one of those creatures, please open a Github issue and use release 1.5.4. You might also want to [read the release notes](https://netlab.tools/release/).
 
-The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
-
-## An overview of tools:
+## An Overview of CLI Commands
 
 **netlab up**
 : Uses **[netlab create](https://netlab.tools/netlab/create/)** to create configuration files, starts the virtual lab, and uses **[netlab initial](https://netlab.tools/netlab/initial/)** to deploy device configurations, including IP addressing, LLDP, OSPF, BGP, IS-IS, EIGRP, VRRP, VLANs, VRFs, MPLS, SR-MPLS, VXLAN, EVPN and SRv6. [More details](https://netlab.tools/netlab/up/)
 
 **netlab down**
 : Destroys the virtual lab. [More details](https://netlab.tools/netlab/down/)
```

### Comparing `networklab-1.5.5.dev3/netsim/addressing.py` & `networklab-1.6.0/netsim/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/collect-configs.ansible` & `networklab-1.6.0/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/config.ansible` & `networklab-1.6.0/netsim/ansible/config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/create-config.ansible` & `networklab-1.6.0/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/initial-config.ansible` & `networklab-1.6.0/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/create-config.yml` & `networklab-1.6.0/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.6.0/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.6.0/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.6.0/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.6.0/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.6.0/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/iosxr/initial.yml` & `networklab-1.6.0/netsim/ansible/tasks/iosxr/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.6.0/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.6.0/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.6.0/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.6.0/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.6.0/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/frr.bgp-config.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/frr.bgp-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.6.0/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.6.0/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.6.0/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/asa.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/eos.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/frr.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/ios.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.6.0/netsim/ansible/templates/initial/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/asa.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/eos.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/frr.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/ios.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/junos.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.6.0/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.6.0/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.6.0/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.6.0/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.6.0/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.6.0/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.6.0/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.6.0/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.6.0/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/junos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/junos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.6.0/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/sr/junos.j2` & `networklab-1.6.0/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/sr/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.6.0/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vptx.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/vptx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.6.0/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.6.0/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.6.0/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.6.0/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.6.0/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.6.0/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.6.0/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.6.0/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.6.0/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/api.py` & `networklab-1.6.0/netsim/api.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/components.py` & `networklab-1.6.0/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/config.py` & `networklab-1.6.0/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/devices.py` & `networklab-1.6.0/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/groups.py` & `networklab-1.6.0/netsim/augment/groups.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/links.py` & `networklab-1.6.0/netsim/augment/links.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/main.py` & `networklab-1.6.0/netsim/augment/main.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/nodes.py` & `networklab-1.6.0/netsim/augment/nodes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/plugin.py` & `networklab-1.6.0/netsim/augment/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/augment/topology.py` & `networklab-1.6.0/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/callback.py` & `networklab-1.6.0/netsim/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/__init__.py` & `networklab-1.6.0/netsim/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import typing
 
 from box import Box
 
 from . import usage
 from .. import augment, common, read_topology
 from .. import __version__
-from ..utils import status
+from ..utils import status as _status
 
 DRY_RUN: bool = False
 
 def common_parse_args(debugging: bool = False) -> argparse.ArgumentParser:
   parser = argparse.ArgumentParser(description='Common argument parsing',add_help=False)
   parser.add_argument('--log', dest='logging', action='store_true',
                   help='Enable basic logging')
@@ -154,26 +154,23 @@
 lab_status_update -- generic lab status callback
 
 * Get the lab ID (or default)
 * Map lab ID into current directory
 * Merge status dictionary or perform status-specific callback
 """
 
-def get_lab_id(topology: Box) -> str:
-  return topology.get('defaults.multilab.id','default') or 'default'    # id could be set to {} due to tool f-string evals
-
 def lab_status_update(
       topology: Box,
       status: Box,
       update: typing.Optional[dict] = None,
       cb: typing.Optional[typing.Callable] = None) -> None:
 
   if DRY_RUN:                                               # Don't update status if we're in dry-run mode 
     return
-  lab_id = get_lab_id(topology)                             # Get the lab ID (or default)
+  lab_id = _status.get_lab_id(topology)                     # Get the lab ID (or default)
   if not lab_id in status:
     status[lab_id].dir = os.getcwd()                        # Map lab ID into current directory
   if not 'providers' in status[lab_id]:                     # Initialize provider list
     status[lab_id].providers = []
 
   if update is not None:                                    # Update lab status from a dictionary
     status[lab_id] = status[lab_id] + update
@@ -196,15 +193,15 @@
 lab_status_change -- change current lab status
 """
 def lab_status_change(topology: Box, new_status: str) -> None:
   global DRY_RUN
   if DRY_RUN:                                              # Don't update status if we're in dry-run mode 
     return
 
-  status.change_status(
+  _status.change_status(
     topology,
     callback = lambda s,t: 
       lab_status_update(t,s,
         update = { 'status': new_status }))
 
 #
 # Main command dispatcher
```

### Comparing `networklab-1.5.5.dev3/netsim/cli/ansible.py` & `networklab-1.6.0/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/clab.py` & `networklab-1.6.0/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/collect.py` & `networklab-1.6.0/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/config.py` & `networklab-1.6.0/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/connect.py` & `networklab-1.6.0/netsim/cli/connect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/create.py` & `networklab-1.6.0/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/down.py` & `networklab-1.6.0/netsim/cli/down.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typing
 import textwrap
 import os
 import sys
 from box import Box
 
 from . import external_commands, set_dry_run, is_dry_run
-from . import lab_status_change,get_lab_id,fs_cleanup,load_snapshot
+from . import lab_status_change,fs_cleanup,load_snapshot
 from .. import read_topology,common,providers
 from ..utils import status,strings
 from .up import provider_probes
 #
 # CLI parser for 'netlab down' command
 #
 def down_parse(args: typing.List[str]) -> argparse.Namespace:
@@ -105,15 +105,15 @@
   external_commands.stop_lab(topology.defaults,p_name,step,"netlab down",exec_command)
   p_module.call('post_stop_lab',p_topology)
 
 '''
 lab_dir_mismatch -- check if the lab instance is running in the current directory
 '''
 def lab_dir_mismatch(topology: Box) -> bool:
-  lab_id = get_lab_id(topology)
+  lab_id = status.get_lab_id(topology)
   lab_status = status.read_status(topology)       # Find current running instance(s)
   if not lab_id in lab_status:                    # This could be a lab instance from pre-status days
     return False                                  # ... in which case we can shut it down
   if lab_id in lab_status and lab_status[lab_id].dir == os.getcwd():
     return False                                 # Lab instance is known  and this is the correct directory        
 
   print(f'''
@@ -124,24 +124,14 @@
 directory, but you might impact the running lab instance.
 ''')
   if not strings.confirm('Do you want to proceed?'):
     common.fatal('aborting lab shutdown request')
 
   return True
 
-'''
-Remove the lab instance/directory from the status file
-'''
-def remove_lab_status(topology: Box) -> None:
-  lab_id = get_lab_id(topology)
-
-  status.change_status(
-    topology,
-    callback = lambda s,t: s.pop(lab_id,None))
-
 """
 Stop external tools
 """
 def stop_external_tools(args: argparse.Namespace, topology: Box) -> None:
   lab_status_change(topology,f'stopping external tools')
   for tool in list(topology.tools.keys()):
     cmds = external_commands.get_tool_command(tool,'down',topology)
@@ -212,11 +202,11 @@
       stop_step = stop_step + 1
       tool_cleanup(topology,True)
 
     external_commands.print_step(stop_step,"Cleanup configuration files",spacing=True)
     down_cleanup(topology,True)
 
   if not mismatch:
-    remove_lab_status(topology)
+    status.remove_lab_status(topology)
 
   if not is_dry_run():
     status.unlock_directory()
```

### Comparing `networklab-1.5.5.dev3/netsim/cli/external_commands.py` & `networklab-1.6.0/netsim/cli/external_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,41 +44,44 @@
 
   if log.VERBOSE or log.debug_active('external'):
     print(f"run_command executing: {cmd}")
 
   if isinstance(cmd,str):
     cmd = [ arg for arg in cmd.split(" ") if arg not in (""," ") ]
 
+  if not cmd:                                               # Skip empty commands
+    return True
+
   try:
     result = subprocess.run(cmd,capture_output=check_result,check=True,text=True)
     if log.debug_active('external'):
       print(f'... run result: {result}')
     if not check_result:
       return True
     if return_stdout:
       return result.stdout
     return result.stdout != ""
   except Exception as ex:
     if not log.QUIET and not ignore_errors:
       print( f"Error executing {stringify(cmd)}:\n  {ex}" )
     return False
 
-def test_probe(p : typing.Union[str,list,Box]) -> bool:
+def test_probe(p : typing.Union[str,list,Box],quiet : bool = False) -> bool:
   if isinstance(p,str):
-    return bool(run_command(p,check_result=True))
+    return bool(run_command(p,check_result=True,ignore_errors=quiet))
 
   elif isinstance(p,list):
     for p_item in p:
-      if not test_probe(p_item):
+      if not test_probe(p_item,quiet):
         return False
     return True
 
   elif isinstance(p,Box):
     OK = bool(run_command(p.cmd,check_result=True,ignore_errors=True))
-    if not OK:
+    if not OK and not quiet:
       log.fatal(p.err)
     return OK
 
   else:
     log.fatal(f"Internal error: invalid probe specification: {p}")
     return False
```

### Comparing `networklab-1.5.5.dev3/netsim/cli/graph.py` & `networklab-1.6.0/netsim/cli/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/initial.py` & `networklab-1.6.0/netsim/cli/initial.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/inspect.py` & `networklab-1.6.0/netsim/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/install.py` & `networklab-1.6.0/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/libvirt.py` & `networklab-1.6.0/netsim/cli/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/read.py` & `networklab-1.6.0/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/report.py` & `networklab-1.6.0/netsim/cli/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # Create a text or HTML report from the current lab topology
 #
 import typing
 import argparse
 
 from . import load_snapshot
-from ..outputs import _TopologyOutput
+from ..outputs import _TopologyOutput, common as outputs_common
 from ..utils import strings,log
 
 #
 # CLI parser for 'netlab report' command
 #
 def report_parse(args: typing.List[str]) -> argparse.Namespace:
   parser = argparse.ArgumentParser(
@@ -37,13 +37,20 @@
 
 def run(cli_args: typing.List[str]) -> None:
   args = report_parse(cli_args)
   topology = load_snapshot(args)
   report_module = _TopologyOutput.load(
                      f'report:{args.report}={args.output or "-"}',
                      topology.defaults.outputs.report)
-  if report_module:
-    report_module.write(topology)
-    if args.output:
-      print(f'Created {args.report} report in {args.output}')
-  else:
+  if not report_module:
     log.fatal('Cannot load the reporting output module, aborting')
+
+  for n in list(topology.nodes.keys()):                     # Add group variables to topology nodes
+    topology.nodes[n] = outputs_common.adjust_inventory_host(
+                          node=topology.nodes[n],
+                          ignore=[ 'no-fields' ],
+                          defaults=topology.defaults,
+                          group_vars=True)
+
+  report_module.write(topology)
+  if args.output:
+    print(f'Created {args.report} report in {args.output}')
```

### Comparing `networklab-1.5.5.dev3/netsim/cli/restart.py` & `networklab-1.6.0/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/status.py` & `networklab-1.6.0/netsim/cli/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/test.py` & `networklab-1.6.0/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/cli/up.py` & `networklab-1.6.0/netsim/cli/up.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 from box import Box
 from pathlib import Path
 
 from . import create
 from . import external_commands, set_dry_run, is_dry_run
 from . import common_parse_args, get_message
-from . import lab_status_update, lab_status_change, get_lab_id
+from . import lab_status_update, lab_status_change
 from .. import providers
 from .. import read_topology
-from ..utils import status,log
+from ..utils import log,status as _status
 
 #
 # Extra arguments for 'netlab up' command
 #
 def up_parse_args(standalone: bool) -> argparse.ArgumentParser:
   parse_parents = [ common_parse_args() ] if standalone else []
   parser = argparse.ArgumentParser(
@@ -84,46 +84,46 @@
 * status_start_lab -- lab initialization has started
 * status_start_provider -- provider activation has started
 * status_config -- configuration deployment has started
 * status_complete -- lab initialization has completed
 """
 
 def lab_status_start(status: Box, topology: Box) -> None:
-  lab_id = get_lab_id(topology)                             # Get the lab ID (or default)
+  lab_id = _status.get_lab_id(topology)                     # Get the lab ID (or default)
   if lab_id in status:
     if status[lab_id].dir != os.getcwd():
       lab_status_update(topology,status,
         update = { 'status': f'conflict -- trying to start lab in {os.getcwd()}'})
       topology.defaults.err_conflict = status[lab_id].dir
       return
 
   lab_status_update(topology,status,
     update = {
       'status': 'starting lab' if not lab_id in status else 'restarting lab',
       'name': topology.name,
       'providers': [] })
 
 def status_start_lab(topology: Box) -> None:
-  status.change_status(
+  _status.change_status(
     topology,
     callback = lambda s,t: lab_status_start(s,t))
 
 def status_start_provider(topology: Box, provider: str) -> None:
-  status.change_status(
+  _status.change_status(
     topology,
     callback = lambda s,t: 
       lab_status_update(t,s,
         update = { 'status': f'starting provider {provider}' },
         cb = lambda s: s.providers.append(provider)))
 
 """
 check_existing_lab -- print an command-specific error message if there'a s lab already running in this directory
 """
 def check_existing_lab() -> None:
-  if not status.is_directory_locked():
+  if not _status.is_directory_locked():
     return
   
   print(f'''
 It looks like you have another lab running in this directory. If you want to
 continue the lab startup process due to a previous failure, please use the
 'netlab up --snapshot' command.
 
@@ -135,16 +135,16 @@
 ''')
   log.fatal('Cannot start another lab in the same directory')
 
 """
 check_lab_instance -- print an error message if the lab instance is already running in a different directory
 """
 def check_lab_instance(topology: Box) -> None:
-  lab_id = get_lab_id(topology)                   # Get the current lab instance ID from lab topology
-  lab_states = status.read_status(topology)       # Read the state of existing lab instances
+  lab_id = _status.get_lab_id(topology)           # Get the current lab instance ID from lab topology
+  lab_states = _status.read_status(topology)      # Read the state of existing lab instances
 
   if not lab_id in lab_states:                    # If this lab instance is not running ==> OK
     return
   
   if lab_states[lab_id].dir == os.getcwd():       # If this lab instance is already running in this directory
     return                                        # ... we'll deal with that a bit later in the process
 
@@ -280,15 +280,15 @@
   p_module.call('pre_output_transform',topology)
 
   status_start_lab(topology)
   if 'err_conflict' in topology.defaults:
     log.fatal(f'race condition, lab instance already running in {topology.defaults.err_conflict}')
 
   if not is_dry_run():
-    status.lock_directory()
+    _status.lock_directory()
 
   step = 3
   external_commands.print_step(step,f"Starting the lab: {p_provider}")
   start_provider_lab(topology,p_provider)
 
   for s_provider in topology[p_provider].providers:
     step += 1
```

### Comparing `networklab-1.5.5.dev3/netsim/cli/usage.txt` & `networklab-1.6.0/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/common.py` & `networklab-1.6.0/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/data/__init__.py` & `networklab-1.6.0/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/data/filemaps.py` & `networklab-1.6.0/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/data/global_vars.py` & `networklab-1.6.0/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/data/types.py` & `networklab-1.6.0/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/data/validate.py` & `networklab-1.6.0/netsim/data/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/defaults/attributes.yml` & `networklab-1.6.0/netsim/defaults/attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/defaults/hints.yml` & `networklab-1.6.0/netsim/defaults/hints.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/__init__.py` & `networklab-1.6.0/netsim/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/arubacx.py` & `networklab-1.6.0/netsim/devices/arubacx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/arubacx.yml` & `networklab-1.6.0/netsim/devices/arubacx.yml`

 * *Files 9% similar despite different names*

```diff
@@ -13,30 +13,34 @@
   ansible_network_os: arubanetworks.aoscx.aoscx
   ansible_connection: network_cli
   #ansible_connection: arubanetworks.aoscx.aoscx
   ansible_user: admin
   ansible_ssh_pass: admin
   netlab_device_type: arubacx
 features:
+  bfd: true
   bgp:
-    local_as: True
-    vrf_local_as: True
-    local_as_ibgp: True
-    activate_af: True
+    activate_af: true
+    local_as: true
+    local_as_ibgp: true
+    vrf_local_as: true
+  evpn:
+    asymmetrical_irb: true
+    irb: true
+  gateway:
+    protocol: [ anycast, vrrp ]
+  mpls:
+    ldp: true
+    vpn: true
+  ospf: true
   vlan:
     #model: l3-switch
     model: switch
     svi_interface_name: vlan{vlan}
     # ArubaOS-CX supports subinterfaces... but not on virtual devices.
     #subif_name: "{ifname}.{vlan.access_id}"
     #native_routed: False
-  evpn:
-    irb: True
-    asymmetrical_irb: True
-  gateway:
-    protocol: [ anycast, vrrp ]
-  mpls:
-    ldp: True
-    vpn: True
+  vrf: true
+  vxlan: true
 external:
   image: none
 graphite.icon: switch
```

### Comparing `networklab-1.5.5.dev3/netsim/devices/asav.py` & `networklab-1.6.0/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/asav.yml` & `networklab-1.6.0/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/csr.yml` & `networklab-1.6.0/netsim/devices/csr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/cumulus.yml` & `networklab-1.6.0/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/cumulus_nvue.yml` & `networklab-1.6.0/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/dellos10.yml` & `networklab-1.6.0/netsim/devices/dellos10.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 description: Dell OS10
 interface_name: ethernet1/1/{ifindex}
 mgmt_if: mgmt1/1/1
 loopback_interface_name: loopback{ifindex}
 features:
   initial:
     ipv4:
-      unnumbered: True
+      unnumbered: true
     ipv6:
-      lla: True
+      lla: true
   bgp:
-    local_as: True
-    vrf_local_as: True
-    activate_af: True
-    ipv6_lla: True
-    rfc8950: True
-  vlan:
-    model: switch
-    svi_interface_name: virtual-network{vlan}
+    activate_af: true
+    ipv6_lla: true
+    local_as: true
+    rfc8950: true
+    vrf_local_as: true
   evpn:
-    irb: True
-    asymmetrical_irb: True
+    asymmetrical_irb: true
+    irb: true
   gateway:
     protocol: [ anycast, vrrp ]
+  ospf: true
+  vlan:
+    model: switch
+    svi_interface_name: virtual-network{vlan}
+  vrf: true
+  vxlan: true
 clab:
   image: vrnetlab/vr-ftosv
   node:
     kind: vr-ftosv
   interface:
     name: eth{ifindex}
 libvirt:
```

### Comparing `networklab-1.5.5.dev3/netsim/devices/eos.py` & `networklab-1.6.0/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/eos.yml` & `networklab-1.6.0/netsim/devices/eos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/frr.yml` & `networklab-1.6.0/netsim/devices/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/iosv.py` & `networklab-1.6.0/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/iosv.yml` & `networklab-1.6.0/netsim/devices/iosv.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/iosxr.yml` & `networklab-1.6.0/netsim/devices/iosxr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/junos.py` & `networklab-1.6.0/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/linux.yml` & `networklab-1.6.0/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/none.yml` & `networklab-1.6.0/netsim/devices/none.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/nxos.yml` & `networklab-1.6.0/netsim/devices/nxos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/routeros7.yml` & `networklab-1.6.0/netsim/devices/routeros7.yml`

 * *Files 15% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 group_vars:
   ansible_network_os: routeros
   ansible_connection: network_cli
   ansible_user: admin
   ansible_ssh_pass: admin
   netlab_device_type: routeros7
 features:
+  bgp: true
   mpls:
-    ldp: True
-    vpn: True
+    ldp: true
+    vpn: true
+  ospf: true
   vlan:
     model: l3-switch
     svi_interface_name: "vlan{vlan}"
     subif_name: "{ifname}-{vlan.access_id}"
-    native_routed: True
+    native_routed: true
+  vrf: true
 clab:
   image: vrnetlab/vr-routeros:7.6
   node:
     kind: vr-ros
   interface:
     name: eth{ifindex-1}
 external:
```

### Comparing `networklab-1.5.5.dev3/netsim/devices/srlinux.yml` & `networklab-1.6.0/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/sros.yml` & `networklab-1.6.0/netsim/devices/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/unknown.py` & `networklab-1.6.0/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/vmx.py` & `networklab-1.6.0/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/vmx.yml` & `networklab-1.6.0/netsim/devices/routeros.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,27 @@
-description: Juniper vMX container
-interface_name: ge-0/0/{ifindex}
-loopback_interface_name: "lo0.{ifindex}"
-ifindex_offset: 0
-mgmt_if: fxp0
+description: Mikrotik RouterOS version 6
+interface_name: ether{ifindex}
+mgmt_if: ether1
+ifindex_offset: 2
+libvirt:
+  image: mikrotik/chr
 group_vars:
+  ansible_network_os: routeros
+  ansible_connection: network_cli
   ansible_user: admin
-  ansible_ssh_pass: "admin@123"
-  ansible_network_os: junos
-  ansible_connection: netconf
-  netlab_console_connection: ssh
-  netlab_device_type: vmx
+  ansible_ssh_pass: admin
 features:
-  initial:
-    ipv4:
-      unnumbered: True
-    ipv6:
-      lla: True
-  ospf:
-    unnumbered: True
-  isis:
-    unnumbered:
-      ipv4: True
-      ipv6: True
+  bgp: true
+  mpls:
+    ldp: true
+    vpn: true
+  ospf: true
   vlan:
     model: router
-    svi_interface_name: irb.{vlan}
-    subif_name: "{ifname}.{vlan.access_id}"
-    mixed_trunk: True
-    native_routed: True
-  mpls:
-    ldp: True
-    vpn: True
-clab:
-  image: vrnetlab/vr-vmx:18.2R1.9
-  node:
-    kind: vr-vmx
-  interface:
-    name: eth{ifindex+1}
+    svi_interface_name: bridge{vlan}
+    subif_name: "{ifname}-{vlan.access_id}"
+    mixed_trunk: true
+    native_routed: true
+  vrf: true
 external:
   image: none
 graphite.icon: router
```

### Comparing `networklab-1.5.5.dev3/netsim/devices/vptx.py` & `networklab-1.6.0/netsim/devices/vptx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/vptx.yml` & `networklab-1.6.0/netsim/devices/vptx.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,24 @@
 description: Juniper vPTX
+parent: junos
 interface_name: et-0/0/{ifindex}
-loopback_interface_name: "lo0.{ifindex}"
-ifindex_offset: 0
 mgmt_if: "re0:mgmt-0"
 group_vars:
-  ansible_user: vagrant
-  ansible_ssh_pass: Vagrant
-  ansible_network_os: junos
-  ansible_connection: netconf
-  netlab_console_connection: ssh
   netlab_device_type: vptx
+
 features:
-  initial:
-    ipv4:
-      unnumbered: True
-    ipv6:
-      lla: True
-  ospf:
-    unnumbered: True
-  isis:
-    unnumbered:
-      ipv4: True
-      ipv6: True
+  evpn: true
   vlan:
     model: l3-switch
     svi_interface_name: irb.{vlan}
     subif_name: "{ifname}.{vlan.access_id}"
-    mixed_trunk: True
-    native_routed: True
-  mpls:
-    ldp: True
-    vpn: True
-external:
-  image: none
-graphite.icon: switch
+    mixed_trunk: true
+    native_routed: true
+  vxlan: true
+
 libvirt:
   image: juniper/vptx
   # New "pre-install hooks"
   pre_install: vptx
   create_template: vptx.xml.j2
   #create:
   #  virt-install --connect=qemu:///system --name=vm_box --arch=x86_64 --vcpus 4 --ram 8192
@@ -46,7 +27,9 @@
   #    --cpu IvyBridge,+vmx
   #    --qemu-commandline="-smbios type=0,vendor=Bochs,version=Bochs -smbios type=3,manufacturer=Bochs -smbios type=1,manufacturer=Bochs,product=Bochs,serial=chassis_no=0:slot=0:type=1:assembly_id=0x0D20:platform=251:master=0:channelized=no"
   #    --network=network:vagrant-libvirt,model=virtio
   #    --network network=vptx_PFE_LINK,model=virtio
   #    --network network=vptx_RPIO_LINK,model=virtio
   #    --network network=vptx_RPIO_LINK,model=virtio
   #    --network network=vptx_PFE_LINK,model=virtio
+
+graphite.icon: switch
```

### Comparing `networklab-1.5.5.dev3/netsim/devices/vsrx.py` & `networklab-1.6.0/netsim/devices/vsrx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/devices/vyos.yml` & `networklab-1.6.0/netsim/devices/vyos.yml`

 * *Files 16% similar despite different names*

```diff
@@ -9,38 +9,42 @@
   ansible_connection: paramiko
   ansible_user: vyos
   ansible_ssh_pass: vyos
   docker_shell: su - vyos
 features:
   initial:
     ipv4:
-      unnumbered: True
+      unnumbered: true
     ipv6:
       lla: True
-  ospf:
-    unnumbered: True
+  bfd: true
   bgp:
-    local_as: True
-    vrf_local_as: True
-    activate_af: True
-    ipv6_lla: True
-    rfc8950: True
+    activate_af: true
+    ipv6_lla: true
+    local_as: true
+    rfc8950: true
+    vrf_local_as: true
+  evpn:
+    asymmetrical_irb: true
+    irb: true
+  gateway:
+    protocol: [ vrrp ]
+  isis: true
   mpls:
-    ldp: True
-    vpn: True
+    ldp: true
+    vpn: true
+  ospf:
+    unnumbered: true
   vlan:
     model: l3-switch
     svi_interface_name: "br0.{vlan}"
     subif_name: "{ifname}.{vlan.access_id}"
-    native_routed: True
-  evpn:
-    irb: True
-    asymmetrical_irb: True
-  gateway:
-    protocol: [ vrrp ]
+    native_routed: true
+  vrf: true
+  vxlan: true
 clab:
   image: ghcr.io/sysoleg/vyos-container
   mtu: 1500
   node:
     kind: linux
     binds:
       '/lib/modules': '/lib/modules'
```

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/default-originate.yml` & `networklab-1.6.0/netsim/extra/ebgp.utils/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/eos.j2` & `networklab-1.6.0/netsim/extra/ebgp.utils/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/frr.j2` & `networklab-1.6.0/netsim/extra/ebgp.utils/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/ios.j2` & `networklab-1.6.0/netsim/extra/ebgp.utils/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/junos.j2` & `networklab-1.6.0/netsim/extra/ebgp.utils/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/plugin.py` & `networklab-1.6.0/netsim/extra/ebgp.utils/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/routeros7.j2` & `networklab-1.6.0/netsim/extra/ebgp.utils/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/srlinux.j2` & `networklab-1.6.0/netsim/extra/ebgp.utils/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/vyos.j2` & `networklab-1.6.0/netsim/extra/ebgp.utils/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/multilab/plugin.py` & `networklab-1.6.0/netsim/extra/multilab/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/proxy-arp/plugin.py` & `networklab-1.6.0/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.6.0/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/extra/proxy-arp/sros.j2` & `networklab-1.6.0/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/ansible.sh` & `networklab-1.6.0/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/containerlab.sh` & `networklab-1.6.0/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/grpc.sh` & `networklab-1.6.0/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/arubacx.txt` & `networklab-1.6.0/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/asav/day0-config` & `networklab-1.6.0/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/csr.txt` & `networklab-1.6.0/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/dellos10.txt` & `networklab-1.6.0/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/eos.txt` & `networklab-1.6.0/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/eos.xml.j2` & `networklab-1.6.0/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/iosv.txt` & `networklab-1.6.0/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.6.0/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/iosxr.txt` & `networklab-1.6.0/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/nxos.txt` & `networklab-1.6.0/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.6.0/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/routeros7.txt` & `networklab-1.6.0/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/vptx/juniper.conf` & `networklab-1.6.0/netsim/install/libvirt/vptx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/vptx/make-config.sh` & `networklab-1.6.0/netsim/install/libvirt/vptx/make-config.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/vptx/run.sh` & `networklab-1.6.0/netsim/install/libvirt/vptx/run.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/vptx.txt` & `networklab-1.6.0/netsim/install/libvirt/vptx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/vptx.xml.j2` & `networklab-1.6.0/netsim/install/libvirt/vptx.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.6.0/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt/vsrx.txt` & `networklab-1.6.0/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/libvirt.sh` & `networklab-1.6.0/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/install/ubuntu.sh` & `networklab-1.6.0/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/__init__.py` & `networklab-1.6.0/netsim/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/_dataplane.py` & `networklab-1.6.0/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/_routing.py` & `networklab-1.6.0/netsim/modules/_routing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/bfd.py` & `networklab-1.6.0/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/bfd.yml` & `networklab-1.6.0/netsim/modules/bfd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BFD (RFC 5880) default settings and attributes
 #
-# Also supported on: eos, csr, iosv
+# Also supported on: eos, csr, iosv, vyos, arubacx
 #
-supported_on: [ srlinux, sros, nxos, vyos, arubacx, none ]
+supported_on: [ srlinux, sros, nxos, none ]
 min_echo_rx: 0      # Echo function, 0=disabled by default
 multiplier: 3       # Detection time multiplier, number of packets lost before down
 attributes:
   global:
     min_tx: { type: int, min_value: 1 }
     min_rx: { type: int, min_value: 1 }
     min_echo_rx: { type: int, min_value: 0 }
```

### Comparing `networklab-1.5.5.dev3/netsim/modules/bgp.py` & `networklab-1.6.0/netsim/modules/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/bgp.yml` & `networklab-1.6.0/netsim/modules/bgp.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # BGP default settings and attributes
 #
-# Also supported on: eos, csr, frr, iosv, nxos
+# Also supported on: eos, csr, frr, iosv, nxos, vyos, routeros, dellos10, routeros7, arubacx, junos (vmx, vsrx, vptx)
 #
-supported_on: [ cumulus, cumulus_nvue, asav, vsrx, vyos, routeros,
-  srlinux, sros, none, dellos10, routeros7, vmx, iosxr, arubacx, vptx, none ]
+supported_on: [ cumulus, cumulus_nvue, asav,
+  srlinux, sros, none, iosxr, none ]
 ebgp_role: external
 advertise_roles: [ stub ]
 advertise_loopback: True
 community:
   ibgp: [ standard, extended ]
   ebgp: [ standard ]
 no_propagate: [ ebgp_role, advertise_roles, rr_list, as_list ]
```

### Comparing `networklab-1.5.5.dev3/netsim/modules/evpn.py` & `networklab-1.6.0/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/evpn.yml` & `networklab-1.6.0/netsim/modules/evpn.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # EVPN default settings and attributes
 #
-# Also supported on eos
+# Also supported on eos, vyos, dellos10, arubacx, vptx
 #
 requires: [ bgp ]
-supported_on: [ sros, srlinux, frr, vyos, dellos10, cumulus, nxos, arubacx, vptx, none ]
+supported_on: [ sros, srlinux, frr, cumulus, nxos, none ]
 no_propagate: [ start_transit_vni, transport, vlan_bundle_service, as ]
 transform_after: [ vlan, vxlan, vrf ]
 config_after: [ vlan, vxlan, vrf ]
 session: [ ibgp ]
 start_transit_vni: 200000
 attributes:
   global:
```

### Comparing `networklab-1.5.5.dev3/netsim/modules/gateway.py` & `networklab-1.6.0/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/gateway.yml` & `networklab-1.6.0/netsim/modules/gateway.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Gateway (FHRP) default settings and attributes
 #
-# Also supported on: eos, csr, nxos, iosv
+# Also supported on: eos, csr, nxos, iosv, vyos, dellos10, arubacx
 #
-supported_on: [ none, cumulus, sros, srlinux, vyos, dellos10, arubacx ]
+supported_on: [ none, cumulus, sros, srlinux ]
 transform_after: [ vlan, vrf, ospf, isis, eigrp ]
 config_after: [ vlan,vrf ]
 id: -2
 protocol: anycast
 anycast:
   mac: 0200.cafe.00ff
   unicast: True
```

### Comparing `networklab-1.5.5.dev3/netsim/modules/isis.py` & `networklab-1.6.0/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/isis.yml` & `networklab-1.6.0/netsim/modules/isis.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ISIS default settings and attributes
 #
-# Also supported on csr, eos, frr, iosv, nxos
+# Also supported on csr, eos, frr, iosv, nxos, vyos, junos (vmx, vsrx, vptx)
 #
-supported_on: [ asav, vsrx, srlinux, sros, vyos, vmx, iosxr, vptx, none ]
+supported_on: [ asav, srlinux, sros, iosxr, none ]
 area: "49.0001"
 type: level-2
 transform_after: [ vlan,vrf ]
 config_after: [ vlan ]
 attributes:
   global:
     af:
```

### Comparing `networklab-1.5.5.dev3/netsim/modules/mpls.py` & `networklab-1.6.0/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/mpls.yml` & `networklab-1.6.0/netsim/modules/mpls.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # MPLS (LDP, BGP LU, L3VPN, 6PE) default settings and attributes
 #
-# Also supported on: eos, csr, frr, iosv
+# Also supported on: eos, csr, frr, iosv, routeros, vyos, routeros7, arubacx, junos (vmx, vsrx, vptx)
 #
-supported_on: [ routeros, vyos, routeros7, sros, vmx, vsrx, none, vptx, arubacx ]
+supported_on: [ sros, none ]
 config_after: [ vlan, ospf, isis, bgp ]
 transform_after: [ vlan, bgp ]
 ldp: True
 attributes:
   global:
     ldp:
       _alt_types: [ bool ]
```

### Comparing `networklab-1.5.5.dev3/netsim/modules/ospf.py` & `networklab-1.6.0/netsim/modules/ospf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/ospf.yml` & `networklab-1.6.0/netsim/modules/ospf.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # OSPFv2/OSPFv3 default settings and attributes
 #
-# Also supported on csr, eos, frr, iosv, nxos
+# Also supported on csr, eos, frr, iosv, nxos, vyos, routeros, dellos10, routeros7, arubacx, junos (vmx, vsrx, vptx)
 #
 area: 0.0.0.0
 supported_on: [
-  arcos, cumulus, cumulus_nvue, fortios, vsrx, vyos, routeros,
-  srlinux, sros, dellos10, routeros7, vmx, iosxr, arubacx, vptx, none ]
+  arcos, cumulus, cumulus_nvue, fortios,
+  srlinux, sros, iosxr, none ]
 transform_after: [ vlan,vrf ]
 config_after: [ vlan ]
 attributes:
   global:
     af:
       _list_to_dict: True
       _alt_types: [ NoneType ]
```

### Comparing `networklab-1.5.5.dev3/netsim/modules/srv6.py` & `networklab-1.6.0/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/srv6.yml` & `networklab-1.6.0/netsim/modules/srv6.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/vlan.py` & `networklab-1.6.0/netsim/modules/vlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/vlan.yml` & `networklab-1.6.0/netsim/modules/vlan.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # VLAN default settings and attributes
 #
-# Also supported on csr, eos, frr, iosv, nxos
+# Also supported on csr, eos, frr, iosv, nxos, vyos, dellos10, routeros, routeros7, arubacx, junos (vmx, vsrx, vptx)
 #
-supported_on: [ vyos, dellos10, srlinux, none, routeros, cumulus, sros, routeros7, vmx, vsrx, arubacx, vptx, none ]
+supported_on: [ srlinux, none, cumulus, sros, none ]
 no_propagate: [ start_vlan_id, mode ]
 start_vlan_id: 1000
 mode: irb
 attributes:
   global:
     mode: { type: str, valid_values: [ bridge, irb, route] }
   node:
```

### Comparing `networklab-1.5.5.dev3/netsim/modules/vrf.py` & `networklab-1.6.0/netsim/modules/vrf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/vxlan.py` & `networklab-1.6.0/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/modules/vxlan.yml` & `networklab-1.6.0/netsim/modules/vxlan.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # VXLAN default settings and attributes
 #
-# Also supported on csr, eos, frr, nxos
+# Also supported on csr, eos, frr, nxos, vyos, dellos10, arubacx, vptx
 #
-supported_on: [ vyos, dellos10, srlinux, cumulus, sros, arubacx, vptx, none ]
+supported_on: [ srlinux, cumulus, sros, none ]
 requires: [ vlan ]
 config_after: [ vrf ] # For platforms that suppport L3 VXLAN, vrfs must be created first
 transform_after: [ vlan, vrf ]
 domain: global
 flooding: static
 start_vni: 100000
 attributes:
```

### Comparing `networklab-1.5.5.dev3/netsim/outputs/__init__.py` & `networklab-1.6.0/netsim/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/outputs/ansible.py` & `networklab-1.6.0/netsim/outputs/ansible.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,16 @@
 
   _files.create_file_from_text(config_file,cfg_text)
   if not common.QUIET:
     print("Created Ansible configuration file: %s" % config_file)
 
 class AnsibleInventory(_TopologyOutput):
 
+  DESCRIPTION :str = 'Ansible inventory and configuration file'
+
   def write(self, topology: Box) -> None:
     check_writeable('Ansible inventory')
     hostfile = self.settings.hostfile or 'hosts.yml'
     configfile = self.settings.configfile or 'ansible.cfg'
     output_format = None
 
     if hasattr(self,'filenames'):
```

### Comparing `networklab-1.5.5.dev3/netsim/outputs/common.py` & `networklab-1.6.0/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/outputs/d2.py` & `networklab-1.6.0/netsim/outputs/d2.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,14 +264,16 @@
   for n,ndata in topology.nodes.items():
     dev_data = topology.defaults.devices[ndata.device]
     ndata.d2.type = dev_data.graphite.icon or 'router'
     ndata.d2.name = n
 
 class Graph(_TopologyOutput):
 
+  DESCRIPTION :str = 'Topology graph in D2 format'
+
   def write(self, topology: Box) -> None:
     graphfile = self.settings.filename or 'graph.d2'
     output_format = 'topology'
 
     topology = get_box(topology)                       # Create a local copy of the topology
     set_d2_attr(topology)
     if hasattr(self,'filenames'):
```

### Comparing `networklab-1.5.5.dev3/netsim/outputs/d2.yml` & `networklab-1.6.0/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/outputs/devices.py` & `networklab-1.6.0/netsim/outputs/devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,16 @@
   if host in (data or {}):
     return data[host]
 
   return None
 
 class DeviceInventory(_TopologyOutput):
 
+  DESCRIPTION :str = 'Create simple device inventory as a YAML file'
+
   def write(self, topology: Box) -> None:
     check_writeable('netlab-devices.yml')
     hostfile = self.settings.hostfile or 'netlab-devices.yml'
     output_format = None
 
     if hasattr(self,'filenames'):
       hostfile = self.filenames[0]
```

### Comparing `networklab-1.5.5.dev3/netsim/outputs/graph.py` & `networklab-1.6.0/netsim/outputs/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,16 @@
 graph_dispatch = {
   'topology': graph_topology,
   'bgp': graph_bgp
 }
 
 class Graph(_TopologyOutput):
 
+  DESCRIPTION :str = 'Topology graph in graphviz format'
+
   def write(self, topology: Box) -> None:
     graphfile = self.settings.filename or 'graph.dot'
     output_format = 'topology'
 
     if hasattr(self,'filenames'):
       graphfile = self.filenames[0]
       if len(self.filenames) > 1:
```

### Comparing `networklab-1.5.5.dev3/netsim/outputs/graphite.py` & `networklab-1.6.0/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/outputs/provider.py` & `networklab-1.6.0/netsim/outputs/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 def write_provider_file(topology: Box, provider: str, filename: typing.Optional[str]) -> None:
   p_module = get_provider_module(topology,provider)
   p_module.create(topology,filename)
 
 class ProviderConfiguration(_TopologyOutput):
 
+  DESCRIPTION :str = 'Create virtualization provider configuration file(s)'
+
   def write(self, topology: Box) -> None:
     check_writeable('provider configuration')
     filename = None
     if hasattr(self,'filenames'):
       filename = self.filenames[0]
       if len(self.filenames) > 1:
         common.error('Extra output filename(s) ignored: %s' % str(self.filenames[1:]),common.IncorrectValue,'provider')
```

### Comparing `networklab-1.5.5.dev3/netsim/outputs/report.py` & `networklab-1.6.0/netsim/outputs/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     return ""
 
 def render(fmt: str, settings: Box, topo: Box) -> str:
   return render_from_settings(settings,fmt,topo) if fmt in settings else render_from_file(fmt,topo)
 
 class REPORT(_TopologyOutput):
 
+  DESCRIPTION :str = 'Create a report from the transformed lab topology data'
+
   def write(self, topo: Box) -> None:
     global EXTRA_PATH
     EXTRA_PATH = _files.get_search_path("reports")
     outfile = self.settings.filename or '-'
     modname = type(self).__name__
 
     if hasattr(self,'filenames'):
```

### Comparing `networklab-1.5.5.dev3/netsim/outputs/tools.py` & `networklab-1.6.0/netsim/outputs/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,14 +61,16 @@
       _files.create_file_from_text(fname,config_text)
       print(f'Created {fname} {config_src}')
     except Exception as e:
       common.error(f'Error writing tool configuration file {fname}\n... {e}')
 
 class ToolConfigs(_TopologyOutput):
 
+  DESCRIPTION :str = 'Create configuration files for external tools'
+
   def write(self, topology: Box) -> None:
     if not 'tools' in topology:
       return
 
     if hasattr(self,'filenames'):
       common.error('Tools output module does not accept extra parameters')
```

### Comparing `networklab-1.5.5.dev3/netsim/outputs/yaml.py` & `networklab-1.6.0/netsim/outputs/yaml.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from ..utils import files as _files
 from ..utils import log,strings
 
 from . import _TopologyOutput,check_writeable
 
 class YAML(_TopologyOutput):
 
+  DESCRIPTION :str = 'Inspect transformed data in YAML format'
+
   def write(self, topo: Box) -> None:
     outfile = self.settings.filename or '-'
     modname = type(self).__name__
 
     if hasattr(self,'filenames'):
       outfile = self.filenames[0]
       if len(self.filenames) > 1:
```

### Comparing `networklab-1.5.5.dev3/netsim/providers/__init__.py` & `networklab-1.6.0/netsim/providers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,7 +267,26 @@
   for n in list(topology.nodes.keys()):             # Remove all nodes not belonging to the current provider
     if topology.nodes[n].provider != provider:
       topology.nodes[n].unmanaged = True
 #      topology.nodes.pop(n,None)
 
   topology.links = [ l for l in topology.links if provider in l.provider ]      # Retain only the links used by current provider
   return topology
+
+"""
+get_forwarded_ports -- build a list of forwarded ports for the specified node
+"""
+def get_forwarded_ports(node: Box, topology: Box) -> list:
+  p = devices.get_provider(node,topology.defaults)
+  fmap = topology.defaults.providers[p].get('forwarded',{})     # Provider-specific forwarded ports
+  if not fmap:                                                  # No forwarded ports?
+    return []                                                   # ... return an empty list
+
+  pmap = topology.defaults.ports                                # Mappings of port names into TCP numbers
+  node_fp = []                                                  # Forwarded ports for the current node
+
+  for fp,fstart in fmap.items():                                # Iterate over forwarded ports
+    if not fp in pmap:                                          # Is the port we're trying to forward known to netlab?
+      continue                                                  # ... nope, bad luck, move on
+    node_fp.append([ fstart + node.id, pmap[fp]])               # Append [host,device] port mapping
+
+  return node_fp
```

### Comparing `networklab-1.5.5.dev3/netsim/providers/clab.py` & `networklab-1.6.0/netsim/providers/clab.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Containerlab provider module
 #
 import subprocess
 import typing
 import shutil
 from box import Box
 
-from . import _Provider
+from . import _Provider,get_forwarded_ports
 from .. import common
 from ..data import filemaps
 from ..cli import is_dry_run,external_commands
 
 def list_bridges( topology: Box ) -> typing.Set[str]:
   return { l.bridge for l in topology.links if l.bridge and l.node_count != 2 and not 'external_bridge' in l.clab }
 
@@ -66,14 +66,24 @@
   if status is False:
     return False
   common.print_verbose( f"Delete OVS bridge '{brname}': {status}" )
   return True
 
 GENERATED_CONFIG_PATH = "clab_files"
 
+def add_forwarded_ports(node: Box, fplist: list) -> None:
+  if not fplist:
+    return
+  
+  node.clab.ports = node.clab.ports or []                       # Make sure the list of forwarded ports is a list
+  for port_map in fplist:                                       # Iterate over forwarded port mappings
+    port_map_string = f'{port_map[0]}:{port_map[1]}'            # Build the containerlab-compatible map entry
+    if not port_map_string in node.clab.ports:                  # ... and add it to the list of forwarded ports
+      node.clab.ports.append(port_map_string)                   # ... if the user didn't do it manually
+
 '''
 normalize_clab_filemaps: convert clab templates and file binds into host:target lists
 '''
 def normalize_clab_filemaps(node: Box) -> None:
   for undot_key in ['clab.binds','clab.config_templates']:
     if not undot_key in node:
       continue
@@ -83,14 +93,18 @@
   
   def augment_node_data(self, node: Box, topology: Box) -> None:
     node.hostname = "clab-%s-%s" % (topology.name,node.name)
     normalize_clab_filemaps(node)
 
     self.create_extra_files_mappings(node,topology)
 
+    node_fp = get_forwarded_ports(node,topology)
+    if node_fp:
+      add_forwarded_ports(node,node_fp)
+
   def post_configuration_create(self, topology: Box) -> None:
     for n in topology.nodes.values():
       if n.get('clab.binds',None):
         self.create_extra_files(n,topology)
 
   def pre_start_lab(self, topology: Box) -> None:
     common.print_verbose('pre-start hook for Containerlab - create any bridges')
```

### Comparing `networklab-1.5.5.dev3/netsim/providers/clab.yml` & `networklab-1.6.0/netsim/providers/clab.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 #
 # CLAB settings
 #
+description: containerlab with Docker
 config: clab.yml
 node_config_attributes: [ type, cmd, env, ports ]
 template: clab.j2
 # Preserve env to allow user to configure PATH
 start: sudo -E containerlab deploy -t clab.yml
 stop: sudo -E containerlab destroy --cleanup -t clab.yml
 act_probe: "docker ps"
 act_title: "Running containers"
 probe:
 - cmd: "containerlab version"
   err: "Containerlab is not installed"
-- cmd: [ bash, '-c', "[[ `containerlab version|awk '/version/ {print $2}'` > '0.40' ]] && echo OK" ]
-  err: "Containerlab version is too old, please upgrade to 0.41 or later"
+- cmd: [ bash, '-c', "[[ `containerlab version|awk '/version/ {print $2}'` > '0.42' ]] && echo OK" ]
+  err: "Containerlab version is too old, please upgrade to 0.43 or later"
 
 cleanup: [ clab.yml,clab_files ]
 bridge_type: bridge # Use 'ovs-bridge' to create Openvswitch bridges
 runtime: docker     # Default runtime, see Containerlab documentation
 attributes:
   node:
     binds:
     kind: str
     config_templates:
     type: str
     cmd: str
     env:
-    ports:
+    ports: list
     image: str
     startup-config: str
     srl-agents:
     license: str
     runtime: str
   interface:
     name: str
```

### Comparing `networklab-1.5.5.dev3/netsim/providers/libvirt.py` & `networklab-1.6.0/netsim/providers/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/providers/libvirt.yml` & `networklab-1.6.0/netsim/providers/libvirt.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #
 # vagrant-libvirt settings
 #
+description: Vagrant with libvirt/KVM
 config: Vagrantfile
 start: vagrant up --provider libvirt
 stop: vagrant destroy -f
 probe:
 - cmd: which kvm-ok
   err: "KVM is not installed"
 - cmd: which virsh
```

### Comparing `networklab-1.5.5.dev3/netsim/read_topology.py` & `networklab-1.6.0/netsim/read_topology.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,59 +2,24 @@
 # Read topology and default settings files
 #
 import os
 import sys
 import typing
 import argparse
 import pathlib
-import fnmatch
 
 from box import Box
-try:
-  from importlib import resources
-  new_resources = hasattr(resources,'files')
-except ImportError:
-  new_resources = False
-  import importlib_resources as resources         # type: ignore
 
 # Related modules
 from . import common
 from . import data
 from .data import types
 from .utils import files as _files
 
 """
-Utility routines for include_yaml functionality
-"""
-
-def get_traversable_path(dir_name : str) -> typing.Any:
-  if 'package:' in dir_name:
-    dir_name = dir_name.replace('package:','')
-    pkg_files: typing.Any = None
-
-    if not new_resources:
-      pkg_files = pathlib.Path(_files.get_moddir())
-    else:
-      package = '.'.join(__name__.split('.')[:-1])
-      pkg_files = resources.files(package)        # type: ignore
-    if dir_name == '':
-      return pkg_files
-    else:
-      return pkg_files.joinpath(dir_name)
-  else:
-    return pathlib.Path(dir_name)
-
-def get_globbed_files(path: typing.Any, glob: str) -> list:
-  if isinstance(path,pathlib.Path):
-    return [ str(fname) for fname in list(path.glob(glob)) ]
-  else:
-    file_names = list(path.iterdir())
-    return fnmatch.filter(file_names,glob)
-
-"""
 include_yaml: Include YAML snippets at any position within a YAML file
 
 * scan all dictionaries for '_include' key
 * every _include value should be a list of files to include
 
 Glob over all files to include:
 * try to read YAML file
@@ -79,16 +44,16 @@
     inc_path = os.path.dirname(source_file)
 
   for inc_name in data._include:                                            # Iterate over included files
     if "~/" in inc_name:
       file_path = os.path.dirname(os.path.expanduser(inc_name))
     else:
       file_path = inc_path + ('/' if '/' in inc_path else '') + os.path.dirname(inc_name)
-    traversable = get_traversable_path(file_path)                           # Get a traversable object
-    inc_files = get_globbed_files(traversable,os.path.basename(inc_name))   # Get all files matching the pattern
+    traversable = _files.get_traversable_path(file_path)                           # Get a traversable object
+    inc_files = _files.get_globbed_files(traversable,os.path.basename(inc_name))   # Get all files matching the pattern
     if not inc_files:
       common.fatal(f'Cannot find file {inc_name} to be included into {source_file}')
       return
 
     for file_name in inc_files:
       yaml_data = read_yaml(filename=file_name)
       if yaml_data is None:
@@ -116,15 +81,15 @@
     common.fatal("read_yaml: have no idea what to do") # pragma: no cover -- sanity check
     return None
 
   if filename in read_cache:
     return Box(read_cache[filename],default_box=True,box_dots=True,default_box_none_transform=False)
 
   if "package:" in filename:
-    pkg_files = get_traversable_path('package:')
+    pkg_files = _files.get_traversable_path('package:')
     with pkg_files.joinpath(filename.replace("package:","")).open('r') as fid:
       pkg_data = read_yaml(string=fid.read())
       if not pkg_data is None:
         include_yaml(pkg_data,filename)
         read_cache[filename] = Box(pkg_data)
       return pkg_data
   else:
```

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/clab/clab.j2` & `networklab-1.6.0/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.6.0/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.6.0/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files 12% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 {%   if 'remote_ifindex' in l: %}
 {%     include "libvirt-tunnel.j2" %}
 {%   else %}
 {%     include "libvirt-bridge.j2" %}
 {%   endif %}
 
 {% endfor %}
+{% include 'forwarded-ports.j2' %}  
   end
```

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.6.0/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vptx-domain.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/vptx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.6.0/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.6.0/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/tools/__init__.py` & `networklab-1.6.0/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/tools/graphite.py` & `networklab-1.6.0/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/tools/graphite.yml` & `networklab-1.6.0/netsim/tools/graphite.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/tools/suzieq.yml` & `networklab-1.6.0/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/topology-defaults.yml` & `networklab-1.6.0/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/utils/files.py` & `networklab-1.6.0/netsim/utils/files.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,25 @@
 # File handling routines
 #
 
 import pathlib
 import os
 import sys
 import typing
+import fnmatch
+
 from . import log
 
+try:
+  from importlib import resources
+  new_resources = hasattr(resources,'files')
+except ImportError:
+  new_resources = False
+  import importlib_resources as resources         # type: ignore
+
 #
 # Find paths to module, user and system directory (needed for various templates)
 #
 def get_moddir() -> pathlib.Path:
   return pathlib.Path(__file__).resolve().parent.parent
 
 def get_userdir() -> pathlib.Path:
@@ -50,14 +59,45 @@
     candidate = os.path.join(dirname, path)
     if os.path.exists(candidate):
       return candidate
 
   return None
 
 #
+# Get a list of files matching a glob pattern
+#
+def get_globbed_files(path: typing.Any, glob: str) -> list:
+  if isinstance(path,pathlib.Path):
+    return [ str(fname) for fname in list(path.glob(glob)) ]
+  else:
+    file_names = list(path.iterdir())
+    return fnmatch.filter(file_names,glob)
+
+#
+# Get a path object that can be used to find files in a file system or in the package
+#
+
+def get_traversable_path(dir_name : str) -> typing.Any:
+  if 'package:' in dir_name:
+    dir_name = dir_name.replace('package:','')
+    pkg_files: typing.Any = None
+
+    if not new_resources:
+      pkg_files = pathlib.Path(get_moddir())
+    else:
+      package = '.'.join(__name__.split('.')[:-2])
+      pkg_files = resources.files(package)        # type: ignore
+    if dir_name == '':
+      return pkg_files
+    else:
+      return pkg_files.joinpath(dir_name)
+  else:
+    return pathlib.Path(dir_name)
+
+#
 # Open, close, and write to file (or STDOUT)
 #
 
 def open_output_file(fname: str) -> typing.TextIO:
   if fname == '-':
     return sys.stdout
```

### Comparing `networklab-1.5.5.dev3/netsim/utils/log.py` & `networklab-1.6.0/netsim/utils/log.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/netsim/utils/status.py` & `networklab-1.6.0/netsim/utils/status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 #
 # Common routines used to implement lab status and locking commands
 #
 
 import typing
 import os
 import sys
+import traceback
 from box import Box
 from filelock import Timeout, FileLock
 
 from ..common import fatal, get_yaml_string,debug_active
 from ..data import get_empty_box
 
 '''
 get_status_filename -- get the name of the netlab status file
 '''
 def get_status_filename(topology: Box) -> str:
   status_file = topology.defaults.lab_status_file or '~/.netlab/status.yaml'
   return os.path.expanduser(status_file)
 
 '''
+Get lab ID for multilab deployments (moved here to be used by more than just CLI routines)
+'''
+def get_lab_id(topology: Box) -> str:
+  return topology.get('defaults.multilab.id','default') or 'default'    # id could be set to {} due to tool f-string evals
+
+'''
 change_status -- change the status of a lab
 
 * Lock the lab status file
 * Read the YAML document in the lab status file
 * Call a callback function to change the status
 * Write the modified YAML document
 * Unlock the lab status file
@@ -66,20 +73,30 @@
   
   try:
     return Box().from_yaml(filename=status_file,default_box=True,box_dots=True)
   except:
     fatal(f'Cannot read lab status file {status_file}')
     return get_empty_box()
 
-lock_file: typing.Final[str] = 'netlab.lock'
+'''
+Remove the lab instance/directory from the status file
+'''
+def remove_lab_status(topology: Box) -> None:
+  lab_id = get_lab_id(topology)
+
+  change_status(
+    topology,
+    callback = lambda s,t: s.pop(lab_id,None))
 
 '''
 lock_directory -- create netlab.lock file in current directory to prevent 
                   overwriting provider configuration files or Ansible inventory
 '''
+lock_file: typing.Final[str] = 'netlab.lock'
+
 def lock_directory() -> None:
   global lock_file
   with open(lock_file, 'w') as f:
     f.write('netlab lock file, do not remove')
 
 '''
 unlock_directory -- remove netlab.lock file in current directory
```

### Comparing `networklab-1.5.5.dev3/netsim/utils/templates.py` & `networklab-1.6.0/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/networklab.egg-info/PKG-INFO` & `networklab-1.6.0/networklab.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.5.dev3
+Version: 1.6.0
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,19 +30,17 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
+The latest release is [release 1.6.0](https://github.com/ipspace/netlab/releases/tag/release_1.6.0). It contains [numerous new features](https://netlab.tools/release/1.6/) that might have a few bugs attached to them. Should you encounter one of those creatures, please open a Github issue and use release 1.5.4. You might also want to [read the release notes](https://netlab.tools/release/).
 
-The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
-
-## An overview of tools:
+## An Overview of CLI Commands
 
 **netlab up**
 : Uses **[netlab create](https://netlab.tools/netlab/create/)** to create configuration files, starts the virtual lab, and uses **[netlab initial](https://netlab.tools/netlab/initial/)** to deploy device configurations, including IP addressing, LLDP, OSPF, BGP, IS-IS, EIGRP, VRRP, VLANs, VRFs, MPLS, SR-MPLS, VXLAN, EVPN and SRv6. [More details](https://netlab.tools/netlab/up/)
 
 **netlab down**
 : Destroys the virtual lab. [More details](https://netlab.tools/netlab/down/)
```

### Comparing `networklab-1.5.5.dev3/networklab.egg-info/SOURCES.txt` & `networklab-1.6.0/networklab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -362,14 +362,22 @@
 netsim/cli/show.py
 netsim/cli/status.py
 netsim/cli/test.py
 netsim/cli/up.py
 netsim/cli/usage.py
 netsim/cli/usage.txt
 netsim/cli/version.py
+netsim/cli/show_commands/__init__.py
+netsim/cli/show_commands/devices.py
+netsim/cli/show_commands/images.py
+netsim/cli/show_commands/module_support.py
+netsim/cli/show_commands/modules.py
+netsim/cli/show_commands/outputs.py
+netsim/cli/show_commands/providers.py
+netsim/cli/show_commands/reports.py
 netsim/data/__init__.py
 netsim/data/filemaps.py
 netsim/data/global_vars.py
 netsim/data/types.py
 netsim/data/validate.py
 netsim/defaults/addressing.yml
 netsim/defaults/attributes.yml
@@ -390,14 +398,15 @@
 netsim/devices/eos.yml
 netsim/devices/fortios.yml
 netsim/devices/frr.yml
 netsim/devices/iosv.py
 netsim/devices/iosv.yml
 netsim/devices/iosxr.yml
 netsim/devices/junos.py
+netsim/devices/junos.yml
 netsim/devices/linux.yml
 netsim/devices/none.yml
 netsim/devices/nxos.yml
 netsim/devices/routeros.yml
 netsim/devices/routeros7.yml
 netsim/devices/srlinux.yml
 netsim/devices/sros.yml
@@ -406,37 +415,29 @@
 netsim/devices/vmx.py
 netsim/devices/vmx.yml
 netsim/devices/vptx.py
 netsim/devices/vptx.yml
 netsim/devices/vsrx.py
 netsim/devices/vsrx.yml
 netsim/devices/vyos.yml
-netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
 netsim/extra/ebgp.utils/default-originate.yml
 netsim/extra/ebgp.utils/eos.j2
 netsim/extra/ebgp.utils/frr.j2
 netsim/extra/ebgp.utils/ios.j2
 netsim/extra/ebgp.utils/junos.j2
 netsim/extra/ebgp.utils/plugin.py
 netsim/extra/ebgp.utils/routeros7.j2
 netsim/extra/ebgp.utils/srlinux.j2
 netsim/extra/ebgp.utils/topology.yml
 netsim/extra/ebgp.utils/vyos.j2
-netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
-netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
 netsim/extra/multilab/plugin.py
-netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
-netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
 netsim/extra/none/none.j2
 netsim/extra/proxy-arp/plugin.py
 netsim/extra/proxy-arp/srlinux.j2
 netsim/extra/proxy-arp/sros.j2
-netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
-netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
-netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
 netsim/install/ansible.sh
 netsim/install/containerlab.sh
 netsim/install/grpc.sh
 netsim/install/libvirt.sh
 netsim/install/ubuntu.sh
 netsim/install/libvirt/arubacx.txt
 netsim/install/libvirt/asav.txt
@@ -450,15 +451,14 @@
 netsim/install/libvirt/nxos.txt
 netsim/install/libvirt/nxos.xml.j2
 netsim/install/libvirt/routeros7.txt
 netsim/install/libvirt/vptx.txt
 netsim/install/libvirt/vptx.xml.j2
 netsim/install/libvirt/vsrx.txt
 netsim/install/libvirt/asav/day0-config
-netsim/install/libvirt/iosxr/iosxr_config.txt
 netsim/install/libvirt/vptx/juniper.conf
 netsim/install/libvirt/vptx/make-config.sh
 netsim/install/libvirt/vptx/run.sh
 netsim/install/libvirt/vsrx/juniper.conf
 netsim/modules/__init__.py
 netsim/modules/_dataplane.py
 netsim/modules/_routing.py
@@ -526,14 +526,15 @@
 netsim/templates/provider/libvirt/csr-domain.j2
 netsim/templates/provider/libvirt/cumulus-domain.j2
 netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
 netsim/templates/provider/libvirt/define-domain.j2
 netsim/templates/provider/libvirt/dellos10-domain.j2
 netsim/templates/provider/libvirt/eos-domain.j2
 netsim/templates/provider/libvirt/fortios-domain.j2
+netsim/templates/provider/libvirt/forwarded-ports.j2
 netsim/templates/provider/libvirt/frr-domain.j2
 netsim/templates/provider/libvirt/iosv-domain.j2
 netsim/templates/provider/libvirt/iosxr-domain.j2
 netsim/templates/provider/libvirt/libvirt-bridge.j2
 netsim/templates/provider/libvirt/libvirt-tunnel.j2
 netsim/templates/provider/libvirt/linux-domain.j2
 netsim/templates/provider/libvirt/none-domain.j2
@@ -549,14 +550,15 @@
 netsim/templates/provider/virtualbox/cumulus-domain.j2
 netsim/templates/provider/virtualbox/eos-domain.j2
 netsim/templates/provider/virtualbox/frr-domain.j2
 netsim/templates/provider/virtualbox/linux-domain.j2
 netsim/templates/provider/virtualbox/nxos-domain.j2
 netsim/templates/provider/virtualbox/virtualbox-network.j2
 netsim/templates/provider/virtualbox/virtualbox-ports.j2
+netsim/templates/provider/virtualbox/vsrx-domain.j2
 netsim/templates/tests/clab.yml
 netsim/templates/tests/libvirt.yml
 netsim/templates/tests/virtualbox.yml
 netsim/tools/__init__.py
 netsim/tools/graphite.py
 netsim/tools/graphite.yml
 netsim/tools/suzieq.yml
```

### Comparing `networklab-1.5.5.dev3/setup.py` & `networklab-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev3/tests/test_transformation.py` & `networklab-1.6.0/tests/test_transformation.py`

 * *Files identical despite different names*

