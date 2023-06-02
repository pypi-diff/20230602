# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.904.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.904.tar", last modified: Thu Jun  1 02:30:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.905.tar", last modified: Fri Jun  2 00:24:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.904.tar` & `tencentcloud-sdk-python-clb-3.0.905.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89842 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)   329261 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/tencentcloud_sdk_python_clb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:30:15.000000 tencentcloud-sdk-python-clb-3.0.904/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89673 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   331659 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:24:18.000000 tencentcloud-sdk-python-clb-3.0.905/setup.cfg
```

### Comparing `tencentcloud-sdk-python-clb-3.0.904/README.rst` & `tencentcloud-sdk-python-clb-3.0.905/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/v20180317/clb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1522,15 +1522,14 @@
 
 
     def ModifyLoadBalancerSla(self, request):
         """本接口（ModifyLoadBalancerSla）用于将按量计费模式的共享型实例升级为性能容量型实例。<br/>
         限制条件：
         - 本接口只支持升级按量计费的CLB实例，包年包月的CLB实例升级请通过控制台进行升级。
         - 升级为性能容量型实例后，不支持再回退到共享型实例。
-        - 目前性能容量型实例处于内测中，如需升级为性能容量型实例，请提交 [内测申请](https://cloud.tencent.com/apply/p/hf45esx99lf)。
         - 传统型负载均衡实例不支持升级为性能容量型实例。
 
         :param request: Request instance for ModifyLoadBalancerSla.
         :type request: :class:`tencentcloud.clb.v20180317.models.ModifyLoadBalancerSlaRequest`
         :rtype: :class:`tencentcloud.clb.v20180317.models.ModifyLoadBalancerSlaResponse`
 
         """
```

### Comparing `tencentcloud-sdk-python-clb-3.0.904/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.905/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1594,30 +1594,30 @@
         :param Number: 创建负载均衡的个数，默认值 1。
         :type Number: int
         :param MasterZoneId: 仅适用于公网负载均衡。设置跨可用区容灾时的主可用区ID，例如 100001 或 ap-guangzhou-1
 注：主可用区是需要承载流量的可用区，备可用区默认不承载流量，主可用区不可用时才使用备可用区，平台将为您自动选择最佳备可用区。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213) 接口查询一个地域的主可用区的列表。
         :type MasterZoneId: str
         :param ZoneId: 仅适用于公网负载均衡。可用区ID，指定可用区以创建负载均衡实例。如：ap-guangzhou-1。
         :type ZoneId: str
-        :param InternetAccessible: 仅适用于公网负载均衡。负载均衡的网络计费模式。
+        :param InternetAccessible: 仅对内网属性的性能容量型实例和公网属性的所有实例生效。
         :type InternetAccessible: :class:`tencentcloud.clb.v20180317.models.InternetAccessible`
         :param VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 DescribeSingleIsp 接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
         :type VipIsp: str
         :param Tags: 购买负载均衡的同时，给负载均衡打上标签，最大支持20个标签键值对。
         :type Tags: list of TagInfo
         :param Vip: 指定VIP申请负载均衡。此参数选填，不填写此参数时自动分配VIP。IPv4和IPv6类型支持此参数，IPv6 NAT64类型不支持。
 注意：当指定VIP创建内网实例、或公网IPv6 BGP实例时，若VIP不属于指定VPC子网的网段内时，会创建失败；若VIP已被占用，也会创建失败。
         :type Vip: str
         :param BandwidthPackageId: 带宽包ID，指定此参数时，网络计费方式（InternetAccessible.InternetChargeType）只支持按带宽包计费（BANDWIDTH_PACKAGE）。
         :type BandwidthPackageId: str
         :param ExclusiveCluster: 独占型实例信息。若创建独占型的内网负载均衡实例，则此参数必填。
         :type ExclusiveCluster: :class:`tencentcloud.clb.v20180317.models.ExclusiveCluster`
         :param SlaType: 创建性能容量型实例。
 <ul><li>若需要创建性能容量型实例，则此参数必填，且取值为：SLA，表示创建按量计费模式下的默认规格的性能容量型实例。
