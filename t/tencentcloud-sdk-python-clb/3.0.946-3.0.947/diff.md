# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.946.tar", last modified: Mon Jul 31 00:22:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.947.tar", last modified: Tue Aug  1 00:33:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.946.tar` & `tencentcloud-sdk-python-clb-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89989 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)   507898 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    90730 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)   507968 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:33:53.000000 tencentcloud-sdk-python-clb-3.0.947/tencentcloud_sdk_python_clb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-clb-3.0.946/setup.py` & `tencentcloud-sdk-python-clb-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/v20180317/clb_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,19 +143,29 @@
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloneLoadBalancer(self, request):
         """克隆负载均衡实例，根据指定的负载均衡实例，复制出相同规则和绑定关系的负载均衡实例。克隆接口为异步操作，克隆的数据以调用CloneLoadBalancer时为准，如果调用CloneLoadBalancer后克隆CLB发生变化，变化规则不会克隆。
 
         限制说明：
-        不支持基础网络和传统型负载均衡、IPv6和NAT64
-        不支持包年包月CLB
-        不支持监听器为 QUIC、端口段
-        不支持后端类型为 目标组、SCF云函数
-        个性化配置、重定向配置、安全组默认放通开关 将不会被克隆，须手工配置
+        实例属性维度限制
+          仅支持克隆按量计费实例，不支持包年包月实例。
+          不支持克隆未关联实例计费项的 CLB。
+          不支持克隆传统型负载均衡实例和高防 CLB。
+          不支持克隆基础网络类型的实例。
+          不支持克隆 IPv6、IPv6 NAT64 版本以及混绑的实例。
+          个性化配置、重定向配置、安全组默认放通开关的配置将不会被克隆，需重新配置。
+          执行克隆操作前，请确保实例上没有使用已过期证书，否则会导致克隆失败。
+        监听器维度限制
+          不支持克隆监听器为 QUIC 类型和端口段的实例。
+          不支持监听器为 TCP_SSL 的内网型负载均衡的实例。
+          不支持克隆七层监听器没有转发规则的实例。
+          当实例的监听器个数超过50个时，不支持克隆。
+        后端服务维度限制
+          不支持克隆绑定的后端服务类型为目标组和 SCF 云函数的实例。
 
         通过接口调用：
         BGP带宽包必须传带宽包id
         独占集群克隆必须传对应的参数，否则按共享型创建
         功能内测中，[申请开通](https://console.cloud.tencent.com/workorder/category?level1_id=6&level2_id=163&source=0&data_title=%E8%B4%9F%E8%BD%BD%E5%9D%87%E8%A1%A1%20CLB&step=1)。
 
         :param request: Request instance for CloneLoadBalancer.
```

### Comparing `tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.947/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1883,15 +1883,15 @@
         :param _SlaveZoneId: 仅适用于公网负载均衡。设置跨可用区容灾时的备可用区ID，例如 100001 或 ap-guangzhou-1
 注：备可用区是主可用区故障后，需要承载流量的可用区。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213) 接口查询一个地域的主/备可用区的列表。
         :type SlaveZoneId: str
         :param _ZoneId: 仅适用于公网负载均衡。可用区ID，指定可用区以创建负载均衡实例。如：ap-guangzhou-1。
         :type ZoneId: str
         :param _InternetAccessible: 仅适用于公网负载均衡。负载均衡的网络计费模式。
         :type InternetAccessible: :class:`tencentcloud.clb.v20180317.models.InternetAccessible`
-        :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 DescribeSingleIsp 接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
+        :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213)  接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
         :type VipIsp: str
         :param _Vip: 指定Vip申请负载均衡。
         :type Vip: str
         :param _Tags: 购买负载均衡同时，给负载均衡打上标签。
         :type Tags: list of TagInfo
         :param _ExclusiveCluster: 独占集群信息。
         :type ExclusiveCluster: :class:`tencentcloud.clb.v20180317.models.ExclusiveCluster`
@@ -2886,22 +2886,22 @@
         :type LoadBalancerId: str
         :param _Ports: 要将监听器创建到哪些端口，每个端口对应一个新的监听器。
         :type Ports: list of int
         :param _Protocol: 监听器协议： TCP | UDP | HTTP | HTTPS | TCP_SSL | QUIC。
         :type Protocol: str
         :param _ListenerNames: 要创建的监听器名称列表，名称与Ports数组按序一一对应，如不需立即命名，则无需提供此参数。
         :type ListenerNames: list of str
-        :param _HealthCheck: 健康检查相关参数，此参数仅适用于TCP/UDP/TCP_SSL监听器。
+        :param _HealthCheck: 健康检查相关参数，此参数仅适用于TCP/UDP/TCP_SSL/QUIC监听器。
         :type HealthCheck: :class:`tencentcloud.clb.v20180317.models.HealthCheck`
         :param _Certificate: 证书相关信息，此参数仅适用于TCP_SSL监听器和未开启SNI特性的HTTPS监听器。此参数和MultiCertInfo不能同时传入。
         :type Certificate: :class:`tencentcloud.clb.v20180317.models.CertificateInput`
         :param _SessionExpireTime: 会话保持时间，单位：秒。可选值：30~3600，默认 0，表示不开启。此参数仅适用于TCP/UDP监听器。
         :type SessionExpireTime: int
         :param _Scheduler: 监听器转发的方式。可选值：WRR、LEAST_CONN
-分别表示按权重轮询、最小连接数， 默认为 WRR。此参数仅适用于TCP/UDP/TCP_SSL监听器。
+分别表示按权重轮询、最小连接数， 默认为 WRR。此参数仅适用于TCP/UDP/TCP_SSL/QUIC监听器。
         :type Scheduler: str
         :param _SniSwitch: 是否开启SNI特性，此参数仅适用于HTTPS监听器。
         :type SniSwitch: int
         :param _TargetType: 后端目标类型，NODE表示绑定普通节点，TARGETGROUP表示绑定目标组。
         :type TargetType: str
         :param _SessionType: 会话保持类型。不传或传NORMAL表示默认会话保持类型。QUIC_CID 表示根据Quic Connection ID做会话保持。QUIC_CID只支持UDP协议。
         :type SessionType: str
@@ -3171,28 +3171,28 @@
         :param _LoadBalancerName: 负载均衡实例的名称，只在创建一个实例的时候才会生效。规则：1-60 个英文、汉字、数字、连接线“-”或下划线“_”。
 注意：如果名称与系统中已有负载均衡实例的名称相同，则系统将会自动生成此次创建的负载均衡实例的名称。
         :type LoadBalancerName: str
         :param _VpcId: 负载均衡后端目标设备所属的网络 ID，如vpc-12345678，可以通过 [DescribeVpcEx](https://cloud.tencent.com/document/product/215/1372) 接口获取。 不填此参数则默认为DefaultVPC。创建内网负载均衡实例时，此参数必填。
         :type VpcId: str
         :param _SubnetId: 在私有网络内购买内网负载均衡实例的情况下，必须指定子网 ID，内网负载均衡实例的 VIP 将从这个子网中产生。创建内网负载均衡实例时，此参数必填。
         :type SubnetId: str
-        :param _ProjectId: 负载均衡实例所属的项目 ID，可以通过 [DescribeProject](https://cloud.tencent.com/document/product/378/4400) 接口获取。不填此参数则视为默认项目。
+        :param _ProjectId: 负载均衡实例所属的项目 ID，可以通过 [DescribeProject](https://cloud.tencent.com/document/api/651/78725) 接口获取。不填此参数则视为默认项目。
         :type ProjectId: int
         :param _AddressIPVersion: 仅适用于公网负载均衡。IP版本，可取值：IPV4、IPV6、IPv6FullChain，不区分大小写，默认值 IPV4。说明：取值为IPV6表示为IPV6 NAT64版本；取值为IPv6FullChain，表示为IPv6版本。
         :type AddressIPVersion: str
         :param _Number: 创建负载均衡的个数，默认值 1。
         :type Number: int
         :param _MasterZoneId: 仅适用于公网负载均衡。设置跨可用区容灾时的主可用区ID，例如 100001 或 ap-guangzhou-1
 注：主可用区是需要承载流量的可用区，备可用区默认不承载流量，主可用区不可用时才使用备可用区，平台将为您自动选择最佳备可用区。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213) 接口查询一个地域的主可用区的列表。
         :type MasterZoneId: str
         :param _ZoneId: 仅适用于公网负载均衡。可用区ID，指定可用区以创建负载均衡实例。如：ap-guangzhou-1。
         :type ZoneId: str
         :param _InternetAccessible: 仅对内网属性的性能容量型实例和公网属性的所有实例生效。
         :type InternetAccessible: :class:`tencentcloud.clb.v20180317.models.InternetAccessible`
-        :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 DescribeSingleIsp 接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
+        :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213)  接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
         :type VipIsp: str
         :param _Tags: 购买负载均衡的同时，给负载均衡打上标签，最大支持20个标签键值对。
         :type Tags: list of TagInfo
         :param _Vip: 指定VIP申请负载均衡。此参数选填，不填写此参数时自动分配VIP。IPv4和IPv6类型支持此参数，IPv6 NAT64类型不支持。
 注意：当指定VIP创建内网实例、或公网IPv6 BGP实例时，若VIP不属于指定VPC子网的网段内时，会创建失败；若VIP已被占用，也会创建失败。
         :type Vip: str
         :param _BandwidthPackageId: 带宽包ID，指定此参数时，网络计费方式（InternetAccessible.InternetChargeType）只支持按带宽包计费（BANDWIDTH_PACKAGE）。
@@ -6470,15 +6470,15 @@
 
     def __init__(self):
         r"""
         :param _LoadBalancerId: 负载均衡实例 ID。
         :type LoadBalancerId: str
         :param _ListenerIds: 要查询的负载均衡监听器 ID 数组，最大为100个。
         :type ListenerIds: list of str
