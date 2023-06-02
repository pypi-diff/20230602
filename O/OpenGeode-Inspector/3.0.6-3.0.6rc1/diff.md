# Comparing `tmp/OpenGeode_Inspector-3.0.6-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Inspector-3.0.6rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 264326 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      175 b- defN 23-Jun-02 09:17 opengeode_inspector/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-Jun-02 09:17 opengeode_inspector/inspector.py
--rw-rw-rw-  2.0 fat   439808 b- defN 23-Jun-02 09:18 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
--rw-rw-rw-  2.0 fat   451072 b- defN 23-Jun-02 09:18 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     5481 b- defN 23-Jun-02 09:18 OpenGeode_Inspector-3.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-02 09:18 OpenGeode_Inspector-3.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jun-02 09:18 OpenGeode_Inspector-3.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      772 b- defN 23-Jun-02 09:18 OpenGeode_Inspector-3.0.6.dist-info/RECORD
-8 files, 897699 bytes uncompressed, 262954 bytes compressed:  70.7%
+Zip file size: 264355 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      175 b- defN 23-May-25 12:58 opengeode_inspector/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-May-25 12:58 opengeode_inspector/inspector.py
+-rw-rw-rw-  2.0 fat   439808 b- defN 23-May-25 13:00 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
+-rw-rw-rw-  2.0 fat   451072 b- defN 23-May-25 13:00 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     5483 b- defN 23-May-25 13:00 OpenGeode_Inspector-3.0.6rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-25 13:00 OpenGeode_Inspector-3.0.6rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-May-25 13:00 OpenGeode_Inspector-3.0.6rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      784 b- defN 23-May-25 13:00 OpenGeode_Inspector-3.0.6rc1.dist-info/RECORD
+8 files, 897713 bytes uncompressed, 262959 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
 Comment: 
 
 Filename: opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.6.dist-info/METADATA
+Filename: OpenGeode_Inspector-3.0.6rc1.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.6.dist-info/WHEEL
+Filename: OpenGeode_Inspector-3.0.6rc1.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.6.dist-info/top_level.txt
+Filename: OpenGeode_Inspector-3.0.6rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.6.dist-info/RECORD
+Filename: OpenGeode_Inspector-3.0.6rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180049d50
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jun  2 09:18:20 2023
+Time/Date		Thu May 25 12:59:27 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000004c200
 SizeOfInitializedData	000000000001f000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000049d50
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00070000
 SizeOfHeaders		00000400
-CheckSum		00077cf3
+CheckSum		0006cc83
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -277,22 +277,22 @@
  00064994	00064c08 00000000 00000000 00068b7c 0004e158
 
 	DLL Name: OpenGeode_basic.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	6894e	  141  ?instance@Singleton@geode@@CAPEAV12@AEBVtype_info@@@Z
 	68b5a	   71  ??Muuid@geode@@QEBA_NAEBU01@@Z
 	68af8	  154  ?log_warn@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
-	68a9a	  201  ?string@uuid@geode@@QEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
+	68a9a	  200  ?string@uuid@geode@@QEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
 	68a78	   69  ??8uuid@geode@@QEBA_NAEBU01@@Z
 	68a4e	  127  ?id@Identifier@geode@@QEBAAEBUuuid@2@XZ
 	689ec	  152  ?log_info@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
 	689be	   89  ?call_initialize@Library@geode@@IEAAXPEBD@Z
 	689a2	   26  ??0Library@geode@@IEAA@XZ
 	68986	   49  ??1Library@geode@@UEAA@XZ
-	68910	  194  ?set_instance@Singleton@geode@@CAXAEBVtype_info@@PEAV12@@Z
+	68910	  193  ?set_instance@Singleton@geode@@CAXAEBVtype_info@@PEAV12@@Z
 
  000649a8	00065330 00000000 00000000 00068be0 0004e880
 
 	DLL Name: absl_hash.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	68b90	   12  ?CombineLargeContiguousImpl64@CityHashState@hash_internal@absl@@CA_K_KPEBE0@Z
 
@@ -13427,15 +13427,15 @@
 	  11d60: 6e 74 5f 74 72 69 61 6e 67 6c 65 5f 70 6f 73 69
 	  11d70: 74 69 6f 6e 40 24 30 32 40 67 65 6f 64 65 40 40
 	  11d80: 59 41 3f 41 57 34 50 6f 73 69 74 69 6f 6e 40 30
 	  11d90: 40 41 45 42 56 3f 24 50 6f 69 6e 74 40 24 30 32
 	  11da0: 40 30 40 41 45 42 56 3f 24 54 72 69 61 6e 67 6c
 	  11db0: 65 40 24 30 32 40 30 40 40 5a 00 00 4f 70 65 6e
 	  11dc0: 47 65 6f 64 65 5f 67 65 6f 6d 65 74 72 79 2e 64
