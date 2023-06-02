# Comparing `tmp/mimseq-1.3.4.tar.gz` & `tmp/mimseq-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimseq-1.3.4.tar", last modified: Wed May 17 14:21:11 2023, max compression
+gzip compressed data, was "dist/mimseq-1.3.5.tar", last modified: Fri Jun  2 14:14:11 2023, max compression
```

## Comparing `mimseq-1.3.4.tar` & `mimseq-1.3.5.tar`

### file list

```diff
@@ -1,204 +1,205 @@
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.357772 mimseq-1.3.4/
--rw-r--r--   0 drew      (1000) users      (100)    35147 2020-01-30 14:46:45.000000 mimseq-1.3.4/LICENSE.txt
--rw-r--r--   0 drew      (1000) users      (100)      264 2021-09-24 14:42:07.000000 mimseq-1.3.4/MANIFEST.in
--rw-r--r--   0 drew      (1000) users      (100)      712 2023-05-17 14:21:11.357772 mimseq-1.3.4/PKG-INFO
--rw-r--r--   0 drew      (1000) users      (100)     5091 2023-02-08 15:18:34.000000 mimseq-1.3.4/README.md
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.189758 mimseq-1.3.4/mimseq/
--rw-r--r--   0 drew      (1000) users      (100)        0 2020-03-19 10:56:10.000000 mimseq-1.3.4/mimseq/__init__.py
--rw-r--r--   0 drew      (1000) users      (100)     8451 2023-03-09 11:17:02.000000 mimseq-1.3.4/mimseq/ccaPlots.R
--rw-r--r--   0 drew      (1000) users      (100)     7683 2022-05-27 09:54:54.000000 mimseq-1.3.4/mimseq/coveragePlot.R
--rw-r--r--   0 drew      (1000) users      (100)     3793 2023-02-08 10:12:49.000000 mimseq-1.3.4/mimseq/crosstalks.py
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.193759 mimseq-1.3.4/mimseq/data/
--rw-r--r--   0 drew      (1000) users      (100)     1677 2023-05-12 08:26:45.000000 mimseq-1.3.4/mimseq/data/additionalMods.txt
--rw-r--r--   0 drew      (1000) users      (100)     2762 2020-06-01 14:20:50.000000 mimseq-1.3.4/mimseq/data/additionalMods_all.txt
--rw-r--r--   0 drew      (1000) users      (100)     1452 2020-06-02 15:55:40.000000 mimseq-1.3.4/mimseq/data/additionalMods_original.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.209760 mimseq-1.3.4/mimseq/data/araTha1-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1593 2023-03-14 10:33:16.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     1191 2023-03-14 10:34:44.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)    18749 2022-05-27 08:41:38.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt
--rw-r--r--   0 drew      (1000) users      (100)    17539 2022-03-07 09:38:20.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt
--rw-r--r--   0 drew      (1000) users      (100)    13643 2019-02-21 17:02:30.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   124283 2019-02-21 17:02:30.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     4384 2022-05-27 09:19:19.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     4120 2022-05-27 09:19:19.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   126268 2023-03-14 10:34:39.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    52698 2018-04-18 00:58:34.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out
--rw-r--r--   0 drew      (1000) users      (100)   230054 2018-04-18 00:58:34.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss
--rw-r--r--   0 drew      (1000) users      (100)    64333 2022-02-25 14:22:30.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   253880 2018-04-18 00:58:33.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss
--rw-r--r--   0 drew      (1000) users      (100)    48286 2023-03-14 10:25:34.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)   116013 2022-03-08 15:21:29.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18895 2019-02-21 16:51:34.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt
--rwxr-xr-x   0 drew      (1000) users      (100)      596 2022-05-27 09:19:14.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py
--rw-r--r--   0 drew      (1000) users      (100)     3325 2023-03-14 09:57:56.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/hg38README.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.213760 mimseq-1.3.4/mimseq/data/ce11-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1595 2023-05-12 07:56:59.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     1058 2023-05-12 07:59:05.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2387 2023-05-12 08:06:56.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   143203 2023-05-12 08:00:15.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    86974 2023-05-12 07:55:09.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-all.tmp.fa
--rw-r--r--   0 drew      (1000) users      (100)    70692 2023-05-12 08:00:57.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)    53802 2018-11-13 17:14:05.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    21452 2018-11-13 17:14:05.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.221761 mimseq-1.3.4/mimseq/data/danRer11-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      361 2020-10-13 15:34:52.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2460 2020-07-14 08:21:01.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   820216 2020-07-14 08:18:14.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)  1748099 2020-07-14 08:15:10.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa
--rw-r--r--   0 drew      (1000) users      (100)  1699762 2020-10-13 15:33:53.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)  2070516 2020-07-14 08:17:34.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)     3196 2020-10-07 14:47:35.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/filterList.txt
--rwxr-xr-x   0 drew      (1000) users      (100)      603 2020-10-13 15:34:55.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/filtertRNAs.py
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.221761 mimseq-1.3.4/mimseq/data/dm6-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    56907 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    31271 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.221761 mimseq-1.3.4/mimseq/data/dm6-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    57209 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    24907 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.221761 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     6233 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    19253 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    35045 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort
--rw-r--r--   0 drew      (1000) users      (100)     2515 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.225762 mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/
--rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)     6884 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa
--rw-r--r--   0 drew      (1000) users      (100)      211 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_tRNA_Lys.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.257764 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1588 2021-07-05 08:53:55.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     3012 2021-07-09 13:07:40.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2502 2021-07-07 13:15:36.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   108501 2021-07-05 09:02:35.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67892 2021-07-05 08:48:49.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa
--rw-r--r--   0 drew      (1000) users      (100)    63236 2021-07-05 09:01:36.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   107333 2021-07-09 13:08:29.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)   107126 2021-07-09 13:07:44.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa
--rw-r--r--   0 drew      (1000) users      (100)    44065 2021-07-05 08:34:36.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    80347 2021-07-05 08:35:51.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    16883 2021-07-05 08:35:37.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt
--rw-r--r--   0 drew      (1000) users      (100)    42271 2021-07-05 08:48:46.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.261764 mimseq-1.3.4/mimseq/data/hg19-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 14:50:02.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      540 2022-04-27 14:52:24.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2021-07-08 09:56:41.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   113031 2022-04-27 14:53:02.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    59255 2018-03-06 03:17:41.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)    46331 2019-07-29 22:32:21.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    17526 2019-07-29 22:32:21.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt
--rw-r--r--   0 drew      (1000) users      (100)    65619 2022-04-27 14:53:56.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.261764 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2435 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    46331 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    80399 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    48831 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.265765 mimseq-1.3.4/mimseq/data/hg38-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2020-10-19 12:52:59.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     3325 2022-07-20 11:41:08.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2022-04-26 11:17:07.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   117384 2021-01-22 10:06:35.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67912 2020-10-05 13:31:33.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   115259 2022-09-07 13:10:51.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)    48137 2020-10-06 09:27:32.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    82347 2020-10-05 11:41:27.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18218 2020-10-05 12:36:55.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.269765 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      931 2022-03-30 09:32:29.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   117384 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67912 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   115376 2022-03-30 09:26:15.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)    48137 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    82347 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18218 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.273765 mimseq-1.3.4/mimseq/data/mm10-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    84788 2020-01-31 16:59:36.000000 mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    47202 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.273765 mimseq-1.3.4/mimseq/data/mm10-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    84575 2020-01-31 17:01:17.000000 mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    40838 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.277766 mimseq-1.3.4/mimseq/data/mm39-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 08:57:47.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      758 2022-04-26 15:03:49.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2452 2022-04-27 08:22:42.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   218566 2022-04-27 08:59:25.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)  4027115 2022-04-26 15:02:32.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   218353 2022-10-27 11:20:21.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa
--rw-r--r--   0 drew      (1000) users      (100)    89234 2021-05-11 08:57:13.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)  1352197 2021-05-16 08:53:54.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt
--rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-09-10 10:00:52.000000 mimseq-1.3.4/mimseq/data/modomics
--rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-06-10 14:49:20.000000 mimseq-1.3.4/mimseq/data/modomics_orig
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.281766 mimseq-1.3.4/mimseq/data/rn7-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      585 2021-11-03 07:29:18.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2560 2021-11-02 09:01:00.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    43272 2021-05-10 08:04:02.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out
--rw-r--r--   0 drew      (1000) users      (100)    92538 2021-05-20 20:42:36.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    83026 2021-11-03 07:29:35.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    49636 2021-11-02 08:58:59.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.281766 mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/
--rw-r--r--   0 drew      (1000) users      (100)      429 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-Phe.fa
--rw-r--r--   0 drew      (1000) users      (100)    56689 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.349772 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      816 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed
--rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:00.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    26478 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    56686 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.349772 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:30.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    56473 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM
--rw-r--r--   0 drew      (1000) users      (100)   111081 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.353772 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/
--rw-r--r--   0 drew      (1000) users      (100)     1107 2021-09-23 14:11:39.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/README.txt
--rw-r--r--   0 drew      (1000) users      (100)      816 2021-09-24 12:57:51.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed
--rw-r--r--   0 drew      (1000) users      (100)     2821 2021-09-24 12:57:51.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2021-09-24 12:57:51.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    26478 2021-09-24 12:57:51.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    57096 2021-09-24 12:59:06.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.353772 mimseq-1.3.4/mimseq/data/sacCer3_modOligos/
--rw-r--r--   0 drew      (1000) users      (100)    26595 2020-03-26 14:57:08.000000 mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    56987 2020-03-26 14:51:11.000000 mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa
--rw-r--r--   0 drew      (1000) users      (100)      320 2020-03-27 13:55:28.000000 mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_oligoRefsOnly.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.357772 mimseq-1.3.4/mimseq/data/schiPomb-972H/
--rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:27:56.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    12387 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    33731 2020-03-11 16:25:12.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    14240 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM
--rw-r--r--   0 drew      (1000) users      (100)    67540 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.357772 mimseq-1.3.4/mimseq/data/schiPomb-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:28:18.000000 mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    33944 2020-03-11 16:24:55.000000 mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20604 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out
--rwxr-xr-x   0 drew      (1000) users      (100)    67935 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/tRNAmatureseq.cm
--rw-r--r--   0 drew      (1000) users      (100)    32195 2022-09-23 11:55:49.000000 mimseq-1.3.4/mimseq/deseq.R
--rwxr-xr-x   0 drew      (1000) users      (100)     7883 2022-06-22 09:54:11.000000 mimseq-1.3.4/mimseq/getCoverage.py
--rwxr-xr-x   0 drew      (1000) users      (100)    28571 2023-05-12 08:16:46.000000 mimseq-1.3.4/mimseq/mimseq.py
--rw-r--r--   0 drew      (1000) users      (100)    52638 2023-04-18 08:46:34.000000 mimseq-1.3.4/mimseq/mmQuant.py
--rw-r--r--   0 drew      (1000) users      (100)    38088 2023-05-17 14:15:31.000000 mimseq-1.3.4/mimseq/modPlot.R
--rw-r--r--   0 drew      (1000) users      (100)     6580 2020-03-17 16:13:32.000000 mimseq-1.3.4/mimseq/modifications
--rw-r--r--   0 drew      (1000) users      (100)    31520 2023-04-18 08:45:46.000000 mimseq-1.3.4/mimseq/splitClusters.py
--rwxr-xr-x   0 drew      (1000) users      (100)    11682 2023-04-18 08:47:35.000000 mimseq-1.3.4/mimseq/ssAlign.py
--rwxr-xr-x   0 drew      (1000) users      (100)     7272 2022-03-08 14:29:47.000000 mimseq-1.3.4/mimseq/tRNAmap.py
--rwxr-xr-x   0 drew      (1000) users      (100)    48869 2023-03-10 13:59:11.000000 mimseq-1.3.4/mimseq/tRNAtools.py
--rw-r--r--   0 drew      (1000) users      (100)       23 2023-05-17 14:17:44.000000 mimseq-1.3.4/mimseq/version.py
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.193759 mimseq-1.3.4/mimseq.egg-info/
--rw-r--r--   0 drew      (1000) users      (100)      712 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/PKG-INFO
--rw-r--r--   0 drew      (1000) users      (100)     7866 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/SOURCES.txt
--rw-r--r--   0 drew      (1000) users      (100)        1 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/dependency_links.txt
--rw-r--r--   0 drew      (1000) users      (100)       46 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/entry_points.txt
--rw-r--r--   0 drew      (1000) users      (100)        1 2023-05-17 14:17:29.000000 mimseq-1.3.4/mimseq.egg-info/not-zip-safe
--rw-r--r--   0 drew      (1000) users      (100)       80 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/requires.txt
--rw-r--r--   0 drew      (1000) users      (100)        7 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/top_level.txt
--rw-r--r--   0 drew      (1000) users      (100)      124 2023-01-17 11:01:06.000000 mimseq-1.3.4/sampleData_HEKvsK562.txt
--rw-r--r--   0 drew      (1000) users      (100)       38 2023-05-17 14:21:11.357772 mimseq-1.3.4/setup.cfg
--rwxr-xr-x   0 drew      (1000) users      (100)     1913 2023-02-08 10:12:49.000000 mimseq-1.3.4/setup.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:11.000000 mimseq-1.3.5/
+-rw-r--r--   0 drew      (1000) users      (100)    35147 2020-01-30 14:46:45.000000 mimseq-1.3.5/LICENSE.txt
+-rw-r--r--   0 drew      (1000) users      (100)      264 2021-09-24 14:42:07.000000 mimseq-1.3.5/MANIFEST.in
+-rw-r--r--   0 drew      (1000) users      (100)      740 2023-06-02 14:14:11.000000 mimseq-1.3.5/PKG-INFO
+-rw-r--r--   0 drew      (1000) users      (100)     5091 2023-02-08 15:18:34.000000 mimseq-1.3.5/README.md
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/
+-rw-r--r--   0 drew      (1000) users      (100)        0 2020-03-19 10:56:10.000000 mimseq-1.3.5/mimseq/__init__.py
+-rw-r--r--   0 drew      (1000) users      (100)     8451 2023-03-09 11:17:02.000000 mimseq-1.3.5/mimseq/ccaPlots.R
+-rw-r--r--   0 drew      (1000) users      (100)     7683 2022-05-27 09:54:54.000000 mimseq-1.3.5/mimseq/coveragePlot.R
+-rw-r--r--   0 drew      (1000) users      (100)     3793 2023-02-08 10:12:49.000000 mimseq-1.3.5/mimseq/crosstalks.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/
+-rw-r--r--   0 drew      (1000) users      (100)     1677 2023-05-12 08:26:45.000000 mimseq-1.3.5/mimseq/data/additionalMods.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2762 2020-06-01 14:20:50.000000 mimseq-1.3.5/mimseq/data/additionalMods_all.txt
+-rw-r--r--   0 drew      (1000) users      (100)     1452 2020-06-02 15:55:40.000000 mimseq-1.3.5/mimseq/data/additionalMods_original.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1593 2023-03-14 10:33:16.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     1191 2023-03-14 10:34:44.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)    18749 2022-05-27 08:41:38.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt
+-rw-r--r--   0 drew      (1000) users      (100)    17539 2022-03-07 09:38:20.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt
+-rw-r--r--   0 drew      (1000) users      (100)    13643 2019-02-21 17:02:30.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   124283 2019-02-21 17:02:30.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     4384 2022-05-27 09:19:19.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     4120 2022-05-27 09:19:19.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   126268 2023-03-14 10:34:39.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    52698 2018-04-18 00:58:34.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out
+-rw-r--r--   0 drew      (1000) users      (100)   230054 2018-04-18 00:58:34.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss
+-rw-r--r--   0 drew      (1000) users      (100)    64333 2022-02-25 14:22:30.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   253880 2018-04-18 00:58:33.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss
+-rw-r--r--   0 drew      (1000) users      (100)    48286 2023-03-14 10:25:34.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)   116013 2022-03-08 15:21:29.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18895 2019-02-21 16:51:34.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)      596 2022-05-27 09:19:14.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py
+-rw-r--r--   0 drew      (1000) users      (100)     3325 2023-03-14 09:57:56.000000 mimseq-1.3.5/mimseq/data/araTha1-eColitK/hg38README.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1595 2023-05-12 07:56:59.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      971 2023-06-02 13:40:46.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2387 2023-05-12 08:06:56.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   143203 2023-05-12 08:00:15.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    86974 2023-05-12 07:55:09.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs-all.tmp.fa
+-rw-r--r--   0 drew      (1000) users      (100)    70692 2023-05-12 08:00:57.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   142990 2023-06-02 13:00:10.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)    53802 2018-11-13 17:14:05.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    21452 2018-11-13 17:14:05.000000 mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      361 2020-10-13 15:34:52.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2460 2020-07-14 08:21:01.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   820216 2020-07-14 08:18:14.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)  1748099 2020-07-14 08:15:10.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa
+-rw-r--r--   0 drew      (1000) users      (100)  1699762 2020-10-13 15:33:53.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)  2070516 2020-07-14 08:17:34.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)     3196 2020-10-07 14:47:35.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/filterList.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)      603 2020-10-13 15:34:55.000000 mimseq-1.3.5/mimseq/data/danRer11-eColitK/filtertRNAs.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/dm6-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/dm6-eColitK/dm6-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    56907 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    31271 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/dm6-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    57209 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    24907 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/dm6-tRNAs/dm6-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     6233 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    19253 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    35045 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort
+-rw-r--r--   0 drew      (1000) users      (100)     2515 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/eschColi-tRNA_Lys/
+-rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)     6884 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa
+-rw-r--r--   0 drew      (1000) users      (100)      211 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/eschColi-tRNA_Lys/eschColi_tRNA_Lys.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1588 2021-07-05 08:53:55.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     3012 2021-07-09 13:07:40.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2502 2021-07-07 13:15:36.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   108501 2021-07-05 09:02:35.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67892 2021-07-05 08:48:49.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa
+-rw-r--r--   0 drew      (1000) users      (100)    63236 2021-07-05 09:01:36.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   107333 2021-07-09 13:08:29.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)   107126 2021-07-09 13:07:44.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa
+-rw-r--r--   0 drew      (1000) users      (100)    44065 2021-07-05 08:34:36.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    80347 2021-07-05 08:35:51.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    16883 2021-07-05 08:35:37.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt
+-rw-r--r--   0 drew      (1000) users      (100)    42271 2021-07-05 08:48:46.000000 mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 14:50:02.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      540 2022-04-27 14:52:24.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2021-07-08 09:56:41.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   113031 2022-04-27 14:53:02.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    59255 2018-03-06 03:17:41.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)    46331 2019-07-29 22:32:21.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    17526 2019-07-29 22:32:21.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt
+-rw-r--r--   0 drew      (1000) users      (100)    65619 2022-04-27 14:53:56.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2435 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    46331 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    80399 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48831 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2020-10-19 12:52:59.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     3325 2022-07-20 11:41:08.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2022-04-26 11:17:07.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   117384 2021-01-22 10:06:35.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67912 2020-10-05 13:31:33.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   115259 2022-09-07 13:10:51.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48137 2020-10-06 09:27:32.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    82347 2020-10-05 11:41:27.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18218 2020-10-05 12:36:55.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-03-30 09:22:21.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      931 2022-03-30 09:32:29.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2022-03-30 09:22:21.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   117384 2022-03-30 09:22:21.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67912 2022-03-30 09:22:21.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   115376 2022-03-30 09:26:15.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48137 2022-03-30 09:22:21.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    82347 2022-03-30 09:22:21.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18218 2022-03-30 09:22:21.000000 mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/mm10-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    84788 2020-01-31 16:59:36.000000 mimseq-1.3.5/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    47202 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/mm10-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    84575 2020-01-31 17:01:17.000000 mimseq-1.3.5/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    40838 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 08:57:47.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      758 2022-04-26 15:03:49.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2022-04-27 08:22:42.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   218566 2022-04-27 08:59:25.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)  4027115 2022-04-26 15:02:32.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   218353 2022-10-27 11:20:21.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa
+-rw-r--r--   0 drew      (1000) users      (100)    89234 2021-05-11 08:57:13.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)  1352197 2021-05-16 08:53:54.000000 mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-09-10 10:00:52.000000 mimseq-1.3.5/mimseq/data/modomics
+-rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-06-10 14:49:20.000000 mimseq-1.3.5/mimseq/data/modomics_orig
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/rn7-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      585 2021-11-03 07:29:18.000000 mimseq-1.3.5/mimseq/data/rn7-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2560 2021-11-02 09:01:00.000000 mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    43272 2021-05-10 08:04:02.000000 mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out
+-rw-r--r--   0 drew      (1000) users      (100)    92538 2021-05-20 20:42:36.000000 mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    83026 2021-11-03 07:29:35.000000 mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    49636 2021-11-02 08:58:59.000000 mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq/data/sacCer3-Phe_SynVsPur/
+-rw-r--r--   0 drew      (1000) users      (100)      429 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-Phe.fa
+-rw-r--r--   0 drew      (1000) users      (100)    56689 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:11.000000 mimseq-1.3.5/mimseq/data/sacCer3-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      816 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:00.000000 mimseq-1.3.5/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    26478 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    56686 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:11.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:30.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    56473 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM
+-rw-r--r--   0 drew      (1000) users      (100)   111081 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:11.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/
+-rw-r--r--   0 drew      (1000) users      (100)     1107 2021-09-23 14:11:39.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)      816 2021-09-24 12:57:51.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2021-09-24 12:57:51.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2021-09-24 12:57:51.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    26478 2021-09-24 12:57:51.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    57096 2021-09-24 12:59:06.000000 mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:11.000000 mimseq-1.3.5/mimseq/data/sacCer3_modOligos/
+-rw-r--r--   0 drew      (1000) users      (100)    26595 2020-03-26 14:57:08.000000 mimseq-1.3.5/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    56987 2020-03-26 14:51:11.000000 mimseq-1.3.5/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa
+-rw-r--r--   0 drew      (1000) users      (100)      320 2020-03-27 13:55:28.000000 mimseq-1.3.5/mimseq/data/sacCer3_modOligos/sacCer3_oligoRefsOnly.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:11.000000 mimseq-1.3.5/mimseq/data/schiPomb-972H/
+-rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:27:56.000000 mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    12387 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    33731 2020-03-11 16:25:12.000000 mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    14240 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM
+-rw-r--r--   0 drew      (1000) users      (100)    67540 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:11.000000 mimseq-1.3.5/mimseq/data/schiPomb-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:28:18.000000 mimseq-1.3.5/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    33944 2020-03-11 16:24:55.000000 mimseq-1.3.5/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20604 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out
+-rwxr-xr-x   0 drew      (1000) users      (100)    67935 2020-01-30 14:46:45.000000 mimseq-1.3.5/mimseq/data/tRNAmatureseq.cm
+-rw-r--r--   0 drew      (1000) users      (100)    32195 2022-09-23 11:55:49.000000 mimseq-1.3.5/mimseq/deseq.R
+-rwxr-xr-x   0 drew      (1000) users      (100)     7883 2023-06-02 14:12:47.000000 mimseq-1.3.5/mimseq/getCoverage.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    28576 2023-06-02 13:42:11.000000 mimseq-1.3.5/mimseq/mimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)    52638 2023-04-18 08:46:34.000000 mimseq-1.3.5/mimseq/mmQuant.py
+-rw-r--r--   0 drew      (1000) users      (100)    38088 2023-05-17 14:15:31.000000 mimseq-1.3.5/mimseq/modPlot.R
+-rw-r--r--   0 drew      (1000) users      (100)     6580 2020-03-17 16:13:32.000000 mimseq-1.3.5/mimseq/modifications
+-rw-r--r--   0 drew      (1000) users      (100)    31520 2023-04-18 08:45:46.000000 mimseq-1.3.5/mimseq/splitClusters.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    11682 2023-04-18 08:47:35.000000 mimseq-1.3.5/mimseq/ssAlign.py
+-rwxr-xr-x   0 drew      (1000) users      (100)     7272 2022-03-08 14:29:47.000000 mimseq-1.3.5/mimseq/tRNAmap.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    48869 2023-03-10 13:59:11.000000 mimseq-1.3.5/mimseq/tRNAtools.py
+-rw-r--r--   0 drew      (1000) users      (100)       23 2023-06-02 14:13:47.000000 mimseq-1.3.5/mimseq/version.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-06-02 14:14:10.000000 mimseq-1.3.5/mimseq.egg-info/
+-rw-r--r--   0 drew      (1000) users      (100)      740 2023-06-02 14:14:09.000000 mimseq-1.3.5/mimseq.egg-info/PKG-INFO
+-rw-r--r--   0 drew      (1000) users      (100)     7914 2023-06-02 14:14:09.000000 mimseq-1.3.5/mimseq.egg-info/SOURCES.txt
+-rw-r--r--   0 drew      (1000) users      (100)        1 2023-06-02 14:14:09.000000 mimseq-1.3.5/mimseq.egg-info/dependency_links.txt
+-rw-r--r--   0 drew      (1000) users      (100)       47 2023-06-02 14:14:09.000000 mimseq-1.3.5/mimseq.egg-info/entry_points.txt
+-rw-r--r--   0 drew      (1000) users      (100)        1 2023-06-02 14:14:09.000000 mimseq-1.3.5/mimseq.egg-info/not-zip-safe
+-rw-r--r--   0 drew      (1000) users      (100)       80 2023-06-02 14:14:09.000000 mimseq-1.3.5/mimseq.egg-info/requires.txt
+-rw-r--r--   0 drew      (1000) users      (100)        7 2023-06-02 14:14:09.000000 mimseq-1.3.5/mimseq.egg-info/top_level.txt
+-rw-r--r--   0 drew      (1000) users      (100)      124 2023-01-17 11:01:06.000000 mimseq-1.3.5/sampleData_HEKvsK562.txt
+-rw-r--r--   0 drew      (1000) users      (100)       38 2023-06-02 14:14:11.000000 mimseq-1.3.5/setup.cfg
+-rwxr-xr-x   0 drew      (1000) users      (100)     1913 2023-02-08 10:12:49.000000 mimseq-1.3.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mimseq-1.3.4/LICENSE.txt` & `mimseq-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/PKG-INFO` & `mimseq-1.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: mimseq
-Version: 1.3.4
+Version: 1.3.5
 Summary: Custom high-throughput tRNA sequencing alignment and quantification pipeline based on modification induced misincorporation cDNA synthesis.
 Home-page: https://github.com/nedialkova-lab/mim-tRNAseq
 Author: Drew Behrens
 Author-email: abehrens@biochem.mpg.de
 License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `mimseq-1.3.4/README.md` & `mimseq-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/ccaPlots.R` & `mimseq-1.3.5/mimseq/ccaPlots.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/coveragePlot.R` & `mimseq-1.3.5/mimseq/coveragePlot.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/crosstalks.py` & `mimseq-1.3.5/mimseq/crosstalks.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/additionalMods.txt` & `mimseq-1.3.5/mimseq/data/additionalMods.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/additionalMods_all.txt` & `mimseq-1.3.5/mimseq/data/additionalMods_all.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/additionalMods_original.txt` & `mimseq-1.3.5/mimseq/data/additionalMods_original.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/README.txt` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/araTha1-eColitK/hg38README.txt` & `mimseq-1.3.5/mimseq/data/araTha1-eColitK/hg38README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/ce11-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.5/mimseq/data/ce11-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/ce11-eColitK/README.txt` & `mimseq-1.3.5/mimseq/data/ce11-eColitK/README.txt`

 * *Files 25% similar despite different names*

```diff
@@ -11,12 +11,9 @@
 ###### NB ######
 Some tRNAs incorrectly named!
 
 
 ### Manually removed sequences due to strange sequence, poor score and issues with infernal alignment with mimseq
 ### See ce11-tRNAs-filtered.fa
 