-        :param _Protocol: 要查询的监听器协议类型，取值 TCP | UDP | HTTP | HTTPS | TCP_SSL。
+        :param _Protocol: 要查询的监听器协议类型，取值 TCP | UDP | HTTP | HTTPS | TCP_SSL | QUIC。
         :type Protocol: str
         :param _Port: 要查询的监听器的端口。
         :type Port: int
         """
         self._LoadBalancerId = None
         self._ListenerIds = None
         self._Protocol = None
@@ -6980,15 +6980,15 @@
         :param _LoadBalancerType: 负载均衡实例的网络类型：
 OPEN：公网属性， INTERNAL：内网属性。
         :type LoadBalancerType: str
         :param _Forward: 负载均衡实例的类型。1：通用的负载均衡实例，0：传统型负载均衡实例。如果不传此参数，则查询所有类型的负载均衡实例。
         :type Forward: int
         :param _LoadBalancerName: 负载均衡实例的名称。
         :type LoadBalancerName: str
-        :param _Domain: 腾讯云为负载均衡实例分配的域名，本参数仅对传统型公网负载均衡才有意义。
+        :param _Domain: 腾讯云为负载均衡实例分配的域名。
         :type Domain: str
         :param _LoadBalancerVips: 负载均衡实例的 VIP 地址，支持多个。
         :type LoadBalancerVips: list of str
         :param _BackendPublicIps: 负载均衡绑定的后端服务的外网 IP，只支持查询云服务器的公网 IP。
         :type BackendPublicIps: list of str
         :param _BackendPrivateIps: 负载均衡绑定的后端服务的内网 IP，只支持查询云服务器的内网 IP。
         :type BackendPrivateIps: list of str
@@ -8628,21 +8628,21 @@
         :type ContextType: str
         :param _SendContext: 自定义探测相关参数。健康检查协议CheckType的值取CUSTOM时，必填此字段，代表健康检查发送的请求内容，只允许ASCII可见字符，最大长度限制500。（仅适用于TCP/UDP监听器）。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SendContext: str
         :param _RecvContext: 自定义探测相关参数。健康检查协议CheckType的值取CUSTOM时，必填此字段，代表健康检查返回的结果，只允许ASCII可见字符，最大长度限制500。（仅适用于TCP/UDP监听器）。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RecvContext: str
-        :param _CheckType: 自定义探测相关参数。健康检查使用的协议：TCP | HTTP | CUSTOM（仅适用于TCP/UDP监听器，其中UDP监听器只支持CUSTOM；如果使用自定义健康检查功能，则必传）。
+        :param _CheckType: 健康检查使用的协议。取值 TCP | HTTP | HTTPS | GRPC | PING | CUSTOM，UDP监听器支持PING/CUSTOM，TCP监听器支持TCP/HTTP/CUSTOM，TCP_SSL/QUIC监听器支持TCP/HTTP，HTTP规则支持HTTP/GRPC，HTTPS规则支持HTTP/HTTPS/GRPC。
 注意：此字段可能返回 null，表示取不到有效值。
         :type CheckType: str
-        :param _HttpVersion: 自定义探测相关参数。健康检查协议CheckType的值取HTTP时，必传此字段，代表后端服务的HTTP版本：HTTP/1.0、HTTP/1.1；（仅适用于TCP监听器）
+        :param _HttpVersion: HTTP版本。健康检查协议CheckType的值取HTTP时，必传此字段，代表后端服务的HTTP版本：HTTP/1.0、HTTP/1.1；（仅适用于TCP监听器）
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpVersion: str
-        :param _SourceIpType: 自定义探测相关参数。健康检查源IP类型：0（使用LB的VIP作为源IP），1（使用100.64网段IP作为源IP），默认值：0
+        :param _SourceIpType: 健康检查源IP类型：0（使用LB的VIP作为源IP），1（使用100.64网段IP作为源IP），默认值：0
 注意：此字段可能返回 null，表示取不到有效值。
         :type SourceIpType: int
         :param _ExtendedCode: GRPC健康检查状态码（仅适用于后端转发协议为GRPC的规则）。默认值为 12，可输入值为数值、多个数值、或者范围，例如 20 或 20,25 或 0-99
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExtendedCode: str
         """
         self._HealthSwitch = None
