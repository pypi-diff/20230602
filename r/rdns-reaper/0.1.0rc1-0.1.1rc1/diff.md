# Comparing `tmp/rdns_reaper-0.1.0rc1.tar.gz` & `tmp/rdns_reaper-0.1.1rc1.tar.gz`

## Comparing `rdns_reaper-0.1.0rc1.tar` & `rdns_reaper-0.1.1rc1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 rdns_reaper-0.1.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rdns_reaper-0.1.0rc1/rdns_reaper/__init__.py
--rw-r--r--   0        0        0    18798 2020-02-02 00:00:00.000000 rdns_reaper-0.1.0rc1/rdns_reaper/rdns_reaper.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 rdns_reaper-0.1.0rc1/.gitignore
--rw-r--r--   0        0        0    35949 2020-02-02 00:00:00.000000 rdns_reaper-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 rdns_reaper-0.1.0rc1/README.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 rdns_reaper-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 rdns_reaper-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/SECURITY.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/rdns_reaper/__init__.py
+-rw-r--r--   0        0        0    18919 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/rdns_reaper/rdns_reaper.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/.gitignore
+-rw-r--r--   0        0        0    35270 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/LICENSE
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/README.md
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/PKG-INFO
```

### Comparing `rdns_reaper-0.1.0rc1/rdns_reaper/rdns_reaper.py` & `rdns_reaper-0.1.1rc1/rdns_reaper/rdns_reaper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,516 +1,532 @@
-import concurrent.futures
-import copy
-import socket
-
-import yaml
-from netaddr import AddrFormatError, IPAddress, IPSet
-
-IPV4_RESERVED_NETWORK_LIST = [
-    "0.0.0.0/8",
-    "100.64.0.0/10",
-    "127.0.0.0/8",
-    "169.254.0.0/16",
-    "192.0.0.0/24",
-    "192.0.2.0/24",
-    "192.88.99.0/24",
-    "198.51.100.0/24",
-    "203.0.113.0/24",
-    "224.0.0.0/4",
-    "233.252.0.0/24",
-    "240.0.0.0/4",
-    "255.255.255.255/32",
-]
-
-IPV4_RFC1918_NETWORK_LIST = [
-    "10.0.0.0/8",
-    "172.16.0.0/12",
-    "192.168.0.0/16",
-]
-
-IPV6_RESERVED_NETWORK_LIST = [
-    "::ffff:0:0/96",
-    "::ffff:0:0:0/96",
-    "64:ff9b::/96",
-    "64:ff9b:1::/48",
-    "100::/64",
-    "2001:0000::/32",
-    "2001:20::/28",
-    "2001:db8::/32",
-    "2002::/16",
-    "fc00::/7",
-    "fe80::/10",
-    "ff00::/8",
-]
-
-
-class RdnsReaper:
-    """Reverse DNS Lookup Engine."""
-
-    def __init__(self, **kwargs):
-        """Initialize class and take in user options.
-
-        Keyword Arguments:
-            allow_reserved_networks (bool, optional): if True disable automatic filtering of
-                reserved networks, must be set to True if checking of any reserved networks
-                is desired.  Can then be supplemented with a custom filter
-            concurrent (int, default = 5): number of concurrent resolver threads
-            limit_to_rfc1918 (bool, optional): limit resolve to IPv4 RFC1918 only
-            filter (str, list of strs, IPSet, optional): filter data
-                can be a string containing an IP Address, list of strings, or an IPSet object
-            filtermode ("block" | "allow", optional): sets filter mode to block list or allow list
-                defaults to block list if not specified
-            filename (str, optional): path and filename for disk based cache in YAML format
-            filemode ("r" | "w"), required if filename set): read only or read-write mode for
-                disk cache, if set to write, resolver may try to update the cache periodically
-                the savefile() function can be called without arguments to force an update
-            unresolvable (str, optional): string to set for each entry if resolving fails
-                None is the default, all other options prevent subsequent lookups if disk based
-                cache is in use
-
-
-        """
-        self._resolver_ip = None
-        self._dns_dict = {}
-        self._concurrent = 5
-        self._options_dict = {
-            "allow_reserved_networks": False,
-            "concurrent": 5,
-            "filemode": None,
-            "filename": None,
-            "filter": None,
-            "filter_mode": None,
-            "limit_to_rfc1918": False,
-        }
-        # Check for RFC1918 filtering
-        if "limit_to_rfc1918" in kwargs:
-            self.limit_to_rfc1918(kwargs["limit_to_rfc1918"])
-        else:
-            self._options_dict["limit_to_rfc1918"] = False
-
-        # Check for custom filtering
-        if kwargs.get("filter") is not None:
-            self.set_filter(kwargs.get("filter"), mode=kwargs.get("filtermode"))
-
-        # Allow reserved network check
-        if kwargs.get("allow_reserved_networks"):
-            self._options_dict["allow_reserved_networks"] = True
-        else:
-            self._options_dict["allow_reserved_networks"] = False
-
-        # Process parallel lookup concurrency
-        if kwargs.get("concurrent"):
-            if isinstance(kwargs["concurrent"], int):
-                self._options_dict["concurrent"] = kwargs["concurrent"]
-            else:
-                raise TypeError
-
-        # Determine how to mark unresolvable entries
-        try:
-            if isinstance(kwargs["unresolvable"], str):
-                self._unresolvable = kwargs["unresolvable"]
-            else:
-                raise TypeError
-        except KeyError:
-            self._unresolvable = None
-
-        try:
-            if isinstance(kwargs["filemode"], str):
-                if kwargs["filemode"] not in ("w", "r"):
-                    raise ValueError
-
-                self._options_dict["filemode"] = kwargs["filemode"]
-            else:
-                raise TypeError
-        except KeyError:
-            pass
-
-        try:
-            if isinstance(kwargs["filename"], str):
-                self._options_dict["filename"] = kwargs["filename"]
-            else:
-                raise TypeError
-        except KeyError:
-            pass
-
-        if (self._options_dict["filename"] is not None) and (
-            self._options_dict["filemode"] in ("r", "w")
-        ):
-            try:
-                self.loadfile(self._options_dict["filename"])
-            except FileNotFoundError:
-                pass
-
-    def __add__(self, new):
-        """Add two instances together and return a deepcopy."""
-        self_copy = copy.deepcopy(self)
-        if isinstance(new, RdnsReaper):
-            self_copy._dns_dict.update(new._dns_dict)
-        elif isinstance(new, str):
-            self_copy.add_ip(new)
-        elif isinstance(new, set):
-            self_copy.add_ip_list(new)
-        elif isinstance(new, list):
-            self_copy.add_ip_list(new)
-        else:
-            raise TypeError
-        return self_copy
-
-    def __contains__(self, ip_address):
-        """Allow for checking of IP in the instance."""
-        if ip_address in self._dns_dict.keys():
-            return True
-        return False
-
-    def __delitem__(self, ip_address):
-        """Remove an item if del() is called."""
-        self.remove_ip(ip_address)
-
-    def __enter__(self):
-        """Return self for use in 'with open()' style blocks."""
-        return self
-
-    def __exit__(self, exception_type, exception_value, traceback):
-        """Save file when class is being destroyed as appropriate."""
-        if (self._options_dict["filename"] is not None) and (self._options_dict["filemode"] == "w"):
-            self.savefile(self._options_dict["filename"])
-
-    def __getitem__(self, ip_address):
-        """Return IP address from internal dictionary, false if not found."""
-        try:
-            IPAddress(ip_address)
-            return self._dns_dict[ip_address]
-        except AddrFormatError as error_case:
-            raise AddrFormatError from error_case
-        except KeyError:
-            return False
-
-    def __iadd__(self, new):
-        """Add two instances together and return."""
-        if isinstance(new, RdnsReaper):
-            self._dns_dict.update(new._dns_dict)
-        elif isinstance(new, str):
-            self.add_ip(new)
-        elif isinstance(new, set):
-            self.add_ip_list(new)
-        elif isinstance(new, list):
-            self.add_ip_list(new)
-        else:
-            raise TypeError
-        return self
-
-    def __iter__(self):
-        """Return an iterator as needed for k, v walking."""
-        return self._ReaperIterator(self)
-
-    def __len__(self):
-        """Determine number of addresses in module."""
-        return len(self._dns_dict)
-
-    def __setitem__(self, ip_address, value):
-        """Allow set/reset of hostname for an IP via index."""
-        self.set_name(ip_address, value)
-
-    def _resolve_function(self, ip_address):
-        try:
-            name = socket.gethostbyaddr(ip_address)[0]
-            self._dns_dict[ip_address] = name
-        except socket.herror:
-            self._dns_dict[ip_address] = self._unresolvable
-
-    def add(self, *args, **kwargs):
-        """Generalized function for adding."""
-        self.__iadd__(*args, **kwargs)
-
-    def add_ip(self, ip_address: str, hostname: str = None) -> bool | str:
-        """Add an IP to the list with option hostname, skip if exists."""
-        if ip_address in self._dns_dict.keys():
-            return True
-
-        try:
-            IPAddress(ip_address)
-            if hostname is None:
-                self._dns_dict.update({ip_address: None})
-            else:
-                self._dns_dict.update({ip_address: hostname})
-            return ip_address
-        except AddrFormatError as error_case:
-            raise TypeError from error_case
-
-    def add_ip_list(self, ip_list: list):
-        """Add all new IP's from a list."""
-        if isinstance(ip_list, set):
-            ip_list = list(ip_list)
-        if not isinstance(ip_list, list):
-            raise TypeError
-        for ip_address in ip_list:
-            self.add_ip(ip_address)
-
-    def allow_reserved_networks(self, option: bool):
-        """Allow users to enable/disable automatic filtering of reserved networks.
-
-        If a user wants to check reserved network IPs (loopbacks, link local, multicast, etc.)
-        they must set this option to True.  Users may manually filter some of the reserved
-        networks with the filter() option.  This option *must* be set to True to resolve any
-        reserved networks.  Using an allow filter with this option set to False will not resolve
-        any reserved networks.
-
-        Args:
-            option (bool): Set to True to disable automatic filtering of reserved networks
-
-        """
-        if not isinstance(option, bool):
-            raise TypeError
-
-        self._options_dict["allow_reserved_networks"] = option
-
-    def clear_all_hostnames(self):
-        """Clear all the hostnames from existing entries."""
-        new_ip_dict = {ip: None for ip in self._dns_dict}
-        self._dns_dict = new_ip_dict
-
-    def clearname(self, ip_address: str):
-        """Clear a specific IP's hostname.
-
-        Args:
-            ip_address (str): A string containing an IP address
-        """
-        try:
-            IPAddress(ip_address)
-        except AddrFormatError as error_case:
-            raise TypeError from error_case
-
-        if ip_address not in self._dns_dict.keys():
-            raise KeyError("Address not found")
-
-        self._dns_dict[ip_address] = None
-
-    def dict(self) -> dict:
-        """Return the internal dictionary to the calling function."""
-        return self._dns_dict
-
-    def get_dict(self) -> dict:
-        """Return the internal dictionary to the calling function."""
-        return self._dns_dict
-
-    def get_filter(self) -> tuple:
-        """Return current filter status."""
-        return (self._options_dict["filter"], self._options_dict["filter_mode"])
-
-    def get_options(self) -> dict:
-        """Return info about the various options set by the user."""
-        return self._options_dict
-
-    def items(self) -> dict:
-        """Return the IP address and hostnames as k, v pairs in list format."""
-        return dict(self._dns_dict.items())
-
-    def keys(self) -> list:
-        """Return the IP address as keys in list format."""
-        return list(self._dns_dict.keys())
-
-    def limit_to_rfc1918(self, value: bool):
-        """Set the RFC1918 filter."""
-        if not isinstance(value, bool):
-            raise TypeError
-        self._options_dict["limit_to_rfc1918"] = value
-
-    def loadfile(self, filename: str):
-        """Load saved data in YAML format.
-
-        Args
-            filename (str): path and filename for the disk based YAML cache file
-        """
-        with open(filename, encoding="UTF-8") as f_handle:
-            f_data = f_handle.read()
-            self._dns_dict = yaml.safe_load(f_data)
-
-    def remove_ip(self, ip_address: str) -> bool:
-        """Remove an IP from the list, return false if not found.
-
-        Args:
-            ip_address (str): A string containing an IP Address to remove
-        """
-        try:
-            IPAddress(ip_address)
-            self._dns_dict.pop(ip_address)
-        except AddrFormatError as error_case:
-            raise TypeError from error_case
-        except KeyError:
-            return False
-        return True
-
-    def _build_resolve_list(self):
-        """Build list of IP's to perform resolver on, shared by serial and parallel methods."""
-        if self._options_dict["limit_to_rfc1918"]:
-            ipv4_skipped_networks = IPSet(IPV4_RESERVED_NETWORK_LIST)
-        elif self._options_dict["allow_reserved_networks"] is False:
-            ipv4_skipped_networks = IPSet(IPV4_RESERVED_NETWORK_LIST)
-        else:
-            ipv4_skipped_networks = IPSet()
-
-        if self._options_dict["allow_reserved_networks"] is False:
-            ipv6_skipped_networks = IPSet(IPV6_RESERVED_NETWORK_LIST)
-        else:
-            ipv6_skipped_networks = IPSet()
-
-        initial_ip_list = [key for key, value in self._dns_dict.items() if value is None]
-
-        pending_ipset = IPSet(initial_ip_list)
-
-        if self._options_dict["filter_mode"] == "block":
-            result_ipset = pending_ipset - self._options_dict["filter"]
-            initial_pending_ips = [str(x) for x in result_ipset]
-        elif self._options_dict["filter_mode"] == "allow":
-            result_ipset = pending_ipset & self._options_dict["filter"]
-            initial_pending_ips = [str(x) for x in result_ipset]
-        else:
-            initial_pending_ips = [str(x) for x in pending_ipset]
-
-        pending_ips = []
-
-        for key in initial_pending_ips:
-            address = IPAddress(key)
-
-            if self._options_dict["limit_to_rfc1918"] is False:
-                if (address.version == 4) and (address not in ipv4_skipped_networks):
-                    pending_ips.append(key)
-                elif (address.version == 6) and (address not in ipv6_skipped_networks):
-                    pending_ips.append(key)
-            else:
-                if address in IPSet(IPV4_RFC1918_NETWORK_LIST):
-                    pending_ips.append(key)
-
-        return pending_ips
-
-    def resolve_all(self):
-        """Resolve all unknown IPs in parallel."""
-        pending_ips = self._build_resolve_list()
-        with concurrent.futures.ThreadPoolExecutor(
-            max_workers=self._options_dict["concurrent"]
-        ) as executor:
-            executor.map(self._resolve_function, set(pending_ips))
-
-    def resolve_all_serial(self):
-        """Resolve all unknown IPs serially."""
-        pending_ips = self._build_resolve_list()
-
-        for address in pending_ips:
-            self._resolve_function(address)
-
-    def savefile(self, filename: str = None):
-        """Save internal dictionary to YAML file."""
-        if (
-            filename is None
-            and self._options_dict["filename"] is not None
-            and self._options_dict["filemode"] == "w"
-        ):
-            filename = self._options_dict["filename"]
-
-        with open(filename, "w", encoding="UTF-8") as f_handle:
-            f_handle.write("---\n")
-            f_handle.write(yaml.dump(self._dns_dict))
-
-    def set_name(self, ip_address: str, hostname: str):
-        """Force the hostname of an IP.
-
-        Args:
-            ip_address (str): String containing an IP address to be modified
-            hostname (str): Desired FQDN hostname to be set for this entry
-                Can be None to reset record to allow for subsequent lookup
-        """
-        try:
-            IPAddress(ip_address)
-        except AddrFormatError as error_case:
-            raise TypeError(f"IP Error: {error_case}") from error_case
-
-        if ip_address not in self._dns_dict.keys():
-            raise KeyError("Address does not exist")
-        self._dns_dict[ip_address] = hostname
-        # except KeyError as error_case:
-        # raise KeyError("Address does not exist")
-
-    def set_filter(self, filter_data: str, **kwargs):
-        """Define a custom filter."""
-        if kwargs.get("mode") is None:
-            self._options_dict["filter_mode"] = "block"
-        elif kwargs.get("mode").lower() in ("allow", "block"):
-            self._options_dict["filter_mode"] = kwargs.get("mode").lower()
-        else:
-            raise ValueError
-
-        if isinstance(filter_data, str):
-            filter_data = IPSet([filter_data])
-        elif isinstance(filter_data, list):
-            filter_data = IPSet(filter_data)
-
-        if not isinstance(filter_data, IPSet):
-            raise TypeError
-
-        self._options_dict["filter"] = filter_data
-
-    def values(self) -> list:
-        """Return the hostnames as values in list format."""
-        return list(self._dns_dict.values())
-
-    @staticmethod
-    def _isrfc1918(address_txt: str | IPAddress) -> bool:
-        """Determine if an address is RFC1918 private or not."""
-        address = IPAddress(address_txt)
-        rfc1918_networks = ["10.0.0.0/8", "172.16.0.0/12", "192.168.0.0/16"]
-        rfc1918_ipset = IPSet(rfc1918_networks)
-
-        if address in rfc1918_ipset:
-            return True
-        return False
-
-    @staticmethod
-    def _isreservedaddress(address_txt: str | IPAddress) -> bool:
-        """Determine if an address is reserved (loopbacks, documentation, etc) or not."""
-        address = IPAddress(address_txt)
-
-        if address.version == 4:
-            return RdnsReaper._isreservedipv4(address_txt)
-        if address.version == 6:
-            return RdnsReaper._isreservedipv6(address_txt)
-
-    @staticmethod
-    def _isreservedipv4(address_txt: str | IPAddress) -> bool:
-        """Determine if an address is reserved (loopbacks, documentation, etc) or not."""
-        address = IPAddress(address_txt)
-
-        if address.version == 4:
-            reserved_network_ipset = IPSet(IPV4_RESERVED_NETWORK_LIST)
-            if address_txt in reserved_network_ipset:
-                return True
-            return False
-
-        raise ValueError
-
-    @staticmethod
-    def _isreservedipv6(address_txt: str | IPAddress) -> bool:
-        """Determine if an address is reserved (loopbacks, documentation, etc) or not."""
-        address = IPAddress(address_txt)
-
-        if address.version == 6:
-            reserved_network_ipset = IPSet(IPV6_RESERVED_NETWORK_LIST)
-            if address_txt in reserved_network_ipset:
-                return True
-            return False
-
-        raise ValueError
-
-    class _ReaperIterator:
-        def __init__(self, parentclass):
-            self.__parentclass = parentclass
-            self.__counter = 0
-            self.__parent_len = len(parentclass)
-            self.__parent_keys = list(parentclass.keys())
-
-        def __next__(self):
-            if self.__counter < self.__parent_len:
-                key = self.__parent_keys[self.__counter]
-                value = self.__parentclass[key]
-                self.__counter += 1
-                return (key, value)
-
-            raise StopIteration
+import concurrent.futures
+import copy
+import socket
+
+import yaml
+from netaddr import AddrFormatError, IPAddress, IPSet
+
+IPV4_RESERVED_NETWORK_LIST = [
+    "0.0.0.0/8",
+    "100.64.0.0/10",
+    "127.0.0.0/8",
+    "169.254.0.0/16",
+    "192.0.0.0/24",
+    "192.0.2.0/24",
+    "192.88.99.0/24",
+    "198.51.100.0/24",
+    "203.0.113.0/24",
+    "224.0.0.0/4",
+    "233.252.0.0/24",
+    "240.0.0.0/4",
+    "255.255.255.255/32",
+]
+
+IPV4_RFC1918_NETWORK_LIST = [
+    "10.0.0.0/8",
+    "172.16.0.0/12",
+    "192.168.0.0/16",
+]
+
+IPV6_RESERVED_NETWORK_LIST = [
+    "::ffff:0:0/96",
+    "::ffff:0:0:0/96",
+    "64:ff9b::/96",
+    "64:ff9b:1::/48",
+    "100::/64",
+    "2001:0000::/32",
+    "2001:20::/28",
+    "2001:db8::/32",
+    "2002::/16",
+    "fc00::/7",
+    "fe80::/10",
+    "ff00::/8",
+]
+
+
+class RdnsReaper:
+    """Reverse DNS Lookup Engine."""
+
+    def __init__(self, **kwargs):
+        """Initialize class and take in user options.
+
+        Keyword Arguments:
+            allow_reserved_networks (bool, optional): if True disable automatic filtering of
+                reserved networks, must be set to True if checking of any reserved networks
+                is desired.  Can then be supplemented with a custom filter
+            autosave (bool, optional): if True, automatically saves the cache file after the
+                resolver runs.  Filename must be present and filemode must be w
+            concurrent (int, default = 5): number of concurrent resolver threads
+            limit_to_rfc1918 (bool, optional): limit resolve to IPv4 RFC1918 only
+            filter (str, list of strs, IPSet, optional): filter data
+                can be a string containing an IP Address, list of strings, or an IPSet object
+            filtermode ("block" | "allow", optional): sets filter mode to block list or allow list
+                defaults to block list if not specified
+            filename (str, optional): path and filename for disk based cache in YAML format
+            filemode ("r" | "w"), required if filename set): read only or read-write mode for
+                disk cache, if set to write, resolver may try to update the cache periodically
+                the savefile() function can be called without arguments to force an update
+            unresolvable (str, optional): string to set for each entry if resolving fails
+                None is the default, all other options prevent subsequent lookups if disk based
+                cache is in use
+
+
+        """
+        self._resolver_ip = None
+        self._dns_dict = {}
+        self._concurrent = 5
+        self._options_dict = {
+            "allow_reserved_networks": False,
+            "autosave": False,
+            "concurrent": 5,
+            "filemode": None,
+            "filename": None,
+            "filter": None,
+            "filter_mode": None,
+            "limit_to_rfc1918": False,
+        }
+        # Check for RFC1918 filtering
+        if "limit_to_rfc1918" in kwargs:
+            self.limit_to_rfc1918(kwargs["limit_to_rfc1918"])
+        else:
+            self._options_dict["limit_to_rfc1918"] = False
+
+        # Check for custom filtering
+        if kwargs.get("filter") is not None:
+            self.set_filter(kwargs.get("filter"), mode=kwargs.get("filtermode"))
+
+        # Allow reserved network check
+        if kwargs.get("allow_reserved_networks"):
+            self._options_dict["allow_reserved_networks"] = True
+        else:
+            self._options_dict["allow_reserved_networks"] = False
+
+        # Process parallel lookup concurrency
+        if kwargs.get("concurrent"):
+            if isinstance(kwargs["concurrent"], int):
+                self._options_dict["concurrent"] = kwargs["concurrent"]
+            else:
+                raise TypeError
+
+        # Determine how to mark unresolvable entries
+        try:
+            if isinstance(kwargs["unresolvable"], str):
+                self._unresolvable = kwargs["unresolvable"]
+            else:
+                raise TypeError
+        except KeyError:
+            self._unresolvable = None
+
+        try:
+            if isinstance(kwargs["filemode"], str):
+                if kwargs["filemode"] not in ("w", "r"):
+                    raise ValueError
+
+                self._options_dict["filemode"] = kwargs["filemode"]
+            else:
+                raise TypeError
+        except KeyError:
+            pass
+
+        try:
+            if isinstance(kwargs["filename"], str):
+                self._options_dict["filename"] = kwargs["filename"]
+            else:
+                raise TypeError
+        except KeyError:
+            pass
+
+        if (self._options_dict["filename"] is not None) and (
+            self._options_dict["filemode"] in ("r", "w")
+        ):
+            try:
+                self.loadfile(self._options_dict["filename"])
+            except FileNotFoundError:
+                pass
+
+        if kwargs.get("autosave") is True:
+            if (self._options_dict["filename"] is not None) and (
+                self._options_dict["filemode"] == "w"
+            ):
+                self._options_dict["autosave"] = True
+            else:
+                raise ValueError(
+                    'Autosave enabled but filename/mode not set correctly.  Filename must be present and mode must be "w".'
+                )
+
+    def __add__(self, new):
+        """Add two instances together and return a deepcopy."""
+        self_copy = copy.deepcopy(self)
+        if isinstance(new, RdnsReaper):
+            self_copy._dns_dict.update(new._dns_dict)
+        elif isinstance(new, str):
+            self_copy.add_ip(new)
+        elif isinstance(new, set):
+            self_copy.add_ip_list(new)
+        elif isinstance(new, list):
+            self_copy.add_ip_list(new)
+        else:
+            raise TypeError
+        return self_copy
+
+    def __contains__(self, ip_address):
+        """Allow for checking of IP in the instance."""
+        if ip_address in self._dns_dict.keys():
+            return True
+        return False
+
+    def __delitem__(self, ip_address):
+        """Remove an item if del() is called."""
+        self.remove_ip(ip_address)
+
+    def __enter__(self):
+        """Return self for use in 'with open()' style blocks."""
+        return self
+
+    def __exit__(self, exception_type, exception_value, traceback):
+        """Save file when class is being destroyed as appropriate."""
+        if (self._options_dict["filename"] is not None) and (self._options_dict["filemode"] == "w"):
+            self.savefile(self._options_dict["filename"])
+
+    def __getitem__(self, ip_address):
+        """Return IP address from internal dictionary, false if not found."""
+        try:
+            IPAddress(ip_address)
+            return self._dns_dict[ip_address]
+        except AddrFormatError as error_case:
+            raise AddrFormatError from error_case
+        except KeyError:
+            return False
+
+    def __iadd__(self, new):
+        """Add two instances together and return."""
+        if isinstance(new, RdnsReaper):
+            self._dns_dict.update(new._dns_dict)
+        elif isinstance(new, str):
+            self.add_ip(new)
+        elif isinstance(new, set):
+            self.add_ip_list(new)
+        elif isinstance(new, list):
+            self.add_ip_list(new)
+        else:
+            raise TypeError
+        return self
+
+    def __iter__(self):
+        """Return an iterator as needed for k, v walking."""
+        return self._ReaperIterator(self)
+
+    def __len__(self):
+        """Determine number of addresses in module."""
+        return len(self._dns_dict)
+
+    def __setitem__(self, ip_address, value):
+        """Allow set/reset of hostname for an IP via index."""
+        self.set_name(ip_address, value)
+
+    def _resolve_function(self, ip_address):
+        try:
+            name = socket.gethostbyaddr(ip_address)[0]
+            self._dns_dict[ip_address] = name
+        except socket.herror:
+            self._dns_dict[ip_address] = self._unresolvable
+
+    def add(self, *args, **kwargs):
+        """Generalized function for adding."""
+        self.__iadd__(*args, **kwargs)
+
+    def add_ip(self, ip_address: str, hostname: str = None):
+        """Add an IP to the list with option hostname, skip if exists."""
+        if ip_address in self._dns_dict.keys():
+            return True
+
+        try:
+            IPAddress(ip_address)
+            if hostname is None:
+                self._dns_dict.update({ip_address: None})
+            else:
+                self._dns_dict.update({ip_address: hostname})
+            return ip_address
+        except AddrFormatError as error_case:
+            raise TypeError from error_case
+
+    def add_ip_list(self, ip_list: list):
+        """Add all new IP's from a list."""
+        if isinstance(ip_list, set):
+            ip_list = list(ip_list)
+        if not isinstance(ip_list, list):
+            raise TypeError
+        for ip_address in ip_list:
+            self.add_ip(ip_address)
+
+    def allow_reserved_networks(self, option: bool):
+        """Allow users to enable/disable automatic filtering of reserved networks.
+
+        If a user wants to check reserved network IPs (loopbacks, link local, multicast, etc.)
+        they must set this option to True.  Users may manually filter some of the reserved
+        networks with the filter() option.  This option *must* be set to True to resolve any
+        reserved networks.  Using an allow filter with this option set to False will not resolve
+        any reserved networks.
+
+        Args:
+            option (bool): Set to True to disable automatic filtering of reserved networks
+
+        """
+        if not isinstance(option, bool):
+            raise TypeError
+
+        self._options_dict["allow_reserved_networks"] = option
+
+    def clear_all_hostnames(self):
+        """Clear all the hostnames from existing entries."""
+        new_ip_dict = {ip: None for ip in self._dns_dict}
+        self._dns_dict = new_ip_dict
+
+    def clearname(self, ip_address: str):
+        """Clear a specific IP's hostname.
+
+        Args:
+            ip_address (str): A string containing an IP address
+        """
+        try:
+            IPAddress(ip_address)
+        except AddrFormatError as error_case:
+            raise TypeError from error_case
+
+        if ip_address not in self._dns_dict.keys():
+            raise KeyError("Address not found")
+
+        self._dns_dict[ip_address] = None
+
+    def dict(self) -> dict:
+        """Return the internal dictionary to the calling function."""
+        return self._dns_dict
+
+    def get_dict(self) -> dict:
+        """Return the internal dictionary to the calling function."""
+        return self._dns_dict
+
+    def get_filter(self) -> tuple:
+        """Return current filter status."""
+        return (self._options_dict["filter"], self._options_dict["filter_mode"])
+
+    def get_options(self) -> dict:
+        """Return info about the various options set by the user."""
+        return self._options_dict
+
+    def items(self):
+        """Return the IP address and hostnames as a dict_items to allow iteration over k, v pairs."""
+        return self._dns_dict.items()
+
+    def keys(self) -> list:
+        """Return the IP address as keys in list format."""
+        return list(self._dns_dict.keys())
+
+    def limit_to_rfc1918(self, value: bool):
+        """Set the RFC1918 filter."""
+        if not isinstance(value, bool):
+            raise TypeError
+        self._options_dict["limit_to_rfc1918"] = value
+
+    def loadfile(self, filename: str):
+        """Load saved data in YAML format.
+
+        Args
+            filename (str): path and filename for the disk based YAML cache file
+        """
+        with open(filename, encoding="UTF-8") as f_handle:
+            f_data = f_handle.read()
+            self._dns_dict = yaml.safe_load(f_data)
+
+    def remove_ip(self, ip_address: str) -> bool:
+        """Remove an IP from the list, return false if not found.
+
+        Args:
+            ip_address (str): A string containing an IP Address to remove
+        """
+        try:
+            IPAddress(ip_address)
+            self._dns_dict.pop(ip_address)
+        except AddrFormatError as error_case:
+            raise TypeError from error_case
+        except KeyError:
+            return False
+        return True
+
+    def _build_resolve_list(self):
+        """Build list of IP's to perform resolver on, shared by serial and parallel methods."""
+        if self._options_dict["limit_to_rfc1918"]:
+            ipv4_skipped_networks = IPSet(IPV4_RESERVED_NETWORK_LIST)
+        elif self._options_dict["allow_reserved_networks"] is False:
+            ipv4_skipped_networks = IPSet(IPV4_RESERVED_NETWORK_LIST)
+        else:
+            ipv4_skipped_networks = IPSet()
+
+        if self._options_dict["allow_reserved_networks"] is False:
+            ipv6_skipped_networks = IPSet(IPV6_RESERVED_NETWORK_LIST)
+        else:
+            ipv6_skipped_networks = IPSet()
+
+        initial_ip_list = [key for key, value in self._dns_dict.items() if value is None]
+
+        pending_ipset = IPSet(initial_ip_list)
+
+        if self._options_dict["filter_mode"] == "block":
+            result_ipset = pending_ipset - self._options_dict["filter"]
+            initial_pending_ips = [str(x) for x in result_ipset]
+        elif self._options_dict["filter_mode"] == "allow":
+            result_ipset = pending_ipset & self._options_dict["filter"]
+            initial_pending_ips = [str(x) for x in result_ipset]
+        else:
+            initial_pending_ips = [str(x) for x in pending_ipset]
+
+        pending_ips = []
+
+        for key in initial_pending_ips:
+            address = IPAddress(key)
+
+            if self._options_dict["limit_to_rfc1918"] is False:
+                if (address.version == 4) and (address not in ipv4_skipped_networks):
+                    pending_ips.append(key)
+                elif (address.version == 6) and (address not in ipv6_skipped_networks):
+                    pending_ips.append(key)
+            else:
+                if address in IPSet(IPV4_RFC1918_NETWORK_LIST):
+                    pending_ips.append(key)
+
+        return pending_ips
+
+    def resolve_all(self):
+        """Resolve all unknown IPs in parallel."""
+        pending_ips = self._build_resolve_list()
+        with concurrent.futures.ThreadPoolExecutor(
+            max_workers=self._options_dict["concurrent"]
+        ) as executor:
+            executor.map(self._resolve_function, set(pending_ips))
+
+        if self._options_dict["autosave"] is True:
+            self.savefile()
+
+    def resolve_all_serial(self):
+        """Resolve all unknown IPs serially."""
+        pending_ips = self._build_resolve_list()
+
+        for address in pending_ips:
+            self._resolve_function(address)
+
+    def savefile(self, filename: str = None):
+        """Save internal dictionary to YAML file."""
+        if (
+            filename is None
+            and self._options_dict["filename"] is not None
+            and self._options_dict["filemode"] == "w"
+        ):
+            filename = self._options_dict["filename"]
+
+        with open(filename, "w", encoding="UTF-8") as f_handle:
+            f_handle.write("---\n")
+            f_handle.write(yaml.dump(self._dns_dict))
+
+    def set_name(self, ip_address: str, hostname: str):
+        """Force the hostname of an IP.
+
+        Args:
+            ip_address (str): String containing an IP address to be modified
+            hostname (str): Desired FQDN hostname to be set for this entry
+                Can be None to reset record to allow for subsequent lookup
+        """
+        try:
+            IPAddress(ip_address)
+        except AddrFormatError as error_case:
+            raise TypeError(f"IP Error: {error_case}") from error_case
+
+        if ip_address not in self._dns_dict.keys():
+            raise KeyError("Address does not exist")
+        self._dns_dict[ip_address] = hostname
+        # except KeyError as error_case:
+        # raise KeyError("Address does not exist")
+
+    def set_filter(self, filter_data: str, **kwargs):
+        """Define a custom filter."""
+        if kwargs.get("mode") is None:
+            self._options_dict["filter_mode"] = "block"
+        elif kwargs.get("mode").lower() in ("allow", "block"):
+            self._options_dict["filter_mode"] = kwargs.get("mode").lower()
+        else:
+            raise ValueError
+
+        if isinstance(filter_data, str):
+            filter_data = IPSet([filter_data])
+        elif isinstance(filter_data, list):
+            filter_data = IPSet(filter_data)
+
+        if not isinstance(filter_data, IPSet):
+            raise TypeError
+
+        self._options_dict["filter"] = filter_data
+
+    def values(self) -> list:
+        """Return the hostnames as values in list format."""
+        return list(self._dns_dict.values())
+
+    @staticmethod
+    def _isrfc1918(address_txt) -> bool:
+        """Determine if an address is RFC1918 private or not."""
+        address = IPAddress(address_txt)
+        rfc1918_networks = ["10.0.0.0/8", "172.16.0.0/12", "192.168.0.0/16"]
+        rfc1918_ipset = IPSet(rfc1918_networks)
+
+        if address in rfc1918_ipset:
+            return True
+        return False
+
+    @staticmethod
+    def _isreservedaddress(address_txt) -> bool:
+        """Determine if an address is reserved (loopbacks, documentation, etc) or not."""
+        address = IPAddress(address_txt)
+
+        if address.version == 4:
+            return RdnsReaper._isreservedipv4(address_txt)
+        if address.version == 6:
+            return RdnsReaper._isreservedipv6(address_txt)
+
+    @staticmethod
+    def _isreservedipv4(address_txt) -> bool:
+        """Determine if an address is reserved (loopbacks, documentation, etc) or not."""
+        address = IPAddress(address_txt)
+
+        if address.version == 4:
+            reserved_network_ipset = IPSet(IPV4_RESERVED_NETWORK_LIST)
+            if address_txt in reserved_network_ipset:
+                return True
+            return False
+
+        raise ValueError
+
+    @staticmethod
+    def _isreservedipv6(address_txt) -> bool:
+        """Determine if an address is reserved (loopbacks, documentation, etc) or not."""
+        address = IPAddress(address_txt)
+
+        if address.version == 6:
+            reserved_network_ipset = IPSet(IPV6_RESERVED_NETWORK_LIST)
+            if address_txt in reserved_network_ipset:
+                return True
+            return False
+
+        raise ValueError
+
+    class _ReaperIterator:
+        def __init__(self, parentclass):
+            self.__parentclass = parentclass
+            self.__counter = 0
+            self.__parent_len = len(parentclass)
+            self.__parent_keys = list(parentclass.keys())
+
+        def __next__(self):
+            if self.__counter < self.__parent_len:
+                key = self.__parent_keys[self.__counter]
+                value = self.__parentclass[key]
+                self.__counter += 1
+                return (key, value)
+
+            raise StopIteration
```

### Comparing `rdns_reaper-0.1.0rc1/LICENSE` & `rdns_reaper-0.1.1rc1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,679 +1,679 @@
-As of version 0.0.12, this project uses the GNU General Public License
-
-For commercial use, please contact the author.
-
-
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+As of version 0.0.12, this project uses the GNU General Public License
+
+For commercial use, please contact the author.
+
+
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `rdns_reaper-0.1.0rc1/README.md` & `rdns_reaper-0.1.1rc1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,155 @@
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdns-reaper)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/rdns-reaper)
-![PyPI](https://img.shields.io/pypi/v/rdns-reaper)
-![piwheels](https://img.shields.io/piwheels/v/rdns-reaper)
-![Read the Docs](https://img.shields.io/readthedocs/rdns_reaper)
-
-rdns-reaper: Reverse DNS Lookup Engine
-======================================
-
-rdns-reaper is a multi-threaded lookup engine for Python v3 to resolve DNS names from IP addresses.  IP addresses can be added to the custom class by a calling program individually or in batches, after which point the client triggers the resolver to execute on all IP addresses.  Once the lookup completes, the calling program can retrieve the data in a variety of ways.
-
-The library currently runs on IPv4 addresses and IPv6 address.  Entries can be cached to disk to prevent excessive querying.  Limited filtering exists to restrict lookups to RFC1918 IPv4 space as an option.
-
-rdns-reaper is currently tested with Python 3.6-3.11
-
-Documentation
--------------
-
-Read our documentation at https://rdns-reaper.readthedocs.io/en/latest/
-
-Object Name Change
-------------------
-
-**Note that starting with version 0.1.0, the reaper object has been renamed from rdns_reaper to RdnsReaper**
-
-For backwards compatability you can use the following import statement until your codebase is updated with the new name: 
-
-```python
->>> from rdns_reaper import RdnsReaper as rdns_reaper
-```
-
-The correct import statement for all new applications is:
-
-```python
->>> from rdns_reaper import RdnsReaper
-```
-
-
-Installation and Usage
-----------------------
-
-
-### PyPI
-```shell
-$ pip install rdns-reaper
-
-#For a specific version (e.g. 0.0.10)
-$ pip install rdns-reaper==0.0.10
-```
-
-### Github with PIP
-```shell
-#Latest Full Release
-$ pip install git+https://github.com/mullaneywt/rdns_reaper/@releases
-
-#Latest Release Candidate
-$ pip install git+https://github.com/mullaneywt/rdns_reaper/
-
-#Specific Release Version (e.g. 0.0.10)
-$ pip install git+https://github.com/mullaneywt/rdns_reaper/@0.0.10
-```
-
-### Usage
-```python
->>> from rdns_reaper import RdnsReaper
->>> rdr = RdnsReaper(limit_to_rfc1918=False, concurrent=20, unresolvable=r"N\A")
-
->>> iplist = ["8.8.8.8", "1.1.1.1", "8.8.4.4"]
->>> rdr.add_ip_list(iplist)
->>> rdr.resolve_all()
-
->>> rdr["1.1.1.1"]
-one.one.one.one
-
->>> for address in rdr:
->>>   print(address)
-{
-	('8.8.8.8', 'dns.google')
-	('1.1.1.1', 'one.one.one.one')
-	('8.8.4.4', 'dns.google')
-}
-```
-
-### Supported parameters
-The following parameters are supported when an instance of rdns_reaper is created:
-|parameter|type|description|default|
-|-|-|-|-|
-| allow_reserved_networks | boolean | Disables automatic filtering of IPv4/IPv6 reserved networks | False |
-| limit_to_rfc1918 | boolean | Limits checking to only IPv4 RFC1918 address space (IPv6 entirely disabled) | False |
-| concurrent | integer | Number of concurrent resolver threads to use | 5 |
-| unresolvable | string | Value to populate if resolving fails | None |
-| filemode | ["r"\|"w"] | read only or read-write disk cache | None |
-| filename | string | Path and filename for YAML formatted disk cache | None |
-| filter | IPSet, string, list of strings | Sets a custom IP filter | None |
-| filtermode | ["allow"\|"block"] | set the filter mode to an allow list or a block list | None |
-
-Note that entries with None as a value will be reprocessed in subsequent resolver runs, while entries with any other value from the `unresolveable` parameter will not be processed again without manual intervention
-
-### Supported operators
-* \+, which can add two rdns_reaper objects, a string with a single IP address, or a set/list with one or more IP addresses 
-* \+=, which can add two rdns_reaper objects, a string with a single IP address, or a set/list with one or more IP addresses
-
-### Supported magic methods
-* contains() - checks if a given string containing an IP address exists in the resolver instance
-* del() - takes a string containing an IP address and removes it from the resolver instance
-* getitem() - returns the resolved name for given string containing an IP address
-* iter() - will provider an iterator that returns address/name tuples
-* len() - number of unique IP addresses in a resolver instance
-
-### Supported custom methods
-* add_ip(IP) - adds an IP address (provided as a string)
-* add_ip_list(IP_LIST) - adds IP addresses (provided as a list of strings)
-* allow_reserved_networks() - disable/enable automatic filter of reserved networks
-* clear_all_hostnames() - resets all names to None across entire instance
-* clearname(IP) - resets a name to None
-* get_dict() - returns a dictionary with addresses as keys and names as values
-* get_filter() - returns a tuple with custom filter information or None if not set
-* get_options() - returns a dictionary listing options that have been set
-* keys() - returns a list of all IP addresses in the instance
-* loadfile() - forces a load of the YAML based disk cache
-* limit_to_rfc1918 - disable/enable automatic filtering to only IPv4 RFC1918 networks
-* remove_ip(IP) - removes an IP address (provided as a string)
-* resolve_all() - launches a threaded resolver process
-* resolve_all_serial() - launches a singular serial resolver process
-* savefile() - forces a save of the YAML based disk cache
-* set_name(IP, NAME) - forces the name for a value (provided as strings)
-* set_filter(IPSet, [mode=]) - sets a custom filter based on an IPSet, IP network in a string, or a list of strings containing IP networks.  Optional mode argument can be `block` or `allow` to set filtering to a block list or allow list
-* values() - returns a list of all DNS names
-
-License
--------
-
-Licensed under GNU GPL V3.0.  See the LICENSE file for more information.
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdns-reaper)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/rdns-reaper)
+![PyPI](https://img.shields.io/pypi/v/rdns-reaper)
+![piwheels](https://img.shields.io/piwheels/v/rdns-reaper)
+![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/mullaneywt/rdns_reaper)
+
+Build Status
+
+![Read the Docs](https://img.shields.io/readthedocs/rdns_reaper)
+![](https://github.com/mullaneywt/rdns_reaper/actions/workflows/releases_build.yaml/badge.svg)
+![](https://github.com/mullaneywt/rdns_reaper/actions/workflows/main_build.yaml/badge.svg)
+![](https://github.com/mullaneywt/rdns_reaper/actions/workflows/dev_build.yaml/badge.svg)
+
+rdns-reaper: Reverse DNS Lookup Engine
+======================================
+
+rdns-reaper is a multi-threaded lookup engine for Python v3 to resolve DNS names from IP addresses.  IP addresses can be added to the custom class by a calling program individually or in batches, after which point the client triggers the resolver to execute on all IP addresses.  Once the lookup completes, the calling program can retrieve the data in a variety of ways.
+
+The library currently runs on IPv4 addresses and IPv6 address.  Entries can be cached to disk to prevent excessive querying.  Limited filtering exists to restrict lookups to RFC1918 IPv4 space as an option.
+
+rdns-reaper is currently tested with Python 3.6-3.11
+
+Documentation
+-------------
+
+Read our documentation at https://rdns-reaper.readthedocs.io/en/latest/
+
+Object Name Change
+------------------
+
+**Note that starting with version 0.1.0, the reaper object has been renamed from rdns_reaper to RdnsReaper**
+
+For backwards compatability you can use the following import statement until your codebase is updated with the new name:
+
+```python
+>>> from rdns_reaper import RdnsReaper as rdns_reaper
+```
+
+The correct import statement for all new applications is:
+
+```python
+>>> from rdns_reaper import RdnsReaper
+```
+
+
+Installation and Usage
+----------------------
+
+
+### PyPI
+```shell
+$ pip install rdns-reaper
+
+#For a specific version (e.g. 0.0.10)
+$ pip install rdns-reaper==0.0.10
+```
+
+### Github with PIP
+```shell
+#Latest Full Release
+$ pip install git+https://github.com/mullaneywt/rdns_reaper/@releases
+
+#Latest Release Candidate
+$ pip install git+https://github.com/mullaneywt/rdns_reaper/
+
+#Specific Release Version (e.g. 0.0.10)
+$ pip install git+https://github.com/mullaneywt/rdns_reaper/@0.0.10
+```
+
+### Usage
+```python
+>>> from rdns_reaper import RdnsReaper
+>>> rdr = RdnsReaper(limit_to_rfc1918=False, concurrent=20, unresolvable=r"N\A")
+
+>>> iplist = ["8.8.8.8", "1.1.1.1", "8.8.4.4"]
+>>> rdr.add_ip_list(iplist)
+>>> rdr.resolve_all()
+
+>>> rdr["1.1.1.1"]
+one.one.one.one
+
+>>> for address in rdr:
+>>>   print(address)
+{
+	('8.8.8.8', 'dns.google')
+	('1.1.1.1', 'one.one.one.one')
+	('8.8.4.4', 'dns.google')
+}
+```
+
+### Supported parameters
+The following parameters are supported when an instance of rdns_reaper is created:
+|parameter|type|description|default|
+|-|-|-|-|
+| allow_reserved_networks | boolean | Disables automatic filtering of IPv4/IPv6 reserved networks | False |
+| autosave | boolean | Automatically saves disk based cache when resolve_all() is called | False |
+| limit_to_rfc1918 | boolean | Limits checking to only IPv4 RFC1918 address space (IPv6 entirely disabled) | False |
+| concurrent | integer | Number of concurrent resolver threads to use | 5 |
+| unresolvable | string | Value to populate if resolving fails | None |
+| filemode | ["r"\|"w"] | read only or read-write disk cache | None |
+| filename | string | Path and filename for YAML formatted disk cache | None |
+| filter | IPSet, string, list of strings | Sets a custom IP filter | None |
+| filtermode | ["allow"\|"block"] | set the filter mode to an allow list or a block list | None |
+
+Note that entries with None as a value will be reprocessed in subsequent resolver runs, while entries with any other value from the `unresolveable` parameter will not be processed again without manual intervention
+
+### Supported operators
+* \+, which can add two rdns_reaper objects, a string with a single IP address, or a set/list with one or more IP addresses
+* \+=, which can add two rdns_reaper objects, a string with a single IP address, or a set/list with one or more IP addresses
+
+### Supported magic methods
+* contains() - checks if a given string containing an IP address exists in the resolver instance
+* del() - takes a string containing an IP address and removes it from the resolver instance
+* getitem() - returns the resolved name for given string containing an IP address
+* iter() - will provider an iterator that returns address/name tuples
+* len() - number of unique IP addresses in a resolver instance
+
+### Supported custom methods
+* add_ip(IP) - adds an IP address (provided as a string)
+* add_ip_list(IP_LIST) - adds IP addresses (provided as a list of strings)
+* allow_reserved_networks() - disable/enable automatic filter of reserved networks
+* clear_all_hostnames() - resets all names to None across entire instance
+* clearname(IP) - resets a name to None
+* get_dict() - returns a dictionary with addresses as keys and names as values
+* get_filter() - returns a tuple with custom filter information or None if not set
+* get_options() - returns a dictionary listing options that have been set
+* keys() - returns a list of all IP addresses in the instance
+* loadfile() - forces a load of the YAML based disk cache
+* limit_to_rfc1918 - disable/enable automatic filtering to only IPv4 RFC1918 networks
+* remove_ip(IP) - removes an IP address (provided as a string)
+* resolve_all() - launches a threaded resolver process
+* resolve_all_serial() - launches a singular serial resolver process
+* savefile() - forces a save of the YAML based disk cache
+* set_name(IP, NAME) - forces the name for a value (provided as strings)
+* set_filter(IPSet, [mode=]) - sets a custom filter based on an IPSet, IP network in a string, or a list of strings containing IP networks.  Optional mode argument can be `block` or `allow` to set filtering to a block list or allow list
+* values() - returns a list of all DNS names
+
+Issues and contributing
+-----------------------
+
+If you find any issues, feel free to create a new issue at our github repository at: https://github.com/mullaneywt/rdns_reaper/issues
+
+Make sure you include information about the version you're running, the environment you're running in, what data you've presented to the lookup engine, and what your responses/error information was.
+
+Feature requests can also be created as an issue on github at the repository above.
+
+For Python developers, if you have a new feature or a bug-fix that you've implemented, please open a pull request with some detailed information about what you intend to add or fix.
+
+If you still having questions, feel free to email the maintainer.
+
+License
+-------
+
+Licensed under GNU GPL V3.0.  See the LICENSE file for more information.
```

