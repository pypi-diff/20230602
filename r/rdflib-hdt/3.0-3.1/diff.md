# Comparing `tmp/rdflib_hdt-3.0.tar.gz` & `tmp/rdflib_hdt-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rdflib_hdt-3.0.tar", last modified: Mon May 11 13:47:53 2020, max compression
+gzip compressed data, was "dist/rdflib_hdt-3.1.tar", last modified: Fri Jun  2 12:21:56 2023, max compression
```

## Comparing `rdflib_hdt-3.0.tar` & `rdflib_hdt-3.1.tar`

### file list

```diff
@@ -1,347 +1,350 @@
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/
--rw-r--r--   0 minier-t   (502) staff       (20)      931 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/MANIFEST.in
--rw-r--r--   0 minier-t   (502) staff       (20)     8391 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/PKG-INFO
--rw-r--r--   0 minier-t   (502) staff       (20)     6524 2020-05-11 13:45:57.000000 rdflib_hdt-3.0/README.rst
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/
--rw-r--r--   0 minier-t   (502) staff       (20)     4866 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Array.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3983 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequence.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1934 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilder.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1636 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderDArray.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1452 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderRG.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1501 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderRRR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1646 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderSDArray.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2265 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceDArray.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3397 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceRG.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3918 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceRRR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1872 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceSDArray.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2690 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitString.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1988 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitmapsSequence.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1354 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Coder.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2156 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/HuffmanCoder.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2431 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1623 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_DAC.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2039 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_DAC_VAR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2208 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_FMN.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1924 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_PT.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1727 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_PhiSpare.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2059 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_Sad.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1680 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_naive.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1865 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Mapper.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1725 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/MapperCont.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1478 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/MapperNone.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1723 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/MapperRev.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2025 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/NPR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2750 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/NPR_CN.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2070 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/NPR_FMN.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2302 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/NSV.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2308 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PSV.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1771 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Permutation.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1354 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationBuilder.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1280 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationBuilderMRRR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1177 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationBuilderWT.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1845 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationMRRR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1632 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationWT.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3682 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/RMQ_succinct.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3431 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/RMQ_succinct_lcp.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2844 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Sequence.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2474 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceAlphPart.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1574 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilder.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1411 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderAlphPart.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1355 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderGMR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1386 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderGMRChunk.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1360 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderStr.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1382 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletMatrix.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1404 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTree.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1402 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTreeNoptrs.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1483 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTreeNoptrsS.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2328 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceGMR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2479 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceGMRChunk.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3794 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SuffixTree.h
--rw-r--r--   0 minier-t   (502) staff       (20)     4656 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SuffixTreeY.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3094 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/TableOffsetRRR.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3969 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/TextIndex.h
--rw-r--r--   0 minier-t   (502) staff       (20)     4496 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/TextIndexCSA.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2736 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/WaveletMatrix.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3438 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/WaveletTree.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3830 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/WaveletTreeNoptrs.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3202 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/WaveletTreeNoptrsS.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2867 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/comparray4.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2503 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/cppUtils.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2072 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/factorization.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2361 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/factorization_var.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2576 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/huff.h
--rw-r--r--   0 minier-t   (502) staff       (20)     4102 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/interface.h
--rw-r--r--   0 minier-t   (502) staff       (20)     8293 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/libcdsBasics.h
--rw-r--r--   0 minier-t   (502) staff       (20)     4486 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/libcdsSDArray.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2881 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/libcdsTrees.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1436 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/mmap.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2234 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/perm.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2116 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/sdarraySadakane.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1208 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/timing.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2428 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_coder.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2123 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_coder_binary.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2133 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_coder_huff.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1893 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_node.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2282 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_node_internal.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1930 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_node_leaf.h
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/
--rw-r--r--   0 minier-t   (502) staff       (20)     3431 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequence.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1325 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderDArray.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1285 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderRG.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1318 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderRRR.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1338 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderSDArray.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     7208 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceDArray.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     9495 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceRG.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)    13121 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceRRR.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3059 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceSDArray.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3477 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/TableOffsetRRR.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)    12336 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/sdarraySadakane.cpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/coders/
--rw-r--r--   0 minier-t   (502) staff       (20)     2756 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/coders/HuffmanCoder.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6027 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/coders/huff.cpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/
--rw-r--r--   0 minier-t   (502) staff       (20)       37 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/Makefile
--rw-r--r--   0 minier-t   (502) staff       (20)     1450 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/Mapper.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2129 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperCont.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1401 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperNone.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2437 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperRev.cpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/
--rw-r--r--   0 minier-t   (502) staff       (20)     1727 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/Permutation.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1242 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationBuilderMRRR.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      941 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationBuilderWT.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1799 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationMRRR.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2345 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationWT.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5781 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/perm.cpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/
--rw-r--r--   0 minier-t   (502) staff       (20)     4754 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/BitmapsSequence.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2423 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/Sequence.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)    11423 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceAlphPart.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1564 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderAlphPart.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1698 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderGMR.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1378 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderGMRChunk.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     9209 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderStr.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1392 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletMatrix.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1887 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTree.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1432 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTreeNoptrs.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1522 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTreeNoptrsS.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6891 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceGMR.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5407 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceGMRChunk.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     8917 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletMatrix.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5330 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTree.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)    14609 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTreeNoptrs.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)    12383 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTreeNoptrsS.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1463 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2726 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder_binary.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3585 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder_huff.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1284 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     9354 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node_internal.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2457 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node_leaf.cpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/
--rw-r--r--   0 minier-t   (502) staff       (20)     3629 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/Array.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1968 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/BitString.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      601 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/cppUtils.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1284 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/timing.cpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/
--rw-r--r--   0 minier-t   (502) staff       (20)     3209 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/ControlInformation.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     7278 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/Dictionary.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3910 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDT.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2436 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTEnums.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3724 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTListener.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3256 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTManager.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2146 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTSpecification.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2142 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTVersion.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6100 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTVocabulary.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4748 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/Header.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6804 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/Iterator.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2354 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/RDF.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3157 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/RDFParser.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1920 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/RDFSerializer.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)    12499 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/SingleTriple.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5233 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/Triples.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/bitsequence/
--rw-r--r--   0 minier-t   (502) staff       (20)     2851 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSeq.h
--rw-r--r--   0 minier-t   (502) staff       (20)    11021 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSequence375.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2947 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSequence375.h
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/
--rw-r--r--   0 minier-t   (502) staff       (20)    16780 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/FourSectionDictionary.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3537 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/FourSectionDictionary.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)    13759 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/KyotoDictionary.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4407 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/KyotoDictionary.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)    21295 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/LiteralDictionary.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4329 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/LiteralDictionary.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)    19650 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/PlainDictionary.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6108 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/PlainDictionary.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/
--rw-r--r--   0 minier-t   (502) staff       (20)    28091 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/BasicHDT.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4820 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/BasicHDT.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4232 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/BasicModifiableHDT.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2284 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/BasicModifiableHDT.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6295 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/ControlInformation.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3514 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/HDTFactory.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2490 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/HDTFactory.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2606 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/HDTManager.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2147 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/HDTSpecification.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1232 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/TripleIDStringIterator.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      769 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/TripleIDStringIterator.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/header/
--rw-r--r--   0 minier-t   (502) staff       (20)     5789 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/header/PlainHeader.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2856 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/header/PlainHeader.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/
--rw-r--r--   0 minier-t   (502) staff       (20)     2838 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/Huffman.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2254 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/Huffman.h
--rw-r--r--   0 minier-t   (502) staff       (20)     7752 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/huff.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2762 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/huff.h
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/
--rw-r--r--   0 minier-t   (502) staff       (20)     2448 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3780 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2817 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3643 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2260 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache2.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3471 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache2.h
--rw-r--r--   0 minier-t   (502) staff       (20)    12102 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_FMIndex.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5182 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_FMIndex.h
--rw-r--r--   0 minier-t   (502) staff       (20)    19165 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_HTFC.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     7021 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_HTFC.h
--rw-r--r--   0 minier-t   (502) staff       (20)    13483 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_PFC.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)    11245 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_PFC.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3350 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/VByte.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2075 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/VByte.h
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/
--rw-r--r--   0 minier-t   (502) staff       (20)     9115 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SSA.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2995 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SSA.h
--rw-r--r--   0 minier-t   (502) staff       (20)    12775 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SuffixArray.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4197 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SuffixArray.h
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/
--rw-r--r--   0 minier-t   (502) staff       (20)     2377 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/binarynode.h
--rw-r--r--   0 minier-t   (502) staff       (20)     5634 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/hutucker.h
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/
--rw-r--r--   0 minier-t   (502) staff       (20)      567 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParser.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3832 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserNtriples.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      635 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserNtriples.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6013 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserSerd.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1593 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserSerd.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)      891 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializer.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1370 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerNTriples.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      567 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerNTriples.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3619 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerSerd.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      609 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerSerd.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/
--rw-r--r--   0 minier-t   (502) staff       (20)     5712 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/AdjacencyList.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2154 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/AdjacencyList.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2679 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/ArraySequence.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2421 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/ArraySequence.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4196 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/HuffmanSequence.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2634 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/HuffmanSequence.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2359 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/IntSequence.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4212 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/IntSequence.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2906 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2536 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     9348 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence2.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6491 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence2.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3999 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/WaveletSequence.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2623 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/WaveletSequence.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/
--rw-r--r--   0 minier-t   (502) staff       (20)     2665 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/BaseJoinBinding.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1989 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/CachedBinding.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1896 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/IndexJoinBinding.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      872 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/IndexJoinBinding.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5791 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/JoinAlgorithms.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      891 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/JoinAlgorithms.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4925 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/MergeJoinBinding.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      899 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/MergeJoinBinding.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4942 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/QueryProcessor.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1655 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/QueryProcessor.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1724 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/SortBinding.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      849 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/SortBinding.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3145 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/TriplePatternBinding.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1331 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/TriplePatternBinding.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1462 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/VarBindingInterface.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1787 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/VarFilterBinding.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)      326 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/joins.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/
--rw-r--r--   0 minier-t   (502) staff       (20)    28091 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriples.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     7571 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriples.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)    24959 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriplesIterators.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     8060 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/PlainTriples.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3926 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/PlainTriples.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5626 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleIterators.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2693 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleIterators.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)    10960 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleListDisk.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4822 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleListDisk.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6115 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleOrderConvert.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2928 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleOrderConvert.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3665 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesComparator.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1641 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesComparator.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     7221 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesKyoto.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4918 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesKyoto.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)    47631 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesList.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5105 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesList.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4656 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/predicateindex.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3301 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/predicateindex.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/
--rw-r--r--   0 minier-t   (502) staff       (20)     5157 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/Histogram.h
--rw-r--r--   0 minier-t   (502) staff       (20)     4214 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/StopWatch.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1989 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/StopWatch.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)      984 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/bitutil.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3328 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/bitutil.h
--rw-r--r--   0 minier-t   (502) staff       (20)     4369 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc16.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2911 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc16.h
--rw-r--r--   0 minier-t   (502) staff       (20)     5651 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc32.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3473 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc32.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3214 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc8.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2536 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc8.h
--rw-r--r--   0 minier-t   (502) staff       (20)     4235 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/fdstream.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     6158 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/fileUtil.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1843 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/fileUtil.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3788 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/filemap.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1655 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/filemap.h
--rw-r--r--   0 minier-t   (502) staff       (20)     3553 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/getopt.c
--rw-r--r--   0 minier-t   (502) staff       (20)     4594 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/lru_cache.h
--rw-r--r--   0 minier-t   (502) staff       (20)     1719 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/lrucache.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)      305 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/mygetopt.h
--rw-r--r--   0 minier-t   (502) staff       (20)     5237 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/propertyutil.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)      960 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/propertyutil.h
--rw-r--r--   0 minier-t   (502) staff       (20)     2023 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/unicode.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/third/
--rw-r--r--   0 minier-t   (502) staff       (20)     4764 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/third/fdstream.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     5148 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/third/gzstream.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4631 2018-11-16 13:21:31.000000 rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/third/gzstream.h
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/include/
--rw-r--r--   0 minier-t   (502) staff       (20)    11009 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/include/docstrings.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     7331 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/include/hdt_document.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1409 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/include/join_iterator.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1435 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/include/join_iterator_bytes.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1404 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/include/pyhdt_types.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2488 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/include/triple_iterator.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2543 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/include/triple_iterator_bytes.hpp
--rw-r--r--   0 minier-t   (502) staff       (20)     2657 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/include/tripleid_iterator.hpp
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/rdflib_hdt/
--rw-r--r--   0 minier-t   (502) staff       (20)      315 2020-05-06 08:22:51.000000 rdflib_hdt-3.0/rdflib_hdt/__init__.py
--rw-r--r--   0 minier-t   (502) staff       (20)     8274 2020-05-11 09:09:33.000000 rdflib_hdt-3.0/rdflib_hdt/hdt_document.py
--rw-r--r--   0 minier-t   (502) staff       (20)     3475 2020-05-10 07:18:30.000000 rdflib_hdt-3.0/rdflib_hdt/hdt_store.py
--rw-r--r--   0 minier-t   (502) staff       (20)     3233 2020-05-10 07:21:12.000000 rdflib_hdt-3.0/rdflib_hdt/iterators.py
--rw-r--r--   0 minier-t   (502) staff       (20)      713 2020-05-10 07:21:44.000000 rdflib_hdt-3.0/rdflib_hdt/mapping.py
--rw-r--r--   0 minier-t   (502) staff       (20)     1663 2020-05-11 11:01:16.000000 rdflib_hdt-3.0/rdflib_hdt/sparql_op.py
--rw-r--r--   0 minier-t   (502) staff       (20)      397 2020-04-20 07:21:23.000000 rdflib_hdt-3.0/rdflib_hdt/types.py
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/rdflib_hdt.egg-info/
--rw-r--r--   0 minier-t   (502) staff       (20)     8391 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/rdflib_hdt.egg-info/PKG-INFO
--rw-r--r--   0 minier-t   (502) staff       (20)    14699 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/rdflib_hdt.egg-info/SOURCES.txt
--rw-r--r--   0 minier-t   (502) staff       (20)        1 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/rdflib_hdt.egg-info/dependency_links.txt
--rw-r--r--   0 minier-t   (502) staff       (20)       15 2020-05-11 13:47:52.000000 rdflib_hdt-3.0/rdflib_hdt.egg-info/top_level.txt
--rw-r--r--   0 minier-t   (502) staff       (20)       30 2020-03-18 11:16:20.000000 rdflib_hdt-3.0/requirements.txt
--rw-r--r--   0 minier-t   (502) staff       (20)      104 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/setup.cfg
--rw-r--r--   0 minier-t   (502) staff       (20)     3293 2020-05-11 13:27:05.000000 rdflib_hdt-3.0/setup.py
-drwxr-xr-x   0 minier-t   (502) staff       (20)        0 2020-05-11 13:47:53.000000 rdflib_hdt-3.0/src/
--rw-r--r--   0 minier-t   (502) staff       (20)     9177 2020-03-18 12:52:24.000000 rdflib_hdt-3.0/src/hdt.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)    15078 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/src/hdt_document.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1774 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/src/join_iterator.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     1911 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/src/join_iterator_bytes.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3800 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/src/triple_iterator.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     3999 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/src/triple_iterator_bytes.cpp
--rw-r--r--   0 minier-t   (502) staff       (20)     4296 2020-03-18 10:54:36.000000 rdflib_hdt-3.0/src/tripleid_iterator.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderDArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderRG.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderRRR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderSDArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceDArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceRG.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceRRR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceSDArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitString.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitmapsSequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Coder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/HuffmanCoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_DAC.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_DAC_VAR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_FMN.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_PT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_PhiSpare.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_Sad.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_naive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Mapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/MapperCont.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/MapperNone.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/MapperRev.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/NPR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/NPR_CN.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/NPR_FMN.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/NSV.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PSV.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Permutation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationBuilderMRRR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationBuilderWT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationMRRR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationWT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/RMQ_succinct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/RMQ_succinct_lcp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Sequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceAlphPart.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderAlphPart.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderGMR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderGMRChunk.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderStr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTreeNoptrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTreeNoptrsS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceGMR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceGMRChunk.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SuffixTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SuffixTreeY.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/TableOffsetRRR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/TextIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/TextIndexCSA.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/WaveletMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/WaveletTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/WaveletTreeNoptrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/WaveletTreeNoptrsS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/comparray4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/cppUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/factorization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/factorization_var.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/huff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/libcdsBasics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/libcdsSDArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/libcdsTrees.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/mmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/perm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/sdarraySadakane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/timing.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_coder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_coder_binary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_coder_huff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_node.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_node_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_node_leaf.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderDArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderRG.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderRRR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderSDArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceDArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceRG.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceRRR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceSDArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/TableOffsetRRR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/sdarraySadakane.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/coders/HuffmanCoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/coders/huff.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/Mapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperCont.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperNone.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperRev.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/Permutation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationBuilderMRRR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationBuilderWT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationMRRR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationWT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/perm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/BitmapsSequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/Sequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceAlphPart.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderAlphPart.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderGMR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderGMRChunk.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderStr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTreeNoptrs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTreeNoptrsS.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceGMR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceGMRChunk.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTreeNoptrs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTreeNoptrsS.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder_binary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder_huff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node_internal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node_leaf.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/Array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/BitString.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/cppUtils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/timing.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/ControlInformation.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/Dictionary.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDT.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTEnums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTListener.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTManager.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTSpecification.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTVersion.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTVocabulary.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/Header.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/Iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/RDF.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/RDFParser.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/RDFSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/SingleTriple.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/Triples.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/bitsequence/
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSeq.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSequence375.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSequence375.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/FourSectionDictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/FourSectionDictionary.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/KyotoDictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/KyotoDictionary.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/LiteralDictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/LiteralDictionary.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/PlainDictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/PlainDictionary.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/
+-rw-r--r--   0 runner    (1001) docker     (123)    28091 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/BasicHDT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/BasicHDT.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/BasicModifiableHDT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/BasicModifiableHDT.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/ControlInformation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/HDTFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/HDTFactory.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/HDTManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/HDTSpecification.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/TripleIDStringIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/TripleIDStringIterator.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/header/
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/header/PlainHeader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/header/PlainHeader.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/Huffman.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/Huffman.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/huff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/huff.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_FMIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_FMIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19165 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_HTFC.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_HTFC.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_PFC.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_PFC.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/VByte.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/VByte.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SSA.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SSA.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SuffixArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SuffixArray.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/binarynode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/hutucker.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserNtriples.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserNtriples.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserSerd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserSerd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerNTriples.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerNTriples.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerSerd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerSerd.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/AdjacencyList.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/AdjacencyList.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/ArraySequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/ArraySequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/HuffmanSequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/HuffmanSequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/IntSequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/IntSequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/WaveletSequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/WaveletSequence.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/BaseJoinBinding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/CachedBinding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/IndexJoinBinding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/IndexJoinBinding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/JoinAlgorithms.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/JoinAlgorithms.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/MergeJoinBinding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/MergeJoinBinding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/QueryProcessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/QueryProcessor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/SortBinding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/SortBinding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/TriplePatternBinding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/TriplePatternBinding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/VarBindingInterface.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/VarFilterBinding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/joins.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/
+-rw-r--r--   0 runner    (1001) docker     (123)    28091 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriples.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriples.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24959 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriplesIterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/PlainTriples.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/PlainTriples.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleIterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleIterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleListDisk.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleListDisk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleOrderConvert.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleOrderConvert.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesComparator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesComparator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesKyoto.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesKyoto.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    47631 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesList.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesList.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/predicateindex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/predicateindex.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/Histogram.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/StopWatch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/StopWatch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/bitutil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/bitutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc16.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc32.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc8.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc8.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/fdstream.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/fileUtil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/fileUtil.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/filemap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/filemap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/getopt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/lru_cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/lrucache.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/mygetopt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/propertyutil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/propertyutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/unicode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/third/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/third/fdstream.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/third/gzstream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-02 12:21:55.000000 rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/third/gzstream.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/include/docstrings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/include/hdt_document.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/include/join_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/include/join_iterator_bytes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/include/pyhdt_types.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/include/triple_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/include/triple_iterator_bytes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/include/tripleid_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/rdflib_hdt/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/rdflib_hdt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/rdflib_hdt/hdt_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/rdflib_hdt/hdt_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/rdflib_hdt/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/rdflib_hdt/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/rdflib_hdt/sparql_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/rdflib_hdt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/rdflib_hdt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/rdflib_hdt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/rdflib_hdt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/rdflib_hdt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/rdflib_hdt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/rdflib_hdt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:21:56.000000 rdflib_hdt-3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/src/hdt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/src/hdt_document.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/src/join_iterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/src/join_iterator_bytes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/src/triple_iterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/src/triple_iterator_bytes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-02 12:19:51.000000 rdflib_hdt-3.1/src/tripleid_iterator.cpp
```

### Comparing `rdflib_hdt-3.0/MANIFEST.in` & `rdflib_hdt-3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/PKG-INFO` & `rdflib_hdt-3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,203 +1,204 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: rdflib_hdt
-Version: 3.0
+Version: 3.1
 Summary: A Store back-end for rdflib to allow for reading and querying HDT documents