@@ -12042,17 +12042,17 @@
         :type LoadBalancerId: str
         :param _ListenerId: 负载均衡监听器ID。
         :type ListenerId: str
         :param _ListenerName: 新的监听器名称。
         :type ListenerName: str
         :param _SessionExpireTime: 会话保持时间，单位：秒。可选值：30~3600，默认 0，表示不开启。此参数仅适用于TCP/UDP监听器。
         :type SessionExpireTime: int
-        :param _HealthCheck: 健康检查相关参数，此参数仅适用于TCP/UDP/TCP_SSL监听器。
+        :param _HealthCheck: 健康检查相关参数，此参数仅适用于TCP/UDP/TCP_SSL/QUIC监听器。
         :type HealthCheck: :class:`tencentcloud.clb.v20180317.models.HealthCheck`
-        :param _Certificate: 证书相关信息，此参数仅适用于HTTPS/TCP_SSL监听器；此参数和MultiCertInfo不能同时传入。
+        :param _Certificate: 证书相关信息，此参数仅适用于HTTPS/TCP_SSL/QUIC监听器；此参数和MultiCertInfo不能同时传入。
         :type Certificate: :class:`tencentcloud.clb.v20180317.models.CertificateInput`
         :param _Scheduler: 监听器转发的方式。可选值：WRR、LEAST_CONN
 分别表示按权重轮询、最小连接数， 默认为 WRR。
         :type Scheduler: str
         :param _SniSwitch: 是否开启SNI特性，此参数仅适用于HTTPS监听器。注意：未开启SNI的监听器可以开启SNI；已开启SNI的监听器不能关闭SNI。
         :type SniSwitch: int
         :param _TargetType: 后端目标类型，NODE表示绑定普通节点，TARGETGROUP表示绑定目标组。
```

### Comparing `tencentcloud-sdk-python-clb-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.947/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.946'
+__version__ = '3.0.947'
```

### Comparing `tencentcloud-sdk-python-clb-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.947/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.946/README.rst` & `tencentcloud-sdk-python-clb-3.0.947/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.947/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

