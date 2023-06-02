# Comparing `tmp/stcgal-1.6.tar.gz` & `tmp/stcgal-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stcgal-1.6.tar", last modified: Mon Sep 24 21:05:22 2018, max compression
+gzip compressed data, was "stcgal-1.8.tar", last modified: Fri Jun  2 12:58:59 2023, max compression
```

## Comparing `stcgal-1.6.tar` & `stcgal-1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2018-09-24 21:05:22.000000 stcgal-1.6/
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2018-09-24 21:05:22.000000 stcgal-1.6/stcgal/
--rw-rw-r--   0 greg      (1000) greg      (1000)    10731 2018-09-24 20:40:30.000000 stcgal-1.6/stcgal/frontend.py
--rw-rw-r--   0 greg      (1000) greg      (1000)       20 2018-09-24 20:57:16.000000 stcgal-1.6/stcgal/__init__.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    26956 2018-08-25 01:42:03.000000 stcgal-1.6/stcgal/options.py
--rwxrwxr-x   0 greg      (1000) greg      (1000)     1222 2017-06-16 07:18:03.000000 stcgal-1.6/stcgal/__main__.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     6294 2018-06-26 22:23:31.000000 stcgal-1.6/stcgal/ihex.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    70210 2018-08-25 01:42:03.000000 stcgal-1.6/stcgal/protocols.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    92457 2018-08-25 02:10:52.000000 stcgal-1.6/stcgal/models.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     2442 2018-08-25 01:42:03.000000 stcgal-1.6/stcgal/utils.py
--rwxrwxr-x   0 greg      (1000) greg      (1000)     2674 2018-09-24 19:29:55.000000 stcgal-1.6/setup.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2018-09-24 21:05:22.000000 stcgal-1.6/stcgal.egg-info/
--rw-rw-r--   0 greg      (1000) greg      (1000)        1 2018-09-24 21:05:22.000000 stcgal-1.6/stcgal.egg-info/dependency_links.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        7 2018-09-24 21:05:22.000000 stcgal-1.6/stcgal.egg-info/top_level.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)      343 2018-09-24 21:05:22.000000 stcgal-1.6/stcgal.egg-info/SOURCES.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)     1933 2018-09-24 21:05:22.000000 stcgal-1.6/stcgal.egg-info/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)       48 2018-09-24 21:05:22.000000 stcgal-1.6/stcgal.egg-info/entry_points.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)       46 2018-09-24 21:05:22.000000 stcgal-1.6/stcgal.egg-info/requires.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)     1520 2018-09-24 19:29:55.000000 stcgal-1.6/README.md
--rw-rw-r--   0 greg      (1000) greg      (1000)     1933 2018-09-24 21:05:22.000000 stcgal-1.6/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)       38 2018-09-24 21:05:22.000000 stcgal-1.6/setup.cfg
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-06-02 12:58:59.274308 stcgal-1.8/
+-rw-r--r--   0 greg      (1000) greg      (1000)     1735 2023-06-02 12:58:59.274308 stcgal-1.8/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     2009 2023-06-01 19:21:33.000000 stcgal-1.8/README.md
+-rw-r--r--   0 greg      (1000) greg      (1000)       38 2023-06-02 12:58:59.274308 stcgal-1.8/setup.cfg
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     2625 2023-06-01 19:21:33.000000 stcgal-1.8/setup.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-06-02 12:58:59.273308 stcgal-1.8/stcgal/
+-rw-r--r--   0 greg      (1000) greg      (1000)       20 2023-06-02 11:09:04.000000 stcgal-1.8/stcgal/__init__.py
+-rwxrwxr-x   0 greg      (1000) greg      (1000)     1222 2021-08-03 12:52:13.000000 stcgal-1.8/stcgal/__main__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    12932 2023-06-02 11:09:04.000000 stcgal-1.8/stcgal/frontend.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     6505 2023-06-01 19:21:33.000000 stcgal-1.8/stcgal/ihex.py
+-rw-r--r--   0 greg      (1000) greg      (1000)   145782 2023-06-01 19:21:33.000000 stcgal-1.8/stcgal/models.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    26957 2023-06-01 19:21:33.000000 stcgal-1.8/stcgal/options.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    89416 2023-06-02 11:09:04.000000 stcgal-1.8/stcgal/protocols.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     2442 2023-06-01 19:21:33.000000 stcgal-1.8/stcgal/utils.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-06-02 12:58:59.273308 stcgal-1.8/stcgal.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)     1735 2023-06-02 12:58:58.000000 stcgal-1.8/stcgal.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)      343 2023-06-02 12:58:59.000000 stcgal-1.8/stcgal.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-06-02 12:58:58.000000 stcgal-1.8/stcgal.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       47 2023-06-02 12:58:59.000000 stcgal-1.8/stcgal.egg-info/entry_points.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       46 2023-06-02 12:58:59.000000 stcgal-1.8/stcgal.egg-info/requires.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        7 2023-06-02 12:58:59.000000 stcgal-1.8/stcgal.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stcgal-1.6/stcgal/frontend.py` & `stcgal-1.8/stcgal/frontend.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,52 +22,63 @@
 
 import sys
 import argparse
 import stcgal
 import serial
 from stcgal.utils import BaudType
 from stcgal.protocols import Stc89Protocol
+from stcgal.protocols import Stc89AProtocol
 from stcgal.protocols import Stc12AProtocol
 from stcgal.protocols import Stc12BProtocol
 from stcgal.protocols import Stc12Protocol
 from stcgal.protocols import Stc15Protocol
 from stcgal.protocols import Stc15AProtocol
 from stcgal.protocols import StcUsb15Protocol
 from stcgal.protocols import Stc8Protocol
+from stcgal.protocols import Stc8dProtocol
+from stcgal.protocols import Stc8gProtocol
 from stcgal.protocols import StcAutoProtocol
 from stcgal.protocols import StcProtocolException
 from stcgal.protocols import StcFramingException
 from stcgal.ihex import IHex
 
 class StcGal:
     """STC ISP flash tool frontend"""
 
     def __init__(self, opts):
         self.opts = opts
+        self.hexFileType = 8
         self.initialize_protocol(opts)
 
     def initialize_protocol(self, opts):
         """Initialize protocol backend"""
         if opts.protocol == "stc89":
             self.protocol = Stc89Protocol(opts.port, opts.handshake, opts.baud)
+        elif opts.protocol == "stc89a":
+            self.protocol = Stc89AProtocol(opts.port, opts.handshake, opts.baud)
         elif opts.protocol == "stc12a":
             self.protocol = Stc12AProtocol(opts.port, opts.handshake, opts.baud)
         elif opts.protocol == "stc12b":
             self.protocol = Stc12BProtocol(opts.port, opts.handshake, opts.baud)
         elif opts.protocol == "stc12":
             self.protocol = Stc12Protocol(opts.port, opts.handshake, opts.baud)
         elif opts.protocol == "stc15a":
-            self.protocol = Stc15AProtocol(opts.port, opts.handshake, opts.baud,
-                                           round(opts.trim * 1000))
+            self.protocol = Stc15AProtocol(opts.port, opts.handshake, opts.baud, round(opts.trim * 1000))
         elif opts.protocol == "stc15":
-            self.protocol = Stc15Protocol(opts.port, opts.handshake, opts.baud,
-                                          round(opts.trim * 1000))
+            self.protocol = Stc15Protocol(opts.port, opts.handshake, opts.baud, round(opts.trim * 1000))
         elif opts.protocol == "stc8":
-            self.protocol = Stc8Protocol(opts.port, opts.handshake, opts.baud,
-                                         round(opts.trim * 1000))
+            self.protocol = Stc8Protocol(opts.port, opts.handshake, opts.baud, round(opts.trim * 1000))
+        elif opts.protocol == "stc8d":
+            self.protocol = Stc8dProtocol(opts.port, opts.handshake, opts.baud, round(opts.trim * 1000))
+        elif opts.protocol == "stc8g":
+            """FIXME Ugly hack, but works until I fully implement the STC8G protocol"""
+            if opts.trim < 27360:
+                self.protocol = Stc8dProtocol(opts.port, opts.handshake, opts.baud, round(opts.trim * 1000))
+            else:
+                self.protocol = Stc8gProtocol(opts.port, opts.handshake, opts.baud, round(opts.trim * 1000))
         elif opts.protocol == "usb15":
             self.protocol = StcUsb15Protocol()
         else:
             self.protocol = StcAutoProtocol(opts.port, opts.handshake, opts.baud)
         self.protocol.debug = opts.debug
 
     def emit_options(self, options):
@@ -86,77 +97,97 @@
         """Load file with Intel Hex autodetection."""
 
         fname = fileobj.name.lower()
         if (fname.endswith(".hex") or fname.endswith(".ihx") or
                 fname.endswith(".ihex")):
             try:
                 hexfile = IHex.read(fileobj)
+                self.hexFileType = hexfile.get_mode()
                 binary = hexfile.extract_data()
                 print("%d bytes (Intel HEX)" %len(binary))
                 return binary
             except ValueError as ex:
                 raise IOError("invalid Intel HEX file (%s)" %ex)
         else:
             binary = fileobj.read()
             print("%d bytes (Binary)" %len(binary))
             return binary
 
     def program_mcu(self):
         """Execute the standard programming flow."""
 
-        code_size = self.protocol.model.code
-        ee_size = self.protocol.model.eeprom
+        if self.opts.option: self.emit_options(self.opts.option)
+
+        if self.protocol.split_code and self.protocol.model.iap:
+            code_size = self.protocol.split_code
+            ee_size = self.protocol.split_eeprom
+        else:
+            code_size = self.protocol.model.code
+            ee_size = self.protocol.model.eeprom
 
         print("Loading flash: ", end="")
         sys.stdout.flush()
         bindata = self.load_file_auto(self.opts.code_image)