### Comparing `rdns_reaper-0.1.0rc1/pyproject.toml` & `rdns_reaper-0.1.1rc1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,100 @@
-[project]
-name="rdns_reaper"
-version="0.1.0.rc1"
-authors=[ 
-  {name ="Will Mullaney",email="rdns-reaper@mullaneywt.anonaddy.com"}
-]
-description="Reverse DNS lookup engine"
-readme = "README.md"
-keywords=["reverse", "dns"]
-license={ text="GNU GPL v3.0" }
-requires-python=">=3.6"
-dependencies=["netaddr>=0.8.0", "pyyaml>=6.0"]
-classifiers = [
-    "Intended Audience :: Developers",
-    "Intended Audience :: Information Technology",
-    "Intended Audience :: System Administrators",
-    "Intended Audience :: Telecommunications Industry",
-    "Operating System :: OS Independent",
-    "Natural Language :: English",
-    "Topic :: Internet",
-    "Topic :: Internet :: Name Service (DNS)",
-    "Topic :: Software Development",
-    "Topic :: Software Development :: Libraries",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Software Development :: Quality Assurance",
-    "Topic :: Software Development :: Testing",
-    "Topic :: System :: Networking",
-    "Topic :: Utilities",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-]
-
-
-
-[project.urls]
-"Home Page" = "https://github.com/mullaneywt/rdns_reaper"
-"Bug Tracker" = "https://github.com/mullaneywt/rdns_reaper/issues"
-"Source" = "https://github.com/mullaneywt/rdns_reaper"
-"Documentation" = "https://rdns-reaper.readthedocs.io"
-
-
-[build-system]
-#requires = ["setuptools", "virtualenv"]
-#build-backend = "setuptools.build_meta"
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.hatch]
-packages = ["rdns_reaper"]
-
-
-[tool.hatch.build.targets.sdist]
-exclude = [
-  "rdns_reaper/test",
-  "/.github",
-  "/docs",
-  ".gitignore",
-  "tox.ini",
-  "requirements.txt"
-]
-
-[tool.hatch.build.targets.wheel]
-packages = ["rdns_reaper"]
-
-[tool.setuptools]
-packages = ["rdns_reaper"]
-
-[tool.black]
-line-length = 100
-target_version = ['py310']
-include = '\.pyi?$'
-exclude = '''
-
-(
-  /(
-      \.eggs         # exclude a few common directories in the
-    | \.git          # root of the project
-    | \.hg
-    | \.mypy_cache
-    | \.tox
-    | \.venv
-    | venv
-    | cleanrun
-    | _build
-    | buck-out
-    | build
-    | dist
-  )/
-  | foo.py           # also separately exclude a file named foo.py in
-                     # the root of the project
-)
-'''
+[project]
+name="rdns_reaper"
+version="0.1.1.rc1"
+authors=[
+  {name ="Will Mullaney",email="rdns-reaper@mullaneywt.anonaddy.com"}
+]
+description="Reverse DNS lookup engine"
+readme = "README.md"
+keywords=["reverse", "dns"]
+license={ text="GNU GPL v3.0" }
+requires-python=">=3.7"
+dependencies=["netaddr>=0.8.0", "pyyaml>=6.0"]
+classifiers = [
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Telecommunications Industry",
+    "Operating System :: OS Independent",
+    "Natural Language :: English",
+    "Topic :: Internet",
+    "Topic :: Internet :: Name Service (DNS)",
+    "Topic :: Software Development",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Software Development :: Quality Assurance",
+    "Topic :: Software Development :: Testing",
+    "Topic :: System :: Networking",
+    "Topic :: Utilities",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+]
+
+
+
+[project.urls]
+"Home Page" = "https://github.com/mullaneywt/rdns_reaper"
+"Bug Tracker" = "https://github.com/mullaneywt/rdns_reaper/issues"
+"Source" = "https://github.com/mullaneywt/rdns_reaper"
+"Documentation" = "https://rdns-reaper.readthedocs.io"
+
+
+[build-system]
+#requires = ["setuptools", "virtualenv"]
+#build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.hatch]
+packages = ["rdns_reaper"]
+
+
+[tool.hatch.build.targets.sdist]
+exclude = [
+  "rdns_reaper/test",
+  "/.github",
+  "/docs",
+  ".gitignore",
+  "tox.ini",
+  "requirements.txt"
+]
+
+[tool.hatch.build.targets.wheel]
+packages = ["rdns_reaper"]
+
+[tool.isort]
+profile = "black"
+
+[tool.setuptools]
+packages = ["rdns_reaper"]
+
+[tool.black]
+line-length = 100
+target_version = ['py310']
+include = '\.pyi?$'
+exclude = '''
+
+(
+  /(
+      \.eggs         # exclude a few common directories in the
+    | \.git          # root of the project
+    | \.hg
+    | \.mypy_cache
+    | \.tox
+    | \.venv
+    | venv
+    | cleanrun
+    | _build
+    | buck-out
+    | build
+    | dist
+  )/
+  | foo.py           # also separately exclude a file named foo.py in
+                     # the root of the project
+)
+'''
```

### Comparing `rdns_reaper-0.1.0rc1/PKG-INFO` & `rdns_reaper-0.1.1rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 Metadata-Version: 2.1
 Name: rdns_reaper