-<ul><li>当您开通了普通规格的性能容量型时，SLA对应超强型1规格。普通规格的性能容量型正在内测中，请提交 [内测申请](https://cloud.tencent.com/apply/p/hf45esx99lf)。</li>
+<ul><li>默认为普通规格的性能容量型实例，SLA对应超强型1规格。
 <li>当您开通了超大型规格的性能容量型时，SLA对应超强型4规格。超大型规格的性能容量型正在内测中，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category)。</li></ul></li><li>若需要创建共享型实例，则无需填写此参数。</li></ul>
         :type SlaType: str
         :param ClientToken: 用于保证请求幂等性的字符串。该字符串由客户生成，需保证不同请求之间唯一，最大值不超过64个ASCII字符。若不指定该参数，则无法保证请求的幂等性。
         :type ClientToken: str
         :param SnatPro: 是否支持绑定跨地域/跨Vpc绑定IP的功能。
         :type SnatPro: bool
         :param SnatIps: 开启绑定跨地域/跨Vpc绑定IP的功能后，创建SnatIp。
@@ -1627,14 +1627,16 @@
         :param SlaveZoneId: 仅适用于公网负载均衡。设置跨可用区容灾时的备可用区ID，例如 100001 或 ap-guangzhou-1
 注：备可用区是主可用区故障后，需要承载流量的可用区。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213) 接口查询一个地域的主/备可用区的列表。
         :type SlaveZoneId: str
         :param EipAddressId: EIP 的唯一 ID，形如：eip-11112222，仅适用于内网负载均衡绑定EIP。
         :type EipAddressId: str
         :param LoadBalancerPassToTarget: Target是否放通来自CLB的流量。开启放通（true）：只验证CLB上的安全组；不开启放通（false）：需同时验证CLB和后端实例上的安全组。
         :type LoadBalancerPassToTarget: bool
+        :param DynamicVip: 创建域名化负载均衡。
+        :type DynamicVip: bool
         """
         self.LoadBalancerType = None
         self.Forward = None
         self.LoadBalancerName = None
         self.VpcId = None
         self.SubnetId = None
         self.ProjectId = None
@@ -1652,14 +1654,15 @@
         self.ClientToken = None
         self.SnatPro = None
         self.SnatIps = None
         self.ClusterTag = None
         self.SlaveZoneId = None
         self.EipAddressId = None
         self.LoadBalancerPassToTarget = None
+        self.DynamicVip = None
 
 
     def _deserialize(self, params):
         self.LoadBalancerType = params.get("LoadBalancerType")
         self.Forward = params.get("Forward")
         self.LoadBalancerName = params.get("LoadBalancerName")
         self.VpcId = params.get("VpcId")
@@ -1693,14 +1696,15 @@
                 obj = SnatIp()
                 obj._deserialize(item)
                 self.SnatIps.append(obj)
         self.ClusterTag = params.get("ClusterTag")
         self.SlaveZoneId = params.get("SlaveZoneId")
         self.EipAddressId = params.get("EipAddressId")
         self.LoadBalancerPassToTarget = params.get("LoadBalancerPassToTarget")
+        self.DynamicVip = params.get("DynamicVip")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4810,15 +4814,15 @@
         :param InternetChargeType: TRAFFIC_POSTPAID_BY_HOUR 按流量按小时后计费 ; BANDWIDTH_POSTPAID_BY_HOUR 按带宽按小时后计费;
 BANDWIDTH_PACKAGE 按带宽包计费;
 注意：此字段可能返回 null，表示取不到有效值。
         :type InternetChargeType: str
         :param InternetMaxBandwidthOut: 最大出带宽，单位Mbps，仅对公网属性的共享型、性能容量型和独占型 CLB 实例、以及内网属性的性能容量型 CLB 实例生效。
 - 对于公网属性的共享型和独占型 CLB 实例，最大出带宽的范围为1Mbps-2048Mbps。
 - 对于公网属性和内网属性的性能容量型 CLB实例
-  - 当您开通了普通规格的性能容量型时，最大出带宽的范围为1Mbps-10240Mbps。普通规格的性能容量型正在内测中，请提交 [内测申请](https://cloud.tencent.com/apply/p/hf45esx99lf)。
+  - 默认为普通规格的性能容量型实例，SLA对应超强型1规格，最大出带宽的范围为1Mbps-10240Mbps。
   - 当您开通了超大型规格的性能容量型时，最大出带宽的范围为1Mbps-61440Mbps。超大型规格的性能容量型正在内测中，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category)。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InternetMaxBandwidthOut: int
         :param BandwidthpkgSubType: 带宽包的类型，如SINGLEISP
 注意：此字段可能返回 null，表示取不到有效值。
         :type BandwidthpkgSubType: str
         """