+        
+        if self.protocol.model.mcs251 and self.hexFileType != 32:
+            print("Invalid input file. MCU is an MCS-251, input file MUST specify a linear", file=sys.stderr)
+            print("base address, i.e. contain a type 04 record. More information at:", file=sys.stderr)
+            print("https://en.wikipedia.org/wiki/Intel_HEX", file=sys.stderr)
+        else:
+            # warn if it overflows
+            if len(bindata) > code_size:
+                print("WARNING: code_image overflows into eeprom segment!", file=sys.stderr)
+            if len(bindata) > (code_size + ee_size):
+                print("WARNING: code_image truncated!", file=sys.stderr)
+                bindata = bindata[0:code_size + ee_size]
+
+            # add eeprom data if supplied
+            if self.opts.eeprom_image:
+                print("Loading EEPROM: ", end="")
+                sys.stdout.flush()
+                eedata = self.load_file_auto(self.opts.eeprom_image)
+                if len(eedata) > ee_size:
+                    print("WARNING: eeprom_image truncated!", file=sys.stderr)
+                    eedata = eedata[0:ee_size]
+                if len(bindata) < code_size:
+                    bindata += bytes([0xff] * (code_size - len(bindata)))
+                elif len(bindata) > code_size:
+                    print("WARNING: eeprom_image overlaps code_image!", file=sys.stderr)
+                    bindata = bindata[0:code_size]
+                bindata += eedata
+
+            # pad to 512 byte boundary
+            if len(bindata) % 512:
+                bindata += b'\xff' * (512 - len(bindata) % 512)
+
+            self.protocol.handshake()
+            self.protocol.erase_flash(len(bindata), code_size)
+            self.protocol.program_flash(bindata)
+            self.protocol.program_options()
+        
+        self.protocol.disconnect()
 
-        # warn if it overflows
-        if len(bindata) > code_size:
-            print("WARNING: code_image overflows into eeprom segment!", file=sys.stderr)
-        if len(bindata) > (code_size + ee_size):
-            print("WARNING: code_image truncated!", file=sys.stderr)
-            bindata = bindata[0:code_size + ee_size]
-
-        # add eeprom data if supplied
-        if self.opts.eeprom_image:
-            print("Loading EEPROM: ", end="")
-            sys.stdout.flush()
-            eedata = self.load_file_auto(self.opts.eeprom_image)
-            if len(eedata) > ee_size:
-                print("WARNING: eeprom_image truncated!", file=sys.stderr)
-                eedata = eedata[0:ee_size]
-            if len(bindata) < code_size:
-                bindata += bytes(code_size - len(bindata))
-            elif len(bindata) > code_size:
-                print("WARNING: eeprom_image overlaps code_image!", file=sys.stderr)
-                bindata = bindata[0:code_size]
-            bindata += eedata
-
-        # pad to 512 byte boundary
-        if len(bindata) % 512:
-            bindata += b'\xff' * (512 - len(bindata) % 512)
+    def erase_mcu(self):
+        """Erase MCU without programming"""
 
-        if self.opts.option: self.emit_options(self.opts.option)
+        code_size = self.protocol.model.code
 
         self.protocol.handshake()
-        self.protocol.erase_flash(len(bindata), code_size)
-        self.protocol.program_flash(bindata)
-        self.protocol.program_options()
+        self.protocol.erase_flash(code_size, code_size)
         self.protocol.disconnect()
 
     def run(self):
         """Run programmer, main entry point."""
 
         if self.opts.version:
             print("stcgal {}".format(stcgal.__version__))
             return 0
 
         try:
-            self.protocol.connect(autoreset=self.opts.autoreset, resetcmd=self.opts.resetcmd)
+            self.protocol.connect(autoreset=self.opts.autoreset, resetcmd=self.opts.resetcmd, resetpin=self.opts.resetpin)
             if isinstance(self.protocol, StcAutoProtocol):
                 if not self.protocol.protocol_name:
                     raise StcProtocolException("cannot detect protocol")
                 base_protocol = self.protocol
                 self.opts.protocol = self.protocol.protocol_name
                 print("Protocol detected: %s" % self.opts.protocol)
                 # recreate self.protocol with proper protocol class
@@ -168,15 +199,16 @@
         except KeyboardInterrupt:
             sys.stdout.flush()
             print("interrupted")
             return 2
         except (StcFramingException, StcProtocolException) as ex:
             sys.stdout.flush()
             print("Protocol error: %s" % ex, file=sys.stderr)
-            self.protocol.disconnect()
+            if not isinstance(self.protocol, StcAutoProtocol):
+                self.protocol.disconnect()
             return 1
         except serial.SerialException as ex:
             sys.stdout.flush()
             print("Serial port error: %s" % ex, file=sys.stderr)
             return 1
         except IOError as ex:
             sys.stdout.flush()
@@ -186,16 +218,18 @@
             sys.stdout.flush()
             print("Unexpected error: %s" % ex, file=sys.stderr)
             return 1
 
         try:
             if self.opts.code_image:
                 self.program_mcu()
-                return 0
-            self.protocol.disconnect()
+            elif self.opts.erase:
+                self.erase_mcu()
+            else:
+                self.protocol.disconnect()
             return 0
         except NameError as ex:
             sys.stdout.flush()
             print("Option error: %s" % ex, file=sys.stderr)
             self.protocol.disconnect()
             return 1
         except (StcFramingException, StcProtocolException) as ex:
@@ -219,22 +253,26 @@
 
 
 def cli():
     # check arguments
     parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter,
                                      description="stcgal {} - an STC MCU ISP flash tool\n".format(stcgal.__version__) +
                                                  "(C) 2014-2018 Grigori Goronzy and others\nhttps://github.com/grigorig/stcgal")
-    parser.add_argument("code_image", help="code segment file to flash (BIN/HEX)", type=argparse.FileType("rb"), nargs='?')
+    exclusives = parser.add_mutually_exclusive_group()
+    exclusives.add_argument("code_image", help="code segment file to flash (BIN/HEX)", type=argparse.FileType("rb"), nargs='?')
     parser.add_argument("eeprom_image", help="eeprom segment file to flash (BIN/HEX)", type=argparse.FileType("rb"), nargs='?')
+    exclusives.add_argument("-e", "--erase", help="only erase flash memory", action="store_true")
     parser.add_argument("-a", "--autoreset", help="cycle power automatically by asserting DTR", action="store_true")
+    parser.add_argument("-A", "--resetpin", help="pin to hold down when using --autoreset (default: DTR)",
+                        choices=["dtr", "rts"], default="dtr")
     parser.add_argument("-r", "--resetcmd",  help="shell command for board power-cycling (instead of DTR assertion)", action="store")
     parser.add_argument("-P", "--protocol", help="protocol version (default: auto)",
-                        choices=["stc89", "stc12a", "stc12b", "stc12", "stc15a", "stc15", "stc8", "usb15", "auto"], default="auto")
+                        choices=["stc89", "stc89a", "stc12a", "stc12b", "stc12", "stc15a", "stc15", "stc8", "stc8d", "stc8g", "usb15", "auto"], default="auto")
     parser.add_argument("-p", "--port", help="serial port device", default="/dev/ttyUSB0")
-    parser.add_argument("-b", "--baud", help="transfer baud rate (default: 19200)", type=BaudType(), default=19200)
+    parser.add_argument("-b", "--baud", help="transfer baud rate (default: 115200)", type=BaudType(), default=115200)
     parser.add_argument("-l", "--handshake", help="handshake baud rate (default: 2400)", type=BaudType(), default=2400)
     parser.add_argument("-o", "--option", help="set option (can be used multiple times, see documentation)", action="append")
     parser.add_argument("-t", "--trim", help="RC oscillator frequency in kHz (STC15+ series only)", type=float, default=0.0)
     parser.add_argument("-D", "--debug", help="enable debug output", action="store_true")
     parser.add_argument("-V", "--version", help="print version info and exit", action="store_true")
     opts = parser.parse_args()
```

### Comparing `stcgal-1.6/stcgal/options.py` & `stcgal-1.8/stcgal/options.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -784,8 +784,8 @@
     def get_flash_split(self):
         return self.msr[4] * 256
 
     def set_flash_split(self, val):
         num_val = Utils.to_int(val)
         if num_val < 512 or num_val > 65024 or (num_val % 512) != 0:
             raise ValueError("must be between 512 and 65024 bytes and a multiple of 512 bytes")
-        self.msr[4] = num_val // 256
+        self.msr[4] = num_val // 256
```

### Comparing `stcgal-1.6/stcgal/__main__.py` & `stcgal-1.8/stcgal/__main__.py`

 * *Files identical despite different names*

### Comparing `stcgal-1.6/stcgal/ihex.py` & `stcgal-1.8/stcgal/ihex.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,39 @@
     """Intel HEX parser and writer"""
 
     @classmethod
     def read(cls, lines):
         """Read Intel HEX data from string or lines"""
         ihex = cls()
 
-        segbase = 0
         for line in lines:
             line = line.strip()
             if not line:
                 continue
 
             t, a, d = ihex.parse_line(line)
             if t == 0x00:
-                ihex.insert_data(segbase + a, d)
+                ihex.insert_data(a, d)
 
             elif t == 0x01:
                 break  # Should we check for garbage after this?
 
             elif t == 0x02:
                 ihex.set_mode(16)
