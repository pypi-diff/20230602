# Comparing `tmp/adqsetup-2.1b4.tar.gz` & `tmp/adqsetup-2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adqsetup-2.1b4.tar", last modified: Wed Oct 12 18:10:39 2022, max compression
+gzip compressed data, was "adqsetup-2.1rc1.tar", last modified: Fri Jun  2 17:37:33 2023, max compression
```

## Comparing `adqsetup-2.1b4.tar` & `adqsetup-2.1rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 petersst  (1000) petersst  (1000)        0 2022-10-12 18:10:39.400750 adqsetup-2.1b4/
--rw-r--r--   0 petersst  (1000) petersst  (1000)     1509 2022-09-28 20:27:20.000000 adqsetup-2.1b4/LICENSE
--rw-r--r--   0 petersst  (1000) petersst  (1000)       15 2022-09-28 20:27:20.000000 adqsetup-2.1b4/MANIFEST.in
--rw-r--r--   0 petersst  (1000) petersst  (1000)    10340 2022-10-12 18:10:39.400750 adqsetup-2.1b4/PKG-INFO
--rw-r--r--   0 petersst  (1000) petersst  (1000)     8175 2022-10-06 18:30:19.000000 adqsetup-2.1b4/README.md
-drwxr-xr-x   0 petersst  (1000) petersst  (1000)        0 2022-10-12 18:10:39.400750 adqsetup-2.1b4/adqsetup.egg-info/
--rw-r--r--   0 petersst  (1000) petersst  (1000)    10340 2022-10-12 18:10:39.000000 adqsetup-2.1b4/adqsetup.egg-info/PKG-INFO
--rw-r--r--   0 petersst  (1000) petersst  (1000)      244 2022-10-12 18:10:39.000000 adqsetup-2.1b4/adqsetup.egg-info/SOURCES.txt
--rw-r--r--   0 petersst  (1000) petersst  (1000)        1 2022-10-12 18:10:39.000000 adqsetup-2.1b4/adqsetup.egg-info/dependency_links.txt
--rw-r--r--   0 petersst  (1000) petersst  (1000)       45 2022-10-12 18:10:39.000000 adqsetup-2.1b4/adqsetup.egg-info/entry_points.txt
--rw-r--r--   0 petersst  (1000) petersst  (1000)        1 2022-10-07 19:34:57.000000 adqsetup-2.1b4/adqsetup.egg-info/not-zip-safe
--rw-r--r--   0 petersst  (1000) petersst  (1000)        9 2022-10-12 18:10:39.000000 adqsetup-2.1b4/adqsetup.egg-info/top_level.txt
--rw-r--r--   0 petersst  (1000) petersst  (1000)   143118 2022-10-12 18:10:38.000000 adqsetup-2.1b4/adqsetup.py
--rw-r--r--   0 petersst  (1000) petersst  (1000)       38 2022-10-12 18:10:39.400750 adqsetup-2.1b4/setup.cfg
--rw-r--r--   0 petersst  (1000) petersst  (1000)      666 2022-10-12 18:10:35.000000 adqsetup-2.1b4/setup.py
+drwxr-xr-x   0 petersst  (1000) petersst  (1000)        0 2023-06-02 17:37:33.120524 adqsetup-2.1rc1/
+-rw-r--r--   0 petersst  (1000) petersst  (1000)     1509 2022-09-28 20:27:20.000000 adqsetup-2.1rc1/LICENSE
+-rw-r--r--   0 petersst  (1000) petersst  (1000)       15 2022-09-28 20:27:20.000000 adqsetup-2.1rc1/MANIFEST.in
+-rw-r--r--   0 petersst  (1000) petersst  (1000)    10341 2023-06-02 17:37:33.120524 adqsetup-2.1rc1/PKG-INFO
+-rw-r--r--   0 petersst  (1000) petersst  (1000)     8175 2023-05-31 18:06:39.000000 adqsetup-2.1rc1/README.md
+drwxr-xr-x   0 petersst  (1000) petersst  (1000)        0 2023-06-02 17:37:33.120524 adqsetup-2.1rc1/adqsetup.egg-info/
+-rw-r--r--   0 petersst  (1000) petersst  (1000)    10341 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/PKG-INFO
+-rw-r--r--   0 petersst  (1000) petersst  (1000)      244 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/SOURCES.txt
+-rw-r--r--   0 petersst  (1000) petersst  (1000)        1 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/dependency_links.txt
+-rw-r--r--   0 petersst  (1000) petersst  (1000)       45 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/entry_points.txt
+-rw-r--r--   0 petersst  (1000) petersst  (1000)        1 2022-10-07 19:34:57.000000 adqsetup-2.1rc1/adqsetup.egg-info/not-zip-safe
+-rw-r--r--   0 petersst  (1000) petersst  (1000)        9 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/top_level.txt
+-rw-r--r--   0 petersst  (1000) petersst  (1000)   150292 2023-06-02 17:37:26.000000 adqsetup-2.1rc1/adqsetup.py
+-rw-r--r--   0 petersst  (1000) petersst  (1000)       38 2023-06-02 17:37:33.120524 adqsetup-2.1rc1/setup.cfg
+-rw-r--r--   0 petersst  (1000) petersst  (1000)      667 2023-06-02 17:33:30.000000 adqsetup-2.1rc1/setup.py
```

### Comparing `adqsetup-2.1b4/LICENSE` & `adqsetup-2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `adqsetup-2.1b4/PKG-INFO` & `adqsetup-2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adqsetup
-Version: 2.1b4
+Version: 2.1rc1
 Summary: A pure Python tool and library to setup ADQ for Intel NICs
 Home-page: https://www.intel.com/content/www/us/en/architecture-and-technology/ethernet/adq-resource-center.html
 Author: Intel
 License: BSD-3-Clause
 Description: # adqsetup
         
         _SPDX-License-Identifier: BSD-3-Clause_
```

