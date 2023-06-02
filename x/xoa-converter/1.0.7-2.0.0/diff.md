# Comparing `tmp/xoa-converter-1.0.7.tar.gz` & `tmp/xoa-converter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-converter-1.0.7.tar", last modified: Thu Feb 16 09:21:26 2023, max compression
+gzip compressed data, was "xoa-converter-2.0.0.tar", last modified: Fri Jun  2 07:47:13 2023, max compression
```

## Comparing `xoa-converter-1.0.7.tar` & `xoa-converter-2.0.0.tar`

### file list

```diff
@@ -1,81 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:26.708964 xoa-converter-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-02-16 09:21:26.708964 xoa-converter-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-16 09:21:26.708964 xoa-converter-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:26.696964 xoa-converter-1.0.7/xoa_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:26.696964 xoa-converter-1.0.7/xoa_converter/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:26.700964 xoa-converter-1.0.7/xoa_converter/converters/rfc2544/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/rfc2544/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/rfc2544/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/rfc2544/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/rfc2544/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:26.700964 xoa-converter-1.0.7/xoa_converter/converters/rfc2889/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/rfc2889/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/rfc2889/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/rfc2889/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/rfc2889/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:26.708964 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/arp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ecpri.json
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ethernet.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ethernet802.3.json
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/fcoe.json
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/fcoetail.json
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/fiberchannel.json
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/geneve.json
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/grecheck.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/grenocheck.json
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv1.json
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv1l0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv1l1.json
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv2l0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv2l1.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/icmp.json
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/icmpv6.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv1.json
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv2.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv3grouprecord.json
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv3l0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv3l1.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv3memreport.json
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/llc.json
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/macctrl.json
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/macctrlpfc.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/mldv2addressrecord.json
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/mpls.json
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/mpls_tp_oam.json
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/nvgre.json
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/pbb.json
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/pwethctrl.json
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/raw.json
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/roe.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/rtcp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/rtp.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/sctp.json
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/snap.json
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/stp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/tcp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/tcpcheck.json
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/udp.json
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/udpcheck.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/vlan.json
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/converters/segment_refs/vxlan.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-16 09:21:12.000000 xoa-converter-1.0.7/xoa_converter/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:26.696964 xoa-converter-1.0.7/xoa_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-02-16 09:21:26.000000 xoa-converter-1.0.7/xoa_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-02-16 09:21:26.000000 xoa-converter-1.0.7/xoa_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 09:21:26.000000 xoa-converter-1.0.7/xoa_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-16 09:21:26.000000 xoa-converter-1.0.7/xoa_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-16 09:21:26.000000 xoa-converter-1.0.7/xoa_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.773327 xoa-converter-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-02 07:47:13.773327 xoa-converter-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 07:47:13.773327 xoa-converter-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/const_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20257 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.773327 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/arp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ecpri.json
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ethernet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ethernet802.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fcoe.json
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fcoetail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fiberchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/geneve.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/grecheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/grenocheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1l0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1l1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv2l0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv2l1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/icmp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/icmpv6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3grouprecord.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3l0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3l1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3memreport.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/llc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/macctrl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/macctrlpfc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mldv2addressrecord.json
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mpls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mpls_tp_oam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/nvgre.json
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/pbb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/pwethctrl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/roe.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/rtcp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/rtp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/sctp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/snap.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/stp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/tcp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/tcpcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/udp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/udpcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/vlan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/vxlan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/top_level.txt
```

### Comparing `xoa-converter-1.0.7/LICENSE` & `xoa-converter-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/PKG-INFO` & `xoa-converter-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-converter
-Version: 1.0.7
+Version: 2.0.0
 Summary: Xena OpenAutomation test configuration converter let you easily migrate your Valkyrie test suites config files (.v2544, .v2889, .v3918, and .v1564) into XOA.
 Home-page: https://github.com/xenanetworks/open-automation-config-converter
 Author: Frank Chen, Maureen Chen, Artem Constantinov
 Author-email: fch@xenanewtorks.com, mch@xenanetworks.com, aco@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