@@ -7297,29 +7301,39 @@
         :param Type: 运营商内具体资源信息，如"CMCC", "CUCC", "CTCC", "BGP", "INTERNAL"。
         :type Type: list of str
         :param Isp: 运营商信息，如"CMCC", "CUCC", "CTCC", "BGP", "INTERNAL"。
         :type Isp: str
         :param AvailabilitySet: 可用资源。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AvailabilitySet: list of ResourceAvailability
+        :param TypeSet: 运营商类型信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TypeSet: list of TypeInfo
         """
         self.Type = None
         self.Isp = None
         self.AvailabilitySet = None
+        self.TypeSet = None
 
 
     def _deserialize(self, params):
         self.Type = params.get("Type")
         self.Isp = params.get("Isp")
         if params.get("AvailabilitySet") is not None:
             self.AvailabilitySet = []
             for item in params.get("AvailabilitySet"):
                 obj = ResourceAvailability()
                 obj._deserialize(item)
                 self.AvailabilitySet.append(obj)
+        if params.get("TypeSet") is not None:
+            self.TypeSet = []
+            for item in params.get("TypeSet"):
+                obj = TypeInfo()
+                obj._deserialize(item)
+                self.TypeSet.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8120,14 +8134,44 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SpecAvailability(AbstractModel):
+    """规格可用性
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SpecType: 规格类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SpecType: str
+        :param Availability: 规格可用性
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Availability: str
+        """
+        self.SpecType = None
+        self.Availability = None
+
+
+    def _deserialize(self, params):
+        self.SpecType = params.get("SpecType")
+        self.Availability = params.get("Availability")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class TagInfo(AbstractModel):
     """负载均衡的标签信息
 
     """
 
     def __init__(self):
         r"""
@@ -8462,14 +8506,49 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class TypeInfo(AbstractModel):
+    """运营商类型信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Type: 运营商类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param SpecAvailabilitySet: 规格可用性
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SpecAvailabilitySet: list of SpecAvailability
+        """
+        self.Type = None
+        self.SpecAvailabilitySet = None
+
+
+    def _deserialize(self, params):
+        self.Type = params.get("Type")
+        if params.get("SpecAvailabilitySet") is not None:
+            self.SpecAvailabilitySet = []
+            for item in params.get("SpecAvailabilitySet"):
+                obj = SpecAvailability()
+                obj._deserialize(item)
+                self.SpecAvailabilitySet.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class ZoneInfo(AbstractModel):
     """可用区相关信息
 
     """
```

### Comparing `tencentcloud-sdk-python-clb-3.0.904/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.905/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.904'
+__version__ = '3.0.905'
```

### Comparing `tencentcloud-sdk-python-clb-3.0.904/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.905/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.904/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.905/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.904
+Version: 3.0.905
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.904/setup.py` & `tencentcloud-sdk-python-clb-3.0.905/setup.py`

 * *Files identical despite different names*