### Comparing `adqsetup-2.1b4/README.md` & `adqsetup-2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `adqsetup-2.1b4/adqsetup.egg-info/PKG-INFO` & `adqsetup-2.1rc1/adqsetup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adqsetup
-Version: 2.1b4
+Version: 2.1rc1
 Summary: A pure Python tool and library to setup ADQ for Intel NICs
 Home-page: https://www.intel.com/content/www/us/en/architecture-and-technology/ethernet/adq-resource-center.html
 Author: Intel
 License: BSD-3-Clause
 Description: # adqsetup
         
         _SPDX-License-Identifier: BSD-3-Clause_
```

### Comparing `adqsetup-2.1b4/adqsetup.py` & `adqsetup-2.1rc1/adqsetup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # 128 byte mutable buffer
         mask = create_string_buffer(_mask(cpus, 1024))
         size = len(mask)
         if libc.sched_setaffinity(c_uint32(pid), c_size_t(size), byref(mask)):
             raise Exception(os.strerror(get_errno()))
 
 
-_VERSION_ = '2.1b4'
+_VERSION_ = '2.1rc1'
 
 ## public API
 
 __all__ = [
     'Config', 'ConfigGlobals', 'ConfigSection', 
     'check_interface'
     ]
@@ -1530,23 +1530,58 @@
     ## include/uapi/linux/rtnetlink.h
     TYPE_MODE   = 1
     TYPE_SHAPER = 2
     MODE_DCB     = 0
     MODE_CHANNEL = 1
     SHAPER_DCB     = 0
     SHAPER_BW_RATE = 1