-Home-page: https://github.com/RDFLib/rdflib-hdt
-Author: Thomas Minier
-Author-email: tminier01@gmail.com
-License: MIT
-Description: |rdflib-htd logo|
-        
-        |Build Status| |PyPI version|
-        
-        A Store back-end for `rdflib <https://github.com/RDFLib>`_ to allow for reading and querying HDT documents.
-        
-        `Online Documentation <https://rdflib.dev/rdflib-hdt/>`_
-        
-        Requirements
-        ============
-        
-        
-        * Python *version 3.6.4 or higher*
-        * `pip <https://pip.pypa.io/en/stable/>`_
-        * **gcc/clang** with **c++11 support**
-        * **Python Development headers**
-          ..
-        
-             You should have the ``Python.h`` header available on your system.\
-             For example, for Python 3.6, install the ``python3.6-dev`` package on Debian/Ubuntu systems.
-        
-        
-        Installation
-        ============
-        
-        Installation using `pipenv <https://github.com/pypa/pipenv>`_ or a `virtualenv <https://virtualenv.pypa.io/en/stable/>`_ is **strongly advised!**
-        
-        PyPi installation (recommended)
-        -------------------------------
-        
-        .. code-block:: bash
-        
-           # you can install using pip
-           pip install rdflib_hdt
-        
-           # or you can use pipenv
-           pipenv install rdflib_hdt
-        
-        Manual installation
-        -------------------
-        
-        **Requirement:** `pipenv <https://github.com/pypa/pipenv>`_ 
-        
-        .. code-block:: bash
-        
-           git clone https://github.com/Callidon/pyHDT
-           cd pyHDT/
-           ./install.sh
-        
-        Getting started
-        ===============
-        
-        You can use the ``rdflib-hdt`` library in two modes: as an rdflib Graph or as a raw HDT document.
-        
-        Graph usage (recommended)
-        -------------------------
-        
-        .. code-block:: python
-        
-           from rdflib import Graph
-           from rdflib_hdt import HDTStore
-           from rdflib.namespace import FOAF
-        
-           # Load an HDT file. Missing indexes are generated automatically
-           # You can provide the index file by putting them in the same directory than the HDT file.
-           store = HDTGraph("test.hdt")
-        
-           # Display some metadata about the HDT document itself
-           print(f"Number of RDF triples: {len(store)}")
-           print(f"Number of subjects: {store.nb_subjects}")
-           print(f"Number of predicates: {store.nb_predicates}")
-           print(f"Number of objects: {store.nb_objects}")
-           print(f"Number of shared subject-object: {store.nb_shared}")
-        
-        
-        Using the RDFlib API, you can also `execute SPARQL queries <https://rdflib.readthedocs.io/en/stable/intro_to_sparql.html>`_ over an HDT document.
-        If you do so, we recommend that you first call the ``optimize_sparql`` function, which optimize
-        the RDFlib SPARQL query engine in the context of HDT documents.
-        
-        .. code-block:: python
-        
-           from rdflib import Graph
-           from rdflib_hdt import HDTStore, optimize_sparql
-        
-           # Calling this function optimizes the RDFlib SPARQL engine for HDT documents
-           optimize_sparql()
-        
-           graph = Graph(store=HDTStore("test.hdt"))
-        
-           # You can execute SPARQL queries using the regular RDFlib API
-           qres = graph.query("""
-           PREFIX foaf: <http://xmlns.com/foaf/0.1/>
-           SELECT ?name ?friend WHERE {
-              ?a foaf:knows ?b.
-              ?a foaf:name ?name.
-              ?b foaf:name ?friend.
-           }""")
-        
-           for row in qres:
-             print(f"{row.name} knows {row.friend}")
-        
-        HDT Document usage
-        ------------------
-        
-        .. code-block:: python
-        
-           from rdflib_hdt import HDTDocument
-        
-           # Load an HDT file. Missing indexes are generated automatically.
-           # You can provide the index file by putting them in the same directory than the HDT file.
-           document = HDTDocument("test.hdt")
-        
-           # Display some metadata about the HDT document itself
-           print(f"Number of RDF triples: {document.total_triples}")
-           print(f"Number of subjects: {document.nb_subjects}")
-           print(f"Number of predicates: {document.nb_predicates}")
-           print(f"Number of objects: {document.nb_objects}")
-           print(f"Number of shared subject-object: {document.nb_shared}")
-        
-           # Fetch all triples that matches { ?s foaf:name ?o }
-           # Use None to indicates variables
-           triples, cardinality = document.search_triples((None, FOAF("name"), None))
-        
-           print(f"Cardinality of (?s foaf:name ?o): {cardinality}")
-           for s, p, o in triples:
-             print(triple)
-        
-           # The search also support limit and offset
-           triples, cardinality = document.search_triples((None, FOAF("name"), None), limit=10, offset=100)
-           # etc ...
-        
-        An HDT document also provides support for evaluating joins over a set of triples patterns.
-        
-        .. code-block:: python
-        
-          from rdflib_hdt import HDTDocument
-          from rdflib import Variable
-          from rdflib.namespace import FOAF, RDF
-          
-          document = HDTDocument("test.hdt")
-          
-          # find the names of two entities that know each other
-          tp_a = (Variable("a"), FOAF("knows"), Variable("b"))
-          tp_b = (Variable("a"), FOAF("name"), Variable("name"))
-          tp_c = (Variable("b"), FOAF("name"), Variable("friend"))
-          query = set([tp_a, tp_b, tp_c])
-          
-          iterator = document.search_join(query)
-          print(f"Estimated join cardinality: {len(iterator)}")
-          
-          # Join results are produced as ResultRow, like in the RDFlib SPARQL API
-          for row in iterator:
-             print(f"{row.name} knows {row.friend}")
-        
-        Handling non UTF-8 strings in python
-        ====================================
-        
-        If the HDT document has been encoded with a non UTF-8 encoding the previous code won't work correctly and will result in a ``UnicodeDecodeError``.
-        More details on how to convert string to str from C++ to Python `here <https://pybind11.readthedocs.io/en/stable/advanced/cast/strings.html>`_
-        
-        To handle this, we doubled the API of the HDT document by adding:
-        
-        
-        * ``search_triples_bytes(...)`` return an iterator of triples as ``(py::bytes, py::bytes, py::bytes)``
-        * ``search_join_bytes(...)`` return an iterator of sets of solutions mapping as ``py::set(py::bytes, py::bytes)``
-        * ``convert_tripleid_bytes(...)`` return a triple as: ``(py::bytes, py::bytes, py::bytes)``
-        * ``convert_id_bytes(...)`` return a ``py::bytes``
-        
-        **Parameters and documentation are the same as the standard version**
-        
-        .. code-block:: python
-        
-           from rdflib_hdt import HDTDocument
-        
-           document = HDTDocument("test.hdt")
-           it = document.search_triple_bytes("", "", "")
-        
-           for s, p, o in it:
-           print(s, p, o) # print b'...', b'...', b'...'
-           # now decode it, or handle any error
-           try:
-              s, p, o = s.decode('UTF-8'), p.decode('UTF-8'), o.decode('UTF-8')
-           except UnicodeDecodeError as err:
-              # try another other codecs, ignore error, etc
-              pass
-        
-        .. |Build Status| image:: https://github.com/RDFLib/rdflib-hdt/workflows/Python%20tests/badge.svg
-           :target: https://github.com/RDFLib/rdflib-hdt/actions?query=workflow%3A%22Python+tests%22
-        .. |PyPI version| image:: https://badge.fury.io/py/rdflib-hdt.svg
-           :target: https://badge.fury.io/py/rdflib-hdt
-        .. |rdflib-htd logo| image:: https://raw.githubusercontent.com/RDFLib/rdflib-hdt/master/docs/source/_static/rdflib-hdt-250.png
-           :target: https://rdflib.dev/rdflib-hdt/
-        
+Author-email: Thomas Minier <tminier01@gmail.com>
+License: MIT License
+Project-URL: homepage, https://rdflib.dev/rdflib-hdt
+Project-URL: repository, https://github.com/RDFLib/rdflib-hdt.git
 Keywords: rdflib,hdt,rdf,semantic web,search