-                segbase = struct.unpack(">H", d[0:2])[0] << 4
+                ihex.linearBaseAddress = struct.unpack(">H", d[0:2])[0] << 4
 
             elif t == 0x03:
                 ihex.set_mode(16)
 
                 cs, ip = struct.unpack(">2H", d[0:2])
                 ihex.set_start((cs, ip))
 
             elif t == 0x04:
                 ihex.set_mode(32)
-                segbase = struct.unpack(">H", d[0:2])[0] << 16
+                ihex.linearBaseAddress = struct.unpack(">H", d[0:2])[0] << 16
 
             elif t == 0x05:
                 ihex.set_mode(32)
                 ihex.set_start(struct.unpack(">I", d[0:4])[0])
 
             else:
                 raise ValueError("Invalid type byte")
@@ -59,14 +58,15 @@
         return ihex
 
     def __init__(self):
         self.areas = {}
         self.start = None
         self.mode = 8
         self.row_bytes = 16
+        self.linearBaseAddress = 0
 
     def set_row_bytes(self, row_bytes):
         """Set output hex file row width (bytes represented per row)."""
         if row_bytes < 1 or row_bytes > 0xff:
             raise ValueError("Value out of range: (%r)" % row_bytes)
         self.row_bytes = row_bytes
 
@@ -101,14 +101,20 @@
 
     def set_start(self, start=None):
         self.start = start
 
     def set_mode(self, mode):
         self.mode = mode
 
+    def get_mode(self):
+        return self.mode
+        
+    def get_linearBaseAddress(self):
+        return self.linearBaseAddress
+
     def get_area(self, addr):
         for start, data in self.areas.items():
             end = start + len(data)
             if addr >= start and addr <= end:
                 return start
 
         return None
@@ -151,16 +157,16 @@
             raise ValueError("Checksums do not match")
 
         return (line_type, addr, data)
 
     def make_line(self, line_type, addr, data):
         line = struct.pack(">BHB", len(data), addr, line_type)
         line += data
-        line += chr(self.calc_checksum(line))
-        return ":" + line.encode("hex").upper() + "\r\n"
+        line += bytes([self.calc_checksum(line)])
+        return ":" + line.hex().upper() + "\r\n"
 
     def write(self):
         """Write Intel HEX data to string"""
         output = ""
 
         for start, data in sorted(self.areas.items()):
             i = 0
@@ -189,29 +195,30 @@
                     newsegbase = addr >> 16
                     addr = addr & 0xFFFF
 
                     if newsegbase != segbase:
                         output += self.make_line(
                             0x04, 0, struct.pack(">H", newsegbase))
                         segbase = newsegbase
+                        segbase = newsegbase
 
                 output += self.make_line(0x00, addr, chunk)
 
                 i += self.row_bytes
                 start += self.row_bytes
 
         if self.start is not None:
             if self.mode == 16:
                 output += self.make_line(
                     0x03, 0, struct.pack(">2H", self.start[0], self.start[1]))
             elif self.mode == 32:
                 output += self.make_line(
                     0x05, 0, struct.pack(">I", self.start))
 
-        output += self.make_line(0x01, 0, "")
+        output += self.make_line(0x01, 0, b"")
         return output
 
     def write_file(self, fname):
         """Write Intel HEX data to file"""
         f = open(fname, "w")
         f.write(self.write())
         f.close()
```

### Comparing `stcgal-1.6/stcgal/protocols.py` & `stcgal-1.8/stcgal/protocols.py`

 * *Files 22% similar despite different names*

```diff
@@ -82,20 +82,23 @@
         self.baud_transfer = baud_transfer
 
         self.mcu_magic = 0
         self.mcu_clock_hz = 0.0
         self.mcu_bsl_version = ""
         self.options = None
         self.model = None
+        self.split_eeprom = None
+        self.split_code = None
         self.uid = None
         self.debug = False
         self.status_packet = None
         self.protocol_name = None
         self.progress = None
         self.progress_cb = self.progress_bar_cb
