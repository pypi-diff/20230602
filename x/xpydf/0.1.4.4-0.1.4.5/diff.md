# Comparing `tmp/xpydf-0.1.4.4.tar.gz` & `tmp/xpydf-0.1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpydf-0.1.4.4.tar", last modified: Tue May 16 07:48:42 2023, max compression
+gzip compressed data, was "xpydf-0.1.4.5.tar", last modified: Thu Jun  1 12:49:41 2023, max compression
```

## Comparing `xpydf-0.1.4.4.tar` & `xpydf-0.1.4.5.tar`

### file list

```diff
@@ -1,257 +1,805 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.292851 xpydf-0.1.4.4/
--rw-r--r--   0 matthijs   (501) staff       (20)    35149 2023-02-17 12:43:21.000000 xpydf-0.1.4.4/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)      118 2023-04-12 11:54:25.000000 xpydf-0.1.4.4/MANIFEST.in
--rw-r--r--   0 matthijs   (501) staff       (20)      846 2023-05-16 07:48:42.292678 xpydf-0.1.4.4/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)      240 2023-04-12 11:54:25.000000 xpydf-0.1.4.4/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)      787 2023-05-16 07:47:45.000000 xpydf-0.1.4.4/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)       38 2023-05-16 07:48:42.292905 xpydf-0.1.4.4/setup.cfg
--rw-r--r--   0 matthijs   (501) staff       (20)     1998 2023-05-05 08:47:39.000000 xpydf-0.1.4.4/setup.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.175081 xpydf-0.1.4.4/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.196257 xpydf-0.1.4.4/src/xpdf-4.04/
--rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-05-16 07:45:10.000000 xpydf-0.1.4.4/src/xpdf-4.04/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)     1330 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/ANNOUNCE
--rw-r--r--   0 matthijs   (501) staff       (20)   139475 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/CHANGES
--rw-r--r--   0 matthijs   (501) staff       (20)     1053 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/CMakeLists.txt
--rw-r--r--   0 matthijs   (501) staff       (20)    17982 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/COPYING
--rw-r--r--   0 matthijs   (501) staff       (20)    35147 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/COPYING3
--rw-r--r--   0 matthijs   (501) staff       (20)     5614 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/INSTALL
--rw-r--r--   0 matthijs   (501) staff       (20)    13778 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/README
--rw-r--r--   0 matthijs   (501) staff       (20)     2002 2023-04-12 11:54:25.000000 xpydf-0.1.4.4/src/xpdf-4.04/aconf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1985 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/aconf.h.in
--rw-r--r--   0 matthijs   (501) staff       (20)      941 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/aconf2.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10676 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/cmake-config.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.205453 xpydf-0.1.4.4/src/xpdf-4.04/fofi/
--rw-r--r--   0 matthijs   (501) staff       (20)     3275 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiBase.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1344 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiBase.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14853 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiEncodings.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiEncodings.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21889 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiIdentifier.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1659 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiIdentifier.h
--rw-r--r--   0 matthijs   (501) staff       (20)    77637 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiTrueType.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8227 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiTrueType.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8796 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiType1.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1434 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiType1.h
--rw-r--r--   0 matthijs   (501) staff       (20)    97383 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiType1C.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8299 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiType1C.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.212496 xpydf-0.1.4.4/src/xpdf-4.04/goo/
--rw-r--r--   0 matthijs   (501) staff       (20)     2748 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/FixedPoint.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     7361 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/FixedPoint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6201 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/GHash.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2209 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/GHash.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2276 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/GList.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2724 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/GList.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2629 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/GMutex.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17722 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/GString.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4269 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/GString.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2406 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/Trace.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1171 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/Trace.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17381 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/gfile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4565 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/gfile.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8259 2023-03-01 15:38:49.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/gmem.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-03-01 15:38:49.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/gmem.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/gmempp.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1714 2023-03-01 15:38:49.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/gmempp.h
--rw-r--r--   0 matthijs   (501) staff       (20)      562 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/gtypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1583 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/goo/parseargs.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.235062 xpydf-0.1.4.4/src/xpdf-4.04/splash/
--rw-r--r--   0 matthijs   (501) staff       (20)   230071 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/Splash.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    20193 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/Splash.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6603 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashBitmap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2881 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashBitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11473 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashClip.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4007 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashClip.h
--rw-r--r--   0 matthijs   (501) staff       (20)      930 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashErrorCodes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13929 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1345 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8902 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFontEngine.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2248 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFontEngine.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4055 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFontFile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2241 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFontFile.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4995 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3666 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9673 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontEngine.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3358 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontEngine.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1589 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontFile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2168 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontFile.h
--rw-r--r--   0 matthijs   (501) staff       (20)      603 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontFileID.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      687 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontFileID.h
--rw-r--r--   0 matthijs   (501) staff       (20)      758 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashGlyphBitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9510 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashMath.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5135 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashPath.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3876 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashPath.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1042 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashPattern.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1447 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashPattern.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9844 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashScreen.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2167 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashScreen.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9521 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3669 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashState.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4155 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashTypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17088 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashXPath.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3761 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashXPath.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12936 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashXPathScanner.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2482 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashXPathScanner.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.277566 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/
--rw-r--r--   0 matthijs   (501) staff       (20)   104374 2023-05-15 13:37:05.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/AcroForm.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5269 2023-05-15 13:34:50.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/AcroForm.h
--rw-r--r--   0 matthijs   (501) staff       (20)    38840 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Annot.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4895 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Annot.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1385 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Array.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1400 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Array.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1387 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/BuiltinFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1080 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/BuiltinFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)   229548 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/BuiltinFontTables.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      556 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/BuiltinFontTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10417 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3178 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    28608 2023-05-15 13:29:26.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Catalog.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4742 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Catalog.h
--rw-r--r--   0 matthijs   (501) staff       (20)    19175 2023-04-13 10:47:41.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3702 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CharCodeToUnicode.h
--rw-r--r--   0 matthijs   (501) staff       (20)      526 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CharTypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8379 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CompactFontTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    45644 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Decrypt.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3530 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Decrypt.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2993 2023-05-15 08:40:36.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Dict.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2088 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Dict.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5247 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/DisplayState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5225 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/DisplayState.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2123 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Error.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1353 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Error.h
--rw-r--r--   0 matthijs   (501) staff       (20)      984 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ErrorCodes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21312 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/FontEncodingTables.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      564 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/FontEncodingTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    36553 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Function.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6722 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Function.h
--rw-r--r--   0 matthijs   (501) staff       (20)   144837 2023-04-13 10:47:44.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Gfx.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11911 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Gfx.h
--rw-r--r--   0 matthijs   (501) staff       (20)    65646 2023-04-13 10:47:45.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GfxFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    12828 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GfxFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)   120789 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GfxState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    43452 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GfxState.h
--rw-r--r--   0 matthijs   (501) staff       (20)   103543 2023-02-21 10:47:30.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GlobalParams.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    23054 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GlobalParams.h
--rw-r--r--   0 matthijs   (501) staff       (20)    34442 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/HTMLGen.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3131 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/HTMLGen.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11293 2023-05-02 12:54:18.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ImageOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3942 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ImageOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8327 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2802 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JArithmeticDecoder.h
--rw-r--r--   0 matthijs   (501) staff       (20)   109724 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JBIG2Stream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4824 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JBIG2Stream.h
--rw-r--r--   0 matthijs   (501) staff       (20)   107255 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JPXStream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11092 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JPXStream.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11674 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Lexer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2035 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Lexer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21632 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Link.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11370 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Link.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2191 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/NameToCharCode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      726 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/NameToCharCode.h
--rw-r--r--   0 matthijs   (501) staff       (20)   117065 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/NameToUnicodeTable.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4471 2023-05-15 08:40:34.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Object.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     9081 2023-05-15 08:40:32.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Object.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12818 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/OptionalContent.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3617 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/OptionalContent.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4001 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Outline.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1774 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Outline.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4131 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/OutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8935 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/OutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    87382 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDF417Barcode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      838 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDF417Barcode.h
--rw-r--r--   0 matthijs   (501) staff       (20)    51111 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFCore.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11579 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFCore.h
--rw-r--r--   0 matthijs   (501) staff       (20)    16078 2023-05-16 07:46:43.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFDoc.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6774 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFDoc.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2530 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFDocEncoding.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      339 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFDocEncoding.h
--rw-r--r--   0 matthijs   (501) staff       (20)   230372 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PSOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    19106 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PSOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3295 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PSTokenizer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      771 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PSTokenizer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13874 2023-03-01 15:38:49.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Page.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6412 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Page.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8100 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Parser.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1674 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Parser.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8588 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PreScanOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4810 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PreScanOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10354 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/SecurityHandler.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3962 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/SecurityHandler.h
--rw-r--r--   0 matthijs   (501) staff       (20)    37941 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ShadingImage.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3215 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ShadingImage.h
--rw-r--r--   0 matthijs   (501) staff       (20)   127634 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/SplashOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    10811 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/SplashOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17471 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Stream-CCITT.h
--rw-r--r--   0 matthijs   (501) staff       (20)   131758 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Stream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    31826 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Stream.h
--rw-r--r--   0 matthijs   (501) staff       (20)   183404 2023-04-13 10:47:47.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TextOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    27134 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TextOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4302 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TextString.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1587 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TextString.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13862 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileCache.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2041 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileCache.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10913 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileCompositor.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1895 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileCompositor.h
--rw-r--r--   0 matthijs   (501) staff       (20)    44674 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8164 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4636 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UTF8.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1408 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UTF8.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6033 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2971 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11532 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeMapTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5024 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeRemapping.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1138 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeRemapping.h
--rw-r--r--   0 matthijs   (501) staff       (20)    73118 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      719 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeTypeTable.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10592 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/WebFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2139 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/WebFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)    18912 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/XFAScanner.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4518 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/XFAScanner.h
--rw-r--r--   0 matthijs   (501) staff       (20)    33740 2023-05-15 08:40:18.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/XRef.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5955 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/XRef.h
--rw-r--r--   0 matthijs   (501) staff       (20)    23997 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Zoox.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6378 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Zoox.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3128 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/config.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5663 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdfdetach.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    12108 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdffonts.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4538 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdfimages.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    15031 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdfinfo.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8525 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftohtml.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    10873 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftopng.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     7820 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftoppm.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11515 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftops.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     9928 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftotext.cc
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.286104 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/
--rw-r--r--   0 matthijs   (501) staff       (20)    30301 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6596 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/QtPDFCore.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14925 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfApp.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2452 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfApp.h
--rw-r--r--   0 matthijs   (501) staff       (20)   148791 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    18968 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfViewer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    54075 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    39531 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfWidget.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13035 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      520 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1327 2022-04-18 21:11:23.000000 xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/xpdf.cc
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.291424 xpydf-0.1.4.4/src/xpydf/
--rw-r--r--   0 matthijs   (501) staff       (20)     6148 2023-05-01 14:11:15.000000 xpydf-0.1.4.4/src/xpydf/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)     3555 2023-05-15 08:40:16.000000 xpydf-0.1.4.4/src/xpydf/ImageDataDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1095 2023-05-05 08:47:39.000000 xpydf-0.1.4.4/src/xpydf/ImageDataDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1121 2023-05-15 08:40:14.000000 xpydf-0.1.4.4/src/xpydf/ImageInfoDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      941 2023-04-12 11:54:25.000000 xpydf-0.1.4.4/src/xpydf/ImageInfoDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4540 2023-05-16 06:32:43.000000 xpydf-0.1.4.4/src/xpydf/PdfLoader.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1118 2023-05-08 13:59:17.000000 xpydf-0.1.4.4/src/xpydf/PdfLoader.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7466 2023-05-09 07:36:01.000000 xpydf-0.1.4.4/src/xpydf/PdfLoaderWrapper.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2198 2023-04-12 11:54:25.000000 xpydf-0.1.4.4/src/xpydf/PyCppConversion.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      441 2023-04-12 11:54:25.000000 xpydf-0.1.4.4/src/xpydf/PyCppConversion.h
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.4.4/src/xpydf/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.4.4/src/xpydf/__init__.pyi
--rw-r--r--   0 matthijs   (501) staff       (20)      760 2023-05-08 13:59:17.000000 xpydf-0.1.4.4/src/xpydf/cXpdfPython.pyi
--rw-r--r--   0 matthijs   (501) staff       (20)     4684 2023-05-08 13:59:17.000000 xpydf-0.1.4.4/src/xpydf/pdf_loader.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1159 2023-05-08 13:59:17.000000 xpydf-0.1.4.4/src/xpydf/pdf_loader.pyi
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.292268 xpydf-0.1.4.4/src/xpydf.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)      846 2023-05-16 07:48:42.000000 xpydf-0.1.4.4/src/xpydf.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     7675 2023-05-16 07:48:42.000000 xpydf-0.1.4.4/src/xpydf.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2023-05-16 07:48:42.000000 xpydf-0.1.4.4/src/xpydf.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       14 2023-05-16 07:48:42.000000 xpydf-0.1.4.4/src/xpydf.egg-info/requires.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       18 2023-05-16 07:48:42.000000 xpydf-0.1.4.4/src/xpydf.egg-info/top_level.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-16 07:48:42.292456 xpydf-0.1.4.4/tests/
--rw-r--r--   0 matthijs   (501) staff       (20)     4094 2023-05-08 13:59:17.000000 xpydf-0.1.4.4/tests/test_pdf_loader.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.610492 xpydf-0.1.4.5/
+-rw-r--r--   0 matthijs   (501) staff       (20)    35149 2023-02-17 12:43:21.000000 xpydf-0.1.4.5/LICENSE
+-rw-r--r--   0 matthijs   (501) staff       (20)      418 2023-06-01 12:38:49.000000 xpydf-0.1.4.5/MANIFEST.in
+-rw-r--r--   0 matthijs   (501) staff       (20)      846 2023-06-01 12:49:41.610329 xpydf-0.1.4.5/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)      240 2023-04-12 11:54:25.000000 xpydf-0.1.4.5/README.md
+-rw-r--r--   0 matthijs   (501) staff       (20)      787 2023-06-01 12:49:30.000000 xpydf-0.1.4.5/pyproject.toml
+-rw-r--r--   0 matthijs   (501) staff       (20)       38 2023-06-01 12:49:41.610533 xpydf-0.1.4.5/setup.cfg
+-rw-r--r--   0 matthijs   (501) staff       (20)     4861 2023-06-01 12:40:37.000000 xpydf-0.1.4.5/setup.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.411263 xpydf-0.1.4.5/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.416939 xpydf-0.1.4.5/src/freetype/
+-rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-05-23 14:26:17.000000 xpydf-0.1.4.5/src/freetype/.DS_Store
+-rw-r--r--   0 matthijs   (501) staff       (20)      453 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/.clang-format
+-rw-r--r--   0 matthijs   (501) staff       (20)       40 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/.git
+-rw-r--r--   0 matthijs   (501) staff       (20)       94 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/.gitignore
+-rw-r--r--   0 matthijs   (501) staff       (20)     7021 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/.gitlab-ci.yml
+-rw-r--r--   0 matthijs   (501) staff       (20)       84 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/.gitmodules
+-rw-r--r--   0 matthijs   (501) staff       (20)     1821 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/.mailmap
+-rw-r--r--   0 matthijs   (501) staff       (20)    21367 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/CMakeLists.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)     2074 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/LICENSE.TXT
+-rw-r--r--   0 matthijs   (501) staff       (20)      846 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/Makefile
+-rw-r--r--   0 matthijs   (501) staff       (20)     3114 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/README
+-rw-r--r--   0 matthijs   (501) staff       (20)     3154 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/README.git
+-rwxr-xr-x   0 matthijs   (501) staff       (20)     4768 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/autogen.sh
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.407366 xpydf-0.1.4.5/src/freetype/builds/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.417552 xpydf-0.1.4.5/src/freetype/builds/mac/
+-rwxr-xr-x   0 matthijs   (501) staff       (20)     1033 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/builds/mac/ascii2mpw.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.418638 xpydf-0.1.4.5/src/freetype/builds/meson/
+-rw-r--r--   0 matthijs   (501) staff       (20)     3019 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/builds/meson/extract_freetype_version.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     2906 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/builds/meson/extract_libtool_version.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     2317 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/builds/meson/generate_reference_docs.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     4596 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/builds/meson/parse_modules_cfg.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3403 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/builds/meson/process_ftoption_h.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1633 2023-05-22 06:59:42.000000 xpydf-0.1.4.5/src/freetype/config.mk
+-rwxr-xr-x   0 matthijs   (501) staff       (20)     4029 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/configure
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.418897 xpydf-0.1.4.5/src/freetype/include/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.419340 xpydf-0.1.4.5/src/freetype/include/dlg/
+-rw-r--r--   0 matthijs   (501) staff       (20)    10834 2023-05-22 06:59:35.000000 xpydf-0.1.4.5/src/freetype/include/dlg/dlg.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7229 2023-05-22 06:59:35.000000 xpydf-0.1.4.5/src/freetype/include/dlg/output.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.430599 xpydf-0.1.4.5/src/freetype/include/freetype/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.432404 xpydf-0.1.4.5/src/freetype/include/freetype/config/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1614 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/config/ftconfig.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    23919 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/config/ftheader.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1443 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/config/ftmodule.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    39628 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/config/ftoption.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4576 2023-05-23 14:26:12.000000 xpydf-0.1.4.5/src/freetype/include/freetype/config/ftstdlib.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7072 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/config/integer-types.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1597 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/config/mac-support.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4207 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/config/public-macros.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   178794 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/freetype.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5470 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftadvanc.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2638 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftbbox.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5322 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftbdf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9051 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftbitmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2786 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftbzip2.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    34179 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftcache.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2933 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftchapters.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4022 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftcid.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    50199 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftcolor.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    47533 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftdriver.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12559 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/fterrdef.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9301 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/fterrors.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2213 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftfntfmt.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4138 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftgasp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    20912 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftglyph.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10625 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftgxval.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4211 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftgzip.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    41833 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftimage.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10696 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftincrem.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11744 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftlcdfil.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7100 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftlist.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4130 2023-05-23 14:26:12.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftlogging.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2768 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftlzw.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7771 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftmac.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    23797 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftmm.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    22544 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftmodapi.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6675 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftmoderr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5346 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftotval.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17402 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftoutln.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6041 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftparams.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4908 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftpfr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6625 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftrender.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4288 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftsizes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7730 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftsnames.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21773 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftstroke.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4483 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftsynth.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8502 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftsystem.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7411 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/fttrigon.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14735 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/fttypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7965 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ftwinfnt.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.438032 xpydf-0.1.4.5/src/freetype/include/freetype/internal/
+-rw-r--r--   0 matthijs   (501) staff       (20)     7498 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/autohint.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2354 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/cffotypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11866 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/cfftypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11499 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/compiler-macros.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    15606 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftcalc.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13332 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftdebug.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9214 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftdrv.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4504 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftgloadr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3242 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/fthash.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    15961 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftmemory.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3003 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftmmtypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    42481 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftobjs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1130 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftpsprop.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7651 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftrfork.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    24053 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftserv.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    23230 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftstream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5918 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/fttrace.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5762 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/ftvalid.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    43241 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/psaux.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    20852 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/pshints.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.442341 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1731 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svbdf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2832 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svcfftl.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2124 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svcid.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1348 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svfntfmt.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1865 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svgldict.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1730 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svgxval.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1080 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svkern.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3996 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svmetric.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8956 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svmm.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1253 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svotval.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1570 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svpfr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1571 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svpostnm.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1677 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svprop.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4272 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svpscmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2469 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svpsinfo.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2079 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svsfnt.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2397 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svttcmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1007 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svtteng.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1251 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svttglyf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1017 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/services/svwinfnt.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    32444 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/sfnt.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1041 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/svginterface.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8208 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/t1types.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    52695 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/tttypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8010 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/internal/wofftypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10457 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/otsvg.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    23188 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/t1tables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    58769 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/ttnameid.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    25227 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/tttables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5145 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/freetype/tttags.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      990 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/include/ft2build.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13071 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/meson.build
+-rw-r--r--   0 matthijs   (501) staff       (20)     1518 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/meson_options.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)     6490 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/modules.cfg
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.410169 xpydf-0.1.4.5/src/freetype/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.449865 xpydf-0.1.4.5/src/freetype/src/autofit/
+-rw-r--r--   0 matthijs   (501) staff       (20)    76975 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afblue.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    16937 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afblue.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    66667 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afcjk.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4211 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afcjk.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3159 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afcover.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2160 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afdummy.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      877 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afdummy.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      984 2023-05-22 06:46:50.000000 xpydf-0.1.4.5/src/freetype/src/autofit/aferrors.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13736 2023-05-23 09:51:54.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afglobal.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     5110 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afglobal.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    47282 2023-05-23 14:26:12.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afhints.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    15948 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afhints.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4719 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afindic.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      840 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afindic.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   113850 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/aflatin.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     6784 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/aflatin.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    24004 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afloader.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2269 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afloader.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13961 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afmodule.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1181 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afmodule.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    34997 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afranges.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1083 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afranges.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11464 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afscript.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    20127 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afshaper.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1655 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afshaper.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    15115 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afstyles.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    18624 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/aftypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      872 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afws-decl.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      966 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/afws-iter.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      832 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/autofit.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3310 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/ft-hb.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1463 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/autofit/ft-hb.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.459527 xpydf-0.1.4.5/src/freetype/src/base/
+-rw-r--r--   0 matthijs   (501) staff       (20)     4906 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftadvanc.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      980 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftbase.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2651 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftbase.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14346 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftbbox.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2177 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftbdf.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    28296 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftbitmap.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    28205 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftcalc.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2540 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftcid.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3416 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftcolor.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    23926 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftdbgmem.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    14105 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftdebug.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1267 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/fterrors.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1203 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftfntfmt.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1551 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftfstype.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1355 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftgasp.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    11421 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftgloadr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    24220 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftglyph.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3125 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftgxval.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     6657 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/fthash.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     6339 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftinit.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    11455 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftlcdfil.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    31521 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftmac.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    18084 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftmm.c
+-rw-r--r--   0 matthijs   (501) staff       (20)   161883 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftobjs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2216 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftotval.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    28599 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftoutln.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1245 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftpatent.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3730 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftpfr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     7500 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftpsprop.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    29493 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftrfork.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4580 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftsnames.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    19273 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftstream.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    64724 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftstroke.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     5374 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftsynth.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     8149 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftsystem.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    10565 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/fttrigon.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3047 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/fttype1.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    10171 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftutil.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1306 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/ftwinfnt.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     8743 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/md5.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1410 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/base/md5.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.460791 xpydf-0.1.4.5/src/freetype/src/bdf/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1234 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/bdf/bdf.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     8121 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/bdf/bdf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    29163 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/bdf/bdfdrivr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1772 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/bdf/bdfdrivr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1584 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/bdf/bdferror.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    68231 2023-05-23 14:26:12.000000 xpydf-0.1.4.5/src/freetype/src/bdf/bdflib.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.461090 xpydf-0.1.4.5/src/freetype/src/bzip2/
+-rw-r--r--   0 matthijs   (501) staff       (20)    12870 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/bzip2/ftbzip2.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.464298 xpydf-0.1.4.5/src/freetype/src/cache/
+-rw-r--r--   0 matthijs   (501) staff       (20)      771 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcache.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    18033 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcbasic.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    14006 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftccache.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    15484 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftccache.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2220 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftccback.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9711 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftccmap.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      999 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcerror.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4964 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcglyph.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    11116 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcglyph.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3677 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcimage.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2675 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcimage.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17267 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcmanag.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     5734 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcmanag.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6868 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcmru.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     8525 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcmru.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11958 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcsbits.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2191 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cache/ftcsbits.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.467564 xpydf-0.1.4.5/src/freetype/src/cff/
+-rw-r--r--   0 matthijs   (501) staff       (20)      725 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cff.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     7312 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffcmap.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2181 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffcmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    39514 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffdrivr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      752 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffdrivr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      959 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cfferrs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    26335 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffgload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1523 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffgload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    75411 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3298 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    35405 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffobjs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1940 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffobjs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    39397 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffparse.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3326 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cffparse.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6772 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cff/cfftoken.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.470787 xpydf-0.1.4.5/src/freetype/src/cid/
+-rw-r--r--   0 matthijs   (501) staff       (20)      958 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/ciderrs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    20567 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidgload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1456 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidgload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    25446 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1115 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13878 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidobjs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3412 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidobjs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8770 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidparse.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3518 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidparse.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7557 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidriver.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      772 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidriver.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4387 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/cidtoken.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      710 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/cid/type1cid.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.471474 xpydf-0.1.4.5/src/freetype/src/dlg/
+-rw-r--r--   0 matthijs   (501) staff       (20)    21039 2023-05-22 06:59:35.000000 xpydf-0.1.4.5/src/freetype/src/dlg/dlg.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      762 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/dlg/dlgwrap.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.478087 xpydf-0.1.4.5/src/freetype/src/gxvalid/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1133 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvalid.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2869 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvalid.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9637 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvbsln.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    54281 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvcommn.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    22980 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvcommn.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1333 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxverror.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9949 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvfeat.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     6054 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvfeat.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13317 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvfgen.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    20588 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvjust.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    27203 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvkern.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     7139 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvlcar.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     8348 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmod.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1093 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmod.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8297 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmort.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2971 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmort.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4329 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmort0.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     8122 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmort1.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    10023 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmort2.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3760 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmort4.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     8009 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmort5.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     5208 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmorx.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2076 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmorx.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3126 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmorx0.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     8464 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmorx1.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    10356 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmorx2.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1674 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmorx4.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     7285 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvmorx5.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     7216 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvopbd.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    10208 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvprop.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     9558 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gxvalid/gxvtrak.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.482480 xpydf-0.1.4.5/src/freetype/src/gzip/
+-rw-r--r--   0 matthijs   (501) staff       (20)     5182 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/adler32.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    32225 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/crc32.c
+-rw-r--r--   0 matthijs   (501) staff       (20)   591749 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/crc32.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    20073 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/ftgzip.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    16625 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/ftzconf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6843 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/gzguts.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12933 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/inffast.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      434 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/inffast.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6332 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/inffixed.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    56083 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/inflate.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     6745 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/inflate.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12993 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/inftrees.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3000 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/inftrees.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    98004 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/zlib.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7355 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/zutil.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     7398 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/gzip/zutil.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.482988 xpydf-0.1.4.5/src/freetype/src/lzw/
+-rw-r--r--   0 matthijs   (501) staff       (20)     9899 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/lzw/ftlzw.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    10565 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/lzw/ftzopen.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     5099 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/lzw/ftzopen.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.485862 xpydf-0.1.4.5/src/freetype/src/otvalid/
+-rw-r--r--   0 matthijs   (501) staff       (20)      773 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvalid.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2127 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvalid.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7882 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvbase.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    27533 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvcommn.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    19343 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvcommn.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1017 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otverror.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8882 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvgdef.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    29663 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvgpos.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      786 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvgpos.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    18463 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvgsub.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     7126 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvjstf.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    13656 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvmath.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     7207 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvmod.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      778 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/otvalid/otvmod.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.488036 xpydf-0.1.4.5/src/freetype/src/pcf/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1253 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcf.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     6373 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21798 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcfdrivr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1358 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcfdrivr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      959 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcferror.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    50270 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcfread.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1361 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcfread.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3382 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcfutil.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1649 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pcf/pcfutil.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.492385 xpydf-0.1.4.5/src/freetype/src/pfr/
+-rw-r--r--   0 matthijs   (501) staff       (20)      708 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4519 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrcmap.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      920 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrcmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5618 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrdrivr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      773 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrdrivr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      962 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrerror.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21931 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrgload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1059 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrgload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    28988 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3425 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17487 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrobjs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2135 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrobjs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21398 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrsbit.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      878 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrsbit.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8090 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pfr/pfrtypes.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.500590 xpydf-0.1.4.5/src/freetype/src/psaux/
+-rw-r--r--   0 matthijs   (501) staff       (20)    25277 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/afmparse.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1825 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/afmparse.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    68657 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/cffdecode.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1825 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/cffdecode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6515 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psarrst.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3476 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psarrst.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      945 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psaux.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1003 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psauxerr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4847 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psauxmod.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1247 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psauxmod.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    19898 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psblues.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     5995 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psblues.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11649 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psconv.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1700 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psconv.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2089 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/pserror.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4024 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/pserror.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3743 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psfixed.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    19883 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psfont.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     5402 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psfont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    25620 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psft.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     5394 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psft.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4501 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psglue.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    66109 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/pshints.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     9869 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/pshints.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   105884 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psintrp.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3074 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psintrp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    66473 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psobjs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    10283 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psobjs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3522 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psread.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2299 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psread.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9233 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psstack.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3695 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/psstack.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2674 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/pstypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11948 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/t1cmap.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3282 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/t1cmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    60726 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/t1decode.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2024 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psaux/t1decode.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.502680 xpydf-0.1.4.5/src/freetype/src/pshinter/
+-rw-r--r--   0 matthijs   (501) staff       (20)    58961 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshalgo.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     6616 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshalgo.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    22377 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshglob.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4860 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshglob.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      671 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshinter.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3002 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshmod.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      741 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshmod.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      978 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshnterr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    31754 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshrec.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4103 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/pshinter/pshrec.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.507412 xpydf-0.1.4.5/src/freetype/src/psnames/
+-rw-r--r--   0 matthijs   (501) staff       (20)    16268 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psnames/psmodule.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      748 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psnames/psmodule.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      999 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psnames/psnamerr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      622 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psnames/psnames.c
+-rw-r--r--   0 matthijs   (501) staff       (20)   268144 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/psnames/pstables.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.509460 xpydf-0.1.4.5/src/freetype/src/raster/
+-rw-r--r--   0 matthijs   (501) staff       (20)     2969 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/raster/ftmisc.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    84634 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/raster/ftraster.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1092 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/raster/ftraster.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5557 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/raster/ftrend1.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      755 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/raster/ftrend1.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      654 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/raster/raster.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1005 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/raster/rasterrs.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.511401 xpydf-0.1.4.5/src/freetype/src/sdf/
+-rw-r--r--   0 matthijs   (501) staff       (20)    38453 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/ftbsdf.c
+-rw-r--r--   0 matthijs   (501) staff       (20)   112098 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/ftsdf.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2914 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/ftsdf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4108 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/ftsdfcommon.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4007 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/ftsdfcommon.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      848 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/ftsdferrs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    16276 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/ftsdfrend.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3386 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/ftsdfrend.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      735 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sdf/sdf.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.519994 xpydf-0.1.4.5/src/freetype/src/sfnt/
+-rw-r--r--   0 matthijs   (501) staff       (20)    13188 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/pngshim.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1184 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/pngshim.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    36683 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfdriver.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      740 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfdriver.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      966 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sferrors.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      908 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfnt.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    48936 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfobjs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1417 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfobjs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12342 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfwoff.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      865 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfwoff.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    66294 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfwoff2.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2124 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/sfwoff2.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6247 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttbdf.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1029 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttbdf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   111890 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttcmap.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3727 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttcmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1227 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttcmapc.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    62115 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttcolr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2526 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttcolr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7964 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttcpal.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1036 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttcpal.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7232 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttkern.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1199 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttkern.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    40643 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2507 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8552 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttmtx.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1289 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttmtx.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13197 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttpost.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1002 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttpost.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    48308 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttsbit.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1672 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttsbit.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10640 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttsvg.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1014 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/ttsvg.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4350 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/woff2tags.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      867 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/sfnt/woff2tags.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.521468 xpydf-0.1.4.5/src/freetype/src/smooth/
+-rw-r--r--   0 matthijs   (501) staff       (20)    62480 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/smooth/ftgrays.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1260 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/smooth/ftgrays.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      997 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/smooth/ftsmerrs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    16549 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/smooth/ftsmooth.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      751 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/smooth/ftsmooth.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      657 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/smooth/smooth.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.522138 xpydf-0.1.4.5/src/freetype/src/svg/
+-rw-r--r--   0 matthijs   (501) staff       (20)     8897 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/svg/ftsvg.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      810 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/svg/ftsvg.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      656 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/svg/svg.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1195 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/svg/svgtypes.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.523747 xpydf-0.1.4.5/src/freetype/src/tools/
+-rw-r--r--   0 matthijs   (501) staff       (20)    11420 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/apinames.c
+-rwxr-xr-x   0 matthijs   (501) staff       (20)     4216 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/chktrcmp.py
+-rw-r--r--   0 matthijs   (501) staff       (20)      770 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/cordic.py
+-rw-r--r--   0 matthijs   (501) staff       (20)   107236 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/glnames.py
+-rwxr-xr-x   0 matthijs   (501) staff       (20)     6188 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/make_distribution_archives.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3969 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/test_afm.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4191 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/test_bbox.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     4826 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/test_trig.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     9927 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/tools/vms_shorten_symbol.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.527859 xpydf-0.1.4.5/src/freetype/src/truetype/
+-rw-r--r--   0 matthijs   (501) staff       (20)      896 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/truetype.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    22144 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttdriver.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      748 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttdriver.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      981 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/tterrors.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    93929 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttgload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1358 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttgload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   131819 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttgxvar.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    13625 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttgxvar.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   220265 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttinterp.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    21599 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttinterp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    43577 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttobjs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)    12076 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttobjs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    16553 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttpload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1661 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttpload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    32091 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttsubpix.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3848 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/truetype/ttsubpix.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.531229 xpydf-0.1.4.5/src/freetype/src/type1/
+-rw-r--r--   0 matthijs   (501) staff       (20)    10669 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1afm.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1285 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1afm.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    24329 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1driver.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      769 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1driver.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      969 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1errors.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    20367 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1gload.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     1193 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1gload.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    82040 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1load.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3285 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1load.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17437 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1objs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3452 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1objs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14896 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1parse.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3735 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1parse.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5083 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/t1tokens.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      720 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type1/type1.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.533640 xpydf-0.1.4.5/src/freetype/src/type42/
+-rw-r--r--   0 matthijs   (501) staff       (20)     6579 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/t42drivr.c
+-rw-r--r--   0 matthijs   (501) staff       (20)      739 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/t42drivr.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      973 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/t42error.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    19226 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/t42objs.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2452 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/t42objs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    40017 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/t42parse.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/t42parse.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1181 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/t42types.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      652 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/type42/type42.c
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.534261 xpydf-0.1.4.5/src/freetype/src/winfonts/
+-rw-r--r--   0 matthijs   (501) staff       (20)      988 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/winfonts/fnterrs.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    35786 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/winfonts/winfnt.c
+-rw-r--r--   0 matthijs   (501) staff       (20)     3104 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/src/winfonts/winfnt.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.410392 xpydf-0.1.4.5/src/freetype/tests/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.534471 xpydf-0.1.4.5/src/freetype/tests/scripts/
+-rwxr-xr-x   0 matthijs   (501) staff       (20)     8869 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/tests/scripts/download-test-fonts.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    41515 2023-05-19 16:13:04.000000 xpydf-0.1.4.5/src/freetype/vms_make.com
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.538636 xpydf-0.1.4.5/src/xpdf-4.04/
+-rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-06-01 12:26:37.000000 xpydf-0.1.4.5/src/xpdf-4.04/.DS_Store
+-rw-r--r--   0 matthijs   (501) staff       (20)     1330 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/ANNOUNCE
+-rw-r--r--   0 matthijs   (501) staff       (20)   139475 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/CHANGES
+-rw-r--r--   0 matthijs   (501) staff       (20)     1053 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/CMakeLists.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)    17982 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/COPYING
+-rw-r--r--   0 matthijs   (501) staff       (20)    35147 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/COPYING3
+-rw-r--r--   0 matthijs   (501) staff       (20)     5614 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/INSTALL
+-rw-r--r--   0 matthijs   (501) staff       (20)    13778 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/README
+-rw-r--r--   0 matthijs   (501) staff       (20)     2002 2023-06-01 12:34:57.000000 xpydf-0.1.4.5/src/xpdf-4.04/aconf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1985 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/aconf.h.in
+-rw-r--r--   0 matthijs   (501) staff       (20)      941 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/aconf2.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10676 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/cmake-config.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.542352 xpydf-0.1.4.5/src/xpdf-4.04/fofi/
+-rw-r--r--   0 matthijs   (501) staff       (20)     3275 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiBase.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1344 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiBase.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14853 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiEncodings.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiEncodings.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21889 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiIdentifier.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1659 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiIdentifier.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    77637 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiTrueType.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8227 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiTrueType.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8796 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiType1.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1434 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiType1.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    97383 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiType1C.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8299 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiType1C.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.547347 xpydf-0.1.4.5/src/xpdf-4.04/goo/
+-rw-r--r--   0 matthijs   (501) staff       (20)     2748 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/FixedPoint.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     7361 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/FixedPoint.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6201 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/GHash.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2209 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/GHash.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2276 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/GList.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2724 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/GList.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2629 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/GMutex.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17722 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/GString.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4269 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/GString.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2406 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/Trace.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1171 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/Trace.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17381 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/gfile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4565 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/gfile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8259 2023-03-01 15:38:49.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/gmem.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-03-01 15:38:49.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/gmem.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/gmempp.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1714 2023-03-01 15:38:49.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/gmempp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      562 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/gtypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1583 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/goo/parseargs.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.556290 xpydf-0.1.4.5/src/xpdf-4.04/splash/
+-rw-r--r--   0 matthijs   (501) staff       (20)   230071 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/Splash.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    20193 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/Splash.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6603 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashBitmap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2881 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashBitmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11473 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashClip.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4007 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashClip.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      930 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashErrorCodes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13929 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1345 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8902 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFontEngine.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2248 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFontEngine.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4055 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFontFile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2241 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFontFile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4995 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3666 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9673 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontEngine.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3358 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontEngine.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1589 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontFile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2168 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontFile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      603 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontFileID.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      687 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontFileID.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      758 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashGlyphBitmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9510 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashMath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5135 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashPath.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3876 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashPath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1042 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashPattern.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1447 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashPattern.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9844 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashScreen.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2167 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashScreen.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9521 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3669 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4155 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashTypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17088 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashXPath.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3761 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashXPath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12936 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashXPathScanner.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2482 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashXPathScanner.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.601788 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/
+-rw-r--r--   0 matthijs   (501) staff       (20)   104374 2023-05-15 13:37:05.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/AcroForm.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5269 2023-05-15 13:34:50.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/AcroForm.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    38840 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Annot.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4895 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Annot.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1385 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Array.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1400 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Array.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1387 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/BuiltinFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1080 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/BuiltinFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   229548 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/BuiltinFontTables.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      556 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/BuiltinFontTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10417 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3178 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    28608 2023-05-15 13:29:26.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Catalog.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4742 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Catalog.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    19175 2023-04-13 10:47:41.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3702 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CharCodeToUnicode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      526 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CharTypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8379 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CompactFontTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    45644 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Decrypt.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3530 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Decrypt.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2993 2023-05-15 08:40:36.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Dict.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2088 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Dict.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5247 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/DisplayState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5225 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/DisplayState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2123 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Error.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1353 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Error.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      984 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ErrorCodes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21312 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/FontEncodingTables.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      564 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/FontEncodingTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    36553 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Function.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6722 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Function.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   144837 2023-06-01 12:26:12.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Gfx.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11911 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Gfx.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    65646 2023-06-01 12:26:12.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GfxFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    12828 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GfxFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   120789 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GfxState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    43452 2023-06-01 12:26:12.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GfxState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   103543 2023-05-19 16:11:38.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GlobalParams.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    23054 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GlobalParams.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    34442 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/HTMLGen.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3131 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/HTMLGen.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11293 2023-05-02 12:54:18.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ImageOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3942 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ImageOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8327 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2802 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JArithmeticDecoder.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   109724 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JBIG2Stream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4824 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JBIG2Stream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   107255 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JPXStream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11092 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JPXStream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11674 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Lexer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2035 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Lexer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21632 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Link.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11370 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Link.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2191 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/NameToCharCode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      726 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/NameToCharCode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   117065 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/NameToUnicodeTable.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4471 2023-05-15 08:40:34.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Object.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     9081 2023-05-15 08:40:32.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Object.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12818 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/OptionalContent.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3617 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/OptionalContent.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4001 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Outline.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1774 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Outline.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4131 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/OutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8935 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/OutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    87382 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDF417Barcode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      838 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDF417Barcode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    51111 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFCore.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11579 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFCore.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    16078 2023-05-16 07:46:43.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFDoc.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6774 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFDoc.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2530 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFDocEncoding.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      339 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFDocEncoding.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   230372 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PSOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    19106 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PSOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3295 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PSTokenizer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      771 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PSTokenizer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13874 2023-03-01 15:38:49.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Page.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6412 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Page.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8100 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Parser.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1674 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Parser.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8588 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PreScanOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4810 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PreScanOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10354 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/SecurityHandler.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3962 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/SecurityHandler.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    37941 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ShadingImage.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3215 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ShadingImage.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   127634 2023-05-19 16:11:47.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/SplashOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    10811 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/SplashOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17471 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Stream-CCITT.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   131758 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Stream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    31826 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Stream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   183399 2023-06-01 12:26:37.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TextOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    27134 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TextOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4302 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TextString.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1587 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TextString.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13862 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileCache.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2041 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileCache.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10913 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileCompositor.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1895 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileCompositor.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    44674 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8164 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4636 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UTF8.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1408 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UTF8.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6033 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2971 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11532 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeMapTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5024 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeRemapping.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1138 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeRemapping.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    73118 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      719 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeTypeTable.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10592 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/WebFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2139 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/WebFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    18912 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/XFAScanner.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4518 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/XFAScanner.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    33740 2023-05-15 08:40:18.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/XRef.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5955 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/XRef.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    23997 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Zoox.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6378 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Zoox.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3128 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/config.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5663 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdfdetach.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    12108 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdffonts.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4538 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdfimages.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    15031 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdfinfo.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8525 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftohtml.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    10873 2023-05-19 13:46:26.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftopng.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     7820 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftoppm.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11515 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftops.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     9928 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftotext.cc
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.604941 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/
+-rw-r--r--   0 matthijs   (501) staff       (20)    30301 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6596 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/QtPDFCore.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14925 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfApp.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2452 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfApp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   148791 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    18968 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfViewer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    54075 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    39531 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfWidget.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13035 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      520 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1327 2022-04-18 21:11:23.000000 xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/xpdf.cc
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.609208 xpydf-0.1.4.5/src/xpydf/
+-rw-r--r--   0 matthijs   (501) staff       (20)     6148 2023-05-01 14:11:15.000000 xpydf-0.1.4.5/src/xpydf/.DS_Store
+-rw-r--r--   0 matthijs   (501) staff       (20)     3768 2023-05-23 14:30:42.000000 xpydf-0.1.4.5/src/xpydf/ImageDataDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1095 2023-05-05 08:47:39.000000 xpydf-0.1.4.5/src/xpydf/ImageDataDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1121 2023-05-15 08:40:14.000000 xpydf-0.1.4.5/src/xpydf/ImageInfoDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      941 2023-04-12 11:54:25.000000 xpydf-0.1.4.5/src/xpydf/ImageInfoDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5725 2023-06-01 12:34:57.000000 xpydf-0.1.4.5/src/xpydf/PdfLoader.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1163 2023-06-01 12:34:57.000000 xpydf-0.1.4.5/src/xpydf/PdfLoader.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8438 2023-06-01 12:34:57.000000 xpydf-0.1.4.5/src/xpydf/PdfLoaderWrapper.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2198 2023-04-12 11:54:25.000000 xpydf-0.1.4.5/src/xpydf/PyCppConversion.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      441 2023-04-12 11:54:25.000000 xpydf-0.1.4.5/src/xpydf/PyCppConversion.h
+-rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.4.5/src/xpydf/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.4.5/src/xpydf/__init__.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)      857 2023-06-01 12:34:57.000000 xpydf-0.1.4.5/src/xpydf/cXpdfPython.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)     5155 2023-06-01 12:34:57.000000 xpydf-0.1.4.5/src/xpydf/pdf_loader.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1246 2023-06-01 12:34:57.000000 xpydf-0.1.4.5/src/xpydf/pdf_loader.pyi
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.609982 xpydf-0.1.4.5/src/xpydf.egg-info/
+-rw-r--r--   0 matthijs   (501) staff       (20)      846 2023-06-01 12:49:41.000000 xpydf-0.1.4.5/src/xpydf.egg-info/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)    25801 2023-06-01 12:49:41.000000 xpydf-0.1.4.5/src/xpydf.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)        1 2023-06-01 12:49:41.000000 xpydf-0.1.4.5/src/xpydf.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       14 2023-06-01 12:49:41.000000 xpydf-0.1.4.5/src/xpydf.egg-info/requires.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       27 2023-06-01 12:49:41.000000 xpydf-0.1.4.5/src/xpydf.egg-info/top_level.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-01 12:49:41.610106 xpydf-0.1.4.5/tests/
+-rw-r--r--   0 matthijs   (501) staff       (20)     4574 2023-06-01 12:34:57.000000 xpydf-0.1.4.5/tests/test_pdf_loader.py
```

### Comparing `xpydf-0.1.4.4/LICENSE` & `xpydf-0.1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/PKG-INFO` & `xpydf-0.1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpydf
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: Python wrapper around the pdftotext and pdfimages functionalities of xpdf.
 Author-email: Matthijs Wesseling <matthijs.wesseling@bigdatarepublic.nl>
 Project-URL: Homepage, https://github.com/Bladieblah/xpdf-python
 Project-URL: Bug Tracker, https://github.com/Bladieblah/xpdf-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `xpydf-0.1.4.4/pyproject.toml` & `xpydf-0.1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xpydf"