-Platform: UNKNOWN
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+|rdflib-htd logo|
+
+|Build Status| |PyPI version|
+
+A Store back-end for `rdflib <https://github.com/RDFLib>`_ to allow for reading and querying HDT documents.
+
+`Online Documentation <https://rdflib.dev/rdflib-hdt/>`_
+
+Requirements
+============
+
+
+* Python *version 3.6.4 or higher*
+* `pip <https://pip.pypa.io/en/stable/>`_
+* **gcc/clang** with **c++11 support**
+* **Python Development headers**
+  ..
+
+     You should have the ``Python.h`` header available on your system.\
+     For example, for Python 3.6, install the ``python3.6-dev`` package on Debian/Ubuntu systems.
+
+
+Installation
+============
+
+Installation using `pipenv <https://github.com/pypa/pipenv>`_ or a `virtualenv <https://virtualenv.pypa.io/en/stable/>`_ is **strongly advised!**
+
+PyPi installation (recommended)
+-------------------------------
+
+.. code-block:: bash
+
+   # you can install using pip
+   pip install rdflib-hdt
+
+   # or you can use pipenv
+   pipenv install rdflib-hdt
+
+Manual installation
+-------------------
+
+**Requirement:** `pipenv <https://github.com/pypa/pipenv>`_ 
+
+.. code-block:: bash
+
+   git clone https://github.com/Callidon/pyHDT
+   cd pyHDT/
+   ./install.sh
+
+Getting started
+===============
+
+You can use the ``rdflib-hdt`` library in two modes: as an rdflib Graph or as a raw HDT document.
+
+Graph usage (recommended)
+-------------------------
+
+.. code-block:: python
+
+   from rdflib import Graph
+   from rdflib_hdt import HDTStore
+   from rdflib.namespace import FOAF
+
+   # Load an HDT file. Missing indexes are generated automatically
+   # You can provide the index file by putting them in the same directory than the HDT file.
+   store = HDTGraph("test.hdt")
+
+   # Display some metadata about the HDT document itself
+   print(f"Number of RDF triples: {len(store)}")
+   print(f"Number of subjects: {store.nb_subjects}")
+   print(f"Number of predicates: {store.nb_predicates}")
+   print(f"Number of objects: {store.nb_objects}")
+   print(f"Number of shared subject-object: {store.nb_shared}")
+
+
+Using the RDFlib API, you can also `execute SPARQL queries <https://rdflib.readthedocs.io/en/stable/intro_to_sparql.html>`_ over an HDT document.
+If you do so, we recommend that you first call the ``optimize_sparql`` function, which optimize
+the RDFlib SPARQL query engine in the context of HDT documents.
+
+.. code-block:: python
+
+   from rdflib import Graph
+   from rdflib_hdt import HDTStore, optimize_sparql
+
+   # Calling this function optimizes the RDFlib SPARQL engine for HDT documents
+   optimize_sparql()
+
+   graph = Graph(store=HDTStore("test.hdt"))
+
+   # You can execute SPARQL queries using the regular RDFlib API
+   qres = graph.query("""
+   PREFIX foaf: <http://xmlns.com/foaf/0.1/>
+   SELECT ?name ?friend WHERE {
+      ?a foaf:knows ?b.
+      ?a foaf:name ?name.
+      ?b foaf:name ?friend.
+   }""")
+
+   for row in qres:
+     print(f"{row.name} knows {row.friend}")
+
+HDT Document usage
+------------------
+
+.. code-block:: python
+
+   from rdflib_hdt import HDTDocument
+
+   # Load an HDT file. Missing indexes are generated automatically.
+   # You can provide the index file by putting them in the same directory than the HDT file.
+   document = HDTDocument("test.hdt")
+
+   # Display some metadata about the HDT document itself
+   print(f"Number of RDF triples: {document.total_triples}")
+   print(f"Number of subjects: {document.nb_subjects}")
+   print(f"Number of predicates: {document.nb_predicates}")
+   print(f"Number of objects: {document.nb_objects}")
+   print(f"Number of shared subject-object: {document.nb_shared}")
+
+   # Fetch all triples that matches { ?s foaf:name ?o }
+   # Use None to indicates variables
+   triples, cardinality = document.search_triples((None, FOAF("name"), None))
+
+   print(f"Cardinality of (?s foaf:name ?o): {cardinality}")
+   for s, p, o in triples:
+     print(triple)
+
+   # The search also support limit and offset
+   triples, cardinality = document.search_triples((None, FOAF("name"), None), limit=10, offset=100)
+   # etc ...
+
+An HDT document also provides support for evaluating joins over a set of triples patterns.
+
+.. code-block:: python
+
+  from rdflib_hdt import HDTDocument
+  from rdflib import Variable
+  from rdflib.namespace import FOAF, RDF
+  
+  document = HDTDocument("test.hdt")
+  
+  # find the names of two entities that know each other
+  tp_a = (Variable("a"), FOAF("knows"), Variable("b"))
+  tp_b = (Variable("a"), FOAF("name"), Variable("name"))
+  tp_c = (Variable("b"), FOAF("name"), Variable("friend"))
+  query = set([tp_a, tp_b, tp_c])
+  
+  iterator = document.search_join(query)
+  print(f"Estimated join cardinality: {len(iterator)}")
+  
+  # Join results are produced as ResultRow, like in the RDFlib SPARQL API
+  for row in iterator:
+     print(f"{row.name} knows {row.friend}")
+
+Handling non UTF-8 strings in python
+====================================
+
+If the HDT document has been encoded with a non UTF-8 encoding the previous code won't work correctly and will result in a ``UnicodeDecodeError``.
+More details on how to convert string to str from C++ to Python `here <https://pybind11.readthedocs.io/en/stable/advanced/cast/strings.html>`_
+
+To handle this, we doubled the API of the HDT document by adding:
+
+
+* ``search_triples_bytes(...)`` return an iterator of triples as ``(py::bytes, py::bytes, py::bytes)``
+* ``search_join_bytes(...)`` return an iterator of sets of solutions mapping as ``py::set(py::bytes, py::bytes)``
+* ``convert_tripleid_bytes(...)`` return a triple as: ``(py::bytes, py::bytes, py::bytes)``
+* ``convert_id_bytes(...)`` return a ``py::bytes``
+
+**Parameters and documentation are the same as the standard version**
+
+.. code-block:: python
+
+   from rdflib_hdt import HDTDocument
+
+   document = HDTDocument("test.hdt")
+   it = document.search_triple_bytes("", "", "")
+
+   for s, p, o in it:
+   print(s, p, o) # print b'...', b'...', b'...'
+   # now decode it, or handle any error
+   try:
+      s, p, o = s.decode('UTF-8'), p.decode('UTF-8'), o.decode('UTF-8')
+   except UnicodeDecodeError as err:
+      # try another other codecs, ignore error, etc
+      pass
+
+.. |Build Status| image:: https://github.com/RDFLib/rdflib-hdt/workflows/Python%20tests/badge.svg
+   :target: https://github.com/RDFLib/rdflib-hdt/actions?query=workflow%3A%22Python+tests%22
+.. |PyPI version| image:: https://badge.fury.io/py/rdflib-hdt.svg
+   :target: https://badge.fury.io/py/rdflib-hdt
+.. |rdflib-htd logo| image:: https://raw.githubusercontent.com/RDFLib/rdflib-hdt/master/docs/source/_static/rdflib-hdt-250.png
+   :target: https://rdflib.dev/rdflib-hdt/
```

### Comparing `rdflib_hdt-3.0/README.rst` & `rdflib_hdt-3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 
 PyPi installation (recommended)
 -------------------------------
 
 .. code-block:: bash
 
    # you can install using pip