+        self.linearBaseAddress = 0
 
     def progress_text_cb(self, current, written, maximum):
         print(current, written, maximum)
 
     def progress_bar_cb(self, current, written, maximum):
         if not self.progress:
             self.progress = tqdm.tqdm(
@@ -129,15 +132,15 @@
         if packet[-1] != self.PACKET_END[0]:
             self.dump_packet(packet)
             raise StcFramingException("incorrect frame end")
 
         return packet[5:-1]
 
     @abstractmethod
-    def write_packet(self, packet_data):
+    def write_packet(self, packet_data, epilogue_len = 0):
         pass
 
     def read_packet(self):
         """Read and check packet from MCU.
 
         Reads a packet of data from the MCU and and do
         validity and checksum checks on it.
@@ -194,30 +197,32 @@
 
         duration = 0
         while True:
             if timeout > 0 and duration > timeout:
                 raise serial.SerialTimeoutException("pulse timeout")
             self.ser.write(character)
             self.ser.flush()
-            time.sleep(0.015)
-            duration += 0.015
+            time.sleep(0.030)
+            duration += 0.030
             if self.ser.inWaiting() > 0: break
 
     def initialize_model(self):
         """Initialize model-specific information"""
 
         self.mcu_magic, = struct.unpack(">H", self.status_packet[20:22])
         try:
             self.model = MCUModelDatabase.find_model(self.mcu_magic)
         except NameError:
             msg = ("WARNING: Unknown model %02X%02X!" %
                 (self.mcu_magic >> 8, self.mcu_magic & 0xff))
             print(msg, file=sys.stderr)
             self.model = MCUModelDatabase.MCUModel(name="UNKNOWN",
                 magic=self.mcu_magic, total=63488, code=63488, eeprom=0)
+        except ValueError as ex:
+            raise StcProtocolException(ex)
 
         # special case for duplicated mcu magic,
         #   0xf294 (STC15F104W, STC15F104E)
         #   0xf2d4 (STC15L104W, STC15L104E)
         # duplicated mcu magic can be found using command,
         #   grep -o 'magic=[^,]*' models.py | sort | uniq -d
         if self.mcu_magic in (0xF294, 0xF2D4):
@@ -256,30 +261,41 @@
         elif clock_hz < 24E6: iap_wait = 0x81
 
         return iap_wait
 
     def set_option(self, name, value):
         self.options.set_option(name, value)
 
-    def reset_device(self, resetcmd=False):
+    def reset_device(self, resetcmd=False, resetpin=False):
         if not resetcmd:
             print("Cycling power: ", end="")
             sys.stdout.flush()
-            self.ser.setDTR(True)
-            time.sleep(0.5)
-            self.ser.setDTR(False)
+            
+            if resetpin == "rts":
+                self.ser.setRTS(True)
+            else:
+                self.ser.setDTR(True)
+				
+            time.sleep(0.25)
+            
+            if resetpin == "rts":
+                self.ser.setRTS(False)
+            else:
+                self.ser.setDTR(False)
+				
+            time.sleep(0.030)
             print("done")
         else:
             print("Cycling power via shell cmd: " + resetcmd)
             os.system(resetcmd)
 
         print("Waiting for MCU: ", end="")
         sys.stdout.flush()
 
-    def connect(self, autoreset=False, resetcmd=False):
+    def connect(self, autoreset=False, resetcmd=False, resetpin=False):
         """Connect to MCU and initialize communication.
 
         Set up serial port, send sync sequence and get part info.
         """
 
         self.ser = serial.Serial(port=self.port, parity=self.PARITY)
         # set baudrate separately to work around a bug with the CH340 driver
@@ -290,15 +306,15 @@
         self.ser.timeout = 0.5
         self.ser.interCharTimeout = 0.5
 
         # avoid glitches if there is something in the input buffer
         self.ser.flushInput()
 
         if autoreset:
-            self.reset_device(resetcmd)
+            self.reset_device(resetcmd, resetpin)
         else:
             print("Waiting for MCU, please cycle power: ", end="")
             sys.stdout.flush()
 
         # send sync, and wait for MCU response
         # ignore errors until we see a valid response
         self.status_packet = None
@@ -370,30 +386,35 @@
 
         protocol_database = [("stc89", r"STC(89|90)(C|LE)\d"),
                              ("stc12a", r"STC12(C|LE)\d052"),
                              ("stc12b", r"STC12(C|LE)(52|56)"),
                              ("stc12", r"(STC|IAP)(10|11|12)\D"),
                              ("stc15a", r"(STC|IAP)15[FL][012]0\d(E|EA|)$"),
                              ("stc15", r"(STC|IAP|IRC)15\D"),
-                             ("stc8", r"(STC|IAP|IRC)8")]
+                             ("stc8d", r"STC8H(3|4|8)K"),
+                             ("stc8d", r"STC32"),
+                             ("stc8d", r"STC8A8K\d\dD4"),
+                             ("stc8g", r"STC8H"),
+                             ("stc8g", r"STC8G"),
+                             ("stc8", r"STC8\D")]
 
         for protocol_name, pattern in protocol_database:
             if re.match(pattern, self.model.name):
                 self.protocol_name = protocol_name
                 break
         else:
             self.protocol_name = None
 
     def initialize_options(self, status_packet):
         raise NotImplementedError
 
     def initialize_status(self, status_packet):
         raise NotImplementedError
 
-    def write_packet(self, packet_data):
+    def write_packet(self, packet_data, epilogue_len = 0):
         raise NotImplementedError
 
 
 class Stc89Protocol(StcBaseProtocol):
     """Protocol handler for STC 89/90 series"""
 
     PARITY = serial.PARITY_NONE
@@ -415,15 +436,15 @@
         if packet_csum != calc_csum:
             self.dump_packet(packet)
             raise StcFramingException("packet checksum mismatch")
 
         payload = StcBaseProtocol.extract_payload(self, packet)
         return payload[:-1]
 
-    def write_packet(self, packet_data):
+    def write_packet(self, packet_data, epilogue_len = 0):
         """Send packet to MCU.
 
         Constructs a packet with supplied payload and sends it to the MCU.
         """
 
         # frame start and direction magic
         packet = bytes()
@@ -516,29 +537,29 @@
         brt, brt_csum, iap, delay = self.calculate_baud()
         print("checking ", end="")
         sys.stdout.flush()
         packet = bytes([0x8f])
         packet += struct.pack(">H", brt)
         packet += bytes([0xff - (brt >> 8), brt_csum, delay, iap])
         self.write_packet(packet)
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
         response = self.read_packet()
         self.ser.baudrate = self.baud_handshake
         if response[0] != 0x8f:
             raise StcProtocolException("incorrect magic in handshake packet")
 
         # switch to baudrate
         print("setting ", end="")
         sys.stdout.flush()
         packet = bytes([0x8e])
         packet += struct.pack(">H", brt)
         packet += bytes([0xff - (brt >> 8), brt_csum, delay])
         self.write_packet(packet)
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
         response = self.read_packet()
         if response[0] != 0x8e:
             raise StcProtocolException("incorrect magic in handshake packet")
 
         # ping-pong test
         print("testing ", end="")
@@ -603,14 +624,247 @@
         self.write_packet(packet)
         response = self.read_packet()
         if response[0] != 0x8d:
             raise StcProtocolException("incorrect magic in option packet")
         print("done")
 
 
+class Stc89AProtocol(StcBaseProtocol):
+    """Protocol handler for STC 89/90 series"""
+
+    PARITY = serial.PARITY_NONE
+    """Parity configuration - these don't use any parity"""
+
+    PROGRAM_BLOCKSIZE = 128
+    """block size for programming flash"""
+
+    def __init__(self, port, baud_handshake, baud_transfer):
+        StcBaseProtocol.__init__(self, port, baud_handshake, baud_transfer)
+
+        self.cpu_6t = None
+
+    def extract_payload(self, packet):
+        """Verify the checksum of packet and return its payload"""
+
+        packet_csum = packet[-2] + (packet[-3] << 8)
+        calc_csum = sum(packet[2:-3]) & 0xffff
+        if packet_csum != calc_csum:
+            self.dump_packet(packet)
+            raise StcFramingException("packet checksum mismatch")
+
+        payload = StcBaseProtocol.extract_payload(self, packet)
+        return payload[:-1]
+
+    def write_packet(self, packet_data):
+        """Send packet to MCU.
+
+        Constructs a packet with supplied payload and sends it to the MCU.
+        """
+
+        # frame start and direction magic
+        packet = bytes()
+        packet += self.PACKET_START
+        packet += self.PACKET_HOST
+
+        # packet length and payload
+        packet += struct.pack(">H", len(packet_data) + 6)
+        packet += packet_data
+
+        # checksum and end code
+        packet += struct.pack(">H", sum(packet[2:]) & 0xffff)
+        packet += self.PACKET_END
+
+        self.dump_packet(packet, receive=False)
+        self.ser.write(packet)
+        self.ser.flush()
+
+    def get_status_packet(self):
+        """Read and decode status packet"""
+
+        status_packet = self.read_packet()
+        if status_packet[0] != 0x50:
+            raise StcProtocolException("incorrect magic in status packet" + str(status_packet[0]))
+        return status_packet
+
+    def initialize_options(self, status_packet):
+        """Initialize options"""
+
+        if len(status_packet) < 20:
+            raise StcProtocolException("invalid options in status packet")
+        self.options = Stc89Option(status_packet[1])
+        self.options.print()
+
+        self.ser.parity = "E"
+
+    def calculate_baud(self):
+        """Calculate MCU baudrate setting.
+
+        Calculate appropriate baudrate settings for the MCU's UART,
+        according to clock frequency and requested baud rate.
+        """
+
+        # timing is different in 6T mode
+        sample_rate = 32 #if self.cpu_6t else 32
+        # baudrate is directly controlled by programming the MCU's BRT register
+        brt = 65536 - round((self.mcu_clock_hz) / (self.baud_transfer * sample_rate))
+        
+        baud_actual = (self.mcu_clock_hz) / (sample_rate * (65536 - brt))
+        baud_error = (abs(self.baud_transfer - baud_actual) * 100.0) / self.baud_transfer
+        if baud_error > 5.0:
+            print("WARNING: baudrate error is %.2f%%. You may need to set a slower rate." %
+                  baud_error, file=sys.stderr)
+
+        # IAP wait states (according to datasheet(s))
+        iap_wait = 0x80
+        if self.mcu_clock_hz < 10E6: iap_wait = 0x83
+        elif self.mcu_clock_hz < 30E6: iap_wait = 0x82
+        elif self.mcu_clock_hz < 50E6: iap_wait = 0x81
+
+        # MCU delay after switching baud rates
+        delay = 0xa0
+
+        return brt, iap_wait
+
+    def initialize_status(self, status_packet):
+        """Decode status packet and store basic MCU info"""
+
+        self.cpu_6t = not bool(status_packet[1] & 1)
+
+        freq_counter = struct.unpack(">H", status_packet[13:15])[0]
+        self.mcu_clock_hz = (12 * freq_counter * self.baud_handshake)
+
+        bl_version, bl_stepping = struct.unpack("BB", status_packet[17:19])
+        bl_minor = status_packet[22] & 0x0f
+        self.mcu_bsl_version = "%d.%d.%d%s" % (bl_version >> 4, bl_version & 0x0f,
+                                               bl_minor, chr(bl_stepping))
+
+    def handshake(self):
+        """Switch to transfer baudrate
+
+        Switches to transfer baudrate and verifies that the setting works with
+        a ping-pong exchange of packets."""
+
+        # check new baudrate
+        print("Switching to %d baud: " % self.baud_transfer, end="")
+        sys.stdout.flush()
+        brt,iap = self.calculate_baud()
+        print("checking ", end="")
+        sys.stdout.flush()
+        packet = bytes([0x01])
+        packet += struct.pack(">H", brt)
+        packet += bytes([iap])
+        self.write_packet(packet)
+        time.sleep(0.2)
+        print(self.baud_transfer)
+        response = self.read_packet()
+        
+        if response[0] != 0x01:
+            raise StcProtocolException("incorrect magic in handshake packet")
+
+        self.ser.baudrate = self.baud_transfer
+
+        # ping-pong test
+        print("testing ", end="")
+        sys.stdout.flush()
+        packet = bytes([0x05, 0x00, 0x00, 0x46, 0xB9])
+        self.write_packet(packet)
+        response = self.read_packet()
+        if response[0] != 0x05:
+            raise StcProtocolException("incorrect magic in handshake packet")
+
+        print("done")
+
+    def reset_device(self, resetcmd=False):
+        if not resetcmd:
+            print("Cycling power: ", end="")
+            sys.stdout.flush()
+            self.ser.setDTR(False)
+            time.sleep(0.5)
+            self.ser.setDTR(True)
+            print("done")
+        else:
+            print("Cycling power via shell cmd: " + resetcmd)
+            os.system(resetcmd)
+
+        print("Waiting for MCU: ", end="")
+        sys.stdout.flush()
+
+    def erase_flash(self, erase_size, _):
+        """Erase the MCU's flash memory.
+
+        Erase the flash memory with a block-erase command.
+        flash_size is ignored; not used on STC 89 series.
+        """
+
+        print("Erasing All blocks: ", end="")
+        sys.stdout.flush()
+        packet = bytes([0x03, 0x00, 0x00, 0x46, 0xB9])
+        self.write_packet(packet)
+        response = self.read_packet()
+        if response[0] != 0x03:
+            raise StcProtocolException("incorrect magic in erase packet")
+
+        print("MCU ID: {:x}{:x}{:x}{:x}{:x}{:x}{:x}".format(response[1],response[2],response[3]
+        ,response[4],response[5],response[6],response[7]))
+
+        print("done")
+
+    def program_flash(self, data):
+        """Program the MCU's flash memory.
+
+        Write data into flash memory, using the PROGRAM_BLOCKSIZE
+        as the block size (depends on MCU's RAM size).
+        """
+        p = 0
+
+        for i in range(0, len(data), self.PROGRAM_BLOCKSIZE):
+            packet = bytes(3)
+            if p == 0:
+                packet = bytes([0x22,0x00,0x00])
+            else:
+                packet = bytes([0x02])
+                packet += int(128 * p).to_bytes(length=2, byteorder='big', signed=True)
+
+            
+            p = p + 1
+            packet += bytes([0x46, 0xB9])
+            packet += data[i:i+self.PROGRAM_BLOCKSIZE]
+            
+            self.write_packet(packet)
+
+            response = self.read_packet()
+            if len(response) < 1 or response[0] != 0x02:
+                raise StcProtocolException("incorrect magic in write packet")
+
+            self.progress_cb(i, self.PROGRAM_BLOCKSIZE, len(data))
+        self.progress_cb(len(data), self.PROGRAM_BLOCKSIZE, len(data))
+
+    def program_options(self):
+        """Program option byte into flash"""
+
+        print("Setting options: ")
+        sys.stdout.flush()
+        msr = self.options.get_msr()
+        packet = bytes([0x04,0x00,0x00,0x46,0xB9, msr])
+        self.write_packet(packet)
+        response = self.read_packet()
+        if response[0] != 0x04:
+            raise StcProtocolException("incorrect magic in option packet")
+        print("done")
+    
+    def disconnect(self):
+        """Disconnect from MCU"""
+
+        # reset mcu
+        packet = bytes([0xFF])
+        self.write_packet(packet)
+        self.ser.close()
+        print("Disconnected!")
+
+
 class Stc12AOptionsMixIn:
     def program_options(self):
         print("Setting options: ", end="")
         sys.stdout.flush()
         msr = self.options.get_msr()
         packet = bytes([0x8d, msr[0], msr[1], msr[2], 0xff, msr[3]])
         packet += struct.pack(">I", int(self.mcu_clock_hz))
@@ -706,27 +960,27 @@
         print("Switching to %d baud: " % self.baud_transfer, end="")
         sys.stdout.flush()
         brt, brt_csum, iap, delay = self.calculate_baud()
         print("checking ", end="")
         sys.stdout.flush()
         packet = bytes([0x8f, 0xc0, brt, 0x3f, brt_csum, delay, iap])
         self.write_packet(packet)
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
         response = self.read_packet()
         self.ser.baudrate = self.baud_handshake
         if response[0] != 0x8f:
             raise StcProtocolException("incorrect magic in handshake packet")
 
         # switch to the settings
         print("setting ", end="")
         sys.stdout.flush()
         packet = bytes([0x8e, 0xc0, brt, 0x3f, brt_csum, delay])
         self.write_packet(packet)
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
         response = self.read_packet()
         if response[0] != 0x8e:
             raise StcProtocolException("incorrect magic in handshake packet")
 
         # ping-pong test
         print("testing ", end="")
@@ -810,15 +1064,15 @@
         if packet_csum != calc_csum:
             self.dump_packet(packet)
             raise StcFramingException("packet checksum mismatch")
 
         payload = StcBaseProtocol.extract_payload(self, packet)
         return payload[:-2]
 
-    def write_packet(self, packet_data):
+    def write_packet(self, packet_data, epilogue_len = 0):
         """Send packet to MCU.
 
         Constructs a packet with supplied payload and sends it to the MCU.
         """
 
         # frame start and direction magic
         packet = bytes()
@@ -828,14 +1082,19 @@
         # packet length and payload
         packet += struct.pack(">H", len(packet_data) + 6)
         packet += packet_data
 
         # checksum and end code
         packet += struct.pack(">H", sum(packet[2:]) & 0xffff)
         packet += self.PACKET_END
+        
+        i = 0
+        while i < epilogue_len:
+            packet += bytes([0x66])
+            i += 1
 
         self.dump_packet(packet, receive=False)
         self.ser.write(packet)
         self.ser.flush()
 
     def initialize_status(self, status_packet):
         """Decode status packet and store basic MCU info"""
@@ -906,27 +1165,27 @@
             raise StcProtocolException("incorrect magic in handshake packet")
 
         # test new settings
         print("testing ", end="")
         sys.stdout.flush()
         packet = bytes([0x8f, 0xc0, brt, 0x3f, brt_csum, delay, iap])
         self.write_packet(packet)
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
         response = self.read_packet()
         self.ser.baudrate = self.baud_handshake
         if response[0] != 0x8f:
             raise StcProtocolException("incorrect magic in handshake packet")
 
         # switch to the settings
         print("setting ", end="")
         sys.stdout.flush()
         packet = bytes([0x8e, 0xc0, brt, 0x3f, brt_csum, delay])
         self.write_packet(packet)
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
         response = self.read_packet()
         if response[0] != 0x84:
             raise StcProtocolException("incorrect magic in handshake packet")
 
         print("done")
 
@@ -1200,15 +1459,15 @@
         sys.stdout.flush()
         iap_wait = self.get_iap_delay(program_speed)
         packet = bytes([0x8e])
         packet += struct.pack(">H", program_trim)
         packet += struct.pack(">B", 230400 // self.baud_transfer)
         packet += bytes([0xa1, 0x64, 0xb8, 0x00, iap_wait, 0x20, 0xff, 0x00])
         self.write_packet(packet)
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
         response = self.read_packet()
         if response[0] != 0x84:
             raise StcProtocolException("incorrect magic in handshake packet")
         print("done")
 
     def program_options(self):
@@ -1390,41 +1649,47 @@
         sys.stdout.flush()
         packet = bytes([0x01])
         packet += bytes(prog_trim)
         # XXX: baud rate calculation is different between MCUs with and without
         # hardware UART. Only one family of models seems to lack a hardware
         # UART, and we can isolate those with a check on the magic.
         # This is a bit of a hack, but it works.
-        bauds = self.baud_transfer if (self.mcu_magic >> 8) == 0xf2 else self.baud_transfer * 4
-        packet += struct.pack(">H", int(65535 - program_speed / bauds))
-        packet += bytes(user_trim)
+        if (self.mcu_magic >> 8) == 0xf2:
+            packet += struct.pack(">H", int(65536 - program_speed / self.baud_transfer))
+            packet += struct.pack(">H", int(65536 - program_speed / 2 * 3 / self.baud_transfer))
+        else:
+            packet += struct.pack(">H", int(65536 - program_speed / (self.baud_transfer * 4)))
+            packet += bytes(reversed(user_trim))
         iap_wait = self.get_iap_delay(program_speed)
         packet += bytes([iap_wait])
         self.write_packet(packet)
         response = self.read_packet()
         if len(response) < 1 or response[0] != 0x01:
             raise StcProtocolException("incorrect magic in handshake packet")
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
 
     def switch_baud_ext(self):
         """Switch baudrate using external clock source"""
 
         print("Switching to %d baud: " % self.baud_transfer, end="")
         sys.stdout.flush()
         packet = bytes([0x01])
         packet += bytes([self.freq_count_24, 0x40])
-        packet += struct.pack(">H", int(65535 - self.mcu_clock_hz / self.baud_transfer / 4))
+        bauds = int(65536 - self.mcu_clock_hz / self.baud_transfer / 4)
+        if bauds >= 65536:
+            raise StcProtocolException("baudrate adjustment failed")
+        packet += struct.pack(">H", bauds)
         iap_wait = self.get_iap_delay(self.mcu_clock_hz)
         packet += bytes([0x00, 0x00, iap_wait])
         self.write_packet(packet)
         response = self.read_packet()
         if len(response) < 1 or response[0] != 0x01:
             raise StcProtocolException("incorrect magic in handshake packet")
-        time.sleep(0.2)
+        time.sleep(0.1)
         self.ser.baudrate = self.baud_transfer
 
         # for switching back to RC, program factory values
         self.trim_value = (self.freq_count_24, 0x40)
         self.trim_frequency = int(24E6)
 
     def handshake(self):
@@ -1454,19 +1719,23 @@
     def erase_flash(self, erase_size, flash_size):
         """Erase the MCU's flash memory.
 
         Erase the flash memory with a block-erase command.
         Note that this protocol always seems to erase everything.
         """
 
-        # XXX: how does partial erase work?
-
         print("Erasing flash: ", end="")
         sys.stdout.flush()
-        packet = bytes([0x03, 0x00])
+        packet = bytes([0x03])
+        if erase_size <= flash_size:
+           # erase flash only
+           packet += bytes([0x00])
+        else:
+           # erase flash and eeprom
+           packet += bytes([0x01])
         if self.bsl_version >= 0x72:
             packet += bytes([0x00, 0x5a, 0xa5])
         self.write_packet(packet)
         response = self.read_packet()
         if len(response) < 1 or response[0] != 0x03:
             raise StcProtocolException("incorrect magic in handshake packet")
         print("done")
@@ -1544,14 +1813,179 @@
         if len(response) < 2 or response[0] != 0x04 or response[1] != 0x54:
             raise StcProtocolException("incorrect magic in option packet")
         print("done")
 
         print("Target UID: %s" % Utils.hexstr(self.uid))
 
 
+class StcUsb15Protocol(Stc15Protocol):
+    """USB should use large blocks"""
+    PROGRAM_BLOCKSIZE = 128
+
+    """VID of STC devices"""
+    USB_VID = 0x5354
+
+    """PID of STC devices"""
+    USB_PID = 0x4312
+
+    def __init__(self):
+        # XXX: this is really ugly!
+        Stc15Protocol.__init__(self, "", 0, 0, 0)
+        self.dev = None
+
+    def dump_packet(self, data, request=0, value=0, index=0, receive=True):
+        if self.debug:
+            print("%s bRequest=%02X wValue=%04X wIndex=%04X data: %s" %
+                  (("<-" if receive else "->"), request, value, index,
+                   Utils.hexstr(data, " ")), file=sys.stderr)
+
+    def read_packet(self):
+        """Read a packet from the MCU"""
+
+        dev2host = usb.util.CTRL_TYPE_VENDOR | usb.util.CTRL_RECIPIENT_DEVICE | usb.util.CTRL_IN
+        packet = self.dev.ctrl_transfer(dev2host, 0, 0, 0, 132).tobytes()
+        if len(packet) < 5 or packet[0] != 0x46 or packet[1] != 0xb9:
+            self.dump_packet(packet)
+            raise StcFramingException("incorrect frame start")
+
+        data_len = packet[2]
+        if (data_len) > len(packet) + 3:
+            self.dump_packet(packet)
+            raise StcFramingException("frame length mismatch")
+
+        data = packet[2:-1]
+        csum = functools.reduce(lambda x, y: x - y, data, 0) & 0xff
+        if csum != packet[-1]:
+            self.dump_packet(packet)
+            raise StcFramingException("frame checksum mismatch")
+
+        self.dump_packet(packet, receive=True)
+        return packet[3:3+data_len]
+
+    def write_packet(self, request, value=0, index=0, data=bytes([0])):
+        """Write USB control packet"""
+
+        # Control transfers are maximum of 8 bytes each, and every
+        # invidual partial transfer is checksummed individually.
+        i = 0
+        chunks = bytes()
+        while i < len(data):
+            c = data[i:i+7]
+            csum = functools.reduce(lambda x, y: x - y, c, 0) & 0xff
+            chunks += c + bytes([csum])
+            i += 7
+
+        self.dump_packet(chunks, request, value, index, receive=False)
+        host2dev = usb.util.CTRL_TYPE_VENDOR | usb.util.CTRL_RECIPIENT_DEVICE | usb.util.CTRL_OUT
+        self.dev.ctrl_transfer(host2dev, request, value, index, chunks)
+
+    def connect(self, autoreset=False, resetcmd=False, resetpin=False):
+        """Connect to USB device and read info packet"""
+
+        # USB support is optional. Provide an error if pyusb is not available.
+        if not _usb_available:
+            raise StcProtocolException(
+                "USB support not available. " +
+                "pyusb is not installed or not working correctly.")
+
+        print("Waiting for MCU, please cycle power: ", end="")
+        sys.stdout.flush()
+
+        self.status_packet = None
+        while not self.status_packet:
+            try:
+                self.dev = usb.core.find(idVendor=self.USB_VID, idProduct=self.USB_PID)
+                if self.dev:
+                    self.dev.set_configuration()
+                    self.status_packet = self.read_packet()
+                    if len(self.status_packet) < 38:
+                        self.status_packet = None
+                        raise StcFramingException
+                else: raise StcFramingException
+            except StcFramingException:
+                time.sleep(0.5)
+            except usb.core.USBError as err:
+                if err.errno == errno.EACCES:
+                    raise IOError(err.strerror)
+
+        self.initialize_model()
+        print("done")
+
+    def handshake(self):
+        print("Initializing: ", end="")
+        sys.stdout.flush()
+
+        # handshake
+        self.write_packet(0x01, 0, 0, bytes([0x03]))
+        response = self.read_packet()
+        if response[0] != 0x01:
+            raise StcProtocolException("incorrect magic in handshake packet")
+
+        # enable/unlock MCU
+        self.write_packet(0x05, 0xa55a, 0)
+        response = self.read_packet()
+        if response[0] == 0x0f:
+            raise StcProtocolException("MCU is locked")
+        if response[0] != 0x05:
+            raise StcProtocolException("incorrect magic in handshake packet")
+
+        print("done")
+
+    def erase_flash(self, code, eeprom):
+        print("Erasing flash: ", end="")
+        sys.stdout.flush()
+        self.write_packet(0x03, 0xa55a, 0)
+        # XXX: better way to detect MCU has finished
+        time.sleep(2)
+        packet = self.read_packet()
+        if packet[0] != 0x03:
+            raise StcProtocolException("incorrect magic in erase packet")
+        self.uid = packet[1:8]
+        print("done")
+
+    def program_flash(self, data):
+        """Program the MCU's flash memory."""
+
+        for i in range(0, len(data), self.PROGRAM_BLOCKSIZE):
+            packet = data[i:i+self.PROGRAM_BLOCKSIZE]
+            while len(packet) < self.PROGRAM_BLOCKSIZE: packet += b"\x00"
+            self.write_packet(0x22 if i == 0 else 0x02, 0xa55a, i, packet)
+            # XXX: better way to detect MCU has finished
+            time.sleep(0.1)
+            response = self.read_packet()
+            if response[0] != 0x02 or response[1] != 0x54:
+                raise StcProtocolException("incorrect magic in write packet")
+            self.progress_cb(i, self.PROGRAM_BLOCKSIZE, len(data))
+        self.progress_cb(len(data), self.PROGRAM_BLOCKSIZE, len(data))
+
+    def program_options(self):
+        print("Setting options: ", end="")
+        sys.stdout.flush()
+
+        # always use 24 MHz pre-tuned value for now
+        self.trim_value = (self.freq_count_24, 0x40)
+        self.trim_frequency = int(24E6)
+
+        packet = self.build_options()
+        self.write_packet(0x04, 0xa55a, 0, packet)
+        # XXX: better way to detect MCU has finished
+        time.sleep(0.5)
+        response = self.read_packet()
+        if response[0] != 0x04 or response[1] != 0x54:
+            raise StcProtocolException("incorrect magic in option packet")
+        print("done")
+
+        print("Target UID: %s" % Utils.hexstr(self.uid))
+
+    def disconnect(self):
+        if self.dev:
+            self.write_packet(0xff)
+            print("Disconnected!")
+
+
 class Stc8Protocol(Stc15Protocol):
     """Protocol handler for STC8 series"""
 
     def __init__(self, port, handshake, baud, trim):
         Stc15Protocol.__init__(self, port, handshake, baud, trim)
         self.trim_divider = None
         self.reference_voltage = None
@@ -1596,14 +2030,17 @@
 
     def print_mcu_info(self):
         """Print additional STC8 info"""
         super().print_mcu_info()
         print("Target ref. voltage: %d mV" % self.reference_voltage)
         print("Target mfg. date: %04d-%02d-%02d" % self.mfg_date)
 
+    def set_option(self, name, value):
+        super().set_option(name, value)
+
     def calibrate(self):
         """Calibrate selected user frequency frequency and switch to selected baudrate."""
 
         # handle uncalibrated chips
         if self.mcu_clock_hz == 0 and self.trim_frequency <= 0:
             raise StcProtocolException("uncalibrated, please provide a trim value")
 
@@ -1660,15 +2097,15 @@
         print("%.03f MHz" % (self.trim_frequency / 1E6))
 
         # switch to programming frequency
         print("Switching to %d baud: " % self.baud_transfer, end="")
         sys.stdout.flush()
         packet = bytes([0x01, 0x00, 0x00])
         bauds = self.baud_transfer * 4
-        packet += struct.pack(">H", round(65535 - 24E6 / bauds))
+        packet += struct.pack(">H", round(65536 - 24E6 / bauds))
         packet += bytes([user_trim[1], user_trim[0]])
         iap_wait = self.get_iap_delay(24E6)
         packet += bytes([iap_wait])
         self.write_packet(packet)
         response = self.read_packet()
         if len(response) < 1 or response[0] != 0x01:
             raise StcProtocolException("incorrect magic in handshake packet")
@@ -1694,170 +2131,248 @@
 
         # reset mcu
         packet = bytes([0xff])
         self.write_packet(packet)
         self.ser.close()
         print("Disconnected!")
 
-class StcUsb15Protocol(Stc15Protocol):
-    """USB should use large blocks"""
-    PROGRAM_BLOCKSIZE = 128
 
-    """VID of STC devices"""
-    USB_VID = 0x5354
+class Stc8dProtocol(Stc8Protocol):
+    """Protocol handler for STC8A8K64D4 series"""
 
-    """PID of STC devices"""
-    USB_PID = 0x4312
-
-    def __init__(self):
-        # XXX: this is really ugly!
-        Stc15Protocol.__init__(self, "", 0, 0, 0)
-        self.dev = None
-
-    def dump_packet(self, data, request=0, value=0, index=0, receive=True):
-        if self.debug:
-            print("%s bRequest=%02X wValue=%04X wIndex=%04X data: %s" %
-                  (("<-" if receive else "->"), request, value, index,
-                   Utils.hexstr(data, " ")), file=sys.stderr)
-
-    def read_packet(self):
-        """Read a packet from the MCU"""
+    def __init__(self, port, handshake, baud, trim):
+        Stc8Protocol.__init__(self, port, handshake, baud, trim)
 
-        dev2host = usb.util.CTRL_TYPE_VENDOR | usb.util.CTRL_RECIPIENT_DEVICE | usb.util.CTRL_IN
-        packet = self.dev.ctrl_transfer(dev2host, 0, 0, 0, 132).tobytes()
-        if len(packet) < 5 or packet[0] != 0x46 or packet[1] != 0xb9:
-            self.dump_packet(packet)
-            raise StcFramingException("incorrect frame start")
+    def set_option(self, name, value):
+        super().set_option(name, value)
+        if name == 'program_eeprom_split':
+            split_point = Utils.to_int(value);
+
+            if self.model.mcs251:
+                """Minimum size is 1K in STC-ISP"""
+                if split_point == 0 and self.model.iap:
+                    split_point = 0x400;
+
+                # CODE starts at 0xFF0000
+                self.split_code = 0x10000;
+                # EEPROM starts at 0xFE0000
+                self.split_eeprom = split_point;
+            else:
+                if split_point == 0 and self.model.iap:
+                    split_point = self.model.code;
 
-        data_len = packet[2]
-        if (data_len) > len(packet) + 3:
-            self.dump_packet(packet)
-            raise StcFramingException("frame length mismatch")
+                self.split_code = split_point;
+                self.split_eeprom = self.model.total - self.split_code;
 
-        data = packet[2:-1]
-        csum = functools.reduce(lambda x, y: x - y, data, 0) & 0xff
-        if csum != packet[-1]:
-            self.dump_packet(packet)
-            raise StcFramingException("frame checksum mismatch")
+    def choose_range(self, packet, response, target_count):
+        """Choose appropriate trim value mean for next round from challenge
+        responses."""
 
-        self.dump_packet(packet, receive=True)
-        return packet[3:3+data_len]
 
-    def write_packet(self, request, value=0, index=0, data=bytes([0])):
-        """Write USB control packet"""
+        challenge_data = packet[2:]
+        calib_data = response[2:]
+        calib_len = response[1]
+        if len(calib_data) < 2 * calib_len:
+            raise StcProtocolException("range calibration data missing")
+        for i in range(calib_len >> 1):
+            count_a, count_b = struct.unpack(
+                ">HH", calib_data[4 * i: 4 * i + 4])
+            trim_a, trim_b, trim_range = struct.unpack(
+                ">BxBB", challenge_data[4 * i:4 * i + 4])
+            if ((count_a <= target_count and count_b >= target_count)):
+                target_trim = round(
+                    (target_count - count_a) * (trim_b - trim_a) / (count_b - count_a) + trim_a)
+                # target_trim will be set at the center of packet in the 2nd calibration
+                if target_trim < 6 or target_trim > 255 - 5:
+                    raise StcProtocolException("frequency trimming failed")
+                return (target_trim, trim_range)
+        return None
 
-        # Control transfers are maximum of 8 bytes each, and every
-        # invidual partial transfer is checksummed individually.
-        i = 0
-        chunks = bytes()
-        while i < len(data):
-            c = data[i:i+7]
-            csum = functools.reduce(lambda x, y: x - y, c, 0) & 0xff
-            chunks += c + bytes([csum])
-            i += 7
+    def choose_trim(self, packet, response, target_count):
+        """Choose best trim for given target count from challenge
+        responses."""
+        calib_data = response[2:]
+        challenge_data = packet[2:]
+        calib_len = response[1]
+        if len(calib_data) < 2 * calib_len:
+            raise StcProtocolException("trim calibration data missing")
+        best = None
+        best_count = sys.maxsize
+        for i in range(calib_len):
+            count, = struct.unpack(">H", calib_data[2 * i: 2 * i + 2])
+            trim_adj, trim_range = struct.unpack(
+                ">BB", challenge_data[2 * i: 2 * i + 2])
+            if abs(count - target_count) < best_count:
+                best_count = abs(count - target_count)
+                best = (trim_adj, trim_range), count
+        if not best:
+            raise StcProtocolException("frequency trimming failed")
+        return best
 
-        self.dump_packet(chunks, request, value, index, receive=False)
-        host2dev = usb.util.CTRL_TYPE_VENDOR | usb.util.CTRL_RECIPIENT_DEVICE | usb.util.CTRL_OUT
-        self.dev.ctrl_transfer(host2dev, request, value, index, chunks)
 
-    def connect(self, autoreset=False, resetcmd=False):
-        """Connect to USB device and read info packet"""
+    def calibrate(self):
+        """Calibrate selected user frequency frequency and switch to selected baudrate."""
 
-        # USB support is optional. Provide an error if pyusb is not available.
-        if not _usb_available:
+        # handle uncalibrated chips
+        if self.mcu_clock_hz == 0 and self.trim_frequency <= 0:
             raise StcProtocolException(
-                "USB support not available. " +
-                "pyusb is not installed or not working correctly.")
-
-        print("Waiting for MCU, please cycle power: ", end="")
-        sys.stdout.flush()
+                "uncalibrated, please provide a trim value")
 
-        self.status_packet = None
-        while not self.status_packet:
-            try:
-                self.dev = usb.core.find(idVendor=self.USB_VID, idProduct=self.USB_PID)
-                if self.dev:
-                    self.dev.set_configuration()
-                    self.status_packet = self.read_packet()
-                    if len(self.status_packet) < 38:
-                        self.status_packet = None
-                        raise StcFramingException
-                else: raise StcFramingException
-            except StcFramingException:
-                time.sleep(0.5)
-            except usb.core.USBError as err:
-                if err.errno == errno.EACCES:
-                    raise IOError(err.strerror)
-
-        self.initialize_model()
-        print("done")
+        # determine target counter
+        user_speed = self.trim_frequency
+        if user_speed <= 0:
+            user_speed = self.mcu_clock_hz
+        target_user_count = round(user_speed / self.baud_handshake)
 
-    def handshake(self):
-        print("Initializing: ", end="")
+        # calibration, round 1
+        print("Target frequency: ", end="")
         sys.stdout.flush()
-
-        # handshake
-        self.write_packet(0x01, 0, 0, bytes([0x03]))
+        packet = bytes([0x00, 0x08])
+        packet += bytes([0x00, 0x00, 0xFF, 0x00])
+        packet += bytes([0x00, 0x10, 0xFF, 0x10])
+        packet += bytes([0x00, 0x20, 0xFF, 0x20])
+        packet += bytes([0x00, 0x30, 0xFF, 0x30])
+        self.write_packet(packet)
+        self.pulse(b"\xfe", timeout=1.0)
         response = self.read_packet()
-        if response[0] != 0x01:
+        if len(response) < 2 or response[0] != 0x00:
             raise StcProtocolException("incorrect magic in handshake packet")
 
-        # enable/unlock MCU
-        self.write_packet(0x05, 0xa55a, 0)
+        # select ranges and trim values
+        for divider in range(1, 6):
+            user_trim = self.choose_range(
+                packet, response, target_user_count * divider)
+            if user_trim is not None:
+                self.trim_divider = divider
+                break
+        if user_trim is None:
+            raise StcProtocolException("frequency trimming unsuccessful")
+
+        # calibration, round 2
+        packet = bytes([0x00, 0x0C])
+        for i in range(-6, 6):
+            packet += bytes([user_trim[0] + i, user_trim[1]])
+        self.write_packet(packet)
+        self.pulse(b"\xfe", timeout=1.0)
         response = self.read_packet()
-        if response[0] == 0x0f:
-            raise StcProtocolException("MCU is locked")
-        if response[0] != 0x05:
+        if len(response) < 2 or response[0] != 0x00:
             raise StcProtocolException("incorrect magic in handshake packet")
 
-        print("done")
+        # select final values
+        user_trim, user_count = self.choose_trim(
+            packet, response, target_user_count * self.trim_divider)
+        self.trim_value = user_trim
+        self.trim_frequency = round(
+            user_count * self.baud_handshake/self.trim_divider)
+        print("Target %.03f MHz" % (user_speed / 1E6))
+        print("Adjusted frequency: %.03f MHz(%.03f%%)" % (
+            (self.trim_frequency / 1E6), (self.trim_frequency*100/user_speed-100)))
 
-    def erase_flash(self, code, eeprom):
-        print("Erasing flash: ", end="")
+        # switch to programming frequency
+        print("Switching to %d baud: " % self.baud_transfer, end="")
         sys.stdout.flush()
-        self.write_packet(0x03, 0xa55a, 0)
-        # XXX: better way to detect MCU has finished
-        time.sleep(2)
-        packet = self.read_packet()
-        if packet[0] != 0x03:
-            raise StcProtocolException("incorrect magic in erase packet")
-        self.uid = packet[1:8]
-        print("done")
+        packet = bytes([0x01, 0x00, 0x00])
+        bauds = self.baud_transfer * 4
+        packet += struct.pack(">H", round(65536 - 24E6 / bauds))
+        packet += bytes([user_trim[1], user_trim[0]])
+        # iap_wait = self.get_iap_delay(24E6)
+        iap_wait = 0x98  # iap_wait for "STC8A8K64D4"
+        packet += bytes([iap_wait])
+        self.write_packet(packet)
+        response = self.read_packet()
+        if len(response) < 1 or response[0] != 0x01:
+            raise StcProtocolException("incorrect magic in handshake packet")
+        self.ser.baudrate = self.baud_transfer
 
-    def program_flash(self, data):
-        """Program the MCU's flash memory."""
+    def build_options(self):
+        """Build a packet of option data from the current configuration."""
+        msr = self.options.get_msr()
+        packet = 40 * bytearray([0xff])
+        packet[3] = 0x00
+        packet[6] = 0x00
+        packet[22] = 0x00
+        packet[24:28] = struct.pack(">I", self.trim_frequency)
+        packet[28:30] = self.trim_value
+        packet[30] = self.trim_divider
+        packet[32] = msr[0]
+        packet[36:40] = msr[1:5]
+        return bytes(packet)
 
-        for i in range(0, len(data), self.PROGRAM_BLOCKSIZE):
-            packet = data[i:i+self.PROGRAM_BLOCKSIZE]
-            while len(packet) < self.PROGRAM_BLOCKSIZE: packet += b"\x00"
-            self.write_packet(0x22 if i == 0 else 0x02, 0xa55a, i, packet)
-            # XXX: better way to detect MCU has finished
-            time.sleep(0.1)
-            response = self.read_packet()
-            if response[0] != 0x02 or response[1] != 0x54:
-                raise StcProtocolException("incorrect magic in write packet")
-            self.progress_cb(i, self.PROGRAM_BLOCKSIZE, len(data))
-        self.progress_cb(len(data), self.PROGRAM_BLOCKSIZE, len(data))
 
-    def program_options(self):
-        print("Setting options: ", end="")
+class Stc8gProtocol(Stc8dProtocol):
+    """Protocol handler for STC8G series"""
+
+    def __init__(self, port, handshake, baud, trim):
+        Stc8dProtocol.__init__(self, port, handshake, baud, trim)
+
+    def calibrate(self):
+        """Calibrate selected user frequency frequency and switch to selected baudrate."""
+
+        # handle uncalibrated chips
+        if self.mcu_clock_hz == 0 and self.trim_frequency <= 0:
+            raise StcProtocolException(
+                "uncalibrated, please provide a trim value")
+
+        # determine target counter
+        user_speed = self.trim_frequency
+        if user_speed <= 0:
+            user_speed = self.mcu_clock_hz
+        target_user_count = round(user_speed / self.baud_handshake)
+
+        # calibration, round 1
+        print("Target frequency: ", end="")
         sys.stdout.flush()
+        packet = bytes([0x00, 0x05])
+        packet += bytes([0x00, 0x00, 0x80, 0x00])
+        packet += bytes([0x00, 0x80, 0x80, 0x80])
+        packet += bytes([0xFF, 0x00])
+        self.write_packet(packet, 12)
+        self.pulse(b"\xfe", timeout=1.0)
+        response = self.read_packet()
+        if len(response) < 2 or response[0] != 0x00:
+            raise StcProtocolException("incorrect magic in handshake packet")
 
-        # always use 24 MHz pre-tuned value for now
-        self.trim_value = (self.freq_count_24, 0x40)
-        self.trim_frequency = int(24E6)
+        # select ranges and trim values
+        for divider in range(1, 6):
+            user_trim = self.choose_range(
+                packet, response, target_user_count * divider)
+            if user_trim is not None:
+                self.trim_divider = divider
+                break
+        if user_trim is None:
+            raise StcProtocolException("frequency trimming unsuccessful")
 
-        packet = self.build_options()
-        self.write_packet(0x04, 0xa55a, 0, packet)
-        # XXX: better way to detect MCU has finished
-        time.sleep(0.5)
+        # calibration, round 2
+        packet = bytes([0x00, 0x0C])
+        for i in range(-6, 6):
+            packet += bytes([user_trim[0] + i, user_trim[1]])
+        self.write_packet(packet, 19)
+        self.pulse(b"\xfe", timeout=1.0)
         response = self.read_packet()
-        if response[0] != 0x04 or response[1] != 0x54:
-            raise StcProtocolException("incorrect magic in option packet")
-        print("done")
+        if len(response) < 2 or response[0] != 0x00:
+            raise StcProtocolException("incorrect magic in handshake packet")
 
-        print("Target UID: %s" % Utils.hexstr(self.uid))
+        # select final values
+        user_trim, user_count = self.choose_trim(
+            packet, response, target_user_count * self.trim_divider)
+        self.trim_value = user_trim
+        self.trim_frequency = round(
+            user_count * self.baud_handshake/self.trim_divider)
+        print("Target %.03f MHz" % (user_speed / 1E6))
+        print("Adjusted frequency: %.03f MHz(%.03f%%)" % (
+            (self.trim_frequency / 1E6), (self.trim_frequency*100/user_speed-100)))
 
-    def disconnect(self):
-        if self.dev:
-            self.write_packet(0xff)
-            print("Disconnected!")
+        # switch to programming frequency
+        print("Switching to %d baud: " % self.baud_transfer, end="")
+        sys.stdout.flush()
+        packet = bytes([0x01, 0x00, 0x00])
+        bauds = self.baud_transfer * 4
+        packet += struct.pack(">H", round(65536 - 24E6 / bauds))
+        packet += bytes([user_trim[1], user_trim[0]])
+        # iap_wait = self.get_iap_delay(24E6)
+        iap_wait = 0x98  # iap_wait for "STC8A8K64D4"
+        packet += bytes([iap_wait])
+        self.write_packet(packet)
+        response = self.read_packet()
+        if len(response) < 1 or response[0] != 0x01:
+            raise StcProtocolException("incorrect magic in handshake packet")
+        self.ser.baudrate = self.baud_transfer
```

### Comparing `stcgal-1.6/stcgal/utils.py` & `stcgal-1.8/stcgal/utils.py`

 * *Files identical despite different names*

### Comparing `stcgal-1.6/setup.py` & `stcgal-1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Topic :: Software Development :: Embedded Systems",
         "Topic :: Software Development",
     ],
     test_suite = "tests",
     tests_require = ["PyYAML"],