-version = "0.1.4.4"
+version = "0.1.4.5"
 authors = [
     { name  = "Matthijs Wesseling", email = "matthijs.wesseling@bigdatarepublic.nl" },
 ]
 
 description = "Python wrapper around the pdftotext and pdfimages functionalities of xpdf."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/.DS_Store` & `xpydf-0.1.4.5/src/xpdf-4.04/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -298,16 +298,16 @@
 00001290: 0101 0000 0000 0000 000d 0000 0000 0000  ................
 000012a0: 0000 0000 0000 0000 008b 0000 0003 0067  ...............g
 000012b0: 006f 006f 6473 636c 626f 6f6c 0000 0000  .o.odsclbool....
 000012c0: 0300 6700 6f00 6f6c 6731 5363 6f6d 7000  ..g.o.olg1Scomp.
 000012d0: 0000 0000 016b 7200 0000 0300 6700 6f00  .....kr.....g.o.
 000012e0: 6f6d 6f44 4462 6c6f 6200 0000 0841 15ef  omoDDblob....A..
 000012f0: 84d4 d7c4 4100 0000 0300 6700 6f00 6f6d  ....A.....g.o.om
-00001300: 6f64 4462 6c6f 6200 0000 08f1 cc18 d3de  odDblob.........
-00001310: d1c4 4100 0000 0300 6700 6f00 6f70 6831  ..A.....g.o.oph1
+00001300: 6f64 4462 6c6f 6200 0000 0841 15ef 84d4  odDblob....A....
+00001310: d7c4 4100 0000 0300 6700 6f00 6f70 6831  ..A.....g.o.oph1
 00001320: 5363 6f6d 7000 0000 0000 0230 0000 0000  Scomp......0....
 00001330: 0300 6700 6f00 6f76 5372 6e6c 6f6e 6700  ..g.o.ovSrnlong.
 00001340: 0000 0100 0000 0600 7300 7000 6c00 6100  ........s.p.l.a.
 00001350: 7300 686c 6731 5363 6f6d 7000 0000 0000  s.hlg1Scomp.....
 00001360: 0679 3400 0000 0600 7300 7000 6c00 6100  .y4.....s.p.l.a.
 00001370: 7300 686d 6f44 4462 6c6f 6200 0000 0800  s.hmoDDblob.....
 00001380: 0080 bd05 07c4 4100 0000 0600 7300 7000  ......A.....s.p.