-
-#### mitochondrial Tyr-GTA missing a 3'-A which leads to inaccuracies in alignment and shows as mostly CCA-less reads in CCA plots ####
-#### Gene should end on CCA and gain an additional CCA after processing
-#### manually added this A
-#### see https://www.nature.com/articles/s41467-020-18068-6#Sec24 (supplementary data 4)
+# remove tRNA-Lys-CTT-7-1 as this is definitely a weird tRNA with extra sequence in D-loop that is not an intron
+# despite high score, this is a strange tRNA (http://gtrnadb.ucsc.edu/genomes/eukaryota/Celeg11/genes/tRNA-Lys-CTT-7-1.html)
```

### Comparing `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-all.fa` & `mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-all.tmp.fa` & `mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs-all.tmp.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-detailed.out` & `mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs_name_map.txt` & `mimseq-1.3.5/mimseq/data/ce11-eColitK/ce11-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa` & `mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa` & `mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/danRer11-eColitK/filterList.txt` & `mimseq-1.3.5/mimseq/data/danRer11-eColitK/filterList.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/danRer11-eColitK/filtertRNAs.py` & `mimseq-1.3.5/mimseq/data/danRer11-eColitK/filtertRNAs.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/dm6-eColitK/dm6-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.out` & `mimseq-1.3.5/mimseq/data/dm6-tRNAs/dm6-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out` & `mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort` & `mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt` & `mimseq-1.3.5/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out` & `mimseq-1.3.5/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa` & `mimseq-1.3.5/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/README.txt` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed` & `mimseq-1.3.5/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.5/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK/README.txt` & `mimseq-1.3.5/mimseq/data/hg19-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa` & `mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out` & `mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt` & `mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/README.txt` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt` & `mimseq-1.3.5/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt` & `mimseq-1.3.5/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM` & `mimseq-1.3.5/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.5/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm39-eColitK/README.txt` & `mimseq-1.3.5/mimseq/data/mm39-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa` & `mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out` & `mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa` & `mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt` & `mimseq-1.3.5/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/modomics` & `mimseq-1.3.5/mimseq/data/modomics`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/modomics_orig` & `mimseq-1.3.5/mimseq/data/modomics_orig`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/rn7-eColitK/README.txt` & `mimseq-1.3.5/mimseq/data/rn7-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out` & `mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out` & `mimseq-1.3.5/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM` & `mimseq-1.3.5/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed` & `mimseq-1.3.5/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa` & `mimseq-1.3.5/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/README.txt` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa` & `mimseq-1.3.5/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa` & `mimseq-1.3.5/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed` & `mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM` & `mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort` & `mimseq-1.3.5/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa` & `mimseq-1.3.5/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa` & `mimseq-1.3.5/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out` & `mimseq-1.3.5/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/data/tRNAmatureseq.cm` & `mimseq-1.3.5/mimseq/data/tRNAmatureseq.cm`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/deseq.R` & `mimseq-1.3.5/mimseq/deseq.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/getCoverage.py` & `mimseq-1.3.5/mimseq/getCoverage.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/mimseq.py` & `mimseq-1.3.5/mimseq/mimseq.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
 				if args.species == 'Atha':
 					args.trnas = os.path.dirname(os.path.realpath(__file__)) + "/data/araTha1-eColitK/araTha1-tRNAs-all.fa"
 					args.trnaout = os.path.dirname(os.path.realpath(__file__)) + "/data/araTha1-eColitK/araTha1-tRNAs-detailed.out"
 					args.mito = os.path.dirname(os.path.realpath(__file__)) + "/data/araTha1-eColitK/araTha1-mitotRNAs.fa"
 					# plastid reference needed for A.thaliana
 					args.plastid = os.path.dirname(os.path.realpath(__file__)) + "/data/araTha1-eColitK/araTha1-plastidtRNAs.fa"
 				if args.species == 'Cele':