-   pip install rdflib_hdt
+   pip install rdflib-hdt
 
    # or you can use pipenv
-   pipenv install rdflib_hdt
+   pipenv install rdflib-hdt
 
 Manual installation
 -------------------
 
 **Requirement:** `pipenv <https://github.com/pypa/pipenv>`_ 
 
 .. code-block:: bash
```

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Array.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Array.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequence.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequence.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilder.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilder.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderDArray.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderDArray.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderRG.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderRG.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderRRR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderRRR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderSDArray.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderSDArray.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceDArray.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceDArray.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceRG.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceRG.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceRRR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceRRR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitSequenceSDArray.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitSequenceSDArray.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitString.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitString.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/BitmapsSequence.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/BitmapsSequence.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Coder.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Coder.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/HuffmanCoder.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/HuffmanCoder.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_DAC.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_DAC.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_DAC_VAR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_DAC_VAR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_FMN.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_FMN.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_PT.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_PT.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_PhiSpare.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_PhiSpare.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_Sad.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_Sad.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/LCP_naive.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/LCP_naive.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Mapper.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Mapper.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/MapperCont.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/MapperCont.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/MapperNone.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/MapperNone.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/MapperRev.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/MapperRev.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/NPR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/NPR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/NPR_CN.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/NPR_CN.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/NPR_FMN.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/NPR_FMN.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/NSV.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/NSV.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PSV.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PSV.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Permutation.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Permutation.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationBuilder.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationBuilder.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationBuilderMRRR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationBuilderMRRR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationBuilderWT.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationBuilderWT.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationMRRR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationMRRR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/PermutationWT.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/PermutationWT.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/RMQ_succinct.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/RMQ_succinct.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/RMQ_succinct_lcp.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/RMQ_succinct_lcp.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/Sequence.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/Sequence.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceAlphPart.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceAlphPart.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilder.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilder.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderAlphPart.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderAlphPart.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderGMR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderGMR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderGMRChunk.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderGMRChunk.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderStr.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderStr.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletMatrix.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletMatrix.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTree.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTree.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTreeNoptrs.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTreeNoptrs.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTreeNoptrsS.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceBuilderWaveletTreeNoptrsS.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceGMR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceGMR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SequenceGMRChunk.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SequenceGMRChunk.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SuffixTree.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SuffixTree.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/SuffixTreeY.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/SuffixTreeY.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/TableOffsetRRR.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/TableOffsetRRR.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/TextIndex.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/TextIndex.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/TextIndexCSA.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/TextIndexCSA.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/WaveletMatrix.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/WaveletMatrix.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/WaveletTree.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/WaveletTree.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/WaveletTreeNoptrs.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/WaveletTreeNoptrs.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/WaveletTreeNoptrsS.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/WaveletTreeNoptrsS.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/comparray4.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/comparray4.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/cppUtils.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/cppUtils.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/factorization.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/factorization.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/factorization_var.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/factorization_var.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/huff.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/huff.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/interface.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/interface.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/libcdsBasics.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/libcdsBasics.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/libcdsSDArray.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/libcdsSDArray.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/libcdsTrees.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/libcdsTrees.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/mmap.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/mmap.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/perm.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/perm.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/sdarraySadakane.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/sdarraySadakane.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/timing.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/timing.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_coder.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_coder.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_coder_binary.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_coder_binary.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_coder_huff.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_coder_huff.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_node.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_node.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_node_internal.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_node_internal.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/include/wt_node_leaf.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/include/wt_node_leaf.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequence.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequence.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderDArray.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderDArray.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderRG.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderRG.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderRRR.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderRRR.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderSDArray.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceBuilderSDArray.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceDArray.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceDArray.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceRG.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceRG.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceRRR.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceRRR.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceSDArray.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/BitSequenceSDArray.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/TableOffsetRRR.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/TableOffsetRRR.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/bitsequence/sdarraySadakane.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/bitsequence/sdarraySadakane.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/coders/HuffmanCoder.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/coders/HuffmanCoder.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/coders/huff.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/coders/huff.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/Mapper.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/Mapper.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperCont.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperCont.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperNone.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperNone.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperRev.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/mapper/MapperRev.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/Permutation.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/Permutation.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationBuilderMRRR.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationBuilderMRRR.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationBuilderWT.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationBuilderWT.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationMRRR.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationMRRR.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationWT.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/PermutationWT.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/permutation/perm.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/permutation/perm.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/BitmapsSequence.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/BitmapsSequence.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/Sequence.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/Sequence.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceAlphPart.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceAlphPart.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderAlphPart.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderAlphPart.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderGMR.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderGMR.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderGMRChunk.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderGMRChunk.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderStr.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderStr.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletMatrix.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletMatrix.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTree.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTree.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTreeNoptrs.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTreeNoptrs.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTreeNoptrsS.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceBuilderWaveletTreeNoptrsS.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceGMR.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceGMR.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceGMRChunk.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/SequenceGMRChunk.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletMatrix.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletMatrix.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTree.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTree.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTreeNoptrs.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTreeNoptrs.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTreeNoptrsS.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/WaveletTreeNoptrsS.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder_binary.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder_binary.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder_huff.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_coder_huff.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node_internal.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node_internal.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node_leaf.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/static/sequence/wt_node_leaf.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/Array.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/Array.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/BitString.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/BitString.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/cppUtils.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/cppUtils.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libcds/src/utils/timing.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libcds/src/utils/timing.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/ControlInformation.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/ControlInformation.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/Dictionary.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/Dictionary.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDT.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDT.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTEnums.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTEnums.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTListener.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTListener.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTManager.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTManager.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTSpecification.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTSpecification.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTVersion.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTVersion.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/HDTVocabulary.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/HDTVocabulary.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/Header.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/Header.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/Iterator.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/Iterator.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/RDF.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/RDF.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/RDFParser.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/RDFParser.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/RDFSerializer.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/RDFSerializer.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/SingleTriple.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/SingleTriple.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/include/Triples.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/include/Triples.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSeq.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSeq.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSequence375.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSequence375.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSequence375.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/bitsequence/BitSequence375.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/FourSectionDictionary.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/FourSectionDictionary.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/FourSectionDictionary.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/FourSectionDictionary.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/KyotoDictionary.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/KyotoDictionary.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/KyotoDictionary.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/KyotoDictionary.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/LiteralDictionary.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/LiteralDictionary.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/LiteralDictionary.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/LiteralDictionary.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/PlainDictionary.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/PlainDictionary.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/dictionary/PlainDictionary.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/dictionary/PlainDictionary.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/BasicHDT.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/BasicHDT.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/BasicHDT.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/BasicHDT.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/BasicModifiableHDT.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/BasicModifiableHDT.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/BasicModifiableHDT.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/BasicModifiableHDT.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/ControlInformation.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/ControlInformation.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/HDTFactory.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/HDTFactory.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/HDTFactory.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/HDTFactory.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/HDTManager.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/HDTManager.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/HDTSpecification.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/HDTSpecification.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/TripleIDStringIterator.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/TripleIDStringIterator.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/hdt/TripleIDStringIterator.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/hdt/TripleIDStringIterator.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/header/PlainHeader.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/header/PlainHeader.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/header/PlainHeader.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/header/PlainHeader.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/Huffman.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/Huffman.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/Huffman.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/Huffman.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/huff.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/huff.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/huffman/huff.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/huffman/huff.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache2.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache2.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache2.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_Cache2.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_FMIndex.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_FMIndex.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_FMIndex.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_FMIndex.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_HTFC.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_HTFC.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_HTFC.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_HTFC.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_PFC.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_PFC.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_PFC.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/CSD_PFC.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/VByte.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/VByte.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/VByte.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/VByte.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SSA.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SSA.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SSA.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SSA.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SuffixArray.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SuffixArray.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SuffixArray.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/fmindex/SuffixArray.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/binarynode.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/binarynode.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/hutucker.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/libdcs/hutucker/hutucker.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParser.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParser.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserNtriples.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserNtriples.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserNtriples.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserNtriples.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserSerd.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserSerd.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserSerd.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFParserSerd.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializer.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializer.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerNTriples.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerNTriples.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerNTriples.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerNTriples.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerSerd.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerSerd.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerSerd.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/rdf/RDFSerializerSerd.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/AdjacencyList.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/AdjacencyList.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/AdjacencyList.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/AdjacencyList.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/ArraySequence.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/ArraySequence.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/ArraySequence.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/ArraySequence.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/HuffmanSequence.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/HuffmanSequence.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/HuffmanSequence.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/HuffmanSequence.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/IntSequence.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/IntSequence.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/IntSequence.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/IntSequence.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence2.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence2.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence2.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/LogSequence2.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/WaveletSequence.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/WaveletSequence.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sequence/WaveletSequence.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sequence/WaveletSequence.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/BaseJoinBinding.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/BaseJoinBinding.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/CachedBinding.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/CachedBinding.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/IndexJoinBinding.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/IndexJoinBinding.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/IndexJoinBinding.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/IndexJoinBinding.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/JoinAlgorithms.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/JoinAlgorithms.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/JoinAlgorithms.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/JoinAlgorithms.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/MergeJoinBinding.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/MergeJoinBinding.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/MergeJoinBinding.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/MergeJoinBinding.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/QueryProcessor.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/QueryProcessor.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/QueryProcessor.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/QueryProcessor.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/SortBinding.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/SortBinding.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/SortBinding.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/SortBinding.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/TriplePatternBinding.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/TriplePatternBinding.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/TriplePatternBinding.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/TriplePatternBinding.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/VarBindingInterface.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/VarBindingInterface.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/sparql/VarFilterBinding.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/sparql/VarFilterBinding.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriples.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriples.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriples.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriples.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriplesIterators.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/BitmapTriplesIterators.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/PlainTriples.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/PlainTriples.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/PlainTriples.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/PlainTriples.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleIterators.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleIterators.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleIterators.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleIterators.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleListDisk.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleListDisk.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleListDisk.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleListDisk.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleOrderConvert.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleOrderConvert.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TripleOrderConvert.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TripleOrderConvert.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesComparator.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesComparator.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesComparator.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesComparator.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesKyoto.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesKyoto.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesKyoto.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesKyoto.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesList.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesList.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/TriplesList.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/TriplesList.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/predicateindex.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/predicateindex.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/triples/predicateindex.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/triples/predicateindex.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/Histogram.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/Histogram.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/StopWatch.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/StopWatch.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/StopWatch.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/StopWatch.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/bitutil.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/bitutil.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/bitutil.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/bitutil.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc16.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc16.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc16.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc16.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc32.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc32.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc32.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc32.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc8.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc8.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/crc8.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/crc8.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/fdstream.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/fdstream.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/fileUtil.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/fileUtil.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/fileUtil.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/fileUtil.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/filemap.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/filemap.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/filemap.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/filemap.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/getopt.c` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/getopt.c`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/lru_cache.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/lru_cache.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/lrucache.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/lrucache.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/propertyutil.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/propertyutil.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/propertyutil.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/propertyutil.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/src/util/unicode.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/src/util/unicode.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/third/fdstream.hpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/third/fdstream.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/third/gzstream.cpp` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/third/gzstream.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/hdt-cpp-1.3.3/libhdt/third/gzstream.h` & `rdflib_hdt-3.1/hdt-cpp-1.3.3/libhdt/third/gzstream.h`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/include/docstrings.hpp` & `rdflib_hdt-3.1/include/docstrings.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/include/hdt_document.hpp` & `rdflib_hdt-3.1/include/hdt_document.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/include/join_iterator.hpp` & `rdflib_hdt-3.1/include/join_iterator.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/include/join_iterator_bytes.hpp` & `rdflib_hdt-3.1/include/join_iterator_bytes.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/include/pyhdt_types.hpp` & `rdflib_hdt-3.1/include/pyhdt_types.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/include/triple_iterator.hpp` & `rdflib_hdt-3.1/include/triple_iterator.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/include/triple_iterator_bytes.hpp` & `rdflib_hdt-3.1/include/triple_iterator_bytes.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/include/tripleid_iterator.hpp` & `rdflib_hdt-3.1/include/tripleid_iterator.hpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/rdflib_hdt/hdt_document.py` & `rdflib_hdt-3.1/rdflib_hdt/hdt_document.py`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/rdflib_hdt/hdt_store.py` & `rdflib_hdt-3.1/rdflib_hdt/hdt_store.py`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/rdflib_hdt/iterators.py` & `rdflib_hdt-3.1/rdflib_hdt/iterators.py`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/rdflib_hdt/mapping.py` & `rdflib_hdt-3.1/rdflib_hdt/mapping.py`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/rdflib_hdt/sparql_op.py` & `rdflib_hdt-3.1/rdflib_hdt/sparql_op.py`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/rdflib_hdt.egg-info/PKG-INFO` & `rdflib_hdt-3.1/rdflib_hdt.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,203 +1,204 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: rdflib-hdt
-Version: 3.0
+Version: 3.1
 Summary: A Store back-end for rdflib to allow for reading and querying HDT documents