-	  11dd0: 6c 6c 00 00 c2 00 3f 73 65 74 5f 69 6e 73 74 61
+	  11dd0: 6c 6c 00 00 c1 00 3f 73 65 74 5f 69 6e 73 74 61
 	  11de0: 6e 63 65 40 53 69 6e 67 6c 65 74 6f 6e 40 67 65
 	  11df0: 6f 64 65 40 40 43 41 58 41 45 42 56 74 79 70 65
 	  11e00: 5f 69 6e 66 6f 40 40 50 45 41 56 31 32 40 40 5a
 	  11e10: 00 00 8d 00 3f 69 6e 73 74 61 6e 63 65 40 53 69
 	  11e20: 6e 67 6c 65 74 6f 6e 40 67 65 6f 64 65 40 40 43
 	  11e30: 41 50 45 41 56 31 32 40 41 45 42 56 74 79 70 65
 	  11e40: 5f 69 6e 66 6f 40 40 40 5a 00 31 00 3f 3f 31 4c
@@ -13451,15 +13451,15 @@
 	  11ee0: 44 55 3f 24 63 68 61 72 5f 74 72 61 69 74 73 40
 	  11ef0: 44 40 73 74 64 40 40 56 3f 24 61 6c 6c 6f 63 61
 	  11f00: 74 6f 72 40 44 40 32 40 40 73 74 64 40 40 40 5a
 	  11f10: 00 00 7f 00 3f 69 64 40 49 64 65 6e 74 69 66 69
 	  11f20: 65 72 40 67 65 6f 64 65 40 40 51 45 42 41 41 45
 	  11f30: 42 55 75 75 69 64 40 32 40 58 5a 00 45 00 3f 3f
 	  11f40: 38 75 75 69 64 40 67 65 6f 64 65 40 40 51 45 42
-	  11f50: 41 5f 4e 41 45 42 55 30 31 40 40 5a 00 00 c9 00
+	  11f50: 41 5f 4e 41 45 42 55 30 31 40 40 5a 00 00 c8 00
 	  11f60: 3f 73 74 72 69 6e 67 40 75 75 69 64 40 67 65 6f
 	  11f70: 64 65 40 40 51 45 42 41 3f 41 56 3f 24 62 61 73
 	  11f80: 69 63 5f 73 74 72 69 6e 67 40 44 55 3f 24 63 68
 	  11f90: 61 72 5f 74 72 61 69 74 73 40 44 40 73 74 64 40
 	  11fa0: 40 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40 44 40
 	  11fb0: 32 40 40 73 74 64 40 40 58 5a 00 00 9a 00 3f 6c
 	  11fc0: 6f 67 5f 77 61 72 6e 40 4c 6f 67 67 65 72 40 67
@@ -101966,15 +101966,18 @@
    18005015a:	(bad)
    18005015b:	addb   $0x0,(%rcx)
    18005015e:	add    %al,(%rax)
    180050160:	shlb   0x18006(%rsi)
    180050166:	add    %al,(%rax)
    180050168:	add    %al,(%rax)
    18005016a:	add    %al,(%rax)
-   18005016c:	fdivl  0x6479(%rbx)
+   18005016c:	scas   %es:(%rdi),%eax
+   18005016d:	pop    %rbx
+   18005016e:	outsl  %ds:(%rsi),(%dx)
+   18005016f:	add    %al,%fs:(%rax)
    180050172:	add    %al,(%rax)
    180050174:	or     $0xec000000,%eax
    180050179:	add    (%rax),%al
    18005017b:	add    %bl,(%rsi,%rcx,1)
    18005017e:	add    $0x4f41c00,%eax
 	...
    18005018f:	add    %bh,(%rax)
@@ -145514,15 +145517,15 @@
    180068902:	outsl  %gs:(%esi),(%dx)
    180068905:	insl   (%dx),%es:(%rdi)
    180068906:	gs je  0x18006897b
    180068909:	jns    0x180068939
    18006890b:	fs insb (%dx),%es:(%rdi)
    18006890d:	insb   (%dx),%es:(%rdi)
    18006890e:	add    %al,(%rax)
-   180068910:	ret    $0x3f00
+   180068910:	roll   $0x3f,(%rax)
    180068913:	jae    0x18006897a
    180068915:	je     0x180068976
    180068917:	imul   $0x636e6174,0x73(%rsi),%ebp
    18006891e:	gs rex push %rbx
    180068921:	imul   $0x6f74656c,0x67(%rsi),%ebp
    180068928:	outsb  %ds:(%rsi),(%dx)
    180068929:	rex