-					args.trnas = os.path.dirname(os.path.realpath(__file__)) + "/data/ce11-eColitK/ce11-tRNAs-all.fa"
+					args.trnas = os.path.dirname(os.path.realpath(__file__)) + "/data/ce11-eColitK/ce11-tRNAs-filtered.fa"
 					args.trnaout = os.path.dirname(os.path.realpath(__file__)) + "/data/ce11-eColitK/ce11-tRNAs-detailed.out"
 					args.mito = os.path.dirname(os.path.realpath(__file__)) + "/data/ce11-eColitK/ce11-mitotRNAs.fa"
 			else:
 				args.species = args.trnas.split("/")[-1].split(".")[0]
 			mimseq(args.trnas, args.trnaout, args.name, args.species, args.out, args.cluster, args.cluster_id, args.cov_diff, \
 				args.posttrans, args.control_cond, args.threads, args.max_multi, args.snp_tolerance, \
 				args.keep_temp, args.cca, args.double_cca, args.min_cov, args.mismatches, args.remap, args.remap_mismatches, \
```

### Comparing `mimseq-1.3.4/mimseq/mmQuant.py` & `mimseq-1.3.5/mimseq/mmQuant.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/modPlot.R` & `mimseq-1.3.5/mimseq/modPlot.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/modifications` & `mimseq-1.3.5/mimseq/modifications`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/splitClusters.py` & `mimseq-1.3.5/mimseq/splitClusters.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/ssAlign.py` & `mimseq-1.3.5/mimseq/ssAlign.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/tRNAmap.py` & `mimseq-1.3.5/mimseq/tRNAmap.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq/tRNAtools.py` & `mimseq-1.3.5/mimseq/tRNAtools.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.4/mimseq.egg-info/PKG-INFO` & `mimseq-1.3.5/mimseq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: mimseq
-Version: 1.3.4
+Version: 1.3.5
 Summary: Custom high-throughput tRNA sequencing alignment and quantification pipeline based on modification induced misincorporation cDNA synthesis.
 Home-page: https://github.com/nedialkova-lab/mim-tRNAseq
 Author: Drew Behrens
 Author-email: abehrens@biochem.mpg.de
 License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `mimseq-1.3.4/mimseq.egg-info/SOURCES.txt` & `mimseq-1.3.5/mimseq.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 mimseq/data/araTha1-eColitK/hg38README.txt
 mimseq/data/ce11-eColitK/FastaHeadersforMimseq.py
 mimseq/data/ce11-eColitK/README.txt
 mimseq/data/ce11-eColitK/ce11-mitotRNAs.fa
 mimseq/data/ce11-eColitK/ce11-tRNAs-all.fa
 mimseq/data/ce11-eColitK/ce11-tRNAs-all.tmp.fa
 mimseq/data/ce11-eColitK/ce11-tRNAs-detailed.out
+mimseq/data/ce11-eColitK/ce11-tRNAs-filtered.fa
 mimseq/data/ce11-eColitK/ce11-tRNAs.bed
 mimseq/data/ce11-eColitK/ce11-tRNAs_name_map.txt
 mimseq/data/danRer11-eColitK/README.txt
 mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa
 mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed
 mimseq/data/danRer11-eColitK/danRer11_eColitK.fa
 mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa
```

### Comparing `mimseq-1.3.4/setup.py` & `mimseq-1.3.5/setup.py`

 * *Files identical despite different names*