-Home-page: https://github.com/RDFLib/rdflib-hdt
-Author: Thomas Minier
-Author-email: tminier01@gmail.com
-License: MIT
-Description: |rdflib-htd logo|
-        
-        |Build Status| |PyPI version|
-        
-        A Store back-end for `rdflib <https://github.com/RDFLib>`_ to allow for reading and querying HDT documents.
-        
-        `Online Documentation <https://rdflib.dev/rdflib-hdt/>`_
-        
-        Requirements
-        ============
-        
-        
-        * Python *version 3.6.4 or higher*
-        * `pip <https://pip.pypa.io/en/stable/>`_
-        * **gcc/clang** with **c++11 support**
-        * **Python Development headers**
-          ..
-        
-             You should have the ``Python.h`` header available on your system.\
-             For example, for Python 3.6, install the ``python3.6-dev`` package on Debian/Ubuntu systems.
-        
-        
-        Installation
-        ============
-        
-        Installation using `pipenv <https://github.com/pypa/pipenv>`_ or a `virtualenv <https://virtualenv.pypa.io/en/stable/>`_ is **strongly advised!**
-        
-        PyPi installation (recommended)
-        -------------------------------
-        
-        .. code-block:: bash
-        
-           # you can install using pip
-           pip install rdflib_hdt
-        
-           # or you can use pipenv
-           pipenv install rdflib_hdt
-        
-        Manual installation
-        -------------------
-        
-        **Requirement:** `pipenv <https://github.com/pypa/pipenv>`_ 
-        
-        .. code-block:: bash
-        
-           git clone https://github.com/Callidon/pyHDT
-           cd pyHDT/
-           ./install.sh
-        
-        Getting started
-        ===============
-        
-        You can use the ``rdflib-hdt`` library in two modes: as an rdflib Graph or as a raw HDT document.
-        
-        Graph usage (recommended)
-        -------------------------
-        
-        .. code-block:: python
-        
-           from rdflib import Graph
-           from rdflib_hdt import HDTStore
-           from rdflib.namespace import FOAF
-        
-           # Load an HDT file. Missing indexes are generated automatically
-           # You can provide the index file by putting them in the same directory than the HDT file.
-           store = HDTGraph("test.hdt")
-        
-           # Display some metadata about the HDT document itself
-           print(f"Number of RDF triples: {len(store)}")
-           print(f"Number of subjects: {store.nb_subjects}")
-           print(f"Number of predicates: {store.nb_predicates}")
-           print(f"Number of objects: {store.nb_objects}")
-           print(f"Number of shared subject-object: {store.nb_shared}")
-        
-        
-        Using the RDFlib API, you can also `execute SPARQL queries <https://rdflib.readthedocs.io/en/stable/intro_to_sparql.html>`_ over an HDT document.
-        If you do so, we recommend that you first call the ``optimize_sparql`` function, which optimize
-        the RDFlib SPARQL query engine in the context of HDT documents.
-        
-        .. code-block:: python
-        
-           from rdflib import Graph
-           from rdflib_hdt import HDTStore, optimize_sparql
-        
-           # Calling this function optimizes the RDFlib SPARQL engine for HDT documents
-           optimize_sparql()
-        
-           graph = Graph(store=HDTStore("test.hdt"))
-        
-           # You can execute SPARQL queries using the regular RDFlib API
-           qres = graph.query("""
-           PREFIX foaf: <http://xmlns.com/foaf/0.1/>
-           SELECT ?name ?friend WHERE {
-              ?a foaf:knows ?b.
-              ?a foaf:name ?name.
-              ?b foaf:name ?friend.
-           }""")
-        
-           for row in qres:
-             print(f"{row.name} knows {row.friend}")
-        
-        HDT Document usage
-        ------------------
-        
-        .. code-block:: python
-        
-           from rdflib_hdt import HDTDocument
-        
-           # Load an HDT file. Missing indexes are generated automatically.
-           # You can provide the index file by putting them in the same directory than the HDT file.
-           document = HDTDocument("test.hdt")
-        
-           # Display some metadata about the HDT document itself
-           print(f"Number of RDF triples: {document.total_triples}")
-           print(f"Number of subjects: {document.nb_subjects}")
-           print(f"Number of predicates: {document.nb_predicates}")
-           print(f"Number of objects: {document.nb_objects}")
-           print(f"Number of shared subject-object: {document.nb_shared}")
-        
-           # Fetch all triples that matches { ?s foaf:name ?o }
-           # Use None to indicates variables
-           triples, cardinality = document.search_triples((None, FOAF("name"), None))
-        
-           print(f"Cardinality of (?s foaf:name ?o): {cardinality}")
-           for s, p, o in triples:
-             print(triple)
-        
-           # The search also support limit and offset
-           triples, cardinality = document.search_triples((None, FOAF("name"), None), limit=10, offset=100)
-           # etc ...
-        
-        An HDT document also provides support for evaluating joins over a set of triples patterns.
-        
-        .. code-block:: python
-        
-          from rdflib_hdt import HDTDocument
-          from rdflib import Variable
-          from rdflib.namespace import FOAF, RDF
-          
-          document = HDTDocument("test.hdt")
-          
-          # find the names of two entities that know each other
-          tp_a = (Variable("a"), FOAF("knows"), Variable("b"))
-          tp_b = (Variable("a"), FOAF("name"), Variable("name"))
-          tp_c = (Variable("b"), FOAF("name"), Variable("friend"))
-          query = set([tp_a, tp_b, tp_c])
-          
-          iterator = document.search_join(query)
-          print(f"Estimated join cardinality: {len(iterator)}")
-          
-          # Join results are produced as ResultRow, like in the RDFlib SPARQL API
-          for row in iterator:
-             print(f"{row.name} knows {row.friend}")
-        
-        Handling non UTF-8 strings in python
-        ====================================
-        
-        If the HDT document has been encoded with a non UTF-8 encoding the previous code won't work correctly and will result in a ``UnicodeDecodeError``.
-        More details on how to convert string to str from C++ to Python `here <https://pybind11.readthedocs.io/en/stable/advanced/cast/strings.html>`_
-        
-        To handle this, we doubled the API of the HDT document by adding:
-        
-        
-        * ``search_triples_bytes(...)`` return an iterator of triples as ``(py::bytes, py::bytes, py::bytes)``
-        * ``search_join_bytes(...)`` return an iterator of sets of solutions mapping as ``py::set(py::bytes, py::bytes)``
-        * ``convert_tripleid_bytes(...)`` return a triple as: ``(py::bytes, py::bytes, py::bytes)``
-        * ``convert_id_bytes(...)`` return a ``py::bytes``
-        
-        **Parameters and documentation are the same as the standard version**
-        
-        .. code-block:: python
-        
-           from rdflib_hdt import HDTDocument
-        
-           document = HDTDocument("test.hdt")
-           it = document.search_triple_bytes("", "", "")
-        
-           for s, p, o in it:
-           print(s, p, o) # print b'...', b'...', b'...'
-           # now decode it, or handle any error
-           try:
-              s, p, o = s.decode('UTF-8'), p.decode('UTF-8'), o.decode('UTF-8')
-           except UnicodeDecodeError as err:
-              # try another other codecs, ignore error, etc
-              pass
-        
-        .. |Build Status| image:: https://github.com/RDFLib/rdflib-hdt/workflows/Python%20tests/badge.svg
-           :target: https://github.com/RDFLib/rdflib-hdt/actions?query=workflow%3A%22Python+tests%22
-        .. |PyPI version| image:: https://badge.fury.io/py/rdflib-hdt.svg
-           :target: https://badge.fury.io/py/rdflib-hdt
-        .. |rdflib-htd logo| image:: https://raw.githubusercontent.com/RDFLib/rdflib-hdt/master/docs/source/_static/rdflib-hdt-250.png
-           :target: https://rdflib.dev/rdflib-hdt/
-        
+Author-email: Thomas Minier <tminier01@gmail.com>
+License: MIT License
+Project-URL: homepage, https://rdflib.dev/rdflib-hdt
+Project-URL: repository, https://github.com/RDFLib/rdflib-hdt.git
 Keywords: rdflib,hdt,rdf,semantic web,search