@@ -145689,22 +145692,20 @@
    180068a8f:	rex.B
    180068a90:	rex.RB
    180068a91:	rex.X push %rbp
    180068a93:	xor    %dh,(%rcx)
    180068a95:	rex
    180068a96:	rex pop %rdx
    180068a98:	add    %al,(%rax)
-   180068a9a:	leave
-   180068a9b:	add    %bh,(%rdi)
-   180068a9d:	jae    0x180068b13
-   180068a9f:	jb     0x180068b0a
-   180068aa1:	outsb  %ds:(%rsi),(%dx)
-   180068aa2:	addr32 rex jne 0x180068b1b
-   180068aa6:	imul   $0x65646f65,0x67(%rax,%rax,2),%esp
-   180068aae:	rex
+   180068a9a:	enter  $0x3f00,$0x73
+   180068a9e:	je     0x180068b12
+   180068aa0:	imul   $0x69757540,0x67(%rsi),%ebp
+   180068aa7:	fs rex
+   180068aa9:	outsl  %gs:(%esi),(%dx)
+   180068aac:	fs gs rex
    180068aaf:	rex push %rcx
    180068ab1:	rex.RB
    180068ab2:	rex.X
    180068ab3:	rex.B (bad)
    180068ab5:	push   %r14
    180068ab7:	(bad)
    180068ab8:	and    $0x62,%al
```

## Comparing `OpenGeode_Inspector-3.0.6.dist-info/METADATA` & `OpenGeode_Inspector-3.0.6rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Inspector
-Version: 3.0.6
+Version: 3.0.6rc1
 Summary: Open source framework for inspecting the validity of geometric models
 Home-page: https://github.com/Geode-solutions/OpenGeode-Inspector
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.1.10)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.9)
+Requires-Dist: opengeode-core (==14.*,>=14.1.9)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.8)
 Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.3)
 Requires-Dist: opengeode-io (==6.*,>=6.0.6)
 
 <h1 align="center">OpenGeode-Inspector<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenGeode module for inspecting meshes and models</h3>
```

### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.6 Summary: Open
+Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.6rc1 Summary: Open
 source framework for inspecting the validity of geometric models Home-page:
 https://github.com/Geode-solutions/OpenGeode-Inspector Author: Geode-solutions
 Author-email: contact@geode-solutions.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown Requires-Dist: opengeode-core
-(==14.*,>=14.1.10) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.9)
+(==14.*,>=14.1.9) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.8)
 Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.3) Requires-Dist:
 opengeode-io (==6.*,>=6.0.6)
               ****** OpenGeode-Inspectorby Geode-solutions ******
           **** OpenGeode module for inspecting meshes and models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
       [Language] [License] [Semantic-release] [Slack_invite] [DOI] --- ##
```

## Comparing `OpenGeode_Inspector-3.0.6.dist-info/RECORD` & `OpenGeode_Inspector-3.0.6rc1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 opengeode_inspector/__init__.py,sha256=PxQ3SsdhF6R2_6Gj0-wVDgy1a-veIjTQApBSB7X5b2U,175
 opengeode_inspector/inspector.py,sha256=gouwVrJtM8c0PoZuR6t9cbtvdpJhrgk_Lvm9PTj-Tws,271
-opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll,sha256=bGtUOgsM4YcSM2JKkKR7EwhPouiP0Q3EGGEIJ9th6oQ,439808
-opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd,sha256=G28f3pVD7UokdkpO_GFGZcDhU2tx07G6KWrQyyCuZT0,451072
-OpenGeode_Inspector-3.0.6.dist-info/METADATA,sha256=R2eI1_kSnqgP-Nn1pvahT7FLx-1mtgK1fH9lpzWSR5s,5481
-OpenGeode_Inspector-3.0.6.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-OpenGeode_Inspector-3.0.6.dist-info/top_level.txt,sha256=HB6mBr33nBKSATXRcJ4Yof7xiFcQAnhw3pFzWTv8zso,20
-OpenGeode_Inspector-3.0.6.dist-info/RECORD,,
+opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll,sha256=OXTn1uJBby6_k9nvHyFxuKBGUnq-UlF3HGnsaGGED1g,439808
+opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd,sha256=AvFBjPGb1Mfm6MdR6vnF9in8c8Rels_q88l3d0G2V9s,451072
+OpenGeode_Inspector-3.0.6rc1.dist-info/METADATA,sha256=uPqLDYunaMWLPtTcD1opjH-GrRh_-n8Gp77loKH-oy0,5483
+OpenGeode_Inspector-3.0.6rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+OpenGeode_Inspector-3.0.6rc1.dist-info/top_level.txt,sha256=HB6mBr33nBKSATXRcJ4Yof7xiFcQAnhw3pFzWTv8zso,20
+OpenGeode_Inspector-3.0.6rc1.dist-info/RECORD,,
```