@@ -325,19 +325,19 @@
 00001440: 6473 5b53 686f 7753 6964 6562 6172 0909  ds[ShowSidebar..
 00001450: 0809 5f10 187b 7b33 3335 2c20 3131 397d  .._..{{335, 119}
 00001460: 2c20 7b39 3537 2c20 3532 377d 7d09 0815  , {957, 527}}...
 00001470: 232f 3b52 5f6b 6c6d 6e6f 8a00 0000 0000  #/;R_klmno......
 00001480: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
 00001490: 0000 0000 0000 0000 0000 8b00 0000 0400  ................
 000014a0: 7800 7000 6400 666c 6731 5363 6f6d 7000  x.p.d.flg1Scomp.
-000014b0: 0000 0000 2f43 6900 0000 0400 7800 7000  ..../Ci.....x.p.
-000014c0: 6400 666d 6f44 4462 6c6f 6200 0000 08fe  d.fmoDDblob.....
-000014d0: ec89 3236 09c5 4100 0000 0400 7800 7000  ..26..A.....x.p.
-000014e0: 6400 666d 6f64 4462 6c6f 6200 0000 085b  d.fmodDblob....[
-000014f0: 9b6b 9b35 09c5 4100 0000 0400 7800 7000  .k.5..A.....x.p.
+000014b0: 0000 0000 2f43 6400 0000 0400 7800 7000  ..../Cd.....x.p.
+000014c0: 6400 666d 6f44 4462 6c6f 6200 0000 08b2  d.fmoDDblob.....
+000014d0: 822f f262 14c5 4100 0000 0400 7800 7000  ./.b..A.....x.p.
+000014e0: 6400 666d 6f64 4462 6c6f 6200 0000 08a0  d.fmodDblob.....
+000014f0: 56a6 a1eb 0bc5 4100 0000 0400 7800 7000  V.....A.....x.p.
 00001500: 6400 6670 6831 5363 6f6d 7000 0000 0000  d.fph1Scomp.....
 00001510: 3380 0000 0000 0400 7800 7000 6400 6676  3.......x.p.d.fv
 00001520: 5372 6e6c 6f6e 6700 0000 0100 0000 0700  Srnlong.........
 00001530: 7800 7000 6400 6600 2d00 7100 746c 6731  x.p.d.f.-.q.tlg1
 00001540: 5363 6f6d 7000 0000 0000 057b b400 0000  Scomp......{....
 00001550: 0700 7800 7000 6400 6600 2d00 7100 746d  ..x.p.d.f.-.q.tm
 00001560: 6f44 4462 6c6f 6200 0000 0800 0080 bd05  oDDblob.........
```

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/ANNOUNCE` & `xpydf-0.1.4.5/src/xpdf-4.04/ANNOUNCE`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/CHANGES` & `xpydf-0.1.4.5/src/xpdf-4.04/CHANGES`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/CMakeLists.txt` & `xpydf-0.1.4.5/src/xpdf-4.04/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/COPYING` & `xpydf-0.1.4.5/src/xpdf-4.04/COPYING`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/COPYING3` & `xpydf-0.1.4.5/src/xpdf-4.04/COPYING3`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/INSTALL` & `xpydf-0.1.4.5/src/xpdf-4.04/INSTALL`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/README` & `xpydf-0.1.4.5/src/xpdf-4.04/README`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/aconf.h` & `xpydf-0.1.4.5/src/xpdf-4.04/aconf.h`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 #define _FILE_OFFSET_BITS 64
 #define _LARGE_FILES 1
 #define _LARGEFILE_SOURCE 1
 
 /*
  * This is defined if using FreeType 2.
  */
-#define HAVE_FREETYPE_H 0
+#define HAVE_FREETYPE_H 1
 
 /*
  * This is defined if using D-Type 4.
  */
 #define HAVE_DTYPE4_H 0
 
 /*
```

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/aconf.h.in` & `xpydf-0.1.4.5/src/xpdf-4.04/aconf.h.in`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/aconf2.h` & `xpydf-0.1.4.5/src/xpdf-4.04/aconf2.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/cmake-config.txt` & `xpydf-0.1.4.5/src/xpdf-4.04/cmake-config.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiBase.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiBase.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiBase.h` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiBase.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiEncodings.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiEncodings.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiEncodings.h` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiEncodings.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiIdentifier.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiIdentifier.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiIdentifier.h` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiIdentifier.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiTrueType.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiTrueType.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiTrueType.h` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiTrueType.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiType1.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiType1.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiType1.h` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiType1.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiType1C.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiType1C.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/fofi/FoFiType1C.h` & `xpydf-0.1.4.5/src/xpdf-4.04/fofi/FoFiType1C.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/FixedPoint.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/FixedPoint.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/FixedPoint.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/FixedPoint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/GHash.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/GHash.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/GHash.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/GHash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/GList.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/GList.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/GList.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/GList.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/GMutex.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/GMutex.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/GString.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/GString.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/GString.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/GString.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/Trace.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/Trace.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/Trace.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/Trace.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/gfile.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/gfile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/gfile.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/gfile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/gmem.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/gmem.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/gmem.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/gmem.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/gmempp.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/gmempp.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/gmempp.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/gmempp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/gtypes.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/gtypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/goo/parseargs.h` & `xpydf-0.1.4.5/src/xpdf-4.04/goo/parseargs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/Splash.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/Splash.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/Splash.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/Splash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashBitmap.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashBitmap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashBitmap.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashBitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashClip.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashClip.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashClip.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashClip.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashErrorCodes.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashErrorCodes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFont.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFont.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFontEngine.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFontEngine.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFontEngine.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFontEngine.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFontFile.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFontFile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFTFontFile.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFTFontFile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFont.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFont.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontEngine.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontEngine.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontEngine.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontEngine.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontFile.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontFile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontFile.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontFile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontFileID.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontFileID.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashFontFileID.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashFontFileID.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashGlyphBitmap.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashGlyphBitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashMath.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashMath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashPath.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashPath.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashPath.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashPath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashPattern.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashPattern.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashPattern.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashPattern.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashScreen.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashScreen.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashScreen.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashScreen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashState.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashState.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashTypes.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashTypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashXPath.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashXPath.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashXPath.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashXPath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashXPathScanner.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashXPathScanner.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/splash/SplashXPathScanner.h` & `xpydf-0.1.4.5/src/xpdf-4.04/splash/SplashXPathScanner.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/AcroForm.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/AcroForm.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/AcroForm.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/AcroForm.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Annot.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Annot.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Annot.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Annot.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Array.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Array.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Array.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Array.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/BuiltinFont.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/BuiltinFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/BuiltinFont.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/BuiltinFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/BuiltinFontTables.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/BuiltinFontTables.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/BuiltinFontTables.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/BuiltinFontTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CMap.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CMap.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Catalog.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Catalog.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Catalog.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Catalog.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CharCodeToUnicode.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CharCodeToUnicode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CharTypes.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CharTypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/CompactFontTables.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/CompactFontTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Decrypt.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Decrypt.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Decrypt.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Decrypt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Dict.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Dict.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Dict.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Dict.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/DisplayState.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/DisplayState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/DisplayState.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/DisplayState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Error.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Error.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Error.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Error.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ErrorCodes.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ErrorCodes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/FontEncodingTables.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/FontEncodingTables.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/FontEncodingTables.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/FontEncodingTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Function.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Function.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Function.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Function.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Gfx.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Gfx.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Gfx.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Gfx.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GfxFont.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GfxFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GfxFont.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GfxFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GfxState.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GfxState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GfxState.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GfxState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GlobalParams.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GlobalParams.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/GlobalParams.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/GlobalParams.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/HTMLGen.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/HTMLGen.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/HTMLGen.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/HTMLGen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ImageOutputDev.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ImageOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ImageOutputDev.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ImageOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JArithmeticDecoder.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JArithmeticDecoder.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JBIG2Stream.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JBIG2Stream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JBIG2Stream.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JBIG2Stream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JPXStream.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JPXStream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/JPXStream.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/JPXStream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Lexer.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Lexer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Lexer.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Lexer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Link.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Link.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Link.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Link.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/NameToCharCode.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/NameToCharCode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/NameToCharCode.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/NameToCharCode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/NameToUnicodeTable.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/NameToUnicodeTable.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Object.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Object.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Object.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Object.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/OptionalContent.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/OptionalContent.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/OptionalContent.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/OptionalContent.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Outline.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Outline.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Outline.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Outline.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/OutputDev.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/OutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/OutputDev.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/OutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDF417Barcode.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDF417Barcode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDF417Barcode.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDF417Barcode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFCore.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFCore.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFCore.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFCore.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFDoc.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFDoc.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFDoc.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFDoc.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PDFDocEncoding.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PDFDocEncoding.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PSOutputDev.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PSOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PSOutputDev.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PSOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PSTokenizer.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PSTokenizer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PSTokenizer.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PSTokenizer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Page.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Page.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Page.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Page.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Parser.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Parser.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Parser.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Parser.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PreScanOutputDev.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PreScanOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/PreScanOutputDev.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/PreScanOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/SecurityHandler.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/SecurityHandler.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/SecurityHandler.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/SecurityHandler.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ShadingImage.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ShadingImage.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/ShadingImage.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/ShadingImage.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/SplashOutputDev.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/SplashOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/SplashOutputDev.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/SplashOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Stream-CCITT.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Stream-CCITT.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Stream.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Stream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Stream.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Stream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TextOutputDev.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TextOutputDev.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1381,16 +1381,15 @@
       curRot = 1;
     } else {
       curRot = 3;
     }
     diagonal = fabs(m[0]) > diagonalThreshold * fabs(m[1]);
   }
   // this matches the 'horiz' test in SplashOutputDev::drawChar()
-  rotated = !(m[0] > 0 && fabs(m[1]) < 0.001 &&
-	      fabs(m[2]) < 0.001 && m[3] < 0);
+  rotated = !(m[0] > 0 && (fabs(m[1]) < 0.001 || fabs(m[2]) < 0.001) && m[3] < 0);
 }
 
 void TextPage::addChar(GfxState *state, double x, double y,
 		       double dx, double dy,
 		       CharCode c, int nBytes, Unicode *u, int uLen) {
   double x1, y1, x2, y2, w1, h1, dx2, dy2, ascent, descent, sp;
   double xMin, yMin, xMax, yMax, xMid, yMid;
```

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TextOutputDev.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TextOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TextString.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TextString.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TextString.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TextString.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileCache.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileCache.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileCache.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileCache.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileCompositor.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileCompositor.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileCompositor.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileCompositor.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileMap.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/TileMap.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/TileMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UTF8.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UTF8.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UTF8.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UTF8.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeMap.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeMap.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeMapTables.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeMapTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeRemapping.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeRemapping.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeRemapping.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeRemapping.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/UnicodeTypeTable.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/UnicodeTypeTable.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/WebFont.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/WebFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/WebFont.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/WebFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/XFAScanner.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/XFAScanner.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/XFAScanner.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/XFAScanner.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/XRef.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/XRef.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/XRef.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/XRef.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Zoox.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Zoox.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/Zoox.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/Zoox.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/config.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/config.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdfdetach.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdfdetach.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdffonts.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdffonts.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdfimages.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdfimages.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdfinfo.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdfinfo.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftohtml.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftohtml.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftopng.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftopng.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftoppm.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftoppm.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftops.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftops.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf/pdftotext.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf/pdftotext.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/QtPDFCore.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/QtPDFCore.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfApp.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfApp.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfApp.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfApp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfViewer.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfViewer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfWidget.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfWidget.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpdf-4.04/xpdf-qt/xpdf.cc` & `xpydf-0.1.4.5/src/xpdf-4.04/xpdf-qt/xpdf.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpydf/.DS_Store` & `xpydf-0.1.4.5/src/xpydf/.DS_Store`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpydf/ImageDataDev.cc` & `xpydf-0.1.4.5/src/xpydf/ImageDataDev.cc`

 * *Files 15% similar despite different names*

```diff
@@ -103,40 +103,50 @@
   images->push_back(image);
 }
 
 void ImageDataDev::drawImageMask(GfxState *state, Object *ref, Stream *str,
     int width, int height, GBool invert,
     GBool inlineImg, GBool interpolate
 ) {
-  char buf[4096];
-  int size, n, i, m;
+  int size, bytesRead, pixelsRead;
+  int rowCount = 0;
+  char buf;
+
   Image image = {
     static_cast<unsigned int>(IMAGE_TYPES::P4),
     static_cast<unsigned int>(width),
     static_cast<unsigned int>(height),
-    static_cast<unsigned int>(height * ((width + 7) / 8)),
+    static_cast<unsigned int>(width * height),
     nullptr
   };
   
-  size = image.size;
+  size = height * ((width + 7) / 8);
   image.data = (unsigned char *)malloc(image.size * sizeof(unsigned char));
   imgNum++;
 
   str->reset();
-  m = 0;
+  pixelsRead = 0;
   while (size > 0) {
-    i = size < (int)sizeof(buf) ? size : (int)sizeof(buf);
-    n = str->getBlock(((char *)image.data) + m, i);
-    
-    if (n < i) {
+    bytesRead = str->getBlock(&buf, 1);
+
+    if (bytesRead == 0) {
       break;
     }
+
+    for (int i = 0; i < sizeof(char) * 8; i++) {
+      image.data[pixelsRead++] = buf & (128 >> i) ? 0xff : 0;
+      rowCount++;
+
+      if (rowCount == width || pixelsRead >= image.size) {
+        rowCount = 0;
+        break;
+      }
+    }
     
-    size -= n;
-    m += n;
+    size -= bytesRead;
   }
 
   str->close();
   
   images->push_back(image);
 }
```

### Comparing `xpydf-0.1.4.4/src/xpydf/ImageDataDev.h` & `xpydf-0.1.4.5/src/xpydf/ImageDataDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpydf/ImageInfoDev.cc` & `xpydf-0.1.4.5/src/xpydf/ImageInfoDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpydf/ImageInfoDev.h` & `xpydf-0.1.4.5/src/xpydf/ImageInfoDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpydf/PdfLoader.h` & `xpydf-0.1.4.5/src/xpydf/PdfLoader.h`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 class PdfLoader {
 public:
     PdfLoader(LoaderConfig config, char *fileName, char *ownerPw = NULL, char *userPw = NULL);
     ~PdfLoader();
     std::vector<std::string> extractText();
     std::vector<PageImageInfo> extractPageInfo();
     std::vector<Image> extractImages(int pageNum);
+    Image pageToImage(int pageNum, int dpi);
     bool isOk();
     int getErrorCode();
 private:
   TextOutputControl textOutControl;
   PDFDoc *doc;
   GString *textFileName;
 };
```

### Comparing `xpydf-0.1.4.4/src/xpydf/PdfLoaderWrapper.cc` & `xpydf-0.1.4.5/src/xpydf/PdfLoaderWrapper.cc`

 * *Files 7% similar despite different names*

```diff
@@ -141,28 +141,52 @@
     
     for (size_t i = 0; i < images.size(); i++) {
       Image image = images[i];
       npy_intp dims[1] = {image.size};
       array = PyArray_SimpleNewFromData(1, dims, NPY_UINT8, image.data);
       
       // Only reshape P6 images, P4 contain multiple pixels per byte
-      if (image.image_type == IMAGE_TYPES::P5) {
+      if (image.image_type == IMAGE_TYPES::P4) {
+        PyObject *shape = Py_BuildValue("ii", image.height, image.width);
+        array = PyArray_Reshape((PyArrayObject *)array, shape);
+      } else if (image.image_type == IMAGE_TYPES::P5) {
         PyObject *shape = Py_BuildValue("ii", image.height, image.width);
         array = PyArray_Reshape((PyArrayObject *)array, shape);
       } else if (image.image_type == IMAGE_TYPES::P6) {
         PyObject *shape = Py_BuildValue("iii", image.height, image.width, 3);
         array = PyArray_Reshape((PyArrayObject *)array, shape);
       }
 
       PyList_SetItem(imageList, i, array);
     }
 
     return Py_BuildValue("O", imageList);
 }
 
+PyObject *pageToImage(PyObject *self, PyObject *args) {
+    vector<string> res;
+    
+    PyObject *loaderCapsule;
+    int pageNum, dpi;
+    PyArg_ParseTuple(args, "Oii", &loaderCapsule, &pageNum, &dpi);
+
+    PdfLoader *loader = (PdfLoader *)PyCapsule_GetPointer(loaderCapsule, "loaderPtr");
+    Image pageImage = loader->pageToImage(pageNum, dpi);
+    
+    PyObject *array;
+    
+    npy_intp dims[1] = {pageImage.size};
+    array = PyArray_SimpleNewFromData(1, dims, NPY_UINT8, pageImage.data);
+    
+    PyObject *shape = Py_BuildValue("iii", pageImage.height, pageImage.width, 3);
+    array = PyArray_Reshape((PyArrayObject *)array, shape);
+
+    return Py_BuildValue("O", array);
+}
+
 PyObject *deleteObject(PyObject *self, PyObject *args) {
     PyObject *loaderCapsule;
     PyArg_ParseTuple(args, "O", &loaderCapsule);
     
     PdfLoader *loader = (PdfLoader *)PyCapsule_GetPointer(loaderCapsule, "loaderPtr");
     
     if (loader) {
@@ -191,14 +215,18 @@
       extractPageInfo, METH_VARARGS,
      "Extract image metadata"},
     
     {"extractImages",
       extractImages, METH_VARARGS,
      "Extract images"},
     
+    {"pageToImage",
+      pageToImage, METH_VARARGS,
+     "Convert a page to an image"},
+    
     {"deleteObject",
       deleteObject, METH_VARARGS,
      "Delete `PdfLoader` object"},
 
     {NULL, NULL, 0, NULL}      // Last function description must be empty.
                                // Otherwise, it will create seg fault while
                                // importing the module.
```

### Comparing `xpydf-0.1.4.4/src/xpydf/PyCppConversion.cc` & `xpydf-0.1.4.5/src/xpydf/PyCppConversion.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4.4/src/xpydf/cXpdfPython.pyi` & `xpydf-0.1.4.5/src/xpydf/cXpdfPython.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -18,8 +18,9 @@
     mapUnknownCharNames: bool = True,
     ownerPw: Optional[str] = None,
     userPw: Optional[str] = None,
 ) -> XpdfPythonCapsule: ...
 def extractText(capsule: XpdfPythonCapsule) -> List[bytes]: ...
 def extractPageInfo(capsule: XpdfPythonCapsule) -> List[PageInfo]: ...
 def extractImages(capsule: XpdfPythonCapsule, page_number: int) -> List[npt.NDArray[Any]]: ...
+def pageToImage(capsule: XpdfPythonCapsule, page_number: int, dpi: int) -> npt.NDArray[Any]: ...
 def deleteObject(capsule: XpdfPythonCapsule) -> None: ...
```

### Comparing `xpydf-0.1.4.4/src/xpydf/pdf_loader.py` & `xpydf-0.1.4.5/src/xpydf/pdf_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,11 +162,29 @@
         """
         images: List[npt.NDArray[Any]] = []
         if self.capsule is not None:
             images = cXpdfPython.extractImages(self.capsule, page_number)
 
         return images
 
+    def page_to_image(self, page_number: int, dpi: int = 150) -> Optional[npt.NDArray[Any]]:
+        """Convert a page to in image, as a numpy array.
+
+        Parameters
+        ----------
+        page_number : int
+            Page to convert
+
+        Returns
+        -------
+        npt.NDArray[Any]
+            Image data.
+        """
+        if self.capsule is not None:
+            return cXpdfPython.pageToImage(self.capsule, page_number, dpi)
+
+        return None
+
     def __del__(self):
         if self.capsule:
             cXpdfPython.deleteObject(self.capsule)
             del self.capsule
```

### Comparing `xpydf-0.1.4.4/src/xpydf/pdf_loader.pyi` & `xpydf-0.1.4.5/src/xpydf/pdf_loader.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -34,8 +34,9 @@
         owner_password: Optional[str] = None,
         user_password: Optional[str] = None,
     ) -> None: ...
     def extract_bytes(self) -> List[bytes]: ...
     def extract_strings(self) -> List[str]: ...
     def extract_page_info(self) -> List[PageInfo]: ...
     def extract_images(self, page_number: int) -> List[npt.NDArray[Any]]: ...
+    def page_to_image(self, page_number: int, dpi: int = 150) -> npt.NDArray[Any]: ...
     def __del__(self) -> None: ...
```

### Comparing `xpydf-0.1.4.4/src/xpydf.egg-info/PKG-INFO` & `xpydf-0.1.4.5/src/xpydf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpydf
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: Python wrapper around the pdftotext and pdfimages functionalities of xpdf.
 Author-email: Matthijs Wesseling <matthijs.wesseling@bigdatarepublic.nl>
 Project-URL: Homepage, https://github.com/Bladieblah/xpdf-python
 Project-URL: Bug Tracker, https://github.com/Bladieblah/xpdf-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `xpydf-0.1.4.4/tests/test_pdf_loader.py` & `xpydf-0.1.4.5/tests/test_pdf_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,8 +110,18 @@
         loader = PdfLoader(str(DATA / "xpdf_tests_password.pdf"), user_password="userpassword")
         text = loader.extract_strings()
         self.assertEqual(1, len(text))
         
         loader = PdfLoader(str(DATA / "xpdf_tests_password.pdf"), owner_password="ownerpassword", user_password="userpassword")
         text = loader.extract_strings()
         self.assertEqual(1, len(text))
-            
+    
+    def test_page_to_image(self):
+        loader = PdfLoader(str(DATA / "xpdf_tests.pdf"))
+        page = loader.page_to_image(1, 150)
+        page_high_res = loader.page_to_image(1, 300)
+
+        self.assertEqual(3, len(page.shape))
+        self.assertEqual(3, len(page_high_res.shape))
+        self.assertEqual(2 * page.shape[0], page_high_res.shape[0])
+        self.assertEqual(2 * page.shape[1], page_high_res.shape[1])
+        self.assertEqual(page.shape[2], page_high_res.shape[2])
```