-Platform: UNKNOWN
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+|rdflib-htd logo|
+
+|Build Status| |PyPI version|
+
+A Store back-end for `rdflib <https://github.com/RDFLib>`_ to allow for reading and querying HDT documents.
+
+`Online Documentation <https://rdflib.dev/rdflib-hdt/>`_
+
+Requirements
+============
+
+
+* Python *version 3.6.4 or higher*
+* `pip <https://pip.pypa.io/en/stable/>`_
+* **gcc/clang** with **c++11 support**
+* **Python Development headers**
+  ..
+
+     You should have the ``Python.h`` header available on your system.\
+     For example, for Python 3.6, install the ``python3.6-dev`` package on Debian/Ubuntu systems.
+
+
+Installation
+============
+
+Installation using `pipenv <https://github.com/pypa/pipenv>`_ or a `virtualenv <https://virtualenv.pypa.io/en/stable/>`_ is **strongly advised!**
+
+PyPi installation (recommended)
+-------------------------------
+
+.. code-block:: bash
+
+   # you can install using pip
+   pip install rdflib-hdt
+
+   # or you can use pipenv
+   pipenv install rdflib-hdt
+
+Manual installation
+-------------------
+
+**Requirement:** `pipenv <https://github.com/pypa/pipenv>`_ 
+
+.. code-block:: bash
+
+   git clone https://github.com/Callidon/pyHDT
+   cd pyHDT/
+   ./install.sh
+
+Getting started
+===============
+
+You can use the ``rdflib-hdt`` library in two modes: as an rdflib Graph or as a raw HDT document.
+
+Graph usage (recommended)
+-------------------------
+
+.. code-block:: python
+
+   from rdflib import Graph
+   from rdflib_hdt import HDTStore
+   from rdflib.namespace import FOAF
+
+   # Load an HDT file. Missing indexes are generated automatically
+   # You can provide the index file by putting them in the same directory than the HDT file.
+   store = HDTGraph("test.hdt")
+
+   # Display some metadata about the HDT document itself
+   print(f"Number of RDF triples: {len(store)}")
+   print(f"Number of subjects: {store.nb_subjects}")
+   print(f"Number of predicates: {store.nb_predicates}")
+   print(f"Number of objects: {store.nb_objects}")
+   print(f"Number of shared subject-object: {store.nb_shared}")
+
+
+Using the RDFlib API, you can also `execute SPARQL queries <https://rdflib.readthedocs.io/en/stable/intro_to_sparql.html>`_ over an HDT document.
+If you do so, we recommend that you first call the ``optimize_sparql`` function, which optimize
+the RDFlib SPARQL query engine in the context of HDT documents.
+
+.. code-block:: python
+
+   from rdflib import Graph
+   from rdflib_hdt import HDTStore, optimize_sparql
+
+   # Calling this function optimizes the RDFlib SPARQL engine for HDT documents
+   optimize_sparql()
+
+   graph = Graph(store=HDTStore("test.hdt"))
+
+   # You can execute SPARQL queries using the regular RDFlib API
+   qres = graph.query("""
+   PREFIX foaf: <http://xmlns.com/foaf/0.1/>
+   SELECT ?name ?friend WHERE {
+      ?a foaf:knows ?b.
+      ?a foaf:name ?name.
+      ?b foaf:name ?friend.
+   }""")
+
+   for row in qres:
+     print(f"{row.name} knows {row.friend}")
+
+HDT Document usage
+------------------
+
+.. code-block:: python
+
+   from rdflib_hdt import HDTDocument
+
+   # Load an HDT file. Missing indexes are generated automatically.
+   # You can provide the index file by putting them in the same directory than the HDT file.
+   document = HDTDocument("test.hdt")
+
+   # Display some metadata about the HDT document itself
+   print(f"Number of RDF triples: {document.total_triples}")
+   print(f"Number of subjects: {document.nb_subjects}")
+   print(f"Number of predicates: {document.nb_predicates}")
+   print(f"Number of objects: {document.nb_objects}")
+   print(f"Number of shared subject-object: {document.nb_shared}")
+
+   # Fetch all triples that matches { ?s foaf:name ?o }
+   # Use None to indicates variables
+   triples, cardinality = document.search_triples((None, FOAF("name"), None))
+
+   print(f"Cardinality of (?s foaf:name ?o): {cardinality}")
+   for s, p, o in triples:
+     print(triple)
+
+   # The search also support limit and offset
+   triples, cardinality = document.search_triples((None, FOAF("name"), None), limit=10, offset=100)
+   # etc ...
+
+An HDT document also provides support for evaluating joins over a set of triples patterns.
+
+.. code-block:: python
+
+  from rdflib_hdt import HDTDocument
+  from rdflib import Variable
+  from rdflib.namespace import FOAF, RDF
+  
+  document = HDTDocument("test.hdt")
+  
+  # find the names of two entities that know each other
+  tp_a = (Variable("a"), FOAF("knows"), Variable("b"))
+  tp_b = (Variable("a"), FOAF("name"), Variable("name"))
+  tp_c = (Variable("b"), FOAF("name"), Variable("friend"))
+  query = set([tp_a, tp_b, tp_c])
+  
+  iterator = document.search_join(query)
+  print(f"Estimated join cardinality: {len(iterator)}")
+  
+  # Join results are produced as ResultRow, like in the RDFlib SPARQL API
+  for row in iterator:
+     print(f"{row.name} knows {row.friend}")
+
+Handling non UTF-8 strings in python
+====================================
+
+If the HDT document has been encoded with a non UTF-8 encoding the previous code won't work correctly and will result in a ``UnicodeDecodeError``.
+More details on how to convert string to str from C++ to Python `here <https://pybind11.readthedocs.io/en/stable/advanced/cast/strings.html>`_
+
+To handle this, we doubled the API of the HDT document by adding:
+
+
+* ``search_triples_bytes(...)`` return an iterator of triples as ``(py::bytes, py::bytes, py::bytes)``
+* ``search_join_bytes(...)`` return an iterator of sets of solutions mapping as ``py::set(py::bytes, py::bytes)``
+* ``convert_tripleid_bytes(...)`` return a triple as: ``(py::bytes, py::bytes, py::bytes)``
+* ``convert_id_bytes(...)`` return a ``py::bytes``
+
+**Parameters and documentation are the same as the standard version**
+
+.. code-block:: python
+
+   from rdflib_hdt import HDTDocument
+
+   document = HDTDocument("test.hdt")
+   it = document.search_triple_bytes("", "", "")
+
+   for s, p, o in it:
+   print(s, p, o) # print b'...', b'...', b'...'
+   # now decode it, or handle any error
+   try:
+      s, p, o = s.decode('UTF-8'), p.decode('UTF-8'), o.decode('UTF-8')
+   except UnicodeDecodeError as err:
+      # try another other codecs, ignore error, etc
+      pass
+
+.. |Build Status| image:: https://github.com/RDFLib/rdflib-hdt/workflows/Python%20tests/badge.svg
+   :target: https://github.com/RDFLib/rdflib-hdt/actions?query=workflow%3A%22Python+tests%22
+.. |PyPI version| image:: https://badge.fury.io/py/rdflib-hdt.svg
+   :target: https://badge.fury.io/py/rdflib-hdt
+.. |rdflib-htd logo| image:: https://raw.githubusercontent.com/RDFLib/rdflib-hdt/master/docs/source/_static/rdflib-hdt-250.png
+   :target: https://rdflib.dev/rdflib-hdt/
```

### Comparing `rdflib_hdt-3.0/rdflib_hdt.egg-info/SOURCES.txt` & `rdflib_hdt-3.1/rdflib_hdt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 hdt-cpp-1.3.3/libcds/include/Array.h
 hdt-cpp-1.3.3/libcds/include/BitSequence.h
 hdt-cpp-1.3.3/libcds/include/BitSequenceBuilder.h
 hdt-cpp-1.3.3/libcds/include/BitSequenceBuilderDArray.h