-Version: 0.1.0rc1
+Version: 0.1.1rc1
 Summary: Reverse DNS lookup engine
 Project-URL: Home Page, https://github.com/mullaneywt/rdns_reaper
 Project-URL: Bug Tracker, https://github.com/mullaneywt/rdns_reaper/issues
 Project-URL: Source, https://github.com/mullaneywt/rdns_reaper
 Project-URL: Documentation, https://rdns-reaper.readthedocs.io
 Author-email: Will Mullaney <rdns-reaper@mullaneywt.anonaddy.com>
 License: GNU GPL v3.0
+License-File: LICENSE
 Keywords: dns,reverse
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Requires-Dist: netaddr>=0.8.0
 Requires-Dist: pyyaml>=6.0
 Description-Content-Type: text/markdown
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdns-reaper)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/rdns-reaper)
 ![PyPI](https://img.shields.io/pypi/v/rdns-reaper)
 ![piwheels](https://img.shields.io/piwheels/v/rdns-reaper)
+![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/mullaneywt/rdns_reaper)
+
+Build Status
+
 ![Read the Docs](https://img.shields.io/readthedocs/rdns_reaper)
+![](https://github.com/mullaneywt/rdns_reaper/actions/workflows/releases_build.yaml/badge.svg)
+![](https://github.com/mullaneywt/rdns_reaper/actions/workflows/main_build.yaml/badge.svg)
+![](https://github.com/mullaneywt/rdns_reaper/actions/workflows/dev_build.yaml/badge.svg)
 
 rdns-reaper: Reverse DNS Lookup Engine
 ======================================
 
 rdns-reaper is a multi-threaded lookup engine for Python v3 to resolve DNS names from IP addresses.  IP addresses can be added to the custom class by a calling program individually or in batches, after which point the client triggers the resolver to execute on all IP addresses.  Once the lookup completes, the calling program can retrieve the data in a variety of ways.
 
 The library currently runs on IPv4 addresses and IPv6 address.  Entries can be cached to disk to prevent excessive querying.  Limited filtering exists to restrict lookups to RFC1918 IPv4 space as an option.
@@ -58,15 +66,15 @@
 Read our documentation at https://rdns-reaper.readthedocs.io/en/latest/
 
 Object Name Change
 ------------------
 
 **Note that starting with version 0.1.0, the reaper object has been renamed from rdns_reaper to RdnsReaper**
 
-For backwards compatability you can use the following import statement until your codebase is updated with the new name: 
+For backwards compatability you can use the following import statement until your codebase is updated with the new name:
 
 ```python
 >>> from rdns_reaper import RdnsReaper as rdns_reaper
 ```
 
 The correct import statement for all new applications is:
 
@@ -121,26 +129,27 @@
 ```
 
 ### Supported parameters
 The following parameters are supported when an instance of rdns_reaper is created:
 |parameter|type|description|default|
 |-|-|-|-|
 | allow_reserved_networks | boolean | Disables automatic filtering of IPv4/IPv6 reserved networks | False |
+| autosave | boolean | Automatically saves disk based cache when resolve_all() is called | False |
 | limit_to_rfc1918 | boolean | Limits checking to only IPv4 RFC1918 address space (IPv6 entirely disabled) | False |
 | concurrent | integer | Number of concurrent resolver threads to use | 5 |
 | unresolvable | string | Value to populate if resolving fails | None |
 | filemode | ["r"\|"w"] | read only or read-write disk cache | None |
 | filename | string | Path and filename for YAML formatted disk cache | None |
 | filter | IPSet, string, list of strings | Sets a custom IP filter | None |
 | filtermode | ["allow"\|"block"] | set the filter mode to an allow list or a block list | None |
 
 Note that entries with None as a value will be reprocessed in subsequent resolver runs, while entries with any other value from the `unresolveable` parameter will not be processed again without manual intervention
 
 ### Supported operators
-* \+, which can add two rdns_reaper objects, a string with a single IP address, or a set/list with one or more IP addresses 
+* \+, which can add two rdns_reaper objects, a string with a single IP address, or a set/list with one or more IP addresses
 * \+=, which can add two rdns_reaper objects, a string with a single IP address, or a set/list with one or more IP addresses
 
 ### Supported magic methods
 * contains() - checks if a given string containing an IP address exists in the resolver instance
 * del() - takes a string containing an IP address and removes it from the resolver instance
 * getitem() - returns the resolved name for given string containing an IP address
 * iter() - will provider an iterator that returns address/name tuples
@@ -162,11 +171,24 @@
 * resolve_all() - launches a threaded resolver process
 * resolve_all_serial() - launches a singular serial resolver process
 * savefile() - forces a save of the YAML based disk cache
 * set_name(IP, NAME) - forces the name for a value (provided as strings)
 * set_filter(IPSet, [mode=]) - sets a custom filter based on an IPSet, IP network in a string, or a list of strings containing IP networks.  Optional mode argument can be `block` or `allow` to set filtering to a block list or allow list
 * values() - returns a list of all DNS names
 
+Issues and contributing
+-----------------------
+
+If you find any issues, feel free to create a new issue at our github repository at: https://github.com/mullaneywt/rdns_reaper/issues
+
+Make sure you include information about the version you're running, the environment you're running in, what data you've presented to the lookup engine, and what your responses/error information was.
+
+Feature requests can also be created as an issue on github at the repository above.
+
+For Python developers, if you have a new feature or a bug-fix that you've implemented, please open a pull request with some detailed information about what you intend to add or fix.
+
+If you still having questions, feel free to email the maintainer.
+
 License
 -------
 
-Licensed under GNU GPL V3.0.  See the LICENSE file for more information.
+Licensed under GNU GPL V3.0.  See the LICENSE file for more information.
```