+    TYPE_MINRATE = 3
+    TYPE_MAXRATE = 4   
 
     _struct = {
         TYPE_MODE: NLAttr._int_struct("H"),
-        TYPE_SHAPER: NLAttr._int_struct("H")
+        TYPE_SHAPER: NLAttr._int_struct("H"),
+        TYPE_MINRATE: NLAttr._int_struct("Q"),
+        TYPE_MAXRATE: NLAttr._int_struct("Q")
     }
 
     def __str__(self):
         return "TCMQAttr(type=%d, data=%r)" % (self.type, self.data)
 
+class TCMQNestAttr(NLAttr):
+    TYPE_MINRATE = 3
+    TYPE_MAXRATE = 4
+    
+    class _nest_array:
+        _item_type = 0
+        def __init__(self, item_type): # type: (str) -> None
+            self._item_type = item_type
+        @classmethod
+        def pack(cls, obj):
+            data = bytearray([]) # changed
+            for i in range(len(obj)):
+                data = data + obj[i]._bytes
+            return data
+        @classmethod
+        def unpack(cls, data, offset=0, length=0): 
+            results = []
+            item = TCMQAttr(cls._item_type, 0)
+            while offset < len(data):
+                attr =item._from(data, offset)
+                results.append(attr)
+                offset += attr.size
+            return results
+        
+    _struct = {
+        TYPE_MINRATE: _nest_array(TYPE_MINRATE),
+        TYPE_MAXRATE: _nest_array(TYPE_MAXRATE),
+    }
+
+    def __str__(self):
+        return "TCMQNestAttr(type=%d, data=%r)" % (self.type, self.data)
 
 class TCFLAttr(NLAttr):
     ## /include/uapi/linux/pkt_cls.h
     TYPE_CLASSID           = 1
     TYPE_INDEV             = 2
     TYPE_ACT               = 3
     TYPE_KEY_ETH_DST       = 4 # /* u8[6] */
@@ -1729,15 +1764,15 @@
 
     class TCmsg(StructTempl, namedtuple("TCmsg", 
             "family index handle parent info")):
         _struct = "B3xiIII"
 
     Clsact = namedtuple("Qdisc", "parent kind")
     Qdisc = namedtuple("Qdisc", 
-        "parent kind num_tc map hw count offset mode shaper")
+        "parent kind num_tc map hw count offset mode shaper min_rate max_rate")
     Filter = namedtuple("Filter", 
         "prio proto src_mac src_addr src_port"
         " dst_mac dst_addr dst_port queue tc action priority")
 
     def __init__(self, ifname, log=None): # type: (str, any) -> None
         self.ifname = ifname
         self.ifindex = if_nametoindex(ifname)
@@ -1775,27 +1810,30 @@
                             pmap = unpack_from("16B", attr.data, 1)
                             hw = unpack_from("B", attr.data, 17)[0]
                             count = unpack_from("16H", attr.data, 18)
                             offset = unpack_from("16H", attr.data, 50)
                             attrs = TCMQAttr.dict(attr.data, 84)
                             mode = attrs.get(TCMQAttr.TYPE_MODE, None)
                             shaper = attrs.get(TCMQAttr.TYPE_SHAPER, None)
