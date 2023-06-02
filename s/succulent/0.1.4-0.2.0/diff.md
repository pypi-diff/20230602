# Comparing `tmp/succulent-0.1.4.tar.gz` & `tmp/succulent-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "succulent-0.1.4.tar", max compression
+gzip compressed data, was "succulent-0.2.0.tar", max compression
```

## Comparing `succulent-0.1.4.tar` & `succulent-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1094 2023-04-18 11:02:21.268343 succulent-0.1.4/LICENSE
--rw-r--r--   0        0        0      708 2023-05-29 13:22:43.505543 succulent-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5841 2023-05-29 13:24:59.974193 succulent-0.1.4/README.md
--rw-r--r--   0        0        0      113 2023-05-29 13:22:52.395173 succulent-0.1.4/succulent/__init__.py
--rw-r--r--   0        0        0     1710 2023-05-28 20:27:47.551677 succulent-0.1.4/succulent/api.py
--rw-r--r--   0        0        0      362 2023-05-24 09:55:47.296058 succulent-0.1.4/succulent/configuration.py
--rw-r--r--   0        0        0     3717 2023-05-29 10:37:54.556319 succulent-0.1.4/succulent/processing.py
--rw-r--r--   0        0        0     6570 1970-01-01 00:00:00.000000 succulent-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-02 11:10:41.241982 succulent-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6839 2023-06-02 11:10:41.242982 succulent-0.2.0/README.md
+-rw-r--r--   0        0        0      683 2023-06-02 11:10:41.242982 succulent-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-06-02 11:10:41.242982 succulent-0.2.0/succulent/__init__.py
+-rw-r--r--   0        0        0     1663 2023-06-02 11:10:41.242982 succulent-0.2.0/succulent/api.py
+-rw-r--r--   0        0        0      349 2023-06-02 11:10:41.242982 succulent-0.2.0/succulent/configuration.py
+-rw-r--r--   0        0        0     3681 2023-06-02 11:10:41.242982 succulent-0.2.0/succulent/processing.py
+-rw-r--r--   0        0        0     7551 2023-06-02 11:10:47.306035 succulent-0.2.0/setup.py
+-rw-r--r--   0        0        0     7490 2023-06-02 11:10:47.306262 succulent-0.2.0/PKG-INFO
```

### Comparing `succulent-0.1.4/LICENSE` & `succulent-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Iztok Fister Jr.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Iztok Fister Jr.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `succulent-0.1.4/README.md` & `succulent-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 3a53 5441 5254 202d 2044 6f20 6e6f 7420  :START - Do not 
 00000030: 7265 6d6f 7665 206f 7220 6d6f 6469 6679  remove or modify
 00000040: 2074 6869 7320 7365 6374 696f 6e20 2d2d   this section --
 00000050: 3e0d 0a5b 215b 416c 6c20 436f 6e74 7269  >..[![All Contri
 00000060: 6275 746f 7273 5d28 6874 7470 733a 2f2f  butors](https://
 00000070: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
 00000080: 6164 6765 2f61 6c6c 5f63 6f6e 7472 6962  adge/all_contrib
-00000090: 7574 6f72 732d 332d 6f72 616e 6765 2e73  utors-3-orange.s
+00000090: 7574 6f72 732d 342d 6f72 616e 6765 2e73  utors-4-orange.s
 000000a0: 7667 3f73 7479 6c65 3d66 6c61 742d 7371  vg?style=flat-sq
 000000b0: 7561 7265 295d 2823 636f 6e74 7269 6275  uare)](#contribu
 000000c0: 746f 7273 2d29 0d0a 3c21 2d2d 2041 4c4c  tors-)..<!-- ALL
 000000d0: 2d43 4f4e 5452 4942 5554 4f52 532d 4241  -CONTRIBUTORS-BA
 000000e0: 4447 453a 454e 4420 2d2d 3e0d 0a0d 0a23  DGE:END -->....#
 000000f0: 2073 7563 6375 6c65 6e74 202d 2043 6f6c   succulent - Col
 00000100: 6c65 6374 2050 4f53 5420 7265 7175 6573  lect POST reques
@@ -158,209 +158,271 @@
 000009d0: 7220 6461 7461 2063 6f6c 6c65 6374 696f  r data collectio
 000009e0: 6e0d 0a2d 2044 6174 6120 636f 6c6c 6563  n..- Data collec
 000009f0: 7469 6f6e 2066 726f 6d20 504f 5354 2072  tion from POST r
 00000a00: 6571 7565 7374 730d 0a2d 2053 746f 7269  equests..- Stori
 00000a10: 6e67 2064 6174 6120 696e 2064 6966 6665  ng data in diffe
 00000a20: 7265 6e74 2066 6f72 6d61 7473 2028 4353  rent formats (CS
 00000a30: 562c 204a 534f 4e2c 2053 514c 6974 6529  V, JSON, SQLite)
-00000a40: 0d0a 0d0a 2323 2049 6e73 7461 6c6c 6174  ....## Installat
-00000a50: 696f 6e0d 0a0d 0a23 2323 2070 6970 0d0a  ion....### pip..
-00000a60: 0d0a 496e 7374 616c 6c20 7375 6363 756c  ..Install succul
-00000a70: 656e 7420 7769 7468 2070 6970 3a0d 0a0d  ent with pip:...
-00000a80: 0a60 6060 7368 0d0a 7069 7020 696e 7374  .```sh..pip inst
-00000a90: 616c 6c20 7375 6363 756c 656e 740d 0a60  all succulent..`
-00000aa0: 6060 0d0a 2323 2320 416c 7069 6e65 204c  ``..### Alpine L
-00000ab0: 696e 7578 0d0a 0d0a 546f 2069 6e73 7461  inux....To insta
-00000ac0: 6c6c 2073 7563 6375 6c65 6e74 206f 6e20  ll succulent on 
-00000ad0: 416c 7069 6e65 204c 696e 7578 2c20 706c  Alpine Linux, pl
-00000ae0: 6561 7365 2075 7365 3a0d 0a0d 0a60 6060  ease use:....```
-00000af0: 7368 0d0a 2420 6170 6b20 6164 6420 7079  sh..$ apk add py
-00000b00: 332d 7375 6363 756c 656e 740d 0a60 6060  3-succulent..```
-00000b10: 0d0a 0d0a 2323 2043 6f6e 7461 696e 6572  ....## Container
-00000b20: 0d0a 0d0a 5b42 6173 6963 2063 6f6e 7461  ....[Basic conta
-00000b30: 696e 6572 2066 6f72 2073 7563 6375 6c65  iner for succule
-00000b40: 6e74 5d28 6874 7470 733a 2f2f 6769 7468  nt](https://gith
-00000b50: 7562 2e63 6f6d 2f66 6972 6566 6c79 2d63  ub.com/firefly-c
-00000b60: 7070 2f73 7563 6375 6c65 6e74 2d63 6f6e  pp/succulent-con
-00000b70: 7461 696e 6572 290d 0a0d 0a23 2320 5573  tainer)....## Us
-00000b80: 6167 650d 0a0d 0a23 2323 2045 7861 6d70  age....### Examp
-00000b90: 6c65 0d0a 0d0a 6060 6070 7974 686f 6e0d  le....```python.
-00000ba0: 0a66 726f 6d20 7375 6363 756c 656e 742e  .from succulent.
-00000bb0: 6170 6920 696d 706f 7274 2053 7563 6375  api import Succu
-00000bc0: 6c65 6e74 4150 490d 0a61 7069 203d 2053  lentAPI..api = S
-00000bd0: 7563 6375 6c65 6e74 4150 4928 686f 7374  ucculentAPI(host
-00000be0: 3d27 302e 302e 302e 3027 2c20 706f 7274  ='0.0.0.0', port
-00000bf0: 3d38 3038 302c 2063 6f6e 6669 673d 2763  =8080, config='c
-00000c00: 6f6e 6669 6775 7261 7469 6f6e 2e79 6d6c  onfiguration.yml
-00000c10: 272c 2066 6f72 6d61 743d 2763 7376 2729  ', format='csv')
-00000c20: 0d0a 6170 692e 7374 6172 7428 290d 0a60  ..api.start()..`
-00000c30: 6060 0d0a 0d0a 2323 2043 6f6e 6669 6775  ``....## Configu
-00000c40: 7261 7469 6f6e 0d0a 496e 2074 6865 2072  ration..In the r
-00000c50: 6f6f 7420 6469 7265 6374 6f72 792c 2063  oot directory, c
-00000c60: 7265 6174 6520 6120 6669 6c65 206e 616d  reate a file nam
-00000c70: 6564 2060 636f 6e66 6967 7572 6174 696f  ed `configuratio
-00000c80: 6e2e 796d 6c60 2061 6e64 2064 6566 696e  n.yml` and defin
-00000c90: 6520 7468 6520 666f 6c6c 6f77 696e 673a  e the following:
-00000ca0: 0d0a 6060 6079 6d6c 0d0a 6461 7461 3a0d  ..```yml..data:.
-00000cb0: 0a20 202d 206e 616d 653a 2023 204d 6561  .  - name: # Mea
-00000cc0: 7375 7265 206e 616d 650d 0a20 2020 206d  sure name..    m
-00000cd0: 696e 3a20 2320 4d69 6e69 6d75 6d20 7661  in: # Minimum va
-00000ce0: 6c75 6520 286f 7074 696f 6e61 6c29 0d0a  lue (optional)..
-00000cf0: 2020 2020 6d61 783a 2023 204d 6178 696d      max: # Maxim
-00000d00: 756d 2076 616c 7565 2028 6f70 7469 6f6e  um value (option
-00000d10: 616c 290d 0a60 6060 0d0a 0d0a 2323 204c  al)..```....## L
-00000d20: 6963 656e 7365 0d0a 0d0a 5468 6973 2070  icense....This p
-00000d30: 6163 6b61 6765 2069 7320 6469 7374 7269  ackage is distri
-00000d40: 6275 7465 6420 756e 6465 7220 7468 6520  buted under the 
-00000d50: 4d49 5420 4c69 6365 6e73 652e 2054 6869  MIT License. Thi
-00000d60: 7320 6c69 6365 6e73 6520 6361 6e20 6265  s license can be
-00000d70: 2066 6f75 6e64 206f 6e6c 696e 6520 6174   found online at
-00000d80: 203c 6874 7470 3a2f 2f77 7777 2e6f 7065   <http://www.ope
-00000d90: 6e73 6f75 7263 652e 6f72 672f 6c69 6365  nsource.org/lice
-00000da0: 6e73 6573 2f4d 4954 3e2e 0d0a 0d0a 2323  nses/MIT>.....##
-00000db0: 2044 6973 636c 6169 6d65 720d 0a0d 0a54   Disclaimer....T
-00000dc0: 6869 7320 6672 616d 6577 6f72 6b20 6973  his framework is
-00000dd0: 2070 726f 7669 6465 6420 6173 2d69 732c   provided as-is,
-00000de0: 2061 6e64 2074 6865 7265 2061 7265 206e   and there are n
-00000df0: 6f20 6775 6172 616e 7465 6573 2074 6861  o guarantees tha
-00000e00: 7420 6974 2066 6974 7320 796f 7572 2070  t it fits your p
-00000e10: 7572 706f 7365 7320 6f72 2074 6861 7420  urposes or that 
-00000e20: 6974 2069 7320 6275 672d 6672 6565 2e20  it is bug-free. 
-00000e30: 5573 6520 6974 2061 7420 796f 7572 206f  Use it at your o
-00000e40: 776e 2072 6973 6b21 0d0a 0d0a 2323 2043  wn risk!....## C
-00000e50: 6f6e 7472 6962 7574 6f72 7320 e29c a80d  ontributors ....
-00000e60: 0a0d 0a54 6861 6e6b 7320 676f 6573 2074  ...Thanks goes t
-00000e70: 6f20 7468 6573 6520 776f 6e64 6572 6675  o these wonderfu
-00000e80: 6c20 7065 6f70 6c65 2028 5b65 6d6f 6a69  l people ([emoji
-00000e90: 206b 6579 5d28 6874 7470 733a 2f2f 616c   key](https://al
-00000ea0: 6c63 6f6e 7472 6962 7574 6f72 732e 6f72  lcontributors.or
-00000eb0: 672f 646f 6373 2f65 6e2f 656d 6f6a 692d  g/docs/en/emoji-
-00000ec0: 6b65 7929 293a 0d0a 0d0a 3c21 2d2d 2041  key)):....<!-- A
-00000ed0: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
-00000ee0: 4c49 5354 3a53 5441 5254 202d 2044 6f20  LIST:START - Do 
-00000ef0: 6e6f 7420 7265 6d6f 7665 206f 7220 6d6f  not remove or mo
-00000f00: 6469 6679 2074 6869 7320 7365 6374 696f  dify this sectio
-00000f10: 6e20 2d2d 3e0d 0a3c 212d 2d20 7072 6574  n -->..<!-- pret
-00000f20: 7469 6572 2d69 676e 6f72 652d 7374 6172  tier-ignore-star
-00000f30: 7420 2d2d 3e0d 0a3c 212d 2d20 6d61 726b  t -->..<!-- mark
-00000f40: 646f 776e 6c69 6e74 2d64 6973 6162 6c65  downlint-disable
-00000f50: 202d 2d3e 0d0a 3c74 6162 6c65 3e0d 0a20   -->..<table>.. 
-00000f60: 203c 7462 6f64 793e 0d0a 2020 2020 3c74   <tbody>..    <t
-00000f70: 723e 0d0a 2020 2020 2020 3c74 6420 616c  r>..      <td al
-00000f80: 6967 6e3d 2263 656e 7465 7222 2076 616c  ign="center" val
-00000f90: 6967 6e3d 2274 6f70 2220 7769 6474 683d  ign="top" width=
-00000fa0: 2231 342e 3238 2522 3e3c 6120 6872 6566  "14.28%"><a href
-00000fb0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000fc0: 2e63 6f6d 2f6c 6168 6f76 6e69 6b74 6164  .com/lahovniktad
-00000fd0: 656a 223e 3c69 6d67 2073 7263 3d22 6874  ej"><img src="ht
-00000fe0: 7470 733a 2f2f 6176 6174 6172 732e 6769  tps://avatars.gi
-00000ff0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00001000: 636f 6d2f 752f 3537 3839 3037 3334 3f76  com/u/57890734?v
-00001010: 3d34 3f73 3d31 3030 2220 7769 6474 683d  =4?s=100" width=
-00001020: 2231 3030 7078 3b22 2061 6c74 3d22 5461  "100px;" alt="Ta
-00001030: 6465 6a20 4c61 686f 766e 696b 222f 3e3c  dej Lahovnik"/><
-00001040: 6272 202f 3e3c 7375 623e 3c62 3e54 6164  br /><sub><b>Tad
-00001050: 656a 204c 6168 6f76 6e69 6b3c 2f62 3e3c  ej Lahovnik</b><
-00001060: 2f73 7562 3e3c 2f61 3e3c 6272 202f 3e3c  /sub></a><br /><
-00001070: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001080: 6769 7468 7562 2e63 6f6d 2f66 6972 6566  github.com/firef
-00001090: 6c79 2d63 7070 2f73 7563 6375 6c65 6e74  ly-cpp/succulent
-000010a0: 2f63 6f6d 6d69 7473 3f61 7574 686f 723d  /commits?author=
-000010b0: 6c61 686f 766e 696b 7461 6465 6a22 2074  lahovniktadej" t
-000010c0: 6974 6c65 3d22 436f 6465 223e f09f 92bb  itle="Code">....
-000010d0: 3c2f 613e 203c 6120 6872 6566 3d22 6874  </a> <a href="ht
-000010e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000010f0: 2f66 6972 6566 6c79 2d63 7070 2f73 7563  /firefly-cpp/suc
-00001100: 6375 6c65 6e74 2f69 7373 7565 733f 713d  culent/issues?q=
-00001110: 6175 7468 6f72 2533 416c 6168 6f76 6e69  author%3Alahovni
-00001120: 6b74 6164 656a 2220 7469 746c 653d 2242  ktadej" title="B
-00001130: 7567 2072 6570 6f72 7473 223e f09f 909b  ug reports">....
-00001140: 3c2f 613e 203c 6120 6872 6566 3d22 2369  </a> <a href="#i
-00001150: 6465 6173 2d6c 6168 6f76 6e69 6b74 6164  deas-lahovniktad
-00001160: 656a 2220 7469 746c 653d 2249 6465 6173  ej" title="Ideas
-00001170: 2c20 506c 616e 6e69 6e67 2c20 2620 4665  , Planning, & Fe
-00001180: 6564 6261 636b 223e f09f a494 3c2f 613e  edback">....</a>
-00001190: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000011a0: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6972  //github.com/fir
-000011b0: 6566 6c79 2d63 7070 2f73 7563 6375 6c65  efly-cpp/succule
-000011c0: 6e74 2f63 6f6d 6d69 7473 3f61 7574 686f  nt/commits?autho
-000011d0: 723d 6c61 686f 766e 696b 7461 6465 6a22  r=lahovniktadej"
-000011e0: 2074 6974 6c65 3d22 446f 6375 6d65 6e74   title="Document
-000011f0: 6174 696f 6e22 3ef0 9f93 963c 2f61 3e3c  ation">....</a><
-00001200: 2f74 643e 0d0a 2020 2020 2020 3c74 6420  /td>..      <td 
-00001210: 616c 6967 6e3d 2263 656e 7465 7222 2076  align="center" v
-00001220: 616c 6967 6e3d 2274 6f70 2220 7769 6474  align="top" widt
-00001230: 683d 2231 342e 3238 2522 3e3c 6120 6872  h="14.28%"><a hr
-00001240: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00001250: 7562 2e63 6f6d 2f41 7961 6e44 6173 3334  ub.com/AyanDas34
-00001260: 3822 3e3c 696d 6720 7372 633d 2268 7474  8"><img src="htt
-00001270: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
-00001280: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001290: 6f6d 2f75 2f35 3336 3130 3632 363f 763d  om/u/53610626?v=
-000012a0: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
-000012b0: 3130 3070 783b 2220 616c 743d 2241 7961  100px;" alt="Aya
-000012c0: 6e20 4461 7322 2f3e 3c62 7220 2f3e 3c73  n Das"/><br /><s
-000012d0: 7562 3e3c 623e 4179 616e 2044 6173 3c2f  ub><b>Ayan Das</
-000012e0: 623e 3c2f 7375 623e 3c2f 613e 3c62 7220  b></sub></a><br 
-000012f0: 2f3e 3c61 2068 7265 663d 2268 7474 7073  /><a href="https
-00001300: 3a2f 2f67 6974 6875 622e 636f 6d2f 6669  ://github.com/fi
-00001310: 7265 666c 792d 6370 702f 7375 6363 756c  refly-cpp/succul
-00001320: 656e 742f 636f 6d6d 6974 733f 6175 7468  ent/commits?auth
-00001330: 6f72 3d41 7961 6e44 6173 3334 3822 2074  or=AyanDas348" t
-00001340: 6974 6c65 3d22 436f 6465 223e f09f 92bb  itle="Code">....
-00001350: 3c2f 613e 203c 6120 6872 6566 3d22 6874  </a> <a href="ht
-00001360: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001370: 2f66 6972 6566 6c79 2d63 7070 2f73 7563  /firefly-cpp/suc
-00001380: 6375 6c65 6e74 2f63 6f6d 6d69 7473 3f61  culent/commits?a
-00001390: 7574 686f 723d 4179 616e 4461 7333 3438  uthor=AyanDas348
-000013a0: 2220 7469 746c 653d 2254 6573 7473 223e  " title="Tests">
-000013b0: e29a a0ef b88f 3c2f 613e 3c2f 7464 3e0d  ......</a></td>.
-000013c0: 0a20 2020 2020 203c 7464 2061 6c69 676e  .      <td align
-000013d0: 3d22 6365 6e74 6572 2220 7661 6c69 676e  ="center" valign
-000013e0: 3d22 746f 7022 2077 6964 7468 3d22 3134  ="top" width="14
-000013f0: 2e32 3825 223e 3c61 2068 7265 663d 2268  .28%"><a href="h
-00001400: 7474 703a 2f2f 7777 772e 697a 746f 6b2d  ttp://www.iztok-
-00001410: 6a72 2d66 6973 7465 722e 6575 2f22 3e3c  jr-fister.eu/"><
-00001420: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001430: 2f61 7661 7461 7273 2e67 6974 6875 6275  /avatars.githubu
-00001440: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f75  sercontent.com/u
-00001450: 2f31 3633 3333 3631 3f76 3d34 3f73 3d31  /1633361?v=4?s=1
-00001460: 3030 2220 7769 6474 683d 2231 3030 7078  00" width="100px
-00001470: 3b22 2061 6c74 3d22 497a 746f 6b20 4669  ;" alt="Iztok Fi
-00001480: 7374 6572 204a 722e 222f 3e3c 6272 202f  ster Jr."/><br /
-00001490: 3e3c 7375 623e 3c62 3e49 7a74 6f6b 2046  ><sub><b>Iztok F
-000014a0: 6973 7465 7220 4a72 2e3c 2f62 3e3c 2f73  ister Jr.</b></s
-000014b0: 7562 3e3c 2f61 3e3c 6272 202f 3e3c 6120  ub></a><br /><a 
-000014c0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-000014d0: 7468 7562 2e63 6f6d 2f66 6972 6566 6c79  thub.com/firefly
-000014e0: 2d63 7070 2f73 7563 6375 6c65 6e74 2f63  -cpp/succulent/c
-000014f0: 6f6d 6d69 7473 3f61 7574 686f 723d 6669  ommits?author=fi
-00001500: 7265 666c 792d 6370 7022 2074 6974 6c65  refly-cpp" title
-00001510: 3d22 436f 6465 223e f09f 92bb 3c2f 613e  ="Code">....</a>
-00001520: 203c 6120 6872 6566 3d22 2369 6465 6173   <a href="#ideas
-00001530: 2d66 6972 6566 6c79 2d63 7070 2220 7469  -firefly-cpp" ti
-00001540: 746c 653d 2249 6465 6173 2c20 506c 616e  tle="Ideas, Plan
-00001550: 6e69 6e67 2c20 2620 4665 6564 6261 636b  ning, & Feedback
-00001560: 223e f09f a494 3c2f 613e 203c 6120 6872  ">....</a> <a hr
-00001570: 6566 3d22 236d 656e 746f 7269 6e67 2d66  ef="#mentoring-f
-00001580: 6972 6566 6c79 2d63 7070 2220 7469 746c  irefly-cpp" titl
-00001590: 653d 224d 656e 746f 7269 6e67 223e f09f  e="Mentoring">..
-000015a0: a791 e280 8df0 9f8f ab3c 2f61 3e3c 2f74  .........</a></t
-000015b0: 643e 0d0a 2020 2020 3c2f 7472 3e0d 0a20  d>..    </tr>.. 
-000015c0: 203c 2f74 626f 6479 3e0d 0a3c 2f74 6162   </tbody>..</tab
-000015d0: 6c65 3e0d 0a0d 0a3c 212d 2d20 6d61 726b  le>....<!-- mark
-000015e0: 646f 776e 6c69 6e74 2d72 6573 746f 7265  downlint-restore
-000015f0: 202d 2d3e 0d0a 3c21 2d2d 2070 7265 7474   -->..<!-- prett
-00001600: 6965 722d 6967 6e6f 7265 2d65 6e64 202d  ier-ignore-end -
-00001610: 2d3e 0d0a 0d0a 3c21 2d2d 2041 4c4c 2d43  ->....<!-- ALL-C
-00001620: 4f4e 5452 4942 5554 4f52 532d 4c49 5354  ONTRIBUTORS-LIST
-00001630: 3a45 4e44 202d 2d3e 0d0a 0d0a 5468 6973  :END -->....This
-00001640: 2070 726f 6a65 6374 2066 6f6c 6c6f 7773   project follows
-00001650: 2074 6865 205b 616c 6c2d 636f 6e74 7269   the [all-contri
-00001660: 6275 746f 7273 5d28 6874 7470 733a 2f2f  butors](https://
-00001670: 6769 7468 7562 2e63 6f6d 2f61 6c6c 2d63  github.com/all-c
-00001680: 6f6e 7472 6962 7574 6f72 732f 616c 6c2d  ontributors/all-
-00001690: 636f 6e74 7269 6275 746f 7273 2920 7370  contributors) sp
-000016a0: 6563 6966 6963 6174 696f 6e2e 2043 6f6e  ecification. Con
-000016b0: 7472 6962 7574 696f 6e73 206f 6620 616e  tributions of an
-000016c0: 7920 6b69 6e64 2077 656c 636f 6d65 210d  y kind welcome!.
-000016d0: 0a                                       .
+00000a40: 0d0a 2d20 4465 6669 6e69 6e67 2062 6f75  ..- Defining bou
+00000a50: 6e64 6172 6965 7320 666f 7220 636f 6c6c  ndaries for coll
+00000a60: 6563 7465 6420 6461 7461 2028 6d69 6e2c  ected data (min,
+00000a70: 206d 6178 290d 0a0d 0a23 2320 496e 7374   max)....## Inst
+00000a80: 616c 6c61 7469 6f6e 0d0a 0d0a 2323 2320  allation....### 
+00000a90: 7069 700d 0a0d 0a49 6e73 7461 6c6c 2073  pip....Install s
+00000aa0: 7563 6375 6c65 6e74 2077 6974 6820 7069  ucculent with pi
+00000ab0: 703a 0d0a 0d0a 6060 6073 680d 0a70 6970  p:....```sh..pip
+00000ac0: 2069 6e73 7461 6c6c 2073 7563 6375 6c65   install succule
+00000ad0: 6e74 0d0a 6060 600d 0a23 2323 2041 6c70  nt..```..### Alp
+00000ae0: 696e 6520 4c69 6e75 780d 0a0d 0a54 6f20  ine Linux....To 
+00000af0: 696e 7374 616c 6c20 7375 6363 756c 656e  install succulen
+00000b00: 7420 6f6e 2041 6c70 696e 6520 4c69 6e75  t on Alpine Linu
+00000b10: 782c 2070 6c65 6173 6520 7573 653a 0d0a  x, please use:..
+00000b20: 0d0a 6060 6073 680d 0a24 2061 706b 2061  ..```sh..$ apk a
+00000b30: 6464 2070 7933 2d73 7563 6375 6c65 6e74  dd py3-succulent
+00000b40: 0d0a 6060 600d 0a0d 0a23 2320 436f 6e74  ..```....## Cont
+00000b50: 6169 6e65 720d 0a0d 0a5b 4261 7369 6320  ainer....[Basic 
+00000b60: 636f 6e74 6169 6e65 7220 666f 7220 7375  container for su
+00000b70: 6363 756c 656e 745d 2868 7474 7073 3a2f  cculent](https:/
+00000b80: 2f67 6974 6875 622e 636f 6d2f 6669 7265  /github.com/fire
+00000b90: 666c 792d 6370 702f 7375 6363 756c 656e  fly-cpp/succulen
+00000ba0: 742d 636f 6e74 6169 6e65 7229 0d0a 0d0a  t-container)....
+00000bb0: 2323 2320 436f 6e66 6967 7572 6174 696f  ### Configuratio
+00000bc0: 6e0d 0a46 6f6c 6c6f 7720 7468 6520 696e  n..Follow the in
+00000bd0: 7374 7275 6374 696f 6e73 2069 6e20 7468  structions in th
+00000be0: 6520 5b63 6f6e 6669 6775 7261 7469 6f6e  e [configuration
+00000bf0: 5d28 2323 636f 6e66 6967 7572 6174 696f  ](##configuratio
+00000c00: 6e29 2073 6563 7469 6f6e 2074 6f20 6465  n) section to de
+00000c10: 6669 6e65 2074 6865 2063 6f6e 6669 6775  fine the configu
+00000c20: 7261 7469 6f6e 2066 696c 652e 0d0a 0d0a  ration file.....
+00000c30: 2323 2320 496e 7374 616c 6c61 7469 6f6e  ### Installation
+00000c40: 0d0a 4275 696c 6420 7468 6520 636f 6e74  ..Build the cont
+00000c50: 6169 6e65 7220 7573 696e 6720 446f 636b  ainer using Dock
+00000c60: 6572 3a0d 0a60 6060 6261 7368 0d0a 646f  er:..```bash..do
+00000c70: 636b 6572 2062 7569 6c64 202d 7420 7375  cker build -t su
+00000c80: 6363 756c 656e 742d 636f 6e74 6169 6e65  cculent-containe
+00000c90: 7220 2e0d 0a60 6060 0d0a 0d0a 416c 7465  r ...```....Alte
+00000ca0: 726e 6174 6976 656c 792c 2079 6f75 2063  rnatively, you c
+00000cb0: 616e 2075 7365 2060 6064 6f63 6b65 722d  an use ``docker-
+00000cc0: 636f 6d70 6f73 6560 603a 0d0a 6060 6062  compose``:..```b
+00000cd0: 6173 680d 0a64 6f63 6b65 7220 636f 6d70  ash..docker comp
+00000ce0: 6f73 6520 6275 696c 640d 0a60 6060 0d0a  ose build..```..
+00000cf0: 0d0a 2323 2320 5573 6167 650d 0a52 756e  ..### Usage..Run
+00000d00: 2074 6865 2063 6f6e 7461 696e 6572 2075   the container u
+00000d10: 7369 6e67 2044 6f63 6b65 723a 0d0a 6060  sing Docker:..``
+00000d20: 6062 6173 680d 0a64 6f63 6b65 7220 7275  `bash..docker ru
+00000d30: 6e20 2d70 2038 3038 303a 3830 3830 2073  n -p 8080:8080 s
+00000d40: 7563 6375 6c65 6e74 2d63 6f6e 7461 696e  ucculent-contain
+00000d50: 6572 0d0a 6060 600d 0a0d 0a41 6c74 6572  er..```....Alter
+00000d60: 6e61 7469 7665 6c79 2c20 796f 7520 6361  natively, you ca
+00000d70: 6e20 7573 6520 6060 646f 636b 6572 2d63  n use ``docker-c
+00000d80: 6f6d 706f 7365 6060 3a0d 0a60 6060 6261  ompose``:..```ba
+00000d90: 7368 0d0a 646f 636b 6572 2063 6f6d 706f  sh..docker compo
+00000da0: 7365 2075 700d 0a60 6060 0d0a 0d0a 2323  se up..```....##
+00000db0: 2055 7361 6765 0d0a 0d0a 2323 2320 4578   Usage....### Ex
+00000dc0: 616d 706c 650d 0a0d 0a60 6060 7079 7468  ample....```pyth
+00000dd0: 6f6e 0d0a 6672 6f6d 2073 7563 6375 6c65  on..from succule
+00000de0: 6e74 2e61 7069 2069 6d70 6f72 7420 5375  nt.api import Su
+00000df0: 6363 756c 656e 7441 5049 0d0a 6170 6920  cculentAPI..api 
+00000e00: 3d20 5375 6363 756c 656e 7441 5049 2868  = SucculentAPI(h
+00000e10: 6f73 743d 2730 2e30 2e30 2e30 272c 2070  ost='0.0.0.0', p
+00000e20: 6f72 743d 3830 3830 2c20 636f 6e66 6967  ort=8080, config
+00000e30: 3d27 636f 6e66 6967 7572 6174 696f 6e2e  ='configuration.
+00000e40: 796d 6c27 2c20 666f 726d 6174 3d27 6373  yml', format='cs
+00000e50: 7627 290d 0a61 7069 2e73 7461 7274 2829  v')..api.start()
+00000e60: 0d0a 6060 600d 0a0d 0a23 2320 436f 6e66  ..```....## Conf
+00000e70: 6967 7572 6174 696f 6e0d 0a49 6e20 7468  iguration..In th
+00000e80: 6520 726f 6f74 2064 6972 6563 746f 7279  e root directory
+00000e90: 2c20 6372 6561 7465 2061 2066 696c 6520  , create a file 
+00000ea0: 6e61 6d65 6420 6063 6f6e 6669 6775 7261  named `configura
+00000eb0: 7469 6f6e 2e79 6d6c 6020 616e 6420 6465  tion.yml` and de
+00000ec0: 6669 6e65 2074 6865 2066 6f6c 6c6f 7769  fine the followi
+00000ed0: 6e67 3a0d 0a60 6060 796d 6c0d 0a64 6174  ng:..```yml..dat
+00000ee0: 613a 0d0a 2020 2d20 6e61 6d65 3a20 2320  a:..  - name: # 
+00000ef0: 4d65 6173 7572 6520 6e61 6d65 0d0a 2020  Measure name..  
+00000f00: 2020 6d69 6e3a 2023 204d 696e 696d 756d    min: # Minimum
+00000f10: 2076 616c 7565 2028 6f70 7469 6f6e 616c   value (optional
+00000f20: 290d 0a20 2020 206d 6178 3a20 2320 4d61  )..    max: # Ma
+00000f30: 7869 6d75 6d20 7661 6c75 6520 286f 7074  ximum value (opt
+00000f40: 696f 6e61 6c29 0d0a 6060 600d 0a0d 0a23  ional)..```....#
+00000f50: 2320 4c69 6365 6e73 650d 0a0d 0a54 6869  # License....Thi
+00000f60: 7320 7061 636b 6167 6520 6973 2064 6973  s package is dis
+00000f70: 7472 6962 7574 6564 2075 6e64 6572 2074  tributed under t
+00000f80: 6865 204d 4954 204c 6963 656e 7365 2e20  he MIT License. 
+00000f90: 5468 6973 206c 6963 656e 7365 2063 616e  This license can
+00000fa0: 2062 6520 666f 756e 6420 6f6e 6c69 6e65   be found online
+00000fb0: 2061 7420 3c68 7474 703a 2f2f 7777 772e   at <http://www.
+00000fc0: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+00000fd0: 6963 656e 7365 732f 4d49 543e 2e0d 0a0d  icenses/MIT>....
+00000fe0: 0a23 2320 4469 7363 6c61 696d 6572 0d0a  .## Disclaimer..
+00000ff0: 0d0a 5468 6973 2066 7261 6d65 776f 726b  ..This framework
+00001000: 2069 7320 7072 6f76 6964 6564 2061 732d   is provided as-
+00001010: 6973 2c20 616e 6420 7468 6572 6520 6172  is, and there ar
+00001020: 6520 6e6f 2067 7561 7261 6e74 6565 7320  e no guarantees 
+00001030: 7468 6174 2069 7420 6669 7473 2079 6f75  that it fits you
+00001040: 7220 7075 7270 6f73 6573 206f 7220 7468  r purposes or th
+00001050: 6174 2069 7420 6973 2062 7567 2d66 7265  at it is bug-fre
+00001060: 652e 2055 7365 2069 7420 6174 2079 6f75  e. Use it at you
+00001070: 7220 6f77 6e20 7269 736b 210d 0a0d 0a23  r own risk!....#
+00001080: 2320 436f 6e74 7269 6275 746f 7273 20e2  # Contributors .
+00001090: 9ca8 0d0a 0d0a 5468 616e 6b73 2067 6f65  ......Thanks goe
+000010a0: 7320 746f 2074 6865 7365 2077 6f6e 6465  s to these wonde
+000010b0: 7266 756c 2070 656f 706c 6520 285b 656d  rful people ([em
+000010c0: 6f6a 6920 6b65 795d 2868 7474 7073 3a2f  oji key](https:/
+000010d0: 2f61 6c6c 636f 6e74 7269 6275 746f 7273  /allcontributors
+000010e0: 2e6f 7267 2f64 6f63 732f 656e 2f65 6d6f  .org/docs/en/emo
+000010f0: 6a69 2d6b 6579 2929 3a0d 0a0d 0a3c 212d  ji-key)):....<!-
+00001100: 2d20 414c 4c2d 434f 4e54 5249 4255 544f  - ALL-CONTRIBUTO
+00001110: 5253 2d4c 4953 543a 5354 4152 5420 2d20  RS-LIST:START - 
+00001120: 446f 206e 6f74 2072 656d 6f76 6520 6f72  Do not remove or
+00001130: 206d 6f64 6966 7920 7468 6973 2073 6563   modify this sec
+00001140: 7469 6f6e 202d 2d3e 0d0a 3c21 2d2d 2070  tion -->..<!-- p
+00001150: 7265 7474 6965 722d 6967 6e6f 7265 2d73  rettier-ignore-s
+00001160: 7461 7274 202d 2d3e 0d0a 3c21 2d2d 206d  tart -->..<!-- m
+00001170: 6172 6b64 6f77 6e6c 696e 742d 6469 7361  arkdownlint-disa
+00001180: 626c 6520 2d2d 3e0d 0a3c 7461 626c 653e  ble -->..<table>
+00001190: 0d0a 2020 3c74 626f 6479 3e0d 0a20 2020  ..  <tbody>..   
+000011a0: 203c 7472 3e0d 0a20 2020 2020 203c 7464   <tr>..      <td
+000011b0: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
+000011c0: 7661 6c69 676e 3d22 746f 7022 2077 6964  valign="top" wid
+000011d0: 7468 3d22 3134 2e32 3825 223e 3c61 2068  th="14.28%"><a h
+000011e0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+000011f0: 6875 622e 636f 6d2f 6c61 686f 766e 696b  hub.com/lahovnik
+00001200: 7461 6465 6a22 3e3c 696d 6720 7372 633d  tadej"><img src=
+00001210: 2268 7474 7073 3a2f 2f61 7661 7461 7273  "https://avatars
+00001220: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00001230: 6e74 2e63 6f6d 2f75 2f35 3738 3930 3733  nt.com/u/5789073
+00001240: 343f 763d 343f 733d 3130 3022 2077 6964  4?v=4?s=100" wid
+00001250: 7468 3d22 3130 3070 783b 2220 616c 743d  th="100px;" alt=
+00001260: 2254 6164 656a 204c 6168 6f76 6e69 6b22  "Tadej Lahovnik"
+00001270: 2f3e 3c62 7220 2f3e 3c73 7562 3e3c 623e  /><br /><sub><b>
+00001280: 5461 6465 6a20 4c61 686f 766e 696b 3c2f  Tadej Lahovnik</
+00001290: 623e 3c2f 7375 623e 3c2f 613e 3c62 7220  b></sub></a><br 
+000012a0: 2f3e 3c61 2068 7265 663d 2268 7474 7073  /><a href="https
+000012b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6669  ://github.com/fi
+000012c0: 7265 666c 792d 6370 702f 7375 6363 756c  refly-cpp/succul
+000012d0: 656e 742f 636f 6d6d 6974 733f 6175 7468  ent/commits?auth
+000012e0: 6f72 3d6c 6168 6f76 6e69 6b74 6164 656a  or=lahovniktadej
+000012f0: 2220 7469 746c 653d 2243 6f64 6522 3ef0  " title="Code">.
+00001300: 9f92 bb3c 2f61 3e20 3c61 2068 7265 663d  ...</a> <a href=
+00001310: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001320: 636f 6d2f 6669 7265 666c 792d 6370 702f  com/firefly-cpp/
+00001330: 7375 6363 756c 656e 742f 6973 7375 6573  succulent/issues
+00001340: 3f71 3d61 7574 686f 7225 3341 6c61 686f  ?q=author%3Alaho
+00001350: 766e 696b 7461 6465 6a22 2074 6974 6c65  vniktadej" title
+00001360: 3d22 4275 6720 7265 706f 7274 7322 3ef0  ="Bug reports">.
+00001370: 9f90 9b3c 2f61 3e20 3c61 2068 7265 663d  ...</a> <a href=
+00001380: 2223 6964 6561 732d 6c61 686f 766e 696b  "#ideas-lahovnik
+00001390: 7461 6465 6a22 2074 6974 6c65 3d22 4964  tadej" title="Id
+000013a0: 6561 732c 2050 6c61 6e6e 696e 672c 2026  eas, Planning, &
+000013b0: 2046 6565 6462 6163 6b22 3ef0 9fa4 943c   Feedback">....<
+000013c0: 2f61 3e20 3c61 2068 7265 663d 2268 7474  /a> <a href="htt
+000013d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000013e0: 6669 7265 666c 792d 6370 702f 7375 6363  firefly-cpp/succ
+000013f0: 756c 656e 742f 636f 6d6d 6974 733f 6175  ulent/commits?au
+00001400: 7468 6f72 3d6c 6168 6f76 6e69 6b74 6164  thor=lahovniktad
+00001410: 656a 2220 7469 746c 653d 2244 6f63 756d  ej" title="Docum
+00001420: 656e 7461 7469 6f6e 223e f09f 9396 3c2f  entation">....</
+00001430: 613e 3c2f 7464 3e0d 0a20 2020 2020 203c  a></td>..      <
+00001440: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00001450: 2220 7661 6c69 676e 3d22 746f 7022 2077  " valign="top" w
+00001460: 6964 7468 3d22 3134 2e32 3825 223e 3c61  idth="14.28%"><a
+00001470: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00001480: 6974 6875 622e 636f 6d2f 4179 616e 4461  ithub.com/AyanDa
+00001490: 7333 3438 223e 3c69 6d67 2073 7263 3d22  s348"><img src="
+000014a0: 6874 7470 733a 2f2f 6176 6174 6172 732e  https://avatars.
+000014b0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+000014c0: 742e 636f 6d2f 752f 3533 3631 3036 3236  t.com/u/53610626
+000014d0: 3f76 3d34 3f73 3d31 3030 2220 7769 6474  ?v=4?s=100" widt
+000014e0: 683d 2231 3030 7078 3b22 2061 6c74 3d22  h="100px;" alt="
+000014f0: 4179 616e 2044 6173 222f 3e3c 6272 202f  Ayan Das"/><br /
+00001500: 3e3c 7375 623e 3c62 3e41 7961 6e20 4461  ><sub><b>Ayan Da
+00001510: 733c 2f62 3e3c 2f73 7562 3e3c 2f61 3e3c  s</b></sub></a><
+00001520: 6272 202f 3e3c 6120 6872 6566 3d22 6874  br /><a href="ht
+00001530: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001540: 2f66 6972 6566 6c79 2d63 7070 2f73 7563  /firefly-cpp/suc
+00001550: 6375 6c65 6e74 2f63 6f6d 6d69 7473 3f61  culent/commits?a
+00001560: 7574 686f 723d 4179 616e 4461 7333 3438  uthor=AyanDas348
+00001570: 2220 7469 746c 653d 2243 6f64 6522 3ef0  " title="Code">.
+00001580: 9f92 bb3c 2f61 3e20 3c61 2068 7265 663d  ...</a> <a href=
+00001590: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000015a0: 636f 6d2f 6669 7265 666c 792d 6370 702f  com/firefly-cpp/
+000015b0: 7375 6363 756c 656e 742f 636f 6d6d 6974  succulent/commit
+000015c0: 733f 6175 7468 6f72 3d41 7961 6e44 6173  s?author=AyanDas
+000015d0: 3334 3822 2074 6974 6c65 3d22 5465 7374  348" title="Test
+000015e0: 7322 3ee2 9aa0 efb8 8f3c 2f61 3e3c 2f74  s">......</a></t
+000015f0: 643e 0d0a 2020 2020 2020 3c74 6420 616c  d>..      <td al
+00001600: 6967 6e3d 2263 656e 7465 7222 2076 616c  ign="center" val
+00001610: 6967 6e3d 2274 6f70 2220 7769 6474 683d  ign="top" width=
+00001620: 2231 342e 3238 2522 3e3c 6120 6872 6566  "14.28%"><a href
+00001630: 3d22 6874 7470 3a2f 2f77 7777 2e69 7a74  ="http://www.izt
+00001640: 6f6b 2d6a 722d 6669 7374 6572 2e65 752f  ok-jr-fister.eu/
+00001650: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001660: 733a 2f2f 6176 6174 6172 732e 6769 7468  s://avatars.gith
+00001670: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00001680: 6d2f 752f 3136 3333 3336 313f 763d 343f  m/u/1633361?v=4?
+00001690: 733d 3130 3022 2077 6964 7468 3d22 3130  s=100" width="10
+000016a0: 3070 783b 2220 616c 743d 2249 7a74 6f6b  0px;" alt="Iztok
+000016b0: 2046 6973 7465 7220 4a72 2e22 2f3e 3c62   Fister Jr."/><b
+000016c0: 7220 2f3e 3c73 7562 3e3c 623e 497a 746f  r /><sub><b>Izto
+000016d0: 6b20 4669 7374 6572 204a 722e 3c2f 623e  k Fister Jr.</b>
+000016e0: 3c2f 7375 623e 3c2f 613e 3c62 7220 2f3e  </sub></a><br />
+000016f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001700: 2f67 6974 6875 622e 636f 6d2f 6669 7265  /github.com/fire
+00001710: 666c 792d 6370 702f 7375 6363 756c 656e  fly-cpp/succulen
+00001720: 742f 636f 6d6d 6974 733f 6175 7468 6f72  t/commits?author
+00001730: 3d66 6972 6566 6c79 2d63 7070 2220 7469  =firefly-cpp" ti
+00001740: 746c 653d 2243 6f64 6522 3ef0 9f92 bb3c  tle="Code">....<
+00001750: 2f61 3e20 3c61 2068 7265 663d 2223 6964  /a> <a href="#id
+00001760: 6561 732d 6669 7265 666c 792d 6370 7022  eas-firefly-cpp"
+00001770: 2074 6974 6c65 3d22 4964 6561 732c 2050   title="Ideas, P
+00001780: 6c61 6e6e 696e 672c 2026 2046 6565 6462  lanning, & Feedb
+00001790: 6163 6b22 3ef0 9fa4 943c 2f61 3e20 3c61  ack">....</a> <a
+000017a0: 2068 7265 663d 2223 6d65 6e74 6f72 696e   href="#mentorin
+000017b0: 672d 6669 7265 666c 792d 6370 7022 2074  g-firefly-cpp" t
+000017c0: 6974 6c65 3d22 4d65 6e74 6f72 696e 6722  itle="Mentoring"
+000017d0: 3ef0 9fa7 91e2 808d f09f 8fab 3c2f 613e  >...........</a>
+000017e0: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+000017f0: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
+00001800: 7661 6c69 676e 3d22 746f 7022 2077 6964  valign="top" wid
+00001810: 7468 3d22 3134 2e32 3825 223e 3c61 2068  th="14.28%"><a h
+00001820: 7265 663d 2268 7474 703a 2f2f 6361 726c  ref="http://carl
+00001830: 6f73 616c 3130 3135 2e67 6974 6875 622e  osal1015.github.
+00001840: 696f 223e 3c69 6d67 2073 7263 3d22 6874  io"><img src="ht
+00001850: 7470 733a 2f2f 6176 6174 6172 732e 6769  tps://avatars.gi
+00001860: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00001870: 636f 6d2f 752f 3231 3238 3330 3134 3f76  com/u/21283014?v
+00001880: 3d34 3f73 3d31 3030 2220 7769 6474 683d  =4?s=100" width=
+00001890: 2231 3030 7078 3b22 2061 6c74 3d22 4f72  "100px;" alt="Or
+000018a0: 6f6d 696f 6e22 2f3e 3c62 7220 2f3e 3c73  omion"/><br /><s
+000018b0: 7562 3e3c 623e 4f72 6f6d 696f 6e3c 2f62  ub><b>Oromion</b
+000018c0: 3e3c 2f73 7562 3e3c 2f61 3e3c 6272 202f  ></sub></a><br /
+000018d0: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+000018e0: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6972  //github.com/fir
+000018f0: 6566 6c79 2d63 7070 2f73 7563 6375 6c65  efly-cpp/succule
+00001900: 6e74 2f69 7373 7565 733f 713d 6175 7468  nt/issues?q=auth
+00001910: 6f72 2533 4163 6172 6c6f 7361 6c31 3031  or%3Acarlosal101
+00001920: 3522 2074 6974 6c65 3d22 4275 6720 7265  5" title="Bug re
+00001930: 706f 7274 7322 3ef0 9f90 9b3c 2f61 3e20  ports">....</a> 
+00001940: 3c61 2068 7265 663d 2223 706c 6174 666f  <a href="#platfo
+00001950: 726d 2d63 6172 6c6f 7361 6c31 3031 3522  rm-carlosal1015"
+00001960: 2074 6974 6c65 3d22 5061 636b 6167 696e   title="Packagin
+00001970: 672f 706f 7274 696e 6720 746f 206e 6577  g/porting to new
+00001980: 2070 6c61 7466 6f72 6d22 3ef0 9f93 a63c   platform">....<
+00001990: 2f61 3e3c 2f74 643e 0d0a 2020 2020 3c2f  /a></td>..    </
+000019a0: 7472 3e0d 0a20 203c 2f74 626f 6479 3e0d  tr>..  </tbody>.
+000019b0: 0a3c 2f74 6162 6c65 3e0d 0a0d 0a3c 212d  .</table>....<!-
+000019c0: 2d20 6d61 726b 646f 776e 6c69 6e74 2d72  - markdownlint-r
+000019d0: 6573 746f 7265 202d 2d3e 0d0a 3c21 2d2d  estore -->..<!--
+000019e0: 2070 7265 7474 6965 722d 6967 6e6f 7265   prettier-ignore
+000019f0: 2d65 6e64 202d 2d3e 0d0a 0d0a 3c21 2d2d  -end -->....<!--
+00001a00: 2041 4c4c 2d43 4f4e 5452 4942 5554 4f52   ALL-CONTRIBUTOR
+00001a10: 532d 4c49 5354 3a45 4e44 202d 2d3e 0d0a  S-LIST:END -->..
+00001a20: 0d0a 5468 6973 2070 726f 6a65 6374 2066  ..This project f
+00001a30: 6f6c 6c6f 7773 2074 6865 205b 616c 6c2d  ollows the [all-
+00001a40: 636f 6e74 7269 6275 746f 7273 5d28 6874  contributors](ht
+00001a50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001a60: 2f61 6c6c 2d63 6f6e 7472 6962 7574 6f72  /all-contributor
+00001a70: 732f 616c 6c2d 636f 6e74 7269 6275 746f  s/all-contributo
+00001a80: 7273 2920 7370 6563 6966 6963 6174 696f  rs) specificatio
+00001a90: 6e2e 2043 6f6e 7472 6962 7574 696f 6e73  n. Contributions
+00001aa0: 206f 6620 616e 7920 6b69 6e64 2077 656c   of any kind wel
+00001ab0: 636f 6d65 210d 0a                        come!..
```

### Comparing `succulent-0.1.4/succulent/api.py` & `succulent-0.2.0/succulent/api.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from flask import Flask, jsonify, request
-from succulent.configuration import Configuration
-from succulent.processing import Processing
-from datetime import datetime
-
-class SucculentAPI:
-    def __init__(self, host, port, config, format='csv'):
-        self.host = host
-        self.port = port
-        self.format = format
-
-        # Configuration file
-        conf = Configuration(config)
-        self.config = conf.load_config()
-
-        # Initialise processing
-        self.processing = Processing(self.config['data'], self.format)
-
-        # Initialise Flask
-        self.app = Flask(__name__)
-        self.app.add_url_rule('/measure', 'url', self.url, methods=['GET'])
-        self.app.add_url_rule('/measure', 'measure', self.measure, methods=['POST'])
-
-    def url(self):
-        # Generate URL
-        parameters = self.processing.parameters()
-
-        # Send response
-        return jsonify({'url': f'{self.host}:{self.port}/measure?{parameters}'}), 200
-
-    def measure(self):
-        try:
-            # Process request
-            self.processing.process(request)
-            
-            # Collect and store timestamp
-            timestamp = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            # You can store the timestamp in a database, file, or any other desired storage mechanism.
-            # Example: database.insert_timestamp(timestamp)
-        except ValueError as err:
-            # Invalid file type
-            return jsonify({'message': str(err)}), 400
-
-        # Send response
-        return jsonify({'message': 'Data stored', 'timestamp': timestamp}), 200
-
-    def start(self):
+from flask import Flask, jsonify, request
+from succulent.configuration import Configuration
+from succulent.processing import Processing
+from datetime import datetime
+
+class SucculentAPI:
+    def __init__(self, host, port, config, format='csv'):
+        self.host = host
+        self.port = port
+        self.format = format
+
+        # Configuration file
+        conf = Configuration(config)
+        self.config = conf.load_config()
+
+        # Initialise processing
+        self.processing = Processing(self.config['data'], self.format)
+
+        # Initialise Flask
+        self.app = Flask(__name__)
+        self.app.add_url_rule('/measure', 'url', self.url, methods=['GET'])
+        self.app.add_url_rule('/measure', 'measure', self.measure, methods=['POST'])
+
+    def url(self):
+        # Generate URL
+        parameters = self.processing.parameters()
+
+        # Send response
+        return jsonify({'url': f'{self.host}:{self.port}/measure?{parameters}'}), 200
+
+    def measure(self):
+        try:
+            # Process request
+            self.processing.process(request)
+            
+            # Collect and store timestamp
+            timestamp = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+            # You can store the timestamp in a database, file, or any other desired storage mechanism.
+            # Example: database.insert_timestamp(timestamp)
+        except ValueError as err:
+            # Invalid file type
+            return jsonify({'message': str(err)}), 400
+
+        # Send response
+        return jsonify({'message': 'Data stored', 'timestamp': timestamp}), 200
+
+    def start(self):
         self.app.run(host=self.host, port=self.port)
```

### Comparing `succulent-0.1.4/succulent/processing.py` & `succulent-0.2.0/succulent/processing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,94 @@
-import os
-import sqlite3
-import inspect
-import pandas as pd
-
-class Processing:
-    def __init__(self, config, format):
-        # Validate format
-        if format not in ['csv', 'json', 'sqlite']:
-            raise ValueError(f'Invalid format: {format}')
-        
-        # Initialise attributes
-        self.directory = os.path.join(os.path.dirname(os.path.abspath(inspect.stack()[2].filename)), 'data')
-        self.format = format
-        self.columns = [configuration['name'] for configuration in config]
-        self.boundaries = [{ 
-            configuration['name']: {
-                key: configuration[key]
-                for key in ['min', 'max']
-                if key in configuration
-            }
-        } for configuration in config if configuration.get('min') is not None or configuration.get('max') is not None]
-        self.df = None  # Initialize df attribute
-    
-    def parameters(self):
-        parameters = [f'{column}=' for column in self.columns]
-        parameters = '&'.join(parameters)
-        return parameters
-    
-    def boundary(self, value, boundary, column):
-        if 'min' in boundary and float(value) < float(boundary['min']):
-            raise ValueError(f'{column} ({value}) is lower than the specified minimum ({boundary["min"]}).')
-        if 'max' in boundary and float(value) > float(boundary['max']):
-            raise ValueError(f'{column} ({value}) is greater than the specified maximum ({boundary["max"]}).')
-        return value
-        
-    def process(self, req):
-        # Directory preparation
-        if not os.path.exists(self.directory):
-            os.makedirs(self.directory)
-
-        # Define paths
-        path = os.path.join(
-            self.directory, f'data.{self.format}'
-        )
-
-        # Load existing data
-        if os.path.exists(path):
-            if self.format == 'csv':
-                self.df = pd.read_csv(path, sep=',')
-            elif self.format == 'json':
-                self.df = pd.read_json(path, orient='records')
-            elif self.format == 'sqlite':
-                conn = sqlite3.connect(path)
-                self.df = pd.read_sql_query("SELECT * FROM data", conn)
-                conn.close()
-            else:
-                raise ValueError(f'Invalid file type: {self.format}')
-        # Initialise new data
-        else:
-            self.df = pd.DataFrame(columns=self.columns)
-
-        # Parse data from request
-        data = {}
-        for column in self.columns:
-            # Request type
-            if req.is_json:
-                value = req.json[column] if column in req.json else None
-            else:
-                value = req.args.get(column, default=None)
-
-            # Boundary check
-            if column in [list(boundaries.keys())[0] for boundaries in self.boundaries]:
-                index = [list(boundaries.keys())[0] for boundaries in self.boundaries].index(column)
-                data[column] = self.boundary(value, self.boundaries[index][column], column)
-            else:
-                data[column] = value
-
-        # Convert data to Series
-        data = pd.Series(data, index=self.columns)
-
-        # Merge data
-        self.df = pd.concat([self.df, data.to_frame().T], ignore_index=True)
-
-        # Store data to device
-        if self.format == 'csv':
-            self.df.to_csv(path, sep=',', index=False)
-        elif self.format == 'json':
-            self.df.to_json(path, orient='records', indent=4)
-        elif self.format == 'sqlite':
-            conn = sqlite3.connect(path)
-            self.df.to_sql('data', conn, if_exists='replace', index=False)
+import os
+import sqlite3
+import inspect
+import pandas as pd
+
+class Processing:
+    def __init__(self, config, format, unittest=True):
+        # Validate format
+        if format not in ['csv', 'json', 'sqlite']:
+            raise ValueError(f'Invalid format: {format}')
+        
+        # Initialise attributes
+        index = 1 if unittest else 2
+        self.directory = os.path.join(os.path.dirname(os.path.abspath(inspect.stack()[index].filename)), 'data')
+        self.format = format
+        self.columns = [configuration['name'] for configuration in config]
+        self.boundaries = [{ 
+            configuration['name']: {
+                key: configuration[key]
+                for key in ['min', 'max']
+                if key in configuration
+            }
+        } for configuration in config if configuration.get('min') is not None or configuration.get('max') is not None]
+        self.df = None  # Initialize df attribute
+    
+    def parameters(self):
+        parameters = [f'{column}=' for column in self.columns]
+        parameters = '&'.join(parameters)
+        return parameters
+    
+    def boundary(self, value, boundary, column):
+        if 'min' in boundary and float(value) < float(boundary['min']):
+            raise ValueError(f'{column} ({value}) is lower than the specified minimum ({boundary["min"]}).')
+        if 'max' in boundary and float(value) > float(boundary['max']):
+            raise ValueError(f'{column} ({value}) is greater than the specified maximum ({boundary["max"]}).')
+        return value
+        
+    def process(self, req):
+        # Directory preparation
+        if not os.path.exists(self.directory):
+            os.makedirs(self.directory)
+
+        # Define paths
+        path = os.path.join(
+            self.directory, f'data.{self.format}'
+        )
+
+        # Load existing data
+        if os.path.exists(path):
+            if self.format == 'csv':
+                self.df = pd.read_csv(path, sep=',')
+            elif self.format == 'json':
+                self.df = pd.read_json(path, orient='records')
+            elif self.format == 'sqlite':
+                conn = sqlite3.connect(path)
+                self.df = pd.read_sql_query("SELECT * FROM data", conn)
+                conn.close()
+            else:
+                raise ValueError(f'Invalid file type: {self.format}')
+        # Initialise new data
+        else:
+            self.df = pd.DataFrame(columns=self.columns)
+
+        # Parse data from request
+        data = {}
+        for column in self.columns:
+            # Request type
+            if req.is_json:
+                value = req.json[column] if column in req.json else None
+            else:
+                value = req.args.get(column, default=None)
+
+            # Boundary check
+            if column in [list(boundaries.keys())[0] for boundaries in self.boundaries]:
+                index = [list(boundaries.keys())[0] for boundaries in self.boundaries].index(column)
+                data[column] = self.boundary(value, self.boundaries[index][column], column)
+            else:
+                data[column] = value
+
+        # Convert data to Series
+        data = pd.Series(data, index=self.columns)
+
+        # Merge data
+        self.df = pd.concat([self.df, data.to_frame().T], ignore_index=True)
+
+        # Store data to device
+        if self.format == 'csv':
+            self.df.to_csv(path, sep=',', index=False)
+        elif self.format == 'json':
+            self.df.to_json(path, orient='records', indent=4)
+        elif self.format == 'sqlite':
+            conn = sqlite3.connect(path)
+            self.df.to_sql('data', conn, if_exists='replace', index=False)
             conn.close()
```

### Comparing `succulent-0.1.4/PKG-INFO` & `succulent-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: succulent
-Version: 0.1.4
+Version: 0.2.0
 Summary: Collect POST requests easily
 Home-page: https://github.com/firefly-cpp/succulent
 License: MIT
 Keywords: data collection,data science,sensor measurements
 Author: Iztok Fister Jr.
 Author-email: iztok@iztok-jr-fister.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/firefly-cpp/succulent
 Description-Content-Type: text/markdown
 
 ---
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 # succulent - Collect POST requests easily
 
 ---
 ![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)
@@ -43,14 +42,15 @@
 
 ## Detailed insights
 The current version includes (but is not limited to) the following functions:
 
 - Request URL generation for data collection
 - Data collection from POST requests
 - Storing data in different formats (CSV, JSON, SQLite)
+- Defining boundaries for collected data (min, max)
 
 ## Installation
 
 ### pip
 
 Install succulent with pip:
 
@@ -65,14 +65,39 @@
 $ apk add py3-succulent
 ```
 
 ## Container
 
 [Basic container for succulent](https://github.com/firefly-cpp/succulent-container)
 
+### Configuration
+Follow the instructions in the [configuration](##configuration) section to define the configuration file.
+
+### Installation
+Build the container using Docker:
+```bash
+docker build -t succulent-container .
+```
+
+Alternatively, you can use ``docker-compose``:
+```bash
+docker compose build
+```
+
+### Usage
+Run the container using Docker:
+```bash
+docker run -p 8080:8080 succulent-container
+```
+
+Alternatively, you can use ``docker-compose``:
+```bash
+docker compose up
+```
+
 ## Usage
 
 ### Example
 
 ```python
 from succulent.api import SucculentAPI
 api = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml', format='csv')
@@ -105,14 +130,15 @@
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lahovniktadej"><img src="https://avatars.githubusercontent.com/u/57890734?v=4?s=100" width="100px;" alt="Tadej Lahovnik"/><br /><sub><b>Tadej Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Alahovniktadej" title="Bug reports">🐛</a> <a href="#ideas-lahovniktadej" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/AyanDas348"><img src="https://avatars.githubusercontent.com/u/53610626?v=4?s=100" width="100px;" alt="Ayan Das"/><br /><sub><b>Ayan Das</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=firefly-cpp" title="Code">💻</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Acarlosal1015" title="Bug reports">🐛</a> <a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