@@ -299,14 +301,15 @@
 rdflib_hdt/iterators.py
 rdflib_hdt/mapping.py
 rdflib_hdt/sparql_op.py
 rdflib_hdt/types.py
 rdflib_hdt.egg-info/PKG-INFO
 rdflib_hdt.egg-info/SOURCES.txt
 rdflib_hdt.egg-info/dependency_links.txt
+rdflib_hdt.egg-info/requires.txt
 rdflib_hdt.egg-info/top_level.txt
 src/hdt.cpp
 src/hdt_document.cpp
 src/join_iterator.cpp
 src/join_iterator_bytes.cpp
 src/triple_iterator.cpp
 src/triple_iterator_bytes.cpp
```

### Comparing `rdflib_hdt-3.0/setup.py` & `rdflib_hdt-3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # setup.py
 # Author: Thomas MINIER - MIT License 2017-2019
 from setuptools import find_packages, setup, Extension
-from os import listdir
+from os import listdir, remove
+from shutil import unpack_archive, move, rmtree
+import urllib.request
 import pybind11
 
-__rdflib_hdt_version__ = "3.0"
+__rdflib_hdt_version__ = "3.1"
 
-with open('README.rst') as file:
-    long_description = file.read()
+def download_hdt_and_unzip():
+    print("Downloading HDT...")
+    urllib.request.urlretrieve("https://github.com/rdfhdt/hdt-cpp/archive/v1.3.3.zip", "v1.3.3.zip")
+    unpack_archive("v1.3.3.zip", "tmp")
+    move("tmp/hdt-cpp-1.3.3", "hdt-cpp-1.3.3")
+    rmtree("tmp")
 