```

### Comparing `stcgal-1.6/stcgal.egg-info/PKG-INFO` & `stcgal-1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: stcgal
-Version: 1.6
+Version: 1.8
 Summary: STC MCU ISP flash tool
 Home-page: https://github.com/grigorig/stcgal
 Author: Grigori Goronzy
 Author-email: greg@kinoho.net
 License: MIT License
-Description: stcgal - STC MCU ISP flash tool
-        ===============================
-        
-        stcgal is a command line flash programming tool for [STC MCU Ltd](http://stcmcu.com/).
-        8051 compatible microcontrollers.
-        
-        STC microcontrollers have an UART/USB based boot strap loader (BSL). It
-        utilizes a packet-based protocol to flash the code memory and IAP
-        memory over a serial link. This is referred to as in-system programming
-        (ISP).  The BSL is also used to configure various (fuse-like) device
-        options. Unfortunately, this protocol is not publicly documented and
-        STC only provide a (crude) Windows GUI application for programming.
-        
-        stcgal is a full-featured Open Source replacement for STC's Windows
-        software; it supports a wide range of MCUs, it is very portable and
-        suitable for automation.
-        
-        [See the GitHub page for more information](https://github.com/grigorig/stcgal).
 Keywords: stc mcu microcontroller 8051 mcs-51
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: usb
+
+stcgal - STC MCU ISP flash tool
+===============================
+
+stcgal is a command line flash programming tool for [STC MCU Ltd](http://stcmcu.com/).
+8051 compatible microcontrollers.
+
+STC microcontrollers have an UART/USB based boot strap loader (BSL). It
+utilizes a packet-based protocol to flash the code memory and IAP
+memory over a serial link. This is referred to as in-system programming
+(ISP).  The BSL is also used to configure various (fuse-like) device
+options. Unfortunately, this protocol is not publicly documented and
+STC only provide a (crude) Windows GUI application for programming.
+
+stcgal is a full-featured Open Source replacement for STC's Windows
+software; it supports a wide range of MCUs, it is very portable and
+suitable for automation.
+
+[See the GitHub page for more information](https://github.com/grigorig/stcgal).
```

### Comparing `stcgal-1.6/README.md` & `stcgal-1.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-[![Build Status](https://travis-ci.org/grigorig/stcgal.svg)](https://travis-ci.org/grigorig/stcgal)
+[![Build Status](https://github.com/grigorig/stcgal/workflows/Python%20package/badge.svg?branch=master)](https://github.com/grigorig/stcgal/actions?query=workflow%3A%22Python+package%22)
+[![Coverage Status](https://coveralls.io/repos/github/grigorig/stcgal/badge.svg?branch=master)](https://coveralls.io/github/grigorig/stcgal?branch=master)
+[![PyPI version](https://badge.fury.io/py/stcgal.svg)](https://badge.fury.io/py/stcgal)
 
 stcgal - STC MCU ISP flash tool
 ===============================
 
 stcgal is a command line flash programming tool for [STC MCU Ltd](http://stcmcu.com/).
 8051 compatible microcontrollers.
 
@@ -16,26 +18,37 @@
 stcgal is a full-featured Open Source replacement for STC's Windows
 software; it supports a wide range of MCUs, it is very portable and
 suitable for automation.
 
 Features
 --------
 
-* Support for STC 89/90/10/11/12/15/8 series
+* Support for STC 89/90/10/11/12/15/8/32 series
 * UART and USB BSL support
 * Display part info
 * Determine operating frequency
 * Program flash memory
 * Program IAP/EEPROM
 * Set device options
 * Read unique device ID (STC 10/11/12/15/8)
 * Trim RC oscillator frequency (STC 15/8)
 * Automatic power-cycling with DTR toggle or a custom shell command
 * Automatic UART protocol detection
 
+Quickstart
+----------
+
+Install stcgal (might need root/administrator privileges):
+    
+    pip3 install stcgal
+
+Call stcgal and show usage:
+
+    stcgal -h
+
 Further information
 -------------------
 
 [Installation](doc/INSTALL.md)
 
 [How to use stcgal](doc/USAGE.md)
```

### Comparing `stcgal-1.6/PKG-INFO` & `stcgal-1.8/stcgal.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: stcgal
-Version: 1.6
+Version: 1.8
 Summary: STC MCU ISP flash tool
 Home-page: https://github.com/grigorig/stcgal
 Author: Grigori Goronzy
 Author-email: greg@kinoho.net
 License: MIT License
-Description: stcgal - STC MCU ISP flash tool
-        ===============================
-        
-        stcgal is a command line flash programming tool for [STC MCU Ltd](http://stcmcu.com/).
-        8051 compatible microcontrollers.
-        
-        STC microcontrollers have an UART/USB based boot strap loader (BSL). It
-        utilizes a packet-based protocol to flash the code memory and IAP
-        memory over a serial link. This is referred to as in-system programming
-        (ISP).  The BSL is also used to configure various (fuse-like) device
-        options. Unfortunately, this protocol is not publicly documented and
-        STC only provide a (crude) Windows GUI application for programming.
-        
-        stcgal is a full-featured Open Source replacement for STC's Windows
-        software; it supports a wide range of MCUs, it is very portable and
-        suitable for automation.
-        
-        [See the GitHub page for more information](https://github.com/grigorig/stcgal).
 Keywords: stc mcu microcontroller 8051 mcs-51
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: usb
+
+stcgal - STC MCU ISP flash tool
+===============================
+
+stcgal is a command line flash programming tool for [STC MCU Ltd](http://stcmcu.com/).
+8051 compatible microcontrollers.
+
+STC microcontrollers have an UART/USB based boot strap loader (BSL). It
+utilizes a packet-based protocol to flash the code memory and IAP
+memory over a serial link. This is referred to as in-system programming
+(ISP).  The BSL is also used to configure various (fuse-like) device
+options. Unfortunately, this protocol is not publicly documented and
+STC only provide a (crude) Windows GUI application for programming.
+
+stcgal is a full-featured Open Source replacement for STC's Windows
+software; it supports a wide range of MCUs, it is very portable and
+suitable for automation.
+
+[See the GitHub page for more information](https://github.com/grigorig/stcgal).
```

