# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.946.tar", last modified: Mon Jul 31 00:39:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.947.tar", last modified: Tue Aug  1 00:59:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.946.tar` & `tencentcloud-sdk-python-vpc-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   334726 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43302 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1324725 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:39:45.000000 tencentcloud-sdk-python-vpc-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   334726 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43302 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1325019 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:59:59.000000 tencentcloud-sdk-python-vpc-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.946/setup.py` & `tencentcloud-sdk-python-vpc-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9904,29 +9904,29 @@
 
     def __init__(self):
         r"""
         :param _VpcId: VPC实例ID。可通过[DescribeVpcs](https://cloud.tencent.com/document/product/215/15778)接口返回值中的VpcId获取。
         :type VpcId: str
         :param _VpnGatewayName: VPN网关名称，最大长度不能超过60个字节。
         :type VpnGatewayName: str
-        :param _InternetMaxBandwidthOut: 公网带宽设置。可选带宽规格：5, 10, 20, 50, 100；单位：Mbps
+        :param _InternetMaxBandwidthOut: 公网带宽设置。可选带宽规格：5, 10, 20, 50, 100, 200, 500, 1000, 3000；单位：Mbps。
         :type InternetMaxBandwidthOut: int
         :param _InstanceChargeType: VPN网关计费模式，PREPAID：表示预付费，即包年包月，POSTPAID_BY_HOUR：表示后付费，即按量计费。默认：POSTPAID_BY_HOUR，如果指定预付费模式，参数InstanceChargePrepaid必填。
         :type InstanceChargeType: str
         :param _InstanceChargePrepaid: 预付费模式，即包年包月相关参数设置。通过该参数可以指定包年包月实例的购买时长、是否设置自动续费等属性。若指定实例的付费模式为预付费则该参数必传。
         :type InstanceChargePrepaid: :class:`tencentcloud.vpc.v20170312.models.InstanceChargePrepaid`
         :param _Zone: 可用区，如：ap-guangzhou-2。
         :type Zone: str
-        :param _Type: VPN网关类型。值“CCN”云联网类型VPN网关，值SSL为SSL-VPN
+        :param _Type: VPN网关类型，默认为IPSEC。值“IPSEC”为VPC型IPSEC VPN网关，值“SSL”为VPC型SSL VPN网关，值“CCN”为云联网型IPSEC VPN网关，值“SSL_CCN”为云联网型SSL VPN网关。
         :type Type: str
-        :param _Tags: 指定绑定的标签列表，例如：[{"Key": "city", "Value": "shanghai"}]
+        :param _Tags: 指定绑定的标签列表，例如：[{"Key": "city", "Value": "shanghai"}]。
         :type Tags: list of Tag
-        :param _CdcId: CDC实例ID
+        :param _CdcId: CDC实例ID。
         :type CdcId: str
-        :param _MaxConnection: SSL-VPN 最大CLIENT 连接数。可选 [5, 10, 20, 50, 100]。仅SSL-VPN 需要选这个参数。
+        :param _MaxConnection: SSL VPN连接数设置，可选规格：5, 10, 20, 50, 100, 200, 500, 1000；单位：个。仅 SSL / SSL_CCN 类型需要选这个参数。
         :type MaxConnection: int
         """
         self._VpcId = None
         self._VpnGatewayName = None
         self._InternetMaxBandwidthOut = None
         self._InstanceChargeType = None
         self._InstanceChargePrepaid = None
@@ -42848,45 +42848,45 @@
         r"""
         :param _VpnGatewayId: 网关实例ID。
         :type VpnGatewayId: str
         :param _VpcId: VPC实例ID。
         :type VpcId: str
         :param _VpnGatewayName: 网关实例名称。
         :type VpnGatewayName: str
-        :param _Type: 网关实例类型：'IPSEC', 'SSL','CCN'。
+        :param _Type: 网关实例类型：'IPSEC', 'SSL','CCN','SSL_CCN'。
         :type Type: str
-        :param _State: 网关实例状态， 'PENDING'：生产中，'DELETING'：删除中，'AVAILABLE'：运行中。
+        :param _State: 网关实例状态， 'PENDING'：生产中，'PENDING_ERROR'：生产失败，'DELETING'：删除中，'DELETING_ERROR'：删除失败，'AVAILABLE'：运行中。
         :type State: str
         :param _PublicIpAddress: 网关公网IP。
         :type PublicIpAddress: str
         :param _RenewFlag: 网关续费类型：'NOTIFY_AND_MANUAL_RENEW'：手动续费，'NOTIFY_AND_AUTO_RENEW'：自动续费，'NOT_NOTIFY_AND_NOT_RENEW'：到期不续费。
         :type RenewFlag: str
-        :param _InstanceChargeType: 网关付费类型：POSTPAID_BY_HOUR：按小时后付费，PREPAID：包年包月预付费，
+        :param _InstanceChargeType: 网关付费类型：POSTPAID_BY_HOUR：按量计费，PREPAID：包年包月预付费。
         :type InstanceChargeType: str
         :param _InternetMaxBandwidthOut: 网关出带宽。
         :type InternetMaxBandwidthOut: int
         :param _CreatedTime: 创建时间。
         :type CreatedTime: str
         :param _ExpiredTime: 预付费网关过期时间。
         :type ExpiredTime: str
         :param _IsAddressBlocked: 公网IP是否被封堵。
         :type IsAddressBlocked: bool
         :param _NewPurchasePlan: 计费模式变更，PREPAID_TO_POSTPAID：包年包月预付费到期转按小时后付费。
         :type NewPurchasePlan: str
-        :param _RestrictState: 网关计费装，PROTECTIVELY_ISOLATED：被安全隔离的实例，NORMAL：正常。
+        :param _RestrictState: 网关计费状态，PROTECTIVELY_ISOLATED：被安全隔离的实例，NORMAL：正常。
         :type RestrictState: str
-        :param _Zone: 可用区，如：ap-guangzhou-2
+        :param _Zone: 可用区，如：ap-guangzhou-2。
         :type Zone: str
-        :param _VpnGatewayQuotaSet: 网关带宽配额信息
+        :param _VpnGatewayQuotaSet: 网关带宽配额信息。
         :type VpnGatewayQuotaSet: list of VpnGatewayQuota
-        :param _Version: 网关实例版本信息
+        :param _Version: 网关实例版本信息。
         :type Version: str
-        :param _NetworkInstanceId: Type值为CCN时，该值表示云联网实例ID
+        :param _NetworkInstanceId: Type值为CCN时，该值表示云联网实例ID。
         :type NetworkInstanceId: str
-        :param _CdcId: CDC 实例ID
+        :param _CdcId: CDC 实例ID。
         :type CdcId: str
         :param _MaxConnection: SSL-VPN 客户端连接数。
         :type MaxConnection: int
         """
         self._VpnGatewayId = None
         self._VpcId = None
         self._VpnGatewayName = None
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.947/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.946/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.947/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.946/README.rst` & `tencentcloud-sdk-python-vpc-3.0.947/README.rst`

 * *Files identical despite different names*