+download_hdt_and_unzip()
 
 def list_files(path: str, extension=".cpp", exclude="S.cpp"):
     """List paths to all files that ends with a given extension"""
     return ["%s/%s" % (path, f) for f in listdir(path) if f.endswith(extension) and (not f.endswith(exclude))]
 
 
 # pyHDT source files
@@ -71,19 +78,15 @@
 hdt_extension = Extension("hdt",
                           sources=sources,
                           include_dirs=include_dirs,
                           extra_compile_args=extra_compile_args,
                           language='c++')
 
 setup(
-    name="rdflib_hdt",
     version=__rdflib_hdt_version__,
-    author="Thomas Minier",
-    author_email="tminier01@gmail.com",
-    url="https://github.com/RDFLib/rdflib-hdt",
-    description="A Store back-end for rdflib to allow for reading and querying HDT documents",
-    long_description=long_description,
-    keywords=["rdflib", "hdt", "rdf", "semantic web", "search"],
-    license="MIT",
     packages=find_packages(exclude=["tests"]),
     ext_modules=[hdt_extension]
 )
+
+print("Cleaning up...")
+rmtree("hdt-cpp-1.3.3")
+remove("v1.3.3.zip")
```

### Comparing `rdflib_hdt-3.0/src/hdt.cpp` & `rdflib_hdt-3.1/src/hdt.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/src/hdt_document.cpp` & `rdflib_hdt-3.1/src/hdt_document.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/src/join_iterator.cpp` & `rdflib_hdt-3.1/src/join_iterator.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/src/join_iterator_bytes.cpp` & `rdflib_hdt-3.1/src/join_iterator_bytes.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/src/triple_iterator.cpp` & `rdflib_hdt-3.1/src/triple_iterator.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/src/triple_iterator_bytes.cpp` & `rdflib_hdt-3.1/src/triple_iterator_bytes.cpp`

 * *Files identical despite different names*

### Comparing `rdflib_hdt-3.0/src/tripleid_iterator.cpp` & `rdflib_hdt-3.1/src/tripleid_iterator.cpp`

 * *Files identical despite different names*