@@ -20,21 +20,23 @@
 License-File: LICENSE
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-converter) [![PyPI](https://img.shields.io/pypi/v/xoa-converter)](https://pypi.python.org/pypi/xoa-converter) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-config-converter) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-test-config-converter/badge/?version=stable)](https://xena-openautomation-test-config-converter.readthedocs.io/en/stable/?badge=stable)
 # Xena OpenAutomation Test Config Converter
 Xena OpenAutomation (XOA) Test Configuration Converter is a supporting tool for users to quickly migrate their Valkyrie test suite configurations into XOA.
 
 ## Introduction
-Xena's test suite applications have only been for Windows platform for a long time. Moving forward, all of Xena's existing and future test suites will be included in Xena OpenAutomation, which is not limited to Windows anymore. 
+The XOA Test Config Converter is an open-source tool hosted on Xena Networks' GitHub repository. It is designed to help users migrate their existing Valkyrie test suite configurations into the XOA format, enabling a seamless transition to the XOA ecosystem for network automation and testing.
 
-We have developed this test configuration converter and made it into a Python package to help users easily migrate their existing Windows test suite configurations (`.v2544` for [Valkyrie2544](https://xenanetworks.com/product/valkyrie2544/), `.v2889` for [Valkyrie2889](https://xenanetworks.com/product/valkyrie2889/), `.v3918` for [Valkyrie3918](https://xenanetworks.com/product/valkyrie3918/), and `.v1564` for [Valkyrie1564](https://xenanetworks.com/product/valkyrie1564/)) into `XOA`.
+Key features of the XOA Test Config Converter include:
 
-For users of XOA who only uses the web GUI to create, import and run tests, there is no need to use this Python package, because [XOA Core](https://github.com/xenanetworks/open-automation-core) is already using this converter.
+1. Conversion support: The tool supports conversion of Valkyrie test suite configuration files to XOA-compatible format, facilitating the integration of existing test cases into the XOA framework.
 
-This converter is meant for those who want to integrate XOA test suites into their own Python environment without using the web GUI at all.
+2. Ease of use: The XOA Test Config Converter is designed to be user-friendly, with a straightforward process for converting test suite configuration files.
+
+3. Compatibility: The converter ensures that the migrated test suite configurations are compatible with XOA Core and can be executed within the XOA ecosystem.
 
 > The purpose of XOA Converter is ONLY to convert Xena Valkyrie test suit applications' configuration files into XOA's configuration files. Thus only four test suite types are supported by XOA Converter as the source config files. 
 
 ## Documentation
 The user documentation is hosted:
 [Xena OpenAutomation Test Config Converter Documentation](https://docs.xenanetworks.com/projects/xoa-config-converter)
```

### Comparing `xoa-converter-1.0.7/README.md` & `xoa-converter-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-converter) [![PyPI](https://img.shields.io/pypi/v/xoa-converter)](https://pypi.python.org/pypi/xoa-converter) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-config-converter) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-test-config-converter/badge/?version=stable)](https://xena-openautomation-test-config-converter.readthedocs.io/en/stable/?badge=stable)
 # Xena OpenAutomation Test Config Converter
 Xena OpenAutomation (XOA) Test Configuration Converter is a supporting tool for users to quickly migrate their Valkyrie test suite configurations into XOA.
 
 ## Introduction
-Xena's test suite applications have only been for Windows platform for a long time. Moving forward, all of Xena's existing and future test suites will be included in Xena OpenAutomation, which is not limited to Windows anymore. 
+The XOA Test Config Converter is an open-source tool hosted on Xena Networks' GitHub repository. It is designed to help users migrate their existing Valkyrie test suite configurations into the XOA format, enabling a seamless transition to the XOA ecosystem for network automation and testing.
 
-We have developed this test configuration converter and made it into a Python package to help users easily migrate their existing Windows test suite configurations (`.v2544` for [Valkyrie2544](https://xenanetworks.com/product/valkyrie2544/), `.v2889` for [Valkyrie2889](https://xenanetworks.com/product/valkyrie2889/), `.v3918` for [Valkyrie3918](https://xenanetworks.com/product/valkyrie3918/), and `.v1564` for [Valkyrie1564](https://xenanetworks.com/product/valkyrie1564/)) into `XOA`.
+Key features of the XOA Test Config Converter include:
 
-For users of XOA who only uses the web GUI to create, import and run tests, there is no need to use this Python package, because [XOA Core](https://github.com/xenanetworks/open-automation-core) is already using this converter.
+1. Conversion support: The tool supports conversion of Valkyrie test suite configuration files to XOA-compatible format, facilitating the integration of existing test cases into the XOA framework.
 
-This converter is meant for those who want to integrate XOA test suites into their own Python environment without using the web GUI at all.
+2. Ease of use: The XOA Test Config Converter is designed to be user-friendly, with a straightforward process for converting test suite configuration files.
+
+3. Compatibility: The converter ensures that the migrated test suite configurations are compatible with XOA Core and can be executed within the XOA ecosystem.
 
 > The purpose of XOA Converter is ONLY to convert Xena Valkyrie test suit applications' configuration files into XOA's configuration files. Thus only four test suite types are supported by XOA Converter as the source config files. 
 
 ## Documentation
 The user documentation is hosted:
 [Xena OpenAutomation Test Config Converter Documentation](https://docs.xenanetworks.com/projects/xoa-config-converter)
```

### Comparing `xoa-converter-1.0.7/setup.py` & `xoa-converter-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/common.py` & `xoa-converter-2.0.0/xoa_converter/converters/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,46 +6,46 @@
     List,
     Optional,
     Set,
     TYPE_CHECKING,
 )
 from pydantic import BaseModel
 from pydantic.fields import Field
-from operator import attrgetter
 
 if TYPE_CHECKING:
     from xoa_converter.converters.rfc2544.model import (
         LegacyStreamProfileHandler as LegacyStreamProfile2544,
     )
     from types import ModuleType
 
 
 CURRENT_FILE_PARENT_PATH = Path(__file__).parent.resolve()
 SEGMENT_REFS_FOLDER = CURRENT_FILE_PARENT_PATH / "segment_refs"
 
 
+
 class PortIdentity(BaseModel):
     tester_id: str
-    tester_index: int
     module_index: int
     port_index: int
 
     @property
     def name(self) -> str:
-        return f"P-{self.tester_index}-{self.module_index}-{self.port_index}"
+        return f"P-{self.tester_id}-{self.module_index}-{self.port_index}"
 
 
 class TestParameters(BaseModel):
     username: str
-    port_identities: Dict[str, Dict]
-    config: Dict
+    port_identities: List[PortIdentity]
+    config: BaseModel
 
     @property
     def get_testers_ids(self) -> Set[str]:
-        return set(map(attrgetter("tester_id"), self.port_identities.values()))
+        return set(port_idnt.tester_id for port_idnt in self.port_identities)
+
 
 
 class LegacySegmentField(BaseModel):
     name: str = Field(alias="Name")
     bit_length: int = Field(alias="BitLength")
     bit_position: Optional[int] = None  # position of current segment
 
@@ -73,19 +73,19 @@
         SEGMENT_REFS_FOLDER / f"{segment_type_value}.json"
     )
     return segment_ref
 
 
 def convert_protocol_segments(
     stream_profile_handler: "LegacyStreamProfile2544",
-) -> Dict:
-    protocol_segments_profile = {}
+) -> List:
+    protocol_segments_profile = []
 
     for profile in stream_profile_handler.entity_list:
-        header_segments = []
+        segments = []
 
         for hs in profile.stream_config.header_segments:
             hw_modifiers = {}
             field_value_ranges = {}
             for hm in profile.stream_config.hw_modifiers:
                 if hm.segment_id == hs.item_id:
                     hw_modifiers[hm.field_name] = dict(
@@ -123,17 +123,16 @@
                         hw_modifier=hw_modifiers.get(field.name),
                         value_range=field_value_ranges.get(field.name),
                     )
                 )
                 segment_value = segment_value[field.bit_length :]
 
             segment = dict(
-                segment_type=hs.segment_type.name.lower(),
+                type=hs.segment_type.name.lower(),
                 fields=converted_fields,
                 checksum_offset=segment_ref.checksum_offset,
             )
-            header_segments.append(segment)
+            segments.append(segment)
+
+        protocol_segments_profile.append(dict(id=profile.item_id, segments=segments))
 
-        protocol_segments_profile[profile.item_id] = dict(
-            header_segments=header_segments
-        )
     return protocol_segments_profile
```

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/fabric.py` & `xoa-converter-2.0.0/xoa_converter/converters/fabric.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from typing import Any, Type, Protocol, Dict
 from xoa_converter import exceptions
 from xoa_converter import types
 from .rfc2544.adapter import Converter2544
+from .rfc3918.adapter import Converter3918
 from .rfc2889.adapter import Converter2889
 
 
 class XoaConverter(Protocol):
     def __init__(self, source_config: str) -> None: ...
     def gen(self) -> Dict[str, Any]: ...
 
 
 def get_converter(test_suite_type: types.TestSuiteType) -> Type[XoaConverter]:
     """Selecting and returning Converter"""
     if test_suite_type == types.TestSuiteType.RFC2544:
         return Converter2544
+    elif test_suite_type == types.TestSuiteType.RFC3918:
+        return Converter3918
     elif test_suite_type == types.TestSuiteType.RFC2889:
         return Converter2889
     raise exceptions.UnknowConverterType(test_suite_type)
```

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/rfc2544/adapter.py` & `xoa-converter-2.0.0/xoa_converter/converters/rfc2544/adapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
 import hashlib
-from typing import List, Dict, Union, TYPE_CHECKING
+from typing import Union, TYPE_CHECKING
 from .model import LegacyModel2544 as old_model
 from ..common import convert_protocol_segments
 
 if TYPE_CHECKING:
     from .model import (
         LegacyBack2Back,
         LegacyLatency,
@@ -13,308 +14,391 @@
         LegacyPortEntity,
         LegacyThroughput,
     )
 
 
 def convert_base_mac_address(mac_address: str) -> str:
     prefix = [hex(int(i)) for i in mac_address.split(",")]
-    return ":".join([p.replace("0x", "").zfill(2).lower() for p in prefix])
+    return "".join([p.replace("0x", "").zfill(2).upper() for p in prefix]).lower()
 
 
 class Converter2544:
     def __init__(self, source_config: str) -> None:
         self.id_map = {}
         self.data = old_model.parse_raw(source_config)
 
-    def __gen_frame_size(self) -> Dict:
+    def __gen_frame_size(self) -> dict:
         packet_size = self.data.test_options.packet_sizes
         packet_size_type = packet_size.packet_size_type
         fz = packet_size.mixed_length_config.frame_sizes
         return dict(
-            packet_size_type=packet_size_type.name.lower(),
-            custom_packet_sizes=packet_size.custom_packet_sizes,
-            fixed_packet_start_size=packet_size.sw_packet_start_size,
+            custom_packet_sizes=list(packet_size.custom_packet_sizes),
             fixed_packet_end_size=packet_size.sw_packet_end_size,
+            fixed_packet_start_size=packet_size.sw_packet_start_size,
             fixed_packet_step_size=packet_size.sw_packet_step_size,
-            varying_packet_min_size=packet_size.hw_packet_min_size,
-            varying_packet_max_size=packet_size.hw_packet_max_size,
-            mixed_sizes_weights=packet_size.mixed_sizes_weights,
             mixed_length_config=fz,
+            mixed_sizes_weights=packet_size.mixed_sizes_weights,
+            packet_size_type=packet_size_type.name.lower(),
+            varying_packet_max_size=packet_size.hw_packet_max_size,
+            varying_packet_min_size=packet_size.hw_packet_min_size,
         )
 
-    def __gen_multi_stream_config(self) -> Dict:
+    def __gen_multi_stream_config(self) -> dict:
         flow_option = self.data.test_options.flow_creation_options
         return dict(
             enable_multi_stream=flow_option.enable_multi_stream,
-            per_port_stream_count=flow_option.per_port_stream_count,
             multi_stream_address_offset=flow_option.multi_stream_address_offset,
             multi_stream_address_increment=flow_option.multi_stream_address_increment,
             multi_stream_mac_base_address=convert_base_mac_address(
                 flow_option.multi_stream_mac_base_address
             ),
+            per_port_stream_count=flow_option.per_port_stream_count,
         )
 
-    def __gen_port_sync_config(self) -> Dict:
+    def __gen_port_sync_config(self) -> dict:
         test_options = self.data.test_options
-
         return dict(
             delay_after_sync_on_second=test_options.sync_on_duration,
-            toggle_port_sync=test_options.toggle_sync_state,
             sync_off_duration_second=test_options.sync_off_duration,
+            toggle_port_sync=test_options.toggle_sync_state,
         )
 
-    def __gen_test_config(self) -> Dict:
-        test_options = self.data.test_options
-        flow_option = test_options.flow_creation_options
-        payload = test_options.payload_definition
-        learning_options = test_options.learning_options
+    def __gen_topology_config(self) -> dict:
         topology = self.data.test_options.topology_config.topology.lower()
         direction = self.data.test_options.topology_config.direction.name.lower()
-        outer_loop_mode = test_options.outer_loop_mode
-        tid_allocation_scope = self.data.tid_allocation_scope
-        flow_creation_type = flow_option.flow_creation_type
-        port_sync_config = self.__gen_port_sync_config()
+        return dict(direction=direction, topology=topology)
+
+    def __gen_frame_size_config(self) -> dict:
         frame_size = self.__gen_frame_size()
+        flow_option = self.data.test_options.flow_creation_options
+        payload = self.data.test_options.payload_definition
+        return dict(
+            frame_sizes=frame_size,
+            payload_pattern="".join(
+                [
+                    hex(int(i)).replace("0x", "").zfill(2)
+                    for i in payload.payload_pattern.split(",")
+                ]
+            ),
+            payload_type=payload.payload_type.lower(),
+            use_micro_tpld_on_demand=flow_option.use_micro_tpld_on_demand,
+        )
+
+    def __gen_flow_creation_config(self):
+        flow_option = self.data.test_options.flow_creation_options
+        flow_creation_type = flow_option.flow_creation_type
+        tid_allocation_scope = self.data.tid_allocation_scope
         return dict(
             flow_creation_type=flow_creation_type.name.lower(),
-            tid_allocation_scope=tid_allocation_scope.name.lower(),
             mac_base_address=convert_base_mac_address(flow_option.mac_base_address),
+            tid_allocation_scope=tid_allocation_scope.name.lower(),
+        )
+
+    def __gen_port_scheduling_config(self):
+        test_options = self.data.test_options
+        return dict(
             enable_speed_reduction_sweep=test_options.enable_speed_reduct_sweep,
-            use_port_sync_start=test_options.use_port_sync_start,
             port_stagger_steps=test_options.port_stagger_steps,
-            outer_loop_mode=outer_loop_mode.name.lower(),
-            mac_learning_mode=learning_options.mac_learning_mode.name.lower(),
-            mac_learning_frame_count=learning_options.mac_learning_retries,
-            toggle_port_sync_config=port_sync_config,
-            learning_rate_pct=learning_options.learning_rate_percent,
-            learning_duration_second=learning_options.learning_duration,
-            use_flow_based_learning_preamble=learning_options.use_flow_based_learning_preamble,
-            flow_based_learning_frame_count=learning_options.flow_based_learning_frame_count,
-            delay_after_flow_based_learning_ms=learning_options.flow_based_learning_delay,
+            use_port_sync_start=test_options.use_port_sync_start,
+        )
+
+    def __gen_l23_learning_options(self):
+        learning_options = self.data.test_options.learning_options
+        flow_option = self.data.test_options.flow_creation_options
+        return dict(
             arp_refresh_enabled=learning_options.arp_refresh_enabled,
             arp_refresh_period_second=learning_options.arp_refresh_period,
+            learning_duration_second=learning_options.learning_duration,
+            learning_rate_pct=learning_options.learning_rate_percent,
             use_gateway_mac_as_dmac=flow_option.use_gateway_mac_as_dmac,
-            should_stop_on_los=test_options.should_stop_on_los,
+        )
+
+    def __gen_flow_based_learning_options(self):
+        learning_options = self.data.test_options.learning_options
+        return dict(
+            delay_after_flow_based_learning_ms=learning_options.flow_based_learning_delay,
+            flow_based_learning_frame_count=learning_options.flow_based_learning_frame_count,
+            use_flow_based_learning_preamble=learning_options.use_flow_based_learning_preamble,
+        )
+
+    def __gen_mac_learning_options(self):
+        learning_options = self.data.test_options.learning_options
+        return dict(
+            mac_learning_frame_count=learning_options.mac_learning_retries,
+            mac_learning_mode=learning_options.mac_learning_mode.name.lower(),
+            toggle_port_sync_config=self.__gen_port_sync_config(),
+        )
+
+    def __gen_test_execution_config(self):
+        outer_loop_mode = self.data.test_options.outer_loop_mode
+        return dict(
+            flow_based_learning_options=self.__gen_flow_based_learning_options(),
+            flow_creation_config=self.__gen_flow_creation_config(),
+            l23_learning_options=self.__gen_l23_learning_options(),
+            mac_learning_options=self.__gen_mac_learning_options(),
+            outer_loop_mode=outer_loop_mode.name.lower(),
+            port_scheduling_config=self.__gen_port_scheduling_config(),
+            repeat_test_until_stopped=False,
+            reset_error_handling=self.__gen_reset_error_handling(),
+        )
+
+    def __gen_reset_error_handling(self):
+        test_options = self.data.test_options
+        return dict(
             delay_after_port_reset_second=test_options.port_reset_delay,
-            topology=topology,
-            direction=direction,
-            frame_sizes=frame_size,
-            use_micro_tpld_on_demand=flow_option.use_micro_tpld_on_demand,
-            payload_type=payload.payload_type,
-            payload_pattern="".join(
-                [
-                    hex(int(i)).replace("0x", "").zfill(2)
-                    for i in payload.payload_pattern.split(",")
-                ]
-            ),
+            should_stop_on_los=test_options.should_stop_on_los,
+        )
+
+    def __gen_test_config(self):
+        return dict(
+            frame_size_config=self.__gen_frame_size_config(),
             multi_stream_config=self.__gen_multi_stream_config(),
+            test_execution_config=self.__gen_test_execution_config(),
+            topology_config=self.__gen_topology_config(),
         )
 
-    def __gen_rate_sweep_option(
-        self,
-        rate_sweep_options: "LegacyRateSweepOptions",
-        burst_resolution: float = 0.0,
-    ) -> Dict:
+    def __gen_rate_sweep_option(self, rate_sweep_options: "LegacyRateSweepOptions"):
         return dict(
-            start_value_pct=rate_sweep_options.start_value,
             end_value_pct=rate_sweep_options.end_value,
+            start_value_pct=rate_sweep_options.start_value,
             step_value_pct=rate_sweep_options.step_value,
-            burst_resolution=burst_resolution,
         )
 
     def __gen_common_option(
         self,
         test_type_conf: Union[
             "LegacyThroughput", "LegacyLatency", "LegacyLoss", "LegacyBack2Back"
         ],
-    ) -> Dict:
+    ):
         duration_type = test_type_conf.duration_type.name.lower()
 
-        is_time_duration = test_type_conf.duration_type.is_time_duration
-        return dict(
-            duration_type=duration_type,
-            duration=test_type_conf.duration
+        is_time_duration = test_type_conf.duration_type.value == "seconds"
+        duration_unit = (
+            test_type_conf.duration_time_unit.name.lower()
             if is_time_duration
-            else test_type_conf.duration_frames,
-            duration_unit=test_type_conf.duration_time_unit.name.lower()
+            else test_type_conf.duration_frame_unit.name.lower().replace("field_", "")
+        )
+        duration = (
+            test_type_conf.duration
             if is_time_duration
-            else test_type_conf.duration_frame_unit.name.lower(),
-            iterations=test_type_conf.iterations,
+            else test_type_conf.duration_frames
         )
+        return dict(
+            duration=duration,
+            duration_type=duration_type,
+            duration_unit=duration_unit,
+            repetition=test_type_conf.iterations,
+        )
+
+    # def __gen_common_option_back_to_back(
+    #     self,
+    #     test_type_conf: Union[
+    #         "LegacyThroughput", "LegacyLatency", "LegacyLoss", "LegacyBack2Back"
+    #     ],
+    # ):
+    #     return dict(repetition=test_type_conf.iterations)
 
     def __gen_rate_iteration_options(
         self, rate_iteration_options: "LegacyRateIterationOptions"
-    ) -> Dict:
+    ):
         return dict(
-            search_type=rate_iteration_options.search_type.name.lower(),
-            result_scope=rate_iteration_options.result_scope.name.lower(),
             initial_value_pct=rate_iteration_options.initial_value,
-            minimum_value_pct=rate_iteration_options.minimum_value,
             maximum_value_pct=rate_iteration_options.maximum_value,
+            minimum_value_pct=rate_iteration_options.minimum_value,
+            result_scope=rate_iteration_options.result_scope.name.lower(),
+            search_type=rate_iteration_options.search_type.name.lower(),
             value_resolution_pct=rate_iteration_options.value_resolution,
         )
 
-    def __gen_throughput(self, throughput: "LegacyThroughput") -> Dict:
+    def __gen_throughput(self, throughput: "LegacyThroughput") -> dict:
         rate_iteration_options = throughput.rate_iteration_options
         return dict(
-            test_type=throughput.test_type.name.lower(),
-            enabled=throughput.enabled,
+            acceptable_loss_pct=rate_iteration_options.acceptable_loss,
             common_options=self.__gen_common_option(throughput),
+            collect_latency_jitter="LatencyCounters"
+            in throughput.report_property_options,
+            enabled=throughput.enabled,
+            pass_criteria_throughput_pct=rate_iteration_options.pass_threshold,
             rate_iteration_options=self.__gen_rate_iteration_options(
                 rate_iteration_options
             ),
-            use_pass_threshold=rate_iteration_options.use_pass_threshold,
-            pass_threshold_pct=rate_iteration_options.pass_threshold,
-            acceptable_loss_pct=rate_iteration_options.acceptable_loss,
-            collect_latency_jitter="LatencyCounters"
-            in throughput.report_property_options,
+            use_pass_criteria=rate_iteration_options.use_pass_threshold,
         )
 
-    def __gen_latency(self, latency: "LegacyLatency") -> Dict:
+    def __gen_latency(self, latency: "LegacyLatency") -> dict:
         return dict(
-            test_type=latency.test_type.name.lower(),
-            enabled=latency.enabled,
             common_options=self.__gen_common_option(latency),
-            rate_sweep_options=self.__gen_rate_sweep_option(latency.rate_sweep_options),
+            enabled=latency.enabled,
             latency_mode=latency.latency_mode.lower(),
+            rate_sweep_options=self.__gen_rate_sweep_option(latency.rate_sweep_options),
             use_relative_to_throughput=latency.rate_relative_tput_max_rate,
         )
 
-    def __gen_loss(self, loss: "LegacyLoss") -> Dict:
+    def __gen_loss(self, loss: "LegacyLoss"):
         return dict(
-            test_type=loss.test_type.name.lower(),
-            enabled=loss.enabled,
             common_options=self.__gen_common_option(loss),
-            rate_sweep_options=self.__gen_rate_sweep_option(loss.rate_sweep_options),
-            use_pass_fail_criteria=loss.use_pass_fail_criteria,
-            acceptable_loss_pct=loss.acceptable_loss,
-            acceptable_loss_type=loss.acceptable_loss_type.lower(),
-            use_gap_monitor=loss.use_gap_monitor,
+            enabled=loss.enabled,
             gap_monitor_start_microsec=loss.gap_monitor_start,
             gap_monitor_stop_frames=loss.gap_monitor_stop,
+            pass_criteria_loss=loss.acceptable_loss,
+            pass_criteria_loss_type=loss.acceptable_loss_type.lower(),
+            rate_sweep_options=self.__gen_rate_sweep_option(loss.rate_sweep_options),
+            use_gap_monitor=loss.use_gap_monitor,
+            use_pass_criteria=loss.use_pass_fail_criteria,
         )
 
-    def __gen_back_to_back(self, back_to_back: "LegacyBack2Back") -> Dict:
+    def __gen_back_to_back(self, back_to_back: "LegacyBack2Back"):
         return dict(
-            test_type=back_to_back.test_type.name.lower(),
-            enabled=back_to_back.enabled,
+            burst_size_iteration_options=dict(
+                burst_resolution=back_to_back.burst_resolution,
+                maximum_burst=back_to_back.duration_frames * back_to_back.duration_frame_unit.scale,
+            ),
             common_options=self.__gen_common_option(back_to_back),
+            enabled=back_to_back.enabled,
             rate_sweep_options=self.__gen_rate_sweep_option(
-                back_to_back.rate_sweep_options, (back_to_back.burst_resolution)
+                back_to_back.rate_sweep_options
             ),
         )
 
-    def __gen_test_type_config(self) -> Dict:
+    def __gen_test_type_config(self) -> dict:
         test_type_option_map = self.data.test_options.test_type_option_map
         return dict(
-            throughput_test=self.__gen_throughput(test_type_option_map.throughput),
-            latency_test=self.__gen_latency(test_type_option_map.latency),
-            frame_loss_rate_test=self.__gen_loss(test_type_option_map.loss),
             back_to_back_test=self.__gen_back_to_back(test_type_option_map.back2_back),
+            frame_loss_rate_test=self.__gen_loss(test_type_option_map.loss),
+            latency_test=self.__gen_latency(test_type_option_map.latency),
+            throughput_test=self.__gen_throughput(test_type_option_map.throughput),
         )
 
-    def __gen_port_identity(self) -> List:
+    def __gen_chassis_id_map(self) -> dict[str, str]:
         chassis_id_map = {}
-        port_identity = {}
-
         for chassis_info in self.data.chassis_manager.chassis_list:
             chassis_id = hashlib.md5(
                 f"{chassis_info.host_name}:{chassis_info.port_number}".encode("utf-8")
             ).hexdigest()
             chassis_id_map[chassis_info.chassis_id] = chassis_id
-        chassis_id_list = list(chassis_id_map.values())
+        return chassis_id_map
+
+    def __gen_port_identity(self) -> list[dict]:
+        chassis_id_map = self.__gen_chassis_id_map()
+        port_identity = []
         for count, p_info in enumerate(self.data.port_handler.entity_list):
             port = p_info.port_ref
             port.chassis_id = chassis_id_map[port.chassis_id]
             identity = dict(
-                tester_id=port.chassis_id,
-                tester_index=chassis_id_list.index(port.chassis_id),
                 module_index=port.module_index,
                 port_index=port.port_index,
+                tester_id=port.chassis_id,
             )
-
             self.id_map[p_info.item_id] = (
-                f"c-P-{identity['tester_index']}-{identity['module_index']}-{identity['port_index']}",
-                f"p{count}",
+                f"P-{identity['tester_id']}-{identity['module_index']}-{identity['port_index']}",
+                count,
             )
-            port_identity[f"p{count}"] = identity
+            port_identity.append(identity)
         return port_identity
 
-    def __gen_ipv4_addr(self, entity: "LegacyPortEntity") -> Dict:
+    def __gen_ipv4_addr(self, entity: "LegacyPortEntity"):
         return dict(
             address=entity.ip_v4_address,
-            routing_prefix=entity.ip_v4_routing_prefix,
             gateway=entity.ip_v4_gateway if entity.ip_v4_gateway else "0.0.0.0",
             public_address=entity.public_ip_address
             if entity.public_ip_address
             else "0.0.0.0",
             public_routing_prefix=entity.public_ip_routing_prefix,
             remote_loop_address=entity.remote_loop_ip_address
             if entity.remote_loop_ip_address
             else "0.0.0.0",
+            routing_prefix=entity.ip_v4_routing_prefix,
         )
 
-    def __gen_ipv6_addr(self, entity: "LegacyPortEntity") -> Dict:
+    def __gen_ipv6_addr(self, entity: "LegacyPortEntity"):
         return dict(
             address=entity.ip_v6_address,
-            routing_prefix=entity.ip_v6_routing_prefix,
             gateway=entity.ip_v6_gateway if entity.ip_v6_gateway else "::",
             public_address=entity.public_ip_address_v6
             if entity.public_ip_address_v6
             else "::",
             public_routing_prefix=entity.public_ip_routing_prefix_v6,
             remote_loop_address=entity.remote_loop_ip_address_v6
             if entity.remote_loop_ip_address_v6
             else "::",
+            routing_prefix=entity.ip_v6_routing_prefix,
         )
 
-    def __gen_port_conf(self, entity: "LegacyPortEntity"):
-        profile_id = self.data.stream_profile_handler.profile_assignment_map.get(
-            f"guid_{entity.item_id}"
-        )
+    def __gen_port_conf(self, ip_v: str, profile_id: str, entity: "LegacyPortEntity"):
+        ip_address = None
+        if ip_v == "ipv4":
+            ip_address = self.__gen_ipv4_addr(entity)
+        elif ip_v == "ipv6":
+            ip_address = self.__gen_ipv6_addr(entity)
         return dict(
-            port_slot=self.id_map[entity.item_id][1],
-            peer_config_slot=self.id_map[entity.pair_peer_id][0]
+            anlt_enabled=bool(entity.anlt_enabled),
+            auto_neg_enabled=bool(entity.auto_neg_enabled),
+            broadr_reach_mode=entity.brr_mode.lower(),
+            fec_mode=entity.fec_mode.name.lower(),
+            inter_frame_gap=entity.inter_frame_gap,
+            ip_address=ip_address,
+            ip_gateway_mac_address=entity.ip_gateway_mac_address,
+            latency_offset_ms=entity.latency_offset,
+            mdi_mdix_mode=entity.mdi_mdix_mode.lower(),
+            peer_slot=self.id_map[entity.pair_peer_id][1]
             if entity.pair_peer_id and entity.pair_peer_id in self.id_map
-            else "",
+            else None,
+            pause_mode_enabled=entity.pause_mode_on,
             port_group=entity.port_group.lower(),
+            port_slot=self.id_map[entity.item_id][1],
             port_speed_mode=entity.port_speed.lower(),
-            ipv4_properties=self.__gen_ipv4_addr(entity),
-            ipv6_properties=self.__gen_ipv6_addr(entity),
-            ip_gateway_mac_address=entity.ip_gateway_mac_address,
-            reply_arp_requests=bool(entity.reply_arp_requests),
-            reply_ping_requests=bool(entity.reply_ping_requests),
-            remote_loop_mac_address=entity.remote_loop_mac_address,
-            inter_frame_gap=entity.inter_frame_gap,
-            speed_reduction_ppm=entity.adjust_ppm,
-            pause_mode_enabled=entity.pause_mode_on,
-            latency_offset_ms=entity.latency_offset,
-            fec_mode=entity.fec_mode.name.lower(),
             port_rate_cap_enabled=bool(entity.enable_port_rate_cap),
-            port_rate_cap_value=entity.port_rate_cap_value,
             port_rate_cap_profile=entity.port_rate_cap_profile.name.lower(),
+            port_rate_cap_value=entity.port_rate_cap_value,
             port_rate_cap_unit=entity.port_rate_cap_unit.name.lower().lstrip("field_"),
-            auto_neg_enabled=bool(entity.auto_neg_enabled),
-            anlt_enabled=bool(entity.anlt_enabled),
-            mdi_mdix_mode=entity.mdi_mdix_mode.lower(),
-            broadr_reach_mode=entity.brr_mode.lower(),
-            profile_id=profile_id,
+            protocol_segment_profile_id=profile_id,
+            remote_loop_mac_address=entity.remote_loop_mac_address,
+            reply_arp_requests=bool(entity.reply_arp_requests),
+            reply_ping_requests=bool(entity.reply_ping_requests),
+            speed_reduction_ppm=entity.adjust_ppm,
         )
 
-    def __generate_port_config(self) -> Dict:
-        port_conf: Dict = {}
+    def __generate_port_config(self, protocol_names: dict) -> list[dict]:
+        ip_version: list = []
+        profile_ids: list = []
+        port_conf: list = []
         for entity in self.data.port_handler.entity_list:
-            port_conf[self.id_map[entity.item_id][0]] = self.__gen_port_conf(entity)
+            profile_id = self.data.stream_profile_handler.profile_assignment_map.get(
+                f"guid_{entity.item_id}"
+            )
+            profile_ids.append(profile_id)
+
+            segment_types = protocol_names[profile_id]
+            ipv4_index = segment_types.index("ipv4") if "ipv4" in segment_types else -1
+            ipv6_index = segment_types.index("ipv6") if "ipv6" in segment_types else -1
+            if ipv4_index == ipv6_index == -1:
+                ip_version.append("none")
+            elif ipv4_index > 0 and ipv6_index == -1:
+                ip_version.append("ipv4")
+            elif ipv6_index > 0 and ipv4_index == -1:
+                ip_version.append("ipv6")
+            elif ipv4_index > ipv6_index:
+                ip_version.append("ipv6")
+            elif ipv6_index > ipv4_index:
+                ip_version.append("ipv4")
+
+        for ip_v, profile_id, entity in zip(
+            ip_version, profile_ids, self.data.port_handler.entity_list
+        ):
+            port_conf.append(self.__gen_port_conf(ip_v, profile_id, entity))
         return port_conf
 
-    def gen(self) -> Dict:
+    def gen(self) -> dict:
+        # self.__gen_port_identity() also updates self.id_map, need to be called first
         port_identities = self.__gen_port_identity()
-        test_conf = self.__gen_test_config()
+        protocol_segments = convert_protocol_segments(self.data.stream_profile_handler)
+        protocol_names = {
+            values["id"]: [i["type"] for i in values["segments"]]
+            for values in protocol_segments
+        }
         config = dict(
-            protocol_segments=convert_protocol_segments(
-                self.data.stream_profile_handler
-            ),
-            test_configuration=test_conf,
+            ports_configuration=self.__generate_port_config(protocol_names),
+            protocol_segments=protocol_segments,
+            test_configuration=self.__gen_test_config(),
             test_types_configuration=self.__gen_test_type_config(),
-            ports_configuration=self.__generate_port_config(),
         )
-        return dict(username="hello", config=config, port_identities=port_identities)
+        return dict(config=config, port_identities=port_identities, username="hello")
```

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/rfc2544/enums.py` & `xoa-converter-2.0.0/xoa_converter/converters/rfc2544/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,23 @@
 
 class LegacyDurationFrameUnit(Enum):
     FRAMES = "frames"
     FIELD_10E3_FRAMES = "kframes"
     FIELD_10E6_FRAMES = "mframes"
     FIELD_10E9_FRAMES = "gframes"
 
+    @property
+    def scale(self) -> int:
+        return {
+            LegacyDurationFrameUnit.FRAMES: 1,
+            LegacyDurationFrameUnit.FIELD_10E3_FRAMES: 1e3,
+            LegacyDurationFrameUnit.FIELD_10E6_FRAMES: 1e6,
+            LegacyDurationFrameUnit.FIELD_10E9_FRAMES: 1e9,
+        }[self]
+
 
 class LegacyTrafficDirection(Enum):
     EAST_TO_WEST = "east_west"
     WEST_TO_EAST = "west_east"
     BIDIRECTIONAL = "bidir"
```

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/rfc2544/model.py` & `xoa-converter-2.0.0/xoa_converter/converters/rfc2544/model.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/rfc2889/adapter.py` & `xoa-converter-2.0.0/xoa_converter/converters/rfc2889/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
 import hashlib
-from typing import Any, Dict, TYPE_CHECKING
+from typing import Any, Dict, TYPE_CHECKING, List
 from .model import (
     LegacyPortRoleHandler,
     ValkyrieConfiguration2889 as old_model,
     LegacyFrameSizesOptions,
 )
 from ..common import (
     PortIdentity,
@@ -18,38 +18,39 @@
 
 
 class Converter2889:
     def __init__(self, source_config: str) -> None:
         self.id_map = {}
         self.data = old_model.parse_raw(source_config)
 
-    def __gen_port_identity(self) -> Dict[str, "PortIdentity"]:
+    def __gen_chassis_id_map(self) -> Dict[str, str]:
         chassis_id_map = {}
-        port_identity = {}
-
         for chassis_info in self.data.chassis_manager.chassis_list:
             chassis_id = hashlib.md5(
                 f"{chassis_info.host_name}:{chassis_info.port_number}".encode("utf-8")
             ).hexdigest()
             chassis_id_map[chassis_info.chassis_id] = chassis_id
+        return chassis_id_map
+
+    def __gen_port_identity(self) -> List["PortIdentity"]:
+        chassis_id_map = self.__gen_chassis_id_map()
+        port_identity = []
+
         count = 0
-        chassis_id_list = list(chassis_id_map.values())
         for p_info in self.data.port_handler.entity_list:
             port = p_info.port_ref
             port.chassis_id = chassis_id_map[port.chassis_id]
             identity = dict(
                 tester_id=port.chassis_id,
-                tester_index=chassis_id_list.index(port.chassis_id),
                 module_index=port.module_index,
                 port_index=port.port_index,
             )
 
-            name = f"P-{identity['tester_index']}-{identity['module_index']}-{identity['port_index']}"
-            self.id_map[p_info.item_id] = (f"{name}", f"p{count}")
-            port_identity[f"p{count}"] = identity
+            self.id_map[p_info.item_id] = (f"P-{port.chassis_id}-{port.module_index}-{port.port_index}", f"p{count}")
+            port_identity.append(identity)
             count += 1
         return port_identity
 
     def __gen_ipv4_addr(self, entity: "LegacyPortEntity") -> Dict[str, Any]:
         return dict(
             address=entity.ip_v4_address,
             routing_prefix=entity.ip_v4_routing_prefix,
@@ -103,18 +104,19 @@
             port_rate_cap_unit=entity.port_rate_cap_unit,
             auto_neg_enabled=bool(entity.auto_neg_enabled),
             anlt_enabled=bool(entity.anlt_enabled),
             mdi_mdix_mode=entity.mdi_mdix_mode,
             broadr_reach_mode=entity.brr_mode,
             profile_id=profile_id,
             item_id=entity.item_id,
+            tester_id=entity.port_ref.chassis_id,
         )
 
-    def __gen_port_config(self) -> Dict[str, Any]:
-        port_conf: Dict = {}
+    def __gen_port_config(self) -> Dict:
+        port_conf = {}
         for entity in self.data.port_handler.entity_list:
             port_conf[self.id_map[entity.item_id][0]] = self.__gen_port_conf(entity)
         return port_conf
 
     def __gen_frame_size(self) -> Dict[str, Any]:
         packet_size = self.data.test_options.packet_sizes
         packet_size_type = packet_size.packet_size_type
```

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/rfc2889/const.py` & `xoa-converter-2.0.0/xoa_converter/converters/rfc2889/const.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/rfc2889/model.py` & `xoa-converter-2.0.0/xoa_converter/converters/rfc2889/model.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/arp.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/arp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ecpri.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ecpri.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ethernet.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ethernet.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/fcoe.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fcoe.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/fiberchannel.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fiberchannel.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/geneve.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/geneve.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/grecheck.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/grecheck.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/grenocheck.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/grenocheck.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv1.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv1l0.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1l0.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv1l1.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1l1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv2l0.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv2l0.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/gtpv2l1.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv2l1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/icmp.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/icmp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/icmpv6.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/icmpv6.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv1.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv2.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv2.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv3grouprecord.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3grouprecord.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv3l0.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3l0.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv3l1.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3l1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/igmpv3memreport.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3memreport.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ip.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ip.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/ipv6.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ipv6.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/llc.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/llc.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/macctrlpfc.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/macctrlpfc.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/mldv2addressrecord.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mldv2addressrecord.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/mpls.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mpls.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/mpls_tp_oam.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mpls_tp_oam.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/nvgre.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/nvgre.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/pbb.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/pbb.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/roe.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/roe.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/rtcp.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/rtcp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/rtp.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/rtp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/sctp.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/sctp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/stp.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/stp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/tcp.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/tcp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/tcpcheck.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/tcpcheck.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/udp.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/udp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/udpcheck.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/udpcheck.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/vlan.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/vlan.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/converters/segment_refs/vxlan.json` & `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/vxlan.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter/entry.py` & `xoa-converter-2.0.0/xoa_converter/entry.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-1.0.7/xoa_converter.egg-info/PKG-INFO` & `xoa-converter-2.0.0/xoa_converter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-converter
-Version: 1.0.7
+Version: 2.0.0
 Summary: Xena OpenAutomation test configuration converter let you easily migrate your Valkyrie test suites config files (.v2544, .v2889, .v3918, and .v1564) into XOA.
 Home-page: https://github.com/xenanetworks/open-automation-config-converter
 Author: Frank Chen, Maureen Chen, Artem Constantinov
 Author-email: fch@xenanewtorks.com, mch@xenanetworks.com, aco@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
@@ -20,21 +20,23 @@
 License-File: LICENSE
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-converter) [![PyPI](https://img.shields.io/pypi/v/xoa-converter)](https://pypi.python.org/pypi/xoa-converter) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-config-converter) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-test-config-converter/badge/?version=stable)](https://xena-openautomation-test-config-converter.readthedocs.io/en/stable/?badge=stable)
 # Xena OpenAutomation Test Config Converter
 Xena OpenAutomation (XOA) Test Configuration Converter is a supporting tool for users to quickly migrate their Valkyrie test suite configurations into XOA.
 
 ## Introduction
-Xena's test suite applications have only been for Windows platform for a long time. Moving forward, all of Xena's existing and future test suites will be included in Xena OpenAutomation, which is not limited to Windows anymore. 
+The XOA Test Config Converter is an open-source tool hosted on Xena Networks' GitHub repository. It is designed to help users migrate their existing Valkyrie test suite configurations into the XOA format, enabling a seamless transition to the XOA ecosystem for network automation and testing.
 
-We have developed this test configuration converter and made it into a Python package to help users easily migrate their existing Windows test suite configurations (`.v2544` for [Valkyrie2544](https://xenanetworks.com/product/valkyrie2544/), `.v2889` for [Valkyrie2889](https://xenanetworks.com/product/valkyrie2889/), `.v3918` for [Valkyrie3918](https://xenanetworks.com/product/valkyrie3918/), and `.v1564` for [Valkyrie1564](https://xenanetworks.com/product/valkyrie1564/)) into `XOA`.
+Key features of the XOA Test Config Converter include:
 
-For users of XOA who only uses the web GUI to create, import and run tests, there is no need to use this Python package, because [XOA Core](https://github.com/xenanetworks/open-automation-core) is already using this converter.
+1. Conversion support: The tool supports conversion of Valkyrie test suite configuration files to XOA-compatible format, facilitating the integration of existing test cases into the XOA framework.
 
-This converter is meant for those who want to integrate XOA test suites into their own Python environment without using the web GUI at all.
+2. Ease of use: The XOA Test Config Converter is designed to be user-friendly, with a straightforward process for converting test suite configuration files.
+
+3. Compatibility: The converter ensures that the migrated test suite configurations are compatible with XOA Core and can be executed within the XOA ecosystem.
 
 > The purpose of XOA Converter is ONLY to convert Xena Valkyrie test suit applications' configuration files into XOA's configuration files. Thus only four test suite types are supported by XOA Converter as the source config files. 
 
 ## Documentation
 The user documentation is hosted:
 [Xena OpenAutomation Test Config Converter Documentation](https://docs.xenanetworks.com/projects/xoa-config-converter)
```

### Comparing `xoa-converter-1.0.7/xoa_converter.egg-info/SOURCES.txt` & `xoa-converter-2.0.0/xoa_converter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 xoa_converter/converters/rfc2544/adapter.py
 xoa_converter/converters/rfc2544/enums.py
 xoa_converter/converters/rfc2544/model.py
 xoa_converter/converters/rfc2889/__init__.py
 xoa_converter/converters/rfc2889/adapter.py
 xoa_converter/converters/rfc2889/const.py
 xoa_converter/converters/rfc2889/model.py
+xoa_converter/converters/rfc3918/__init__.py
+xoa_converter/converters/rfc3918/adapter.py
+xoa_converter/converters/rfc3918/const_conv.py
+xoa_converter/converters/rfc3918/field.py
+xoa_converter/converters/rfc3918/legacy.py
 xoa_converter/converters/segment_refs/arp.json
 xoa_converter/converters/segment_refs/ecpri.json
 xoa_converter/converters/segment_refs/ethernet.json
 xoa_converter/converters/segment_refs/ethernet802.3.json
 xoa_converter/converters/segment_refs/fcoe.json
 xoa_converter/converters/segment_refs/fcoetail.json
 xoa_converter/converters/segment_refs/fiberchannel.json
```