+                            attrs_nest = TCMQNestAttr.dict(attr.data, 100)
+                            min_rate = attrs_nest.get(TCMQNestAttr.TYPE_MINRATE, None)
+                            max_rate = attrs_nest.get(TCMQNestAttr.TYPE_MAXRATE, None)
                             results.append(self.Qdisc(
                                 msg.parent, kind, num_tc, pmap, hw, 
-                                count, offset, mode, shaper
+                                count, offset, mode, shaper, min_rate, max_rate
                             ))
                             break
                         elif kind == 'clsact':
                             results.append(self.Clsact(msg.parent, kind))
                             break
             return results
 
     def qdisc_add(self, parent=None, kind=None, 
-            pmap=None, count=None, offset=None):
-        # type: (int, str, list[int], list[int], list[int]) -> None
+            pmap=None, count=None, offset=None, min_rate=None, max_rate=None):
+        # type: (int, str, list[int], list[int], list[int], list[int], list[int]) -> None
         with RNLConn() as conn:
             handle = 0
             if parent == self.TC_H_CLSACT:
                 handle = self._tc_h_make(parent, 0)
             msg = NLMessage(
                 type=NLMessage.RTM_NEWQDISC,
                 flags=NLMessage.FLAG_REQUEST | NLMessage.FLAG_ACK | 
@@ -1806,23 +1844,49 @@
             msg.data = msg.data + TCAttr(TCAttr.TYPE_KIND, kind)._bytes
             if kind == 'mqprio':
                 # normalize maps and limit to 16 TCs
                 max_tc = self.TC_QOPT_MAX_QUEUE
                 pmap = pmap[:max_tc]
                 count = count[:len(pmap)]
                 offset = offset[:len(pmap)]
-                # nested attrs
-                msg.data = msg.data + TCAttr(
-                    TCAttr.TYPE_OPTIONS, 
-                    pack("B", len(pmap)) + _pack_list(pmap, 'B', max_tc) 
-                    + pack("B", 1) + _pack_list(count, 'H', max_tc) 
-                    + _pack_list(offset, 'H', max_tc)
-                    + b'\x00' * 2 # DWORD alignment padding
-                    + TCMQAttr(TCMQAttr.TYPE_MODE, TCMQAttr.MODE_CHANNEL)._bytes
-                )._bytes
+                if min_rate is not None or max_rate is not None:
+                    minrate = array('Q', [0] * 16)
+                    for i in range(len(min_rate)):
+                        pnum = pack("Q", min_rate[i] if min_rate[i] is not None else 0)
+                        num = unpack("Q", pnum)[0] * 125000
+                        minrate[i] = num
+                    maxrate = array('Q', [0] * 16)
+                    for i in range(len(max_rate)):
+                        pnum = pack("Q", max_rate[i] if max_rate[i] is not None else 0)
+                        num = unpack("Q", pnum)[0] * 125000
+                        maxrate[i] = num
+                    # nested attrs
+                    min_rates = [TCMQAttr(TCMQAttr.TYPE_MINRATE, minrate[i]) for i in range(16)]
+                    max_rates = [TCMQAttr(TCMQAttr.TYPE_MAXRATE, maxrate[i]) for i in range(16)]
+                    msg.data = msg.data + TCAttr(
+                        TCAttr.TYPE_OPTIONS, 
+                        pack("B", len(pmap)) + _pack_list(pmap, 'B', max_tc) 
+                        + pack("B", 1) + _pack_list(count, 'H', max_tc) 
+                        + _pack_list(offset, 'H', max_tc)
+                        + b'\x00' * 2 # DWORD alignment padding
+                        + TCMQAttr(TCMQAttr.TYPE_MODE, TCMQAttr.MODE_CHANNEL)._bytes
+                        + TCMQAttr(TCMQAttr.TYPE_SHAPER, TCMQAttr.SHAPER_BW_RATE)._bytes
+                        + TCMQNestAttr(TCMQNestAttr.TYPE_MINRATE, min_rates)._bytes
+                        + TCMQNestAttr(TCMQNestAttr.TYPE_MAXRATE, max_rates)._bytes
+                    )._bytes
+                else:
+                    # nested attrs
+                    msg.data = msg.data + TCAttr(
+                        TCAttr.TYPE_OPTIONS, 
+                        pack("B", len(pmap)) + _pack_list(pmap, 'B', max_tc) 
+                        + pack("B", 1) + _pack_list(count, 'H', max_tc) 
+                        + _pack_list(offset, 'H', max_tc)
+                        + b'\x00' * 2 # DWORD alignment padding
+                        + TCMQAttr(TCMQAttr.TYPE_MODE, TCMQAttr.MODE_CHANNEL)._bytes
+                    )._bytes
             conn.send(msg)
             if self.log:
                 if parent == self.TC_H_ROOT and kind == "mqprio":
                     self._log(
                         "tc qdisc add dev %s root mqprio" \
                         " num_tc %d map %s queues %s hw 1 mode channel" %
                         (self.ifname, len(pmap), 
@@ -2473,24 +2537,49 @@
         if self.bp_stop is not None:
             flags[self._channel_pkt + '-clean-bp-stop'] = self.bp_stop
         if self.bp_stop_cfg is not None:
             flags[self._channel_pkt + '-clean-bp-stop-cfg'] = self.bp_stop_cfg
         self.ethtool.flags(flags)        
 
 ## config classes
+class Filters(object):
+    # direction: str = 'ingress', prio: int = 1, proto: str = 'tcp', src_mac: str = None, src_addr: str = None, src_port: int = None, 
+    # dst_mac: str = None, dst_addr: str = None, dst_port: int = None, queue: int = None, tc: int = None, action: str = None, priority: int = None
+    Filter = namedtuple("Filter", 
+    "protocol mac addr port remote_addr remote_port tc queue")
+    _filters = []
+    def add(self, protocol, mac, addr, port, remote_addr, remote_port, tc, queue):
+        # type: (str, str, str, int, str, int, int, int) -> None
+        filter = self.Filter(protocol, mac, addr, port, remote_addr, remote_port, tc, queue)
+        for f in self._filters:
+            score = 0
+            for i in range(len(filter) - 2):
+                if f[i] == filter[i] or f[i] is None or filter[i] is None:
+                    score += 1
+            if score == len(filter):
+                raise Exception("conflicting mac, addr, port, remote_addr, or remote_port")
+        self._filters.append(filter)
+    def create(self, dev, skbedit=False, log=None):
+        # type: (str, bool, any) -> dict[str, list[TCtool.Filter]]
+        tc = TCtool(dev, log)
+        for f in self._filters:
+            tc.filter_add('ingress', f.tc, f.protocol, src_addr=f.addr, )
+            if skbedit:
+                tc.filter_add()
+        return tc.filter_list()
 
 class ConfigBase(object):
     
     # a dictionary of callables that defines
     # the schema of the config section
     _schema = {}
 
     ## custom schema formats
     @staticmethod
-    def _bool(s):
+    def _bool(s): # type (Any) -> bool
         '''
         Parse a <bool> on/off flag 
         '''
         try:
             s = str(s).lower()
             if s in ['on', 'true', 'yes', '1']:
                 return True
@@ -2498,15 +2587,22 @@
                 return False
             else:
                 raise Exception()
         except:
             raise Exception("%r is not a valid boolean" % s)
 
     @staticmethod
-    def _int_list(s): # type (str) -> list
+    def _str_lower(s): # type (Any) -> str
+        ''' 
+        Parse a case insensitive value 
+        '''
+        return str(s).lower()
+
+    @staticmethod
+    def _int_list(s): # type (Any) -> list
         '''
         Parse a comma-seperated list of integers with ranges
         '''
         l = []
         for v in str(s).split(','):
             v = v.strip()
             if '-' in v:
@@ -2516,15 +2612,15 @@
                     l.append(i)
             else:
                 l.append(int(v))
         # remove duplicates and sort 
         return sorted(set(l))
 
     @staticmethod
-    def _str_list(s): # type (str) -> list
+    def _str_list(s): # type (Any) -> list
         ''' 
         Parse a comma-seperated list of strings 
         '''
         l = []
         for v in str(s).split(','):
             l.append(v.strip())
         # remove duplicates and sort 
@@ -2557,19 +2653,19 @@
         try:
             for key, value in conf.items():
                 # normalize key
                 # key = key.strip().lower().replace('-', '').replace('_', '')
                 key = key.strip().lower().replace('-', '_')
                 if isinstance(value, str):
                     # normalize value
-                    value = value.strip().lower()
-                    if value == 'auto' or value == '':
+                    value = value.strip()
+                    if value.lower() == 'auto' or value == '':
                         value = None
                 if isinstance(value, list):
-                    value = ','.join([str(v) for v in value])
+                    value = ','.join([str(v).strip() for v in value])
                 if key in self._schema:
                     if value is not None and callable(self._schema[key]):
                         # use schema callable to convert value
                         value = self._schema[key](value)
                     # assign to class attribute
                     setattr(self, key, value)
         except Exception as e:    
@@ -2584,31 +2680,34 @@
 
 
 class ConfigGlobals(ConfigBase):
 
     # a dictionary of callables that defines
     # the schema of the config dict/file
     _schema = {
-        'arpfilter': ConfigBase._bool,
+        'arpfilter': ConfigBase._bool, 
         'bpstop': ConfigBase._bool,
         'bpstop_cfg': ConfigBase._bool,
         'busypoll': int,
         'busyread': int,
         'cpus': ConfigBase._int_list,
-        'dev': str,
-        'numa': str,
-        'optimize': ConfigBase._bool,
-        'priority': str,
+        'dev': str, 
+        'queues': int, 
+        'min_rate': int,
+        'max_rate': int,
+        'numa': ConfigBase._str_lower,
+        'optimize': ConfigBase._bool, 
+        'priority': ConfigBase._str_lower,
         'queues': int,
         'rxadapt': ConfigBase._bool,
         'rxring': int,
         'rxusecs': int,
         'txadapt': ConfigBase._bool,
         'txring': int,
-        'txusecs': int
+        'txusecs': int,
     }
 
     def __init__(self, source=None): # type: (dict) -> None
         '''
         Create a new ConfigGlobals instance 
         optionally from a dictionary
         '''
@@ -2617,14 +2716,16 @@
         self.arpfilter = False
         self.bpstop = None
         self.bpstop_cfg = None
         self.busypoll = None
         self.busyread = None
         self.cpus = None
         self.dev = None
+        self.min_rate = None
+        self.max_rate = None
         self.numa = None
         self.optimize = None
         self.priority = None
         self.queues = None
         self.rxadapt = None
         self.rxring = None
         self.rxusecs = None
@@ -2671,23 +2772,25 @@
 
     # a dictionary of callables that defines
     # the schema of the config dict/file
     _schema = {
         'addrs': ConfigBase._str_list,
         'cpus': ConfigBase._int_list,
         'mac': str,
-        'mode': str,
-        'numa': str,
+        'min_rate': int,
+        'max_rate': int,
+        'mode': ConfigBase._str_lower,
+        'numa': ConfigBase._str_lower,
         'pollers': int,
         'poller_timeout': int,
-        'ports': ConfigBase._int_list,
-        'protocol': str,
+        'ports': ConfigBase._int_list, 
+        'protocol': ConfigBase._str_lower,
         'queues': int,
+        'remote_ports': ConfigBase._int_list, 
         'remote_addrs': ConfigBase._str_list,
-        'remote_ports': ConfigBase._int_list
     }
 
     @property
     def _isfiltered(self): # type: () -> bool
         return any([self.mac, self.addrs, self.ports, self.remote_addrs, self.remote_ports])
 
     def __init__(self, name=None, source=None): # type (str, dict) -> None
@@ -2696,23 +2799,26 @@
         optionally from a dictionary
         '''
         super(ConfigSection, self).__init__(name)
         # attributes
         self.addrs = None
         self.cpus = None
         self.mac = None
+        self.min_rate = None
+        self.max_rate = None
         self.mode = None
         self.numa = None
         self.pollers = 0
         self.poller_timeout = 10000
         self.ports = None
         self.protocol = None
         self.queues = None
         self.remote_addrs = None
         self.remote_ports = None
+        self._filters = []
         # initialize section with source
         if source is not None:
             if not isinstance(source, dict):
                 raise Exception("source must be a dictionary")
             self._parse(source)
 
     def __str__(self): # type () -> str
@@ -2805,24 +2911,24 @@
                 tc.filter_add(
                     'ingress', tcid, protocol, src_addr=addr, 
                     src_port=port, tc=tcid
                 )
                 if skbedit:
                     tc.filter_add(
                         'egress', tcid, protocol, dst_addr=addr, 
-                        dst_port=port, action='skbedit', priority=1
+                        dst_port=port, action='skbedit', priority=tcid
                     )
         elif addr:
             tc.filter_add(
                 'ingress', tcid, protocol, src_addr=addr, tc=tcid
             )
             if skbedit:
                 tc.filter_add(
                     'egress', tcid, protocol, dst_addr=addr, 
-                    action='skbedit', priority=1
+                    action='skbedit', priority=tcid
                 )
 
     @staticmethod
     def _set_queue_filters(tc, tcid, queue, protocol, addrs=None, port=None, mac=None, skbedit=False): 
         # type: (TCtool, int, int, str, str, int, str, bool) -> None
         if addrs:
             for addr in addrs:             
@@ -2844,14 +2950,45 @@
             )
             if skbedit:
                 tc.filter_add(
                     'egress', tcid, protocol, src_mac=mac, 
                     src_port=port, action='skbedit', priority=tcid
                 )
 
+    # def _create_filters(self):
+    #     filters = Filters()
+    #     if self.addrs:
+    #         for addr in self.addrs:
+    #             if addr and '/' not in addr:
+    #                 addr = addr + '/32'
+    #             for port in self.ports:
+    #                 filters.add(
+    #                     Filter(self.protocol, self.mac, addr, port, None, None)
+    #                 )
+    #     elif self.ports:
+    #         for port in self.ports:
+    #             filters.add(
+    #                 Filter(self.protocol, self.mac, None, port, None, None)
+    #             )
+    #     elif self.mac:
+    #         filters.add(Filter(self.protocol, self.mac, None, None, None, None))
+    #     if self.remote_addrs:
+    #         for addr in self.remote_addrs:
+    #             if addr and '/' not in addr:
+    #                 addr = addr + '/32'
+    #             for port in self.remote_ports:
+    #                 filters.add(
+    #                     Filter(self.protocol, None, None, None, addr, port)
+    #                 )
+    #     elif self.remote_ports:
+    #         for port in self.remote_ports:
+    #             filters.add(
+    #                 Filter(self.protocol, None, None, None, None, port)
+    #             )
+
     def _set_filters(self, dev, skbedit=False, log=None): 
         # type: (str, bool, any) -> None
         # create ingress & egress filters
         if not self._isfiltered:
             return
         def _tc_filters(self, dev, skbedit, log):
             tc = TCtool(dev, log)
@@ -2940,15 +3077,18 @@
     def _load(self, fp): # type: (any) -> None
         '''
         Loads then parses a config from a file-like object
         '''
         try:
             # load filepath as config file
             conf = SafeConfigParser()
-            conf.readfp(fp)
+            if sys.version[:1] == '3':
+                conf.read_file(fp)
+            else:
+                conf.readfp(fp)
         except:
             # raise Exception("unable to load %r" % filepath)
             raise
         # convert ConfigParser object to a dict
         config = OrderedDict()
         print(conf.sections())
         for key in conf.sections():
@@ -3000,27 +3140,27 @@
             if value is not None:
                 if isinstance(value, list) or isinstance(value, set):
                     if len(value):
                         value = ','.join([str(v) for v in value])
                     else:
                         value = None
                 if value is not None:
-                    conf.set('globals', key, str(value).lower())
+                    conf.set('globals', key, str(value))
         del(config['globals'])
         for name, section in config.items():
             conf.add_section(name)
             for key, value in section.items():
                 if value is not None:
                     if isinstance(value, list) or isinstance(value, set):
                         if len(value):
                             value = ','.join([str(v) for v in value])
                         else:
                             value = None
                 if value is not None:
-                    conf.set(name, key, str(value).lower())
+                    conf.set(name, key, str(value))
         buf = StringIO()
         conf.write(buf)
         return buf.getvalue().strip()
 
     @staticmethod
     def _cpu_mask(cpu): # type(int) -> str
         '''
@@ -3062,14 +3202,22 @@
         for sec in self._sections.values():
             # TODO: check for proper power-of-two queue counts for each TC
             requested += sec.queues
         # if requested > self._queues:
         if requested > 256:
             raise Exception("Not enough queues available")
         
+    def _check_min_rate(self): # type() -> None
+        requested = self.globals.min_rate if self.globals.min_rate is not None else 0
+        for sec in self._sections.values():
+            requested += sec.min_rate if sec.min_rate is not None else 0
+        speed = _readfile("/sys/class/net/%s/speed" % self.globals.dev)
+        if requested > int(speed):
+            raise Exception("Total min_rate exceeds device speed")
+
     def _cleanup(self): # type: () -> None
         '''
         Attempt to cleanup setup from previous run
         '''
         self._printhead("cleanup")
         # turn off napi threads if available
         if os.path.exists("/sys/class/net/%s/threaded" % self.globals.dev):
@@ -3222,17 +3370,22 @@
 
     def _set_tcs(self): # type: () -> None
         self._printhead("setting traffic classes")
         self._log("## qdisc and tc setup ##")
         tc = TCtool(self.globals.dev, self.log)
         # create root mqprio qdisc
         count = [section.queues for _, section in self]
+        min_rate = [section.min_rate for _, section in self]
+        max_rate = [section.max_rate for _, section in self]
         pmap = [i for i in range(len(count))]
         offset = [sum(count[:i]) for i in range(len(count))]
-        tc.qdisc_add(tc.TC_H_ROOT, 'mqprio', pmap, count, offset)
+        tc.qdisc_add(tc.TC_H_ROOT, 'mqprio', pmap, count, offset,
+            min_rate if any(x is not None for x in min_rate) else None,
+            max_rate if any(x is not None for x in max_rate) else None
+            )
         if self._isfiltered \
                 and not any([t.kind == 'clsact' for t in tc.qdisc_list()]):
             # create classifier (ingress+egress) qdisc if needed
             tc.qdisc_add(tc.TC_H_CLSACT, 'clsact')
         # display results
         for t in tc.qdisc_list():
             if t.kind == "mqprio":
@@ -3383,23 +3536,25 @@
                 raise Exception("Shared mode is not currently supported on VF netdevs")
         if any([s.pollers for s in self._sections.values()]):
             self.globals.busypoll = 0
             self.globals.busyread = 0
             _printhead("when using pollers, " \
                 "busypoll and/or busyread cannot be enabled - " \
                 "setting both to zero", 93)
+        # check for conflicting filters
         self._assign_auto_cpus(self.inventory)
 
     def apply(self): # type: () -> None
         '''
         Applies the current config to the target system
         '''
         self._log("### cleanup ###")
         self._cleanup()
         self._check_queues()
+        self._check_min_rate()
         self.settings = Settings(self.globals.dev, self.log)
         self._set_sysctls()
         self._set_interface_flags()
         self._printhead("modifying system and network settings")
         self._log("", "### configuration ###")
         self._print(self.settings)
         self.settings.apply()
```

### Comparing `adqsetup-2.1b4/setup.py` & `adqsetup-2.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='adqsetup',
-    version='2.1b4',
+    version='2.1rc1',
     description='A pure Python tool and library to setup ADQ for Intel NICs',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',    
     url='https://www.intel.com/content/www/us/en/architecture-and-technology/ethernet/adq-resource-center.html',
     author='Intel',
     license='BSD-3-Clause',
     py_modules=['adqsetup'],
```

