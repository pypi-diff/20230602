# Comparing `tmp/SPAIC-0.6.1a0.tar.gz` & `tmp/SPAIC-0.6.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPAIC-0.6.1a0.tar", last modified: Fri Dec  9 08:08:56 2022, max compression
+gzip compressed data, was "SPAIC-0.6.2.0.0.tar", last modified: Fri Jun  2 01:36:33 2023, max compression
```

## Comparing `SPAIC-0.6.1a0.tar` & `SPAIC-0.6.2.0.0.tar`

### file list

```diff
@@ -1,76 +1,87 @@
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.472556 SPAIC-0.6.1a0/
--rw-rw-r--   0 crj       (1000) crj       (1000)    11357 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/LICENSE
--rw-rw-r--   0 crj       (1000) crj       (1000)    13660 2022-12-09 08:08:56.476554 SPAIC-0.6.1a0/PKG-INFO
--rw-rw-r--   0 crj       (1000) crj       (1000)    12543 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/README.md
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.424580 SPAIC-0.6.1a0/SPAIC.egg-info/
--rw-rw-r--   0 crj       (1000) crj       (1000)    13660 2022-12-09 08:08:56.000000 SPAIC-0.6.1a0/SPAIC.egg-info/PKG-INFO
--rw-rw-r--   0 crj       (1000) crj       (1000)     1606 2022-12-09 08:08:56.000000 SPAIC-0.6.1a0/SPAIC.egg-info/SOURCES.txt
--rw-rw-r--   0 crj       (1000) crj       (1000)        1 2022-12-09 08:08:56.000000 SPAIC-0.6.1a0/SPAIC.egg-info/dependency_links.txt
--rw-rw-r--   0 crj       (1000) crj       (1000)       53 2022-12-09 08:08:56.000000 SPAIC-0.6.1a0/SPAIC.egg-info/requires.txt
--rw-rw-r--   0 crj       (1000) crj       (1000)        6 2022-12-09 08:08:56.000000 SPAIC-0.6.1a0/SPAIC.egg-info/top_level.txt
--rw-rw-r--   0 crj       (1000) crj       (1000)     1154 2022-12-09 08:08:56.476554 SPAIC-0.6.1a0/setup.cfg
--rw-rw-r--   0 crj       (1000) crj       (1000)      324 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/setup.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.424580 SPAIC-0.6.1a0/spaic/
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.428578 SPAIC-0.6.1a0/spaic/Backend/
--rw-rw-r--   0 crj       (1000) crj       (1000)    60484 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Backend/Backend.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      154 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/Backend/Builder.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    24749 2022-11-16 08:30:16.000000 SPAIC-0.6.1a0/spaic/Backend/Torch_Backend.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      135 2022-11-29 07:15:36.000000 SPAIC-0.6.1a0/spaic/Backend/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.436574 SPAIC-0.6.1a0/spaic/IO/
--rw-rw-r--   0 crj       (1000) crj       (1000)     6523 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/IO/Dataloader.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    67724 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/IO/Dataset.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5921 2022-09-19 07:10:34.000000 SPAIC-0.6.1a0/spaic/IO/Environment.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     4408 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/IO/Initializer.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     7072 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/IO/Pipeline.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      387 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/IO/SignalGenerator.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      136 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/IO/__init__.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5279 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/IO/sampler.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    32180 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/IO/utils.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.440572 SPAIC-0.6.1a0/spaic/Learning/
--rw-rw-r--   0 crj       (1000) crj       (1000)     8751 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Learning/Conv_RSTDP.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     8541 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Learning/Conv_STDP.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    13736 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Learning/Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    14049 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Learning/RSTDP.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     3492 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Learning/STBP_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     4714 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Learning/STCA_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    16660 2022-12-02 02:52:41.000000 SPAIC-0.6.1a0/spaic/Learning/STDP_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    10761 2022-11-30 06:50:54.000000 SPAIC-0.6.1a0/spaic/Learning/SpikeProp_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    10619 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Learning/Tempotron_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      573 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Learning/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.444570 SPAIC-0.6.1a0/spaic/Library/
--rw-rw-r--   0 crj       (1000) crj       (1000)      349 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/Library/Library.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    19730 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Library/Network_loader.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    16330 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Library/Network_saver.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      806 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/Library/STCA_music_network.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      222 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/Library/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.448568 SPAIC-0.6.1a0/spaic/Monitor/
--rw-rw-r--   0 crj       (1000) crj       (1000)    19672 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Monitor/Monitor.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      158 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/Monitor/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.460562 SPAIC-0.6.1a0/spaic/Network/
--rw-rw-r--   0 crj       (1000) crj       (1000)    33830 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Network/Assembly.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     7205 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Network/BaseModule.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    14325 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Network/ConnectPolicy.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    49760 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Network/Connections.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     3854 2022-08-16 07:05:57.000000 SPAIC-0.6.1a0/spaic/Network/Construct.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     4879 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Network/DelayQueue.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    18713 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Network/Network.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    16155 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Network/Synapse.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    40677 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Network/Topology.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      316 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/Network/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.468558 SPAIC-0.6.1a0/spaic/Neuron/
--rw-rw-r--   0 crj       (1000) crj       (1000)     8145 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Neuron/Actions.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    21279 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Neuron/Decoders.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    15808 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Neuron/Encoders.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     8540 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Neuron/Generators.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     3751 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Neuron/Module.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    60111 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Neuron/Neuron.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    27640 2022-12-09 08:05:02.000000 SPAIC-0.6.1a0/spaic/Neuron/Node.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     6871 2022-11-10 07:01:11.000000 SPAIC-0.6.1a0/spaic/Neuron/Rewards.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      316 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/Neuron/__init__.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     1792 2022-12-09 08:08:34.000000 SPAIC-0.6.1a0/spaic/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2022-12-09 08:08:56.472556 SPAIC-0.6.1a0/spaic/utils/
--rw-rw-r--   0 crj       (1000) crj       (1000)       24 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/utils/__init__.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5077 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/utils/fftweight.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     8291 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/utils/filters.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     2844 2022-08-16 07:05:57.000000 SPAIC-0.6.1a0/spaic/utils/gtgram.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5010 2022-08-03 05:27:07.000000 SPAIC-0.6.1a0/spaic/utils/plot.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.361873 SPAIC-0.6.2.0.0/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    11357 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/LICENSE
+-rw-rw-r--   0 crj       (1000) crj       (1000)    13662 2023-06-02 01:36:33.361873 SPAIC-0.6.2.0.0/PKG-INFO
+-rw-rw-r--   0 crj       (1000) crj       (1000)    12543 2022-12-09 10:34:18.000000 SPAIC-0.6.2.0.0/README.md
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.349874 SPAIC-0.6.2.0.0/SPAIC.egg-info/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    13662 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/PKG-INFO
+-rw-rw-r--   0 crj       (1000) crj       (1000)     1901 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/SOURCES.txt
+-rw-rw-r--   0 crj       (1000) crj       (1000)        1 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/dependency_links.txt
+-rw-rw-r--   0 crj       (1000) crj       (1000)       53 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/requires.txt
+-rw-rw-r--   0 crj       (1000) crj       (1000)        6 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/top_level.txt
+-rw-rw-r--   0 crj       (1000) crj       (1000)     1154 2023-06-02 01:36:33.361873 SPAIC-0.6.2.0.0/setup.cfg
+-rw-rw-r--   0 crj       (1000) crj       (1000)      324 2022-12-09 10:34:18.000000 SPAIC-0.6.2.0.0/setup.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.349874 SPAIC-0.6.2.0.0/spaic/
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.353874 SPAIC-0.6.2.0.0/spaic/Backend/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    67350 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Backend/Backend.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      154 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Backend/Builder.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    29893 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Backend/Torch_Backend.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      135 2022-11-29 07:15:36.000000 SPAIC-0.6.2.0.0/spaic/Backend/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.353874 SPAIC-0.6.2.0.0/spaic/IO/
+-rw-rw-r--   0 crj       (1000) crj       (1000)     6527 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/IO/Dataloader.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    67724 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/IO/Dataset.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5921 2022-09-19 07:10:34.000000 SPAIC-0.6.2.0.0/spaic/IO/Environment.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     4408 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/IO/Initializer.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     7072 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/IO/Pipeline.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      391 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/IO/SignalGenerator.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      136 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/IO/__init__.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5279 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/IO/sampler.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    32180 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/IO/utils.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.353874 SPAIC-0.6.2.0.0/spaic/Learning/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    15353 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Backprop_RSTDP.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8763 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Conv_RSTDP.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8553 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Conv_STDP.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     2076 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/FiniteDifference.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    16759 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    16941 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/RSTDP.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     3269 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Rate_Modulation.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     3545 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/STBP_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     4755 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/STCA_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    16506 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/STDP_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    10761 2023-06-02 01:33:47.000000 SPAIC-0.6.2.0.0/spaic/Learning/SpikeProp_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     2520 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/SurrogateBP_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    10620 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Tempotron_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      571 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/__init__.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     7759 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/surrogate.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/Library/
+-rw-rw-r--   0 crj       (1000) crj       (1000)      357 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Library/Library.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    20447 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Library/Network_loader.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    17000 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Library/Network_saver.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      806 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Library/STCA_music_network.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      222 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Library/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/Monitor/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    20942 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Monitor/Monitor.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      158 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Monitor/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/Network/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    35207 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Assembly.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    11527 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/BaseModule.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    14325 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/Network/ConnectPolicy.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    85318 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Connections.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     3858 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Construct.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5442 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/DelayQueue.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    21572 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Network.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    24642 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Synapse.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    43003 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Topology.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      316 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Network/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/Neuron/
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8145 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Actions.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    23816 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Decoders.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    16388 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Encoders.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8635 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Generators.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     3952 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Module.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    85703 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Neuron.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    28015 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Node.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     6893 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Rewards.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      316 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Neuron/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/UI/
+-rw-rw-r--   0 crj       (1000) crj       (1000)      676 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/UI/OnlineSpikePlot.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      309 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/UI/Visualization.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      134 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/UI/__init__.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     1946 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.361873 SPAIC-0.6.2.0.0/spaic/utils/
+-rw-rw-r--   0 crj       (1000) crj       (1000)      876 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/utils/AnimateScatter.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)       24 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/utils/__init__.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5077 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/utils/fftweight.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8291 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/utils/filters.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     2844 2022-08-16 07:05:57.000000 SPAIC-0.6.2.0.0/spaic/utils/gtgram.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      631 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/utils/memory.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5010 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/utils/plot.py
```

### Comparing `SPAIC-0.6.1a0/LICENSE` & `SPAIC-0.6.2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/PKG-INFO` & `SPAIC-0.6.2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPAIC
-Version: 0.6.1a0
+Version: 0.6.2.0.0
 Summary: The spaic platform simulation training platform is a network construction, forward simulation and learning training platform developed for spiking neural networks.
 Home-page: https://github.com/ZhejianglabNCRC/SPAIC/
 Author: zjlab
 Author-email: hongchf@zhejianglab.com
 Maintainer: hongchaofei
 Maintainer-email: hongchf@zhejianglab.com
 License: Apache-2.0 license
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: SPAIC Version: 0.6.1a0 Summary: The spaic platform
-simulation training platform is a network construction, forward simulation and
-learning training platform developed for spiking neural networks. Home-page:
-https://github.com/ZhejianglabNCRC/SPAIC/ Author: zjlab Author-email:
-hongchf@zhejianglab.com Maintainer: hongchaofei Maintainer-email:
+Metadata-Version: 2.1 Name: SPAIC Version: 0.6.2.0.0 Summary: The spaic
+platform simulation training platform is a network construction, forward
+simulation and learning training platform developed for spiking neural
+networks. Home-page: https://github.com/ZhejianglabNCRC/SPAIC/ Author: zjlab
+Author-email: hongchf@zhejianglab.com Maintainer: hongchaofei Maintainer-email:
 hongchf@zhejianglab.com License: Apache-2.0 license Project-URL: Documentation,
 https://spaic.readthedocs.io/ Project-URL: Source Code, https://github.com/
 ZhejianglabNCRC/SPAIC Project-URL: Issue Tracker, https://github.com/
 ZhejianglabNCRC/SPAIC/issues Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `SPAIC-0.6.1a0/README.md` & `SPAIC-0.6.2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/SPAIC.egg-info/PKG-INFO` & `SPAIC-0.6.2.0.0/SPAIC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPAIC
-Version: 0.6.1a0
+Version: 0.6.2.0.0
 Summary: The spaic platform simulation training platform is a network construction, forward simulation and learning training platform developed for spiking neural networks.
 Home-page: https://github.com/ZhejianglabNCRC/SPAIC/
 Author: zjlab
 Author-email: hongchf@zhejianglab.com
 Maintainer: hongchaofei
 Maintainer-email: hongchf@zhejianglab.com
 License: Apache-2.0 license
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: SPAIC Version: 0.6.1a0 Summary: The spaic platform
-simulation training platform is a network construction, forward simulation and
-learning training platform developed for spiking neural networks. Home-page:
-https://github.com/ZhejianglabNCRC/SPAIC/ Author: zjlab Author-email:
-hongchf@zhejianglab.com Maintainer: hongchaofei Maintainer-email:
+Metadata-Version: 2.1 Name: SPAIC Version: 0.6.2.0.0 Summary: The spaic
+platform simulation training platform is a network construction, forward
+simulation and learning training platform developed for spiking neural
+networks. Home-page: https://github.com/ZhejianglabNCRC/SPAIC/ Author: zjlab
+Author-email: hongchf@zhejianglab.com Maintainer: hongchaofei Maintainer-email:
 hongchf@zhejianglab.com License: Apache-2.0 license Project-URL: Documentation,
 https://spaic.readthedocs.io/ Project-URL: Source Code, https://github.com/
 ZhejianglabNCRC/SPAIC Project-URL: Issue Tracker, https://github.com/
 ZhejianglabNCRC/SPAIC/issues Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `SPAIC-0.6.1a0/SPAIC.egg-info/SOURCES.txt` & `SPAIC-0.6.2.0.0/SPAIC.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,29 @@
 spaic/IO/Environment.py
 spaic/IO/Initializer.py
 spaic/IO/Pipeline.py
 spaic/IO/SignalGenerator.py
 spaic/IO/__init__.py
 spaic/IO/sampler.py
 spaic/IO/utils.py
+spaic/Learning/Backprop_RSTDP.py
 spaic/Learning/Conv_RSTDP.py
 spaic/Learning/Conv_STDP.py
+spaic/Learning/FiniteDifference.py
 spaic/Learning/Learner.py
 spaic/Learning/RSTDP.py
+spaic/Learning/Rate_Modulation.py
 spaic/Learning/STBP_Learner.py
 spaic/Learning/STCA_Learner.py
 spaic/Learning/STDP_Learner.py
 spaic/Learning/SpikeProp_Learner.py
+spaic/Learning/SurrogateBP_Learner.py
 spaic/Learning/Tempotron_Learner.py
 spaic/Learning/__init__.py
+spaic/Learning/surrogate.py
 spaic/Library/Library.py
 spaic/Library/Network_loader.py
 spaic/Library/Network_saver.py
 spaic/Library/STCA_music_network.py
 spaic/Library/__init__.py
 spaic/Monitor/Monitor.py
 spaic/Monitor/__init__.py
@@ -53,12 +58,17 @@
 spaic/Neuron/Encoders.py
 spaic/Neuron/Generators.py
 spaic/Neuron/Module.py
 spaic/Neuron/Neuron.py
 spaic/Neuron/Node.py
 spaic/Neuron/Rewards.py
 spaic/Neuron/__init__.py
+spaic/UI/OnlineSpikePlot.py
+spaic/UI/Visualization.py
+spaic/UI/__init__.py
+spaic/utils/AnimateScatter.py
 spaic/utils/__init__.py
 spaic/utils/fftweight.py
 spaic/utils/filters.py
 spaic/utils/gtgram.py
+spaic/utils/memory.py
 spaic/utils/plot.py
```

### Comparing `SPAIC-0.6.1a0/setup.cfg` & `SPAIC-0.6.2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/Backend/Backend.py` & `SPAIC-0.6.2.0.0/spaic/Backend/Backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 @project: SPAIC
 @filename: Backend
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 @description:
 定义网络仿真使用的backend，如 Pytorch, Tensorflow, CUDA, 达尔文芯片等，以及相应的微分方程求解方法比如 Euler, 2阶 Runge-Kutta等
 """
+import sys
 from abc import abstractmethod, ABC
 from collections import OrderedDict
-from ..Network.BaseModule import BaseModule, VariableAgent, Op
-from ..Network.DelayQueue import DelayQueue
+from typing import Dict
+from spaic.Network.BaseModule import BaseModule, VariableAgent, Op
+from spaic.Network.DelayQueue import DelayQueue
+from spaic.IO.Initializer import BaseInitializer
 import numpy as np
-import torch
+import networkx as nx
+import matplotlib.pyplot as plt
 
 backends = dict()
 
 
 class Backend(ABC):
     '''
     Basic backend class. All specified backend backend should subclass it.
@@ -70,39 +74,48 @@
 
     backend_name = 'None'
     def __init__(self, dt=0.1):
         super(Backend, self).__init__()
         self.device = None
         self.runtime = None
         self.builded = False
+        self.partition = None
         self.dt = dt  # the length of a backend timestep
         self.time = 0.0  # current backend time
         self.n_time_step = 0  # the num of current time step
         self._batch_size = 1
 
         self._variables = dict()  # build from orderedDict to Tuple
+        self._update_dict = dict()
+        self._reduce_dict = dict()
+        self._temp_dict = dict()
         self._parameters_dict = dict()
         self._clamp_parameter_dict = dict()
         self._delay_dict = dict()  # store conduction delays
         self._SparseVariables_dict = dict()
         self._InitVariables_dict = dict()
+        self._variable_agent_dict: Dict[VariableAgent] = dict()
+        self._temp_agent_dict: Dict[VariableAgent] = dict()
 
         self._operations = list()
         self._standalone_operations = list()
         self._initial_operations = list()
 
         self._monitors = list()  # TODO: need to add to update
         self._stored_states = dict()  # TODO: store network self._variables in the dict
+        self.full_enable_grad = False
+        self.forward_build = False #标识连接间有没有一步delay
 
         self.basic_operate['threshold'] = self.threshold
         self.basic_operate['reset'] = self.reset
         self.basic_operate['var_linear'] = self.var_linear
         self.basic_operate['mat_linear'] = self.mat_linear
         self.basic_operate['mat_mult_weight'] = self.mat_mult_weight
         self.basic_operate['mat_mult_weight_complex'] = self.mat_mult_weight_complex
+        self.basic_operate['mat_mult_weight_2complex'] = self.mat_mult_weight_2complex
         self.basic_operate['mat_mult_pre'] = self.mat_mult_pre
         self.basic_operate['mat_mult'] = self.mat_mult
         self.basic_operate['bmm'] = self.bmm
         self.basic_operate['ger'] = self.ger
         self.basic_operate['sparse_mat_mult_weight'] = self.sparse_mat_mult_weight
         self.basic_operate['var_mult'] = self.var_mult
         self.basic_operate['add'] = self.add
@@ -123,14 +136,15 @@
         self.basic_operate['sin'] = self.sin
         self.basic_operate['cos'] = self.cos
         self.basic_operate['tan'] = self.tan
         self.basic_operate['log'] = self.log
         self.basic_operate['log2'] = self.log2
         self.basic_operate['log10'] = self.log10
 
+        self.basic_operate['upsample'] = self.upsample
         self.basic_operate['conv_max_pool2d'] = self.conv_max_pool2d
         self.basic_operate['conv_avg_pool2d'] = self.conv_avg_pool2d
         self.basic_operate['conv_add_bias'] = self.conv_add_bias
         self.basic_operate['max_pool2d'] = self.max_pool2d
         self.basic_operate['post_max_pool2d_complex'] = self.post_max_pool2d_complex
         self.basic_operate['avg_pool2d'] = self.avg_pool2d
         self.basic_operate['batchnorm2d'] = self.batchnorm2d
@@ -138,14 +152,15 @@
         self.basic_operate['reshape_mat_mult'] = self.reshape_mat_mult
         self.basic_operate['exp'] = self.exp
         self.basic_operate['mult_sum_weight'] = self.mult_sum_weight
         self.basic_operate['im2col_indices'] = self.im2col_indices
         self.basic_operate['conv2d_flatten'] = self.conv2d_flatten
         self.basic_operate['feature_map_flatten'] = self.feature_map_flatten
         self.basic_operate['weight_norm'] = self.weight_norm
+        self.basic_operate['to'] = self.to
 
         self.param_init_operate['uniform'] = self.uniform
         self.param_init_operate['normal'] = self.normal
         self.param_init_operate['xavier_uniform'] = self.xavier_uniform
         self.param_init_operate['xavier_noraml'] = self.xavier_normal
         self.param_init_operate['kaiming_uniform'] = self.kaiming_uniform
         self.param_init_operate['kaiming_normal'] = self.kaiming_normal
@@ -164,14 +179,30 @@
 
     def get_batch_size(self):
         return self._batch_size
 
     def set_runtime(self, runtime):
         self.runtime = runtime
 
+    def register_basic_op(self, name, op_function):
+        """
+        register the function as basic operation to backend's _basic_operation dict
+        Args:
+            name:
+            op_function:
+
+        Returns:
+
+        """
+        name = name.lower()
+        assert callable(op_function)
+        if name in self.basic_operate:
+            raise ValueError(('A model with the name "%s" has already been registered') % name)
+
+        self.basic_operate[name] = op_function
 
 
     def build_graph(self):
         '''
         Build a computation graph before performing the calculation.
         Note that only the basic operations are redefiend into the _graph_operations list. The format of _graph_operations is as follows:
         [(dict_type, ret_var_name), operation_name, [(dict_type1, input_var_name1),(dict_type2, input_var_name2),...]].
@@ -207,227 +238,291 @@
         ##  for push_operation build  ##
         ################################
         update_dict = dict()
         reduce_dict = dict()
 
         for ind, op in enumerate(push_operations):
             outputs = []
-            label_outputs = []
+            agent_outputs = []
             # if the operation return one variable, then it is appended into a list, to accordant with multi-variable returns
             if len(op.output) == 1:
                 outputs.append(op.func())
             else:
                 outputs = op.func()
             # return variable is a list
             for ind, var_name in enumerate(op.output):
                 if var_name in self._variables:
                     # when the same ret_var_name occurs more than once, op.output is added to the reduce_dict of _graph_var_dicts
                     if var_name in update_dict:
                         reduce_dict[var_name] = [update_dict[var_name], outputs[ind]]
-                        label_outputs.append(('reduce_dict', var_name))
+                        agent_outputs.append(self._variable_agent_dict[var_name].new_labeled_agent('reduce_dict'))
                         # # add op.output into graph: reduce_dict
                         # self._graph_var_dicts['reduce_dict'][op.output] = []
                         # revise the first reduce operation
                         for gop in self._push_operations:
-                            tmp_label_outputs = gop.output
-                            for tmp_ind, tmp_label in enumerate(tmp_label_outputs):
-                                if tmp_label[1] == var_name:
-                                    tmp_label_outputs[tmp_ind] = ('reduce_dict', var_name)
+                            for var in gop.output:
+                                assert isinstance(var, VariableAgent)
+                                if var.var_name == var_name:
+                                    var.dict_label = 'reduce_dict'
                                     break
                         del update_dict[var_name]
                     elif var_name in reduce_dict:
                         reduce_dict[var_name].append(outputs[ind])
-                        label_outputs.append(('reduce_dict', var_name))
+                        agent_outputs.append(self._variable_agent_dict[var_name].new_labeled_agent('reduce_dict'))
                     else:
                         # In the push_operation, new data is directly pushed to update_dict, as
                         # there is no need to remain the last step variable value
                         update_dict[var_name] = outputs[ind]
-                        label_outputs.append(('update_dict', var_name))
+                        agent_outputs.append(self._variable_agent_dict[var_name].new_labeled_agent('update_dict'))
                 else:
                     raise ValueError("No state variable to get the input ")
 
             # add the operation to built graph
-            op.output = label_outputs
+            op.output = agent_outputs
+            for agent in agent_outputs:
+                agent.set_funcs.append(op)
             self._push_operations.append(op)
 
         # for var_name in reduce_dict:
         #     # add the reduce_sum operation into the graph
         #     self._graph_operations.append(
         #         [[('update_dict', var_name)], self.reduce_sum_update, [('reduce_dict', var_name)]])
 
         #################################
         ##  for graph_operation build  ##
         #################################
         temp_dict = dict()
-        # update_dict = dict()
-        # reduce_dict = dict()
+        self.owners = set()
         temp_reduce_sum_ops = []
-
+        self._temp_agent_dict = dict()
         for ind, op in enumerate(graph_operations):
             inputs = []
-            label_inputs = []
+            agent_inputs = []
             for var_name in op.input:
                 # try:
                 #     var_name in self._variables
                 # except:
                 #     a = 1
 
                 if '[updated]' in var_name:
                     var_name = var_name.replace("[updated]", "")
 
                     if var_name in update_dict:
                         inputs.append(update_dict[var_name])
-                        label_inputs.append(('update_dict', var_name))
+                        agent_inputs.append(self._variable_agent_dict[var_name].new_labeled_agent('update_dict'))
                     elif var_name in reduce_dict:
                         # if the reduce_dict[var_name] is frozen: do reduce_sum operation before this op, and put the value to update_dict
                         # if not use the old variables dict
 
-                        fronzen = True
+                        frozen = True
                         op_len = len(graph_operations)
                         for search_id in range(ind + 1, op_len):
                             if var_name in graph_operations[search_id].output:
-                                fronzen = False
-                        if fronzen:
+                                frozen = False
+                        if frozen: # all reduce_dict append ops have been done before this call
                             value = self.reduce_sum(self.stack(reduce_dict[var_name]))
                             inputs.append(value)
-                            label_inputs.append(('update_dict', var_name))
+                            agent_inputs.append(self._variable_agent_dict[var_name].new_labeled_agent('update_dict'))
                             temp_reduce_sum_ops.append((var_name, len(reduce_dict[var_name])))
                             # add the reduce_sum operation into the graph
                             self._graph_operations.append(
-                                Op([('update_dict', var_name)], self.reduce_sum_update, [('reduce_dict', var_name)], owner=self, requires_grad=True))
+                                Op([self._variable_agent_dict[var_name].new_labeled_agent('update_dict')],
+                                   self.reduce_sum_update,
+                                   [self._variable_agent_dict[var_name].new_labeled_agent('reduce_dict')],
+                                   func=self.reduce_sum_update, owner=self, requires_grad=True))
                         else:
                             assert var_name in self._variables
                             inputs.append(self._variables[var_name])
-                            label_inputs.append(('variables_dict', var_name))
+                            agent_inputs.append(self._variable_agent_dict[var_name].new_labeled_agent('variables_dict'))
                     elif var_name in self._variables:
                         inputs.append(self._variables[var_name])
-                        label_inputs.append(('variables_dict', var_name))
+                        agent_inputs.append(self._variable_agent_dict[var_name].new_labeled_agent('variables_dict'))
 
                     else:
                         raise ValueError(" No State Variable [%s] in the update_dict" % var_name)
                 elif var_name in self._variables:
                     inputs.append(self._variables[var_name])
-                    label_inputs.append(('variables_dict', var_name))
+                    if var_name not in self._variable_agent_dict:
+                        self._variable_agent_dict[var_name] = VariableAgent(self, var_name)
+                    agent_inputs.append(self._variable_agent_dict[var_name].new_labeled_agent('variables_dict'))
+
 
                 elif var_name in temp_dict:
                     inputs.append(temp_dict[var_name])
-                    label_inputs.append(('temp_dict', var_name))
+                    if var_name in self._temp_agent_dict:
+                        agent_inputs.append(self._temp_agent_dict[var_name])
+                    else:
+                        raise ValueError("asking a temp variable that has not been declared")
                 else:
                     raise ValueError(" No State Variable [%s] in the variable dict" % var_name)
 
             outputs = []
-            label_outputs = []
+            agent_outputs = []
             if len(op.output) == 0:
                 self.var_check(op.func, inputs)
                 op.func(*inputs)
             else:
                 self.var_check(op.func, inputs)
+                self.remove_tensor(inputs)
                 if len(op.output) == 1:
                     outputs.append(op.func(*inputs))
+
                 else:
                     outputs = op.func(*inputs)
                 for ind, var_name in enumerate(op.output):
                     if var_name in self._variables:
                         # when the same ret_var_name occurs more than once, op.output is added to the reduce_dict of _graph_var_dicts
                         if var_name in update_dict:
                             reduce_dict[var_name] = [update_dict[var_name], outputs[ind]]
-                            label_outputs.append(('reduce_dict', var_name))
+                            agent_outputs.append(self._variable_agent_dict[var_name].new_labeled_agent('reduce_dict'))
                             # # add op.output into graph: reduce_dict
-                            # self._graph_var_dicts['reduce_dict'][op.output] = []
                             # revise the first reduce operation
                             InGop = True
                             for pop in self._push_operations:
                                 tmp_label_outputs = pop.output
-                                for tmp_ind, tmp_label in enumerate(tmp_label_outputs):
-                                    if tmp_label[1] == var_name:
-                                        tmp_label_outputs[tmp_ind] = ('reduce_dict', var_name)
+                                for var in pop.output:
+                                    if var.var_name == var_name:
+                                        var.dict_label = 'reduce_dict'
                                         InGop = False
                                         break
                                 else:
                                     continue
                                 break
-
                             for gop in self._graph_operations:
-                                for tmp_ind, tmp_input in enumerate(gop.input):
-                                    tmp_label, tmp_name = tmp_input
-                                    if tmp_label =='update_dict' and tmp_name == var_name:
-                                        gop.input[tmp_ind] = ('variables_dict', var_name)
+                                # for all operations need the updated reduce_dict variable as input before reduce_sum are converted to use old variables_dict variables
+                                for tmp_input in gop.input:
+                                    if tmp_input.dict_label =='update_dict' and tmp_input.var_name == var_name:
+                                        tmp_input.dict_label = 'variables_dict'
                                 if InGop:
                                     for gop in self._graph_operations:
-                                        tmp_label_outputs = gop.output
-                                        for tmp_ind, tmp_label in enumerate(tmp_label_outputs):
-                                            if tmp_label[1] == var_name:
-                                                tmp_label_outputs[tmp_ind] = ('reduce_dict', var_name)
+                                        for output in gop.output:
+                                            if output.var_name == var_name:
+                                                output.dict_label = 'reduce_dict'
                                                 break
                             del update_dict[var_name]
                         elif var_name in reduce_dict:
                             reduce_dict[var_name].append(outputs[ind])
-                            label_outputs.append(('reduce_dict', var_name))
+                            agent_outputs.append(self._variable_agent_dict[var_name].new_labeled_agent('reduce_dict'))
                         else:
                             update_dict[var_name] = outputs[ind]
-                            label_outputs.append(('update_dict', var_name))
+                            agent_outputs.append(self._variable_agent_dict[var_name].new_labeled_agent('update_dict'))
                     else:
                         temp_dict[var_name] = outputs[ind]
-                        label_outputs.append(('temp_dict', var_name))
+                        if var_name in self._temp_agent_dict:
+                            # raise ValueError("setting value to temp variable multiple times")
+                            pass
+                            # Whether allow duplication of name
+                        else:
+                            agent_outputs.append(VariableAgent(self, var_name, dict_label='temp_dict'))
+                            self._temp_agent_dict[var_name] = agent_outputs[-1]
+
 
             # add the operation to built graph
-            op.input = label_inputs
-            op.output = label_outputs
+            op.input = agent_inputs
+            op.output = agent_outputs
+            for agent in agent_inputs:
+                agent.get_funcs.append(op)
+            for agent in agent_outputs:
+                agent.set_funcs.append(op)
             self._graph_operations.append(op)
 
         for reduce_op in temp_reduce_sum_ops:
             reduce_len = len(reduce_dict[reduce_op[0]])
             if reduce_len != reduce_op[1]:
                 raise ValueError(
                     "Can't use [updated] tag for variable: %s, as it is a reduce_dict variable which is have updating conflict" %
                     reduce_op[0])
             else:
                 del reduce_dict[reduce_op[0]]
         # for reduced variables that not used within [update]
         for var_name in reduce_dict:
             # add the reduce_sum operation into the graph
             self._graph_operations.append(
-                Op([('update_dict', var_name)], self.reduce_sum_update, [('reduce_dict', var_name)], owner=self, requires_grad=True))
+                Op([self._variable_agent_dict[var_name].new_labeled_agent('update_dict')],
+                   self.reduce_sum_update, [self._variable_agent_dict[var_name].new_labeled_agent('reduce_dict')],
+                   func=self.reduce_sum_update, owner=self, requires_grad=True))
 
         #################################
         ##  for fetch_operation build  ##
         #################################
         for ind, op in enumerate(fetch_operations):
             inputs = []
-            label_inputs = []
+            agent_inputs = []
             for var_name in op.input:
                 if '[updated]' in var_name:
                     # there is no need to have updated tag, as all variables computed in graph_operation have benn updated
                     var_name = var_name.replace("[updated]", "")
                 if var_name in self._variables:
                     inputs.append(self._variables[var_name])
-                    label_inputs.append(('variables_dict', var_name))
+                    agent_inputs.append(self._variable_agent_dict[var_name].new_labeled_agent('variables_dict'))
                 # elif var_name in temp_dict:
                 #     inputs.append(temp_dict[var_name])
                 #     label_inputs.append(('temp_dict', var_name))
                 else:
                     raise ValueError(" No State Variable [%s] in the update_dict" % var_name)
 
             self.var_check(op.func, inputs)
             op.func(*inputs)
 
+            op.input = agent_inputs
             # add the operation to built graph
-            op.input = label_inputs
             self._fetch_operations.append(op)
 
         # self._variables.update(update_dict)
         # for ii in range(len(self._graph_operations)):
         #     self._graph_operations[ii] = tuple(self._graph_operations[ii])
         self._graph_operations = tuple(self._graph_operations)
+
         self.set_func_grad()
 
+        self.groups, self.isolate = self.get_dependency()
+        self.get_place()
 
+    def get_dependency(self):
+        if self.partition:
+            g = nx.DiGraph()
+            for ind,op in enumerate(self._graph_operations):
+                op.set_identifier(ind)
+            g.add_nodes_from([op._identifier for op in self._graph_operations])
+            for ind,op in enumerate(self._graph_operations):
+                for output in op.output:
+                    for get_op in output.get_funcs:
+                        if op._identifier < get_op._identifier:
+                            g.add_edge(op._identifier, get_op._identifier)
+
+            plt.figure(figsize=(100,100))
+            nx.draw_networkx(g)
+            # plt.savefig('test.jpg')
+            
+            isolate = []
+            leaf = []
+            for i in range(len(self._graph_operations)):
+                if g.degree(i) == 0:
+                    isolate.append(i)
+                else:
+                    if g.out_degree(i) == 0:
+                        leaf.append(i)
 
+            g = g.to_undirected()
+            groups = set()
+            for i in leaf:
+                group = frozenset(nx.dfs_tree(g,i))
+                groups.add(group)
+        else:
+            groups = [self._graph_operations]
+            isolate = []
+        return groups, isolate
 
     def set_func_grad(self):
+        if self.full_enable_grad:
+            for op in self._operations:
+                op.requires_grad = True
+            for op in self._initial_operations:
+                op.requires_grad = True
+
         for op in self._operations:
             if op.requires_grad:
                 op.func = self.to_grad_func(op.func)
             else:
                 op.func = self.to_nograd_func(op.func)
 
         for op in self._initial_operations:
@@ -462,69 +557,69 @@
             # if '[updated]' in op.output[1]:
             #     op_name = op.output[1].strip('[updated]')
             #     if op_name in self._graph_var_dicts['update_dict'] and op_name in self._graph_var_dicts['variables_dict']:
             #         self._graph_var_dicts['update_dict'][op_name] = self._graph_var_dicts['temp_dict'][op.output[1]]  # 更新返回名中带[updated]的变量的值
 
         return  # tuple(self._graph_var_dicts['variables_dict'].values())
 
-    def graph_update_step(self, variables, update_dict, reduce_dict):
-        temp_dict = dict()
-        # update_dict = dict()
-        # reduce_dict = dict()
+    def get_place(self):
+        if self.partition:
+            for ind,g in enumerate(self.groups):
+                c = []
+                g = [self._graph_operations[x] for x in g]
+                for op in g:
+                    for input in op.input:
+                        if input._var_name.split(':')[-1] == '{weight}':
+                            c.append(self._variables[input._var_name].device)
+                place = max(set(c),key = c.count)
+                for op in g:
+                    op.place = place
+            g = [self._graph_operations[x] for x in self.isolate]
+            for ind,op in enumerate(g):
+                for input in op.input:
+                    if input._var_name.split(':')[-1] == '{weight}':
+                        op.place = self._variables[input._var_name].device
+                        break
+                    else:
+                        op.place = self.device[ind % self.device_count]
+        else:
+            for ind,op in enumerate(self._graph_operations):
+                for input in op.input:
+                    if input._var_name.split(':')[-1] == '{weight}':
+                        op.place = self._variables[input._var_name].device
+                        break
+                    else:
+                        op.place = self.device[ind % self.device_count]
 
+    def graph_update_step(self):
         for op in self._graph_operations:
             # for inputs
             inputs = []
             for var in op.input:
-                if var[0] == 'variables_dict':
-                    inputs.append(variables[var[1]])
-                elif var[0] == 'temp_dict':
-                    inputs.append(temp_dict[var[1]])
-                elif var[0] == 'update_dict':
-                    inputs.append(update_dict[var[1]])
-                elif var[0] == 'reduce_dict':
-                    inputs.append(reduce_dict[var[1]])
+                inputs.append(var.value)
             # compute the operation
             result = op.func(*inputs)
             if len(op.output) == 1: result = [result]
             # assign the result variables
             for ind, var in enumerate(op.output):
-                if var[0] == 'temp_dict':
-                    temp_dict[var[1]] = result[ind]
-                elif var[0] == 'update_dict':
-                    update_dict[var[1]] = result[ind]
-                elif var[0] == 'reduce_dict':
-                    if var[1] in reduce_dict:
-                        reduce_dict[var[1]].append(result[ind])
-                    else:
-                        reduce_dict[var[1]] = [result[ind]]
-
-        return update_dict
+                var.value = result[ind]
 
     def push_update_step(self):
-        reduce_dict = dict()
-        update_dict = dict()
         for op in self._push_operations:
             result = op.func()
             if len(op.output) == 1: result = [result]
             for ind, var in enumerate(op.output):
-                if var[0] == 'update_dict':
-                    update_dict[var[1]] = result[ind]
-                elif var[1] in reduce_dict:
-                    reduce_dict[var[1]].append(result[ind])
-                else:
-                    reduce_dict[var[1]] = [result[ind]]
-        return update_dict, reduce_dict
+                var.value = result[ind]
 
     def fetch_update_step(self):
         for op in self._fetch_operations:
             # for inputs
             inputs = []
             for var in op.input:
-                inputs.append(self._variables[var[1]])
+                inputs.append(var.value)
             op.func(*inputs)
 
     def initial_step(self):
         '''
         Initialize network variables.
         '''
 
@@ -537,14 +632,15 @@
                 self._InitVariables_dict[key] = self._variables[key].detach()
 
         # Initialize untrainable variables
         self._variables.clear()
 
         # Initialize system spacial variables such as backend dt
         self._variables['[dt]'] = self.dt
+        self._variables['[batch_size]'] = self._batch_size
 
         for key, value in self._InitVariables_dict.items():
             self._variables[key] = value
 
         # Initialize the trainable parameters
         for key, clamp_code in self._clamp_parameter_dict.items():
             clamp_code[0](*clamp_code[1])
@@ -622,31 +718,38 @@
         '''
         Update the return variables of standalone operations and basic operations and current backend time.
         Returns:
             tuple(self._variables.values())
         '''
 
         # push input data
-        update_dict, reduce_dict = self.push_update_step()
+        self.push_update_step()
 
         # static graph compuation
-        update_dict = self.graph_update_step(self._variables, update_dict, reduce_dict)
+        if self.device_count > 1:
+            self.graph_update_step_multigpu()
+        else:
+            self.graph_update_step()
 
         # Update time and state variables
         self.n_time_step += 1
         self.time = round(self.n_time_step * self.dt, 2)
-        self._variables.update(update_dict)
+        self._variables.update(self._update_dict)
 
         # fetch output data
         self.fetch_update_step()
 
         # Record Variables
         for monitor in self._monitors:
             monitor.update_step(self._variables)
 
+        self._reduce_dict = dict()
+        self._temp_dict = dict()
+        self._update_dict = dict()
+
         return tuple(self._variables.values())
 
     def update_time_steps(self):
         while (self.runtime > self.time - self.last_time):
             self.update_step()
 
     def r_update_step(self):
@@ -773,52 +876,66 @@
         Returns:
 
         '''
         NotImplementedError()
 
 
     def add_variable(self, module: BaseModule, name: str, shape, value=None, is_parameter=False, is_sparse=False, init=None, init_param=None,
-                     min=None, max=None, is_constant=False):
+                     min=None, max=None, is_constant=False, prefer_device=None):
         '''
         Add variables from front objects to _variables of Backend and get copies to assign to _parameters_dict and _InitVariables_dict.
         Args:
             module (spaic.BaseModule) : the parent Module object the variable is belongs to
             name (str): the name of the added variable
             shape (list, int): the shape of the variable
             value (optional): the value of the variable
             is_parameter (bool, optional): whether the variable is trainable
-            init (optinal):
+            init (optional):
         '''
         if is_parameter:
-            self._parameters_dict[name] = self.add_backend_variable(module, name, shape, value, grad=True, is_sparse=is_sparse,
-                                                                    init=init, init_param=init_param)
+            if isinstance(value, BaseInitializer):
+                self._parameters_dict[name] = self.add_backend_variable(module, name, shape, None, grad=True, is_sparse=is_sparse,
+                                                                        init=value.__class__.__name__, init_param=value.__dict__, prefer_device=prefer_device)
+            else:
+                self._parameters_dict[name] = self.add_backend_variable(module, name, shape, value, grad=True, is_sparse=is_sparse,
+                                                                        init=init, init_param=init_param, prefer_device=prefer_device)
             # store clamp operations
             if min is not None and max is not None:
                 self._clamp_parameter_dict[name] = (self.clamp_, [self._parameters_dict[name], min, max])
             elif min is not None:
                 self._clamp_parameter_dict[name] = (self.clamp_min_, [self._parameters_dict[name], min])
             elif max is not None:
                 self._clamp_parameter_dict[name] = (self.clamp_max_, [self._parameters_dict[name], max])
 
 
         # 稀疏矩阵weight非叶子节点，反传的时候更新的是weight中的value,但前向计算的时候用的是weight,所以对于稀疏矩阵要单独用个dict记录以便初始化
         elif is_sparse:
             self._SparseVariables_dict[name] = self.add_backend_variable(module, name, shape, value, grad=True,
-                                                                         is_sparse=is_sparse, init=init,init_param=init_param)
+                                                                         is_sparse=is_sparse, init=init,init_param=init_param, prefer_device=prefer_device)
         elif is_constant:
             self._InitVariables_dict[name] = value
+        elif isinstance(value, BaseInitializer):
+            self._InitVariables_dict[name] = self.add_backend_variable(module, name, shape, None, grad=False,
+                                                                       is_sparse=is_sparse, init=value.__class__.__name__,
+                                                                       init_param=value.__dict__, prefer_device=prefer_device)
         else:
             self._InitVariables_dict[name] = self.add_backend_variable(module, name, shape, value, grad=False,
                                                                        is_sparse=is_sparse, init=init,
-                                                                       init_param=init_param)
+                                                                       init_param=init_param, prefer_device=prefer_device)
 
         var_agent = VariableAgent(self, name, is_parameter)
+        self._variable_agent_dict[name] = var_agent
         return var_agent
 
-    def has_variable(self, name):
+    def has_variable(self, name: str):
+        if name.endswith('[updated]'):
+            name = name.replace("[updated]", "")
+        elif name.endswith('[stay]'):
+            name = name.replace("[stay]", "")
+
         if name in self._variables:
             return True
         elif name in self._InitVariables_dict:
             return True
         elif name in self._parameters_dict:
             return True
         elif name in self._SparseVariables_dict:
@@ -829,15 +946,15 @@
     def add_delay(self, var_name, max_delay):
         max_len = int(max_delay / self.dt)
         if var_name in self._delay_dict:
             if self._delay_dict[var_name].max_len < max_len:
                 self._delay_dict[var_name].max_len = max_len
         else:
             self._delay_dict[var_name] = DelayQueue(var_name, max_len, self)
-            self.init_op_to_backend(None, self._delay_dict[var_name].initial, [var_name, ])
+            self.register_initial(Op(None, self._delay_dict[var_name].initial, [var_name, '[batch_size]'], owner=self, requires_grad=True))
             self.register_standalone(Op(None, self._delay_dict[var_name].push, [var_name, ], owner=self, requires_grad=True))
         return self._delay_dict[var_name]
 
 
     @abstractmethod
     def add_backend_variable(self, module: BaseModule, name, shape, value=None, grad=False, is_sparse=False, init=None, init_param=None):
         '''
@@ -875,29 +992,27 @@
         elif op.output is None:
             op.output = []
         if isinstance(op.input, str):
             op.input = [op.input]
         elif op.input is None:
             op.input = []
 
-        if op.func in self.basic_operate:
-            op.func = self.basic_operate[op.func]
+        if op.func_name in self.basic_operate:
+            op.func = self.basic_operate[op.func_name]
             if not isinstance(op.owner, Backend):
                 assert isinstance(op.owner, BaseModule)
                 op.owner._ops.append(op)
             op.operation_type = "_operations"
             self._operations.append(op)
-        elif callable(op.func):
+        elif callable(op.func_name):
             self.register_standalone(op)
         else:
             raise ValueError("No operation %s in basic_operate" % op.func)
 
 
-
-
     def register_standalone(self, op):
         '''
         Add standalone operations from front objects to _standalone_operations of Backend.
         '''
         assert isinstance(op, Op)
         if isinstance(op.output, str):
             op.output = [op.output]
@@ -907,31 +1022,34 @@
             op.input = [op.input]
         elif op.input is None:
             op.input = []
         if not isinstance(op.owner, Backend):
             assert isinstance(op.owner, BaseModule)
             op.owner._ops.append(op)
 
+        assert callable(op.func_name)
+        op.func = op.func_name
         op.operation_type = "_operations"
         self._operations.append(op)
 
 
     def register_initial(self, op):
         '''
         Add initial operations from front objects to _initial_operations of Backend..
         op  = {output, func, input, owner, place, requires_grad}
         '''
         assert isinstance(op, Op)
         if isinstance(op.func, str):
-            if op.func in self.basic_operate:
-                op.func = self.basic_operate[op.func]
+            if op.func_name in self.basic_operate:
+                op.func = self.basic_operate[op.func_name]
             else:
                 raise ValueError("No operation %s in basic_operate" % op.func)
         else:
-            assert callable(op.func)
+            assert callable(op.func_name)
+            op.func = op.func_name
         if isinstance(op.input, str):
             op.input  = [op.input]
         elif op.input is None:
             op.input = []
         if isinstance(op.output, str):
             op.output = [op.output]
         elif op.output is None:
@@ -1142,15 +1260,15 @@
         ----------
         x
         kernel
         Returns
         -------
         '''
     @abstractmethod
-    def conv_2d_complex(self, x, kernel, stride, padding, dilation, groups, beta):
+    def conv_2d_complex(self, x, kernel, stride, padding, dilation, groups, beta, delay=None):
         '''
 
         Args:
             x:
             kernel:
             stride:
             padding:
@@ -1159,16 +1277,28 @@
             beta:
 
         Returns:
 
         '''
 
     @abstractmethod
+    def conv_trans2d(self, x, kernel, stride, padding, dilation, groups):
+        '''
+            transposed conv 2d
+            Parameters
+            ----------
+            x
+            kernel
+            Returns
+            -------
+            '''
+    @abstractmethod
     def conv_trans1d(self, x, kernel):
         '''
+        transposed conv 1d
         Parameters
         ----------
         x
         kernel
         Returns
         -------
         '''
@@ -1268,15 +1398,18 @@
             X (Tensor): the second input to be multiplied
         Returns:
             mat_mult_weight(A,X)
         '''
         NotImplementedError()
 
     @abstractmethod
-    def mat_mult_weight_complex(self, A, X, beta):
+    def mat_mult_weight_complex(self, A, X, beta, delay=None):
+        NotImplementedError()
+    @abstractmethod
+    def mat_mult_weight_2complex(self, A, X, beta):
         NotImplementedError()
 
     @abstractmethod
     def mat_mult_pre(self, A, X):
         '''
         Matrix product.
         Args:
@@ -1295,14 +1428,17 @@
             x:
 
         Returns:
 
         '''
 
     @abstractmethod
+    def upsample(self,x, scale):
+        NotImplementedError()
+    @abstractmethod
     def mat_mult(self, A, X):
         '''
         Matrix product.
         Args:
             A (Tensor): the first input to be multiplied
             X (Tensor): the second input to be multiplied
         Returns:
@@ -1519,14 +1655,25 @@
         '''
         Args:
             data(tensor): an n-dimensional torch.Tensor
             constant_value(float): the value to fill the tensor with
         Returns:
             torch.nn.init.constant_(data, constant_value)
         '''
+        NotImplementedError()
+
+    @abstractmethod
+    def to(self, data, device):
+        '''
+        Args:
+            data(tensor): an n-dimensional torch.Tensor
+            constant_value(float): the value to fill the tensor with
+        Returns:
+            torch.nn.init.constant_(data, constant_value)
+        '''
         NotImplementedError()
 
     @abstractmethod
     def weight_norm(self, weight, amp):
         '''
 
         w = g/||v|| * v
```

### Comparing `SPAIC-0.6.1a0/spaic/Backend/Torch_Backend.py` & `SPAIC-0.6.2.0.0/spaic/Backend/Torch_Backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 import torch
 import numpy as np
 # from torch import fx
 #from torch.nn import Module, Parameter
 import torch.nn.functional as fn
 import torch.nn as nn
 from typing import Tuple, Dict, Callable
+from collections import defaultdict
+from torch.cuda.amp import autocast
+import torch.distributed
+import threading
 
 class Torch_Engine(torch.nn.Module):
     def __init__(self, graph_operations):
         super(Torch_Engine, self).__init__()
         self._graph_operations = graph_operations
 
     def forward(self, variables: Dict[str,torch.Tensor]):
@@ -58,16 +62,17 @@
 
 
 class Torch_Backend(Backend):
     backend_name = 'pytorch'
 
     def __init__(self, device='cpu'):
         super(Torch_Backend, self).__init__()
-
-        self.device = device[0] if isinstance(device,list) else device
+        self.device = device if isinstance(device,list) else [device]
+        self.device0 = self.device[0]
+        self.device_count = len(self.device)
         self.data_type = torch.float32
         self.debug_data = []
         self.nograd_decorator = torch.no_grad()
         self.enablegrad_decorator = torch.enable_grad()
         pass
 
     def build(self):
@@ -86,122 +91,185 @@
         self.graph_update_step = self.engine
         # print(self.engine.code)
 
     def build_graph(self):
 
         for key, value in self._InitVariables_dict.items():
             if isinstance(value, torch.Tensor):
-                value = value.to(self.device)
+                value = value.to(self.device0)
                 self._InitVariables_dict[key] = value
 
         super(Torch_Backend, self).build_graph()
 
+    def remove_tensor(self, inputs):
+        if not torch.is_tensor(inputs[0]):
+            device = inputs[1].device
+        else:
+            device = inputs[0].device
+        for ind,t in enumerate(inputs):
+            if torch.is_tensor(t):
+                inputs[ind] = t.to(device)
+
+    def is_insert(self,inputs):
+        if len(inputs) == 0:
+            return False
+        elif len(set(inputs)) < len(inputs):
+            return True
+
+    def move_compute_and_assign_tensors(self,op):
+        inputs = []
+        for var in op.input:
+            if torch.is_tensor(var.value):
+                var.value = var.value.to(op.place)
+                inputs.append(var.value)
+            elif isinstance(var.value, list):
+                for ind,x in enumerate(var.value):
+                    if torch.is_tensor(x):
+                        var.value[ind] = x.to(op.place)
+                inputs.append(var.value)
+            else:
+                inputs.append(var.value)
+        result = op.func(*inputs)
+        if len(op.output) == 1: result = [result]
+        for ind, var in enumerate(op.output):
+            var.value = result[ind]
+
+    def graph_update_step_multigpu(self):
+        def _worker(*tuple):
+            grad_enabled, autocast_enabled = torch.is_grad_enabled(), torch.is_autocast_enabled()
+            for group in sorted(tuple):
+                op = self._graph_operations[group]
+                # with torch.cuda.device(self.device[index]), autocast(enabled=autocast_enabled):
+                self.move_compute_and_assign_tensors(op)
+
+        if self.partition:
+            if self.partition == 'multithread':
+                threads = [threading.Thread(target=_worker,args=group) for group in self.groups]
+                for thread in threads:
+                    thread.start()
+                for thread in threads:
+                    thread.join()
+            if self.partition == 'thread1':
+                for group in self.groups:
+                    for i in sorted(group):
+                        op = self._graph_operations[i]
+                        self.move_compute_and_assign_tensors(op)
+            for op in self.isolate:
+                op = self._graph_operations[op]
+                self.move_compute_and_assign_tensors(op)
+        else:
+            for group in self.groups:
+                for op in group:
+                    self.move_compute_and_assign_tensors(op)
+
     def to_nograd_func(self, func):
         return self.nograd_decorator(func)
 
     def to_grad_func(self, func):
         return self.enablegrad_decorator(func)
 
-
-    # def graph_update_step(self):
-    #
-    #     for op in self._graph_operations:
-    #         inputs = []
-    #         for var in op.input:
-    #             inputs.append(self._graph_var_dicts[var[0]][var[1]])
-    #
-    #         if op.output[0] is 'reduce_dict':
-    #             self._graph_var_dicts['reduce_dict'][op.output[1]].append(op.func(*inputs))
-    #         else:
-    #             self._graph_var_dicts[op.output[0]][op.output[1]] = op.func(*inputs)
-    #
-    #     return tuple(self._graph_var_dicts['variables_dict'].values())
-
     #  As of now, autograd support floating point Tensor types ( half, float, double and bfloat16) and complex Tensor types (cfloat, cdouble).
-    def add_backend_variable(self, module, name, shape, value=None, grad=False, is_sparse=False, init=None, init_param=None):
+    def add_backend_variable(self, module, name, shape, value=None, grad=False, is_sparse=False, init=None, init_param=None, prefer_device=None):
         '''
         Parameters
         ----------
         name
         shape
         value
         init
         Returns
         -------
         '''
+        l = len(self._parameters_dict)
+        if prefer_device != None:
+            device0 = self.device[prefer_device]
+        else:
+            device0 = self.device[l % self.device_count]
 
         if init_param is None:
             init_param = dict()
-        if value is not None:
+        if init is not None:
+            # self._variables[name] = self.init_param(grad, init)
+            data = torch.empty(shape, dtype=self.data_type, device=device0, requires_grad=grad)
+            init = init.lower()
+            if init in self.param_init_operate.keys():
+                self._variables[name] = self.param_init_operate[init](data, **init_param)
+            else:
+                raise ValueError("No initialize method: %s in param_init_operate" % init)
+        elif value is not None:
+        # if value is not None:
             if hasattr(value, "__len__"):
-                if tuple(value.shape) == (1,) and isinstance(value, torch.Tensor):
-                    self._variables[name] = value.to(self.device) * torch.ones(shape, dtype=self.data_type, device=self.device,
-                                                               requires_grad=grad)
+                if (value.shape == torch.Size([1,]) or value.shape == torch.Size([])) and isinstance(value, torch.Tensor):
+                    self._variables[name] = (value.to(self.device0) * torch.ones(shape, dtype=self.data_type, device=self.device0)).clone()
+                    self._variables[name].requires_grad = grad
                 elif tuple(value.shape) != tuple(shape):
                     raise ValueError("Value is not scalar and the shape of Value is not equal to shape")
                 # add a sparse matrices with all dimensions greater than 2
                 elif is_sparse:
                     i = np.nonzero(value)
                     v = value[i]
 
                     # Index for sparse matrix
                     sparse_index = name + '_sparse_index'
-                    self._variables[sparse_index] = torch.LongTensor(i).to(device=self.device)
+                    self._variables[sparse_index] = torch.LongTensor(i).to(device=self.device0)
                     self._InitVariables_dict[sparse_index] = self._variables[sparse_index]
 
                     # Value for sparse matrix
                     sparse_value = name + '_sparse_value'
                     if init is not None:
                         # self._variables[sparse_value] = self.init_param(True, init)
-                        data = torch.empty(shape, dtype=self.data_type, device=self.device, requires_grad=True)
+                        data = torch.empty(shape, dtype=self.data_type, device=self.device0, requires_grad=True)
                         self._variables[sparse_value] = self.param_init_operate[init](data, **init_param)
                     else:
-                        self._variables[sparse_value] = torch.tensor(v, dtype=self.data_type, requires_grad=True, device=self.device)
+                        self._variables[sparse_value] = torch.tensor(v, dtype=self.data_type, requires_grad=True, device=self.device0)
                     self._parameters_dict[sparse_value] = self._variables[sparse_value]
 
                     # The shape of sparse matrix
                     sparse_shape = name + '_sparse_shape'
                     self._variables[sparse_shape] = torch.Size(shape)
                     self._InitVariables_dict[sparse_shape] = self._variables[sparse_shape]
 
                     # Sparse matrix
                     self._variables[name] = torch.sparse.FloatTensor(self._variables[sparse_index], self._variables[sparse_value], self._variables[sparse_shape])
                 else:
                     # add a non sparse matrices with all dimensions greater than 2
                     if init is not None:
-                        data = torch.empty(shape, dtype=self.data_type, device=self.device, requires_grad=grad)
+                        data = torch.empty(shape, dtype=self.data_type, device=self.device0, requires_grad=grad)
                         init = init.lower()
                         if init in self.param_init_operate.keys():
                             self._variables[name] = self.param_init_operate[init](data, **init_param)
                         else:
                             raise ValueError("No initialize method: %s in param_init_operate" % init)
                     else:
                         if isinstance(value, torch.Tensor):
-                            self._variables[name] = value.clone().detach().to(self.device)
+                            # device0 = random.choice(self.device)
+                            self._variables[name] = value.clone().detach().to(device0)
                         else:
-                            self._variables[name] = torch.tensor(value, dtype=self.data_type, device=self.device,
+                            self._variables[name] = torch.tensor(value, dtype=self.data_type, device=device0,
                                                                    requires_grad=grad)
 
             elif len(shape) == 0:
                 # add constant
-                self._variables[name] = torch.tensor(value, dtype=self.data_type, device=self.device, requires_grad=grad)
+                self._variables[name] = torch.tensor(value, dtype=self.data_type, device=self.device0, requires_grad=grad)
 
             else:
                 # add a matrix through constant
                 if init is not None:
                     # self._variables[name] = self.init_param(grad, init)
-                    data = value*torch.ones(shape, dtype=self.data_type, device=self.device, requires_grad=grad)
+                    data = value*torch.ones(shape, dtype=self.data_type, device=device0, requires_grad=grad)
                     init = init.lower()
                     if init in self.param_init_operate.keys():
                         self._variables[name] = self.param_init_operate[init](data, **init_param)
                     else:
                         raise ValueError("No initialize method: %s in param_init_operate" % init)
                 else:
-                    self._variables[name] = value*torch.ones(shape, dtype=self.data_type, device=self.device, requires_grad=grad)
-
+                    # add a matrix through constant
+                    self._variables[name] = (
+                                value * torch.ones(shape, dtype=self.data_type, device=self.device0)).clone()
+                    self._variables[name].requires_grad = grad
         return self._variables[name]
 
     def set_variable_value(self, name, value, is_parameter):
         if is_parameter:
             assert name in self._parameters_dict
             assert self._parameters_dict[name].shape == value.shape
             if not isinstance(value, torch.Tensor):
@@ -277,40 +345,49 @@
 
     def scatter(self, x, indices):
         return torch.scatter(x, dim=0, index=indices)
 
     def conv1d(self, x, kernel):
         return torch.conv1d(x, kernel)
 
-    def conv_trans1d(self, x, kernel):
-        return torch.conv_transpose1d(x, kernel)
+    def conv_trans1d(self, x, kernel, bias=None):
+        return torch.conv_transpose1d(x, kernel, bias)
 
-    def conv_2d(self, x, kernel, stride, padding, dilation, groups):
+
+    def conv_2d(self, x, kernel, stride, padding, dilation, groups, padding_mode='constant'):
         if x.dim() == kernel.dim() + 1:
             xshape = list(x.shape)
             xshape[0] = xshape[0]*xshape[1]
             extend_size = xshape[1]
             xshape.pop(1)
-            out = fn.conv2d(x.reshape(xshape), kernel, stride=stride, padding=padding, dilation=dilation, groups=groups)
+            out = fn.conv2d(x.reshape(xshape), kernel, stride=stride, padding=padding, dilation=dilation, groups=groups, padding_mode=padding_mode)
             outshape = list(out.shape)
             outshape[0] = outshape[0]//extend_size
             outshape.insert(1, extend_size)
             return out.view(outshape)
         else:
             return fn.conv2d(x, kernel, stride=stride, padding=padding, dilation=dilation, groups=groups)
 
-    def conv_2d_complex(self, x, kernel, stride, padding, dilation, groups, beta):
+    def conv_2d_complex(self, x, kernel, stride, padding, dilation, groups, beta, delay=None):
         if x.dtype.is_complex:
-            x = beta ** x.imag * (x.real * (0 + 1.0j))
+            if delay is not None:
+                d_delay = delay/self.dt
+                d_delay = torch.ceil(d_delay) - d_delay
+                x = beta ** (x.imag+d_delay) * (x.real * (0 + 1.0j))
+            else:
+                x = beta ** x.imag * (x.real * (0 + 1.0j))
         else:
             x = x*(0+1.0j)
         real = fn.conv2d(x.real, kernel, stride=stride, padding=padding, dilation=dilation, groups=groups)
         imag = fn.conv2d(x.imag, kernel, stride=stride, padding=padding, dilation=dilation, groups=groups)
         return torch.complex(real, imag)
 
+    def conv_trans2d(self, x, kernel, stride=1, padding=0, dilation=0, groups=1):
+        return torch.conv_transpose2d(x, kernel,stride=stride, padding=padding, dilation=dilation, groups=groups)
+
 
 
     def conv_max_pool2d(self, x, kernel, pool_kernel, stride, pool_stride, padding, pool_padding, dilation, groups):
         return fn.max_pool2d(fn.conv2d(x, kernel, stride=stride, padding=padding,
                              dilation=dilation, groups=groups), kernel_size=pool_kernel,
                              stride=pool_stride, padding=pool_padding)
 
@@ -396,37 +473,72 @@
         Returns
         -------
         '''
 
         X = X.permute(1, 0)
         return torch.matmul(A, X)
 
-    def mat_mult_weight_complex(self, A, X, beta):
+
+    def mat_mult_weight_complex(self, A, X, beta, delay=None):
         '''
         Parameters
         ----------
         A--->preGroup:input
         X--->postGroup:weight
         beta---> postGroup:beta_complex
         Returns
         -------
         '''
         if A.dtype.is_complex:
-            A = A.unsqueeze(-2)
             beta = beta.unsqueeze(-1)
-            real = A.real
-            imag = A.imag
-            O = beta ** imag * (real * (0 + 1.0j))
+            if delay is not None:
+                A = A.permute(0,2,1)
+                real = A.real
+                imag = A.imag
+                d_delay = delay.unsqueeze(0)/self.dt
+                d_delay = torch.ceil(d_delay) - d_delay
+                O = beta ** (imag+d_delay) * (real * (0 + 1.0j))
+            else:
+                A = A.unsqueeze(-2)
+                real = A.real
+                imag = A.imag
+                O = beta ** imag * (real * (0 + 1.0j))
+            # if torch.any(torch.isnan(O)):
+            #     print("real:", real)
+            #     print("real:", real)
+            #     print("imag:", imag)
+            #     print("O:", O)
+            #     raise ValueError(" nan mat_mult_complex error")
             return torch.sum(O * X, dim=-1)
+        elif delay is not None:
+            A = A.permute(0, 2, 1)
+            return torch.sum(A * X, dim=-1)*(0.0+1.0j)
         else:
             X = X.permute(1, 0)
             Out = torch.matmul(A.to(X.dtype), X)
             Out = Out*(0.0+1.0j)
+            # if torch.any(torch.isnan(Out)):
+            #     print("input:", A)
+            #     print("weight:", X)
+            #     print("Out:", Out)
+            #     raise ValueError(" nan mat_mult_complex error")
             return Out
 
+    def mat_mult_weight_2complex(self, A, X, beta, delay=None):
+        if A.dtype.is_complex:
+            A = A.unsqueeze(-2).unsqueeze(-1)
+            beta = beta.unsqueeze(-1)
+            real = A.real
+            imag = A.imag
+            O = torch.sum((beta ** imag * (real * (0 + 1.0j))) * X, dim=-2)
+            return O
+        else:
+            A = A.unsqueeze(-2).unsqueeze(-1)
+            O = torch.sum(A*X, dim=-2)
+            return O
 
     def mat_mult_pre(self, A, X):
         '''
         Parameters
         ----------
         A--->preGroup:input
         X--->postGroup:weight
@@ -484,15 +596,15 @@
         return result
 
     def var_mult(self, A, X):
         return A * X
 
     def mult_sum_weight(self, A, X):
         # X = X.permute(1, 0)
-        A = A.permute(0, 2, 1)
+        # A = A.permute(0, 2, 1)
         return torch.sum(A * X, dim=-1)
 
     def mat_linear(self, A, X, b):
         return torch.matmul(A, X) + b
 
     def var_linear(self, A, X, b):
 
@@ -505,14 +617,16 @@
         return data.detach().cpu().numpy()
 
     def to_tensor(self, data):
         if isinstance(data, torch.Tensor):
             return data.to(torch.float).to(self.device)
         else:
             return torch.tensor(data, dtype=torch.float, device=self.device)
+    def upsample(self,x, scale):
+        return torch.nn.functional.interpolate(x, scale_factor=scale, mode='nearest')
 
     def exp(self, x):
         return torch.exp(x)
 
 
     def clamp_(self, data, min, max):
         with torch.no_grad():
@@ -625,14 +739,17 @@
         return torch.nn.init.sparse_(data, sparsity, std)
 
     def weight_norm(self, weight, amp):
         w_norm = torch.norm(weight, p=2, dim=1, keepdim=True)
         # print(amp.item(), w_norm.item())
         return weight*amp/w_norm
 
+    #TODO: THis "TO" should be named to_device
+    def to(self, x, device):
+        return x.to(device)
 
     def sin(self, x):
         return torch.sin(x)
 
     def cos(self, x):
         return torch.cos(x)
```

### Comparing `SPAIC-0.6.1a0/spaic/IO/Dataloader.py` & `SPAIC-0.6.2.0.0/spaic/IO/Dataloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @project: SPAIC
 @filename: Dataloader
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 @description:
 定义数据导入模块
 """
-from ..IO.sampler import *
+from spaic.IO.sampler import *
 import numpy as np
 
 # Dataloader class is written by referring to https://github.com/pytorch/pytorch/blob/master/torch/utils/data/dataloader.py.
 class _BaseDatasetFetcher(object):
     def __init__(self, dataset, auto_collation, collate_fn, drop_last):
         self.dataset = dataset
         self.auto_collation = auto_collation
```

### Comparing `SPAIC-0.6.1a0/spaic/IO/Dataset.py` & `SPAIC-0.6.2.0.0/spaic/IO/Dataset.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/IO/Environment.py` & `SPAIC-0.6.2.0.0/spaic/IO/Environment.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/IO/Initializer.py` & `SPAIC-0.6.2.0.0/spaic/IO/Initializer.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/IO/Pipeline.py` & `SPAIC-0.6.2.0.0/spaic/IO/Pipeline.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/IO/sampler.py` & `SPAIC-0.6.2.0.0/spaic/IO/sampler.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/IO/utils.py` & `SPAIC-0.6.2.0.0/spaic/IO/utils.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/Learning/Conv_RSTDP.py` & `SPAIC-0.6.2.0.0/spaic/Learning/Conv_RSTDP.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 @contact: mwyuan94@gmail.com
 @project: PyCharm
 @filename: Conv_RSTDP.py
 @time:2021/12/30 13:49
 @description:
 """
 from .Learner import Learner
-from ..Network.BaseModule import Op
-from ..Network.Connections import conv_connect
-from ..IO.utils import im2col
+from spaic.Network.BaseModule import Op
+from spaic.Network.Connections import conv_connect
+from spaic.IO.utils import im2col
 import numpy as np
 import torch
 
 class Conv2d_RSTDP(Learner):
     """
     Reward-modulated STDP. Adapted from `(Florian 2007)
     <https://florian.io/papers/2007_Florian_Modulated_STDP.pdf>`.
```

### Comparing `SPAIC-0.6.1a0/spaic/Learning/Conv_STDP.py` & `SPAIC-0.6.2.0.0/spaic/Learning/Conv_STDP.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 @contact: mwyuan94@gmail.com
 @project: PyCharm
 @filename: Conv_STDP.py
 @time:2022/1/6 13:51
 @description:
 """
 from .Learner import Learner
-from ..Network.Connections import conv_connect
-from ..IO.utils import im2col
-from ..Network.BaseModule import Op
+from spaic.Network.Connections import conv_connect
+from spaic.IO.utils import im2col
+from spaic.Network.BaseModule import Op
 import numpy as np
 import torch
 
 class Conv2d_STDP(Learner):
     """
     Conv STDP
     Args:
```

### Comparing `SPAIC-0.6.1a0/spaic/Learning/Learner.py` & `SPAIC-0.6.2.0.0/spaic/Learning/Learner.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 @filename: Learner
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 
 @description:
 定义学习模块，包括各种学习算法对仿真计算过程中插入的各种计算模块，以及记录需要学习连接的接口
 """
-# from ..Network.Connection import Connection
-# from ..Neuron.Neuron import NeuronGroup
-from ..Network.Assembly import BaseModule
+# from spaic.Network.Connection import Connection
+# from spaic.Neuron.Neuron import NeuronGroup
+from spaic.Network.Assembly import BaseModule
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 import torch
+import spaic
 import torch.nn.functional as F
 import numpy as np
 
 class Learner(BaseModule, ABC):
 
     '''
         Base learner model for all the learner model.
@@ -37,15 +38,15 @@
 
         Methods:
             add_trainable(self, trainable) : Add target object (Network, Assembly, Connection,
                             or list of them) to the trainable container
             build(self, backend) : Build Learner, choose the backend as user wish, if we have already finished the api.
 
     '''
-
+    _class_label = '<learner>'
     learning_algorithms = dict()
     learning_optims = dict()
     optim_dict = {'Adam': torch.optim.Adam, 'AdamW': torch.optim.AdamW,
                   'SparseAdam': torch.optim.SparseAdam, 'Adamax': torch.optim.Adamax,
                   'ASGD': torch.optim.ASGD, 'LBFGS': torch.optim.LBFGS,
                   'RMSprop': torch.optim.RMSprop, 'Rpop': torch.optim.Rprop,
                   'SGD': torch.optim.SGD, 'Adadelta': torch.optim.Adadelta,
@@ -56,36 +57,41 @@
                         'MultiStepLR': torch.optim.lr_scheduler.MultiStepLR,
                         'ExponentialLR': torch.optim.lr_scheduler.ExponentialLR,
                         'CosineAnnealingLR': torch.optim.lr_scheduler.CosineAnnealingLR,
                         'ReduceLROnPlateau': torch.optim.lr_scheduler.ReduceLROnPlateau,
                         'CyclicLR': torch.optim.lr_scheduler.CyclicLR,
                         'CosineAnnealingWarmRestarts': torch.optim.lr_scheduler.CosineAnnealingWarmRestarts}
 
-    def __init__(self, trainable=None, pathway=None, algorithm=('STCA', 'STBP', 'RSTDP', '...'), **kwargs):
+    def __init__(self, trainable=None, pathway=None, algorithm=('STCA', 'STBP', 'RSTDP', '...'), name=None, **kwargs):
 
         super(Learner, self).__init__()
 
         self.parameters = kwargs
         self.super_parameters = OrderedDict()
         self.backend_functions = OrderedDict()
 
-        self.name = None
+        self.name = self.set_name(name)
         self.optim_name = None
         self.optim = None
         self.lr_schedule_name = None
         self.gradient_based = True
         self.prefered_backend = ['pytorch']
         self.trainable_groups = OrderedDict()
         self.trainable_connections = OrderedDict()
         self.trainable_nodes = OrderedDict()
         self.trainable_modules = OrderedDict()
         self.trainable_others = OrderedDict()
         self.init_trainable = trainable
         self.training_param_name = []
         self.param_run_update = kwargs.get("param_run_update", False)
+        self._variables = dict()
+        self._constant_variables = dict()
+        self._tau_constant_variables = dict()
+        self._tau_membrane_variables = dict()
+
 
         self.pathway_groups = OrderedDict()
         self.pathway_connections = OrderedDict()
         self.pathway_nodes = OrderedDict()
         self.pathway_modules = OrderedDict()
         self.pathway_others = OrderedDict()
         self.init_pathway = pathway
@@ -95,19 +101,19 @@
 
     def add_trainable(self, trainable: list):
         '''
             Add target object (Assembly, Connection, or list of them) to the trainable container
             Args:
                 trainable(list) : The trainable target waiting for added.
         '''
-        from ..Network.Assembly import Assembly
-        from ..Network.Connections import Connection
-        from ..Neuron.Neuron import NeuronGroup
-        from ..Neuron.Module import Module
-        from ..Neuron.Node import Node
+        from spaic.Network.Assembly import Assembly
+        from spaic.Network.Connections import Connection
+        from spaic.Neuron.Neuron import NeuronGroup
+        from spaic.Neuron.Module import Module
+        from spaic.Neuron.Node import Node
 
         if not isinstance(trainable, list):
             trainable = [trainable]
 
         for target in trainable:
             if isinstance(target, NeuronGroup):
                 self.trainable_groups[target.id] = target
@@ -128,19 +134,19 @@
 
     def add_pathway(self, pathway: list):
         '''
             Add target object (Assembly, Connection, or list of them) to the pathway container
             Args:
                 pathway(list) : The pathway target waiting for added.
         '''
-        from ..Network.Assembly import Assembly
-        from ..Network.Connections import Connection
-        from ..Neuron.Neuron import NeuronGroup
-        from ..Neuron.Module import Module
-        from ..Neuron.Node import Node
+        from spaic.Network.Assembly import Assembly
+        from spaic.Network.Connections import Connection
+        from spaic.Neuron.Neuron import NeuronGroup
+        from spaic.Neuron.Module import Module
+        from spaic.Neuron.Node import Node
 
         if not isinstance(pathway, list):
             pathway = [pathway]
 
         for target in pathway:
             if isinstance(target, NeuronGroup):
                 self.pathway_groups[target.id] = target
@@ -154,28 +160,27 @@
                 for sub_t in target.get_groups():
                     pathway.append(sub_t)
                 for sub_t in target.get_connections():
                     pathway.append(sub_t)
             elif isinstance(target, BaseModule):
                 self.pathway_others[target.id] = target
 
-    def build(self, backend):
+    def build(self, backend: spaic.Backend):
         '''
             Build Learner, choose the backend as user wish, if we have already finished the api.
             Args:
                 backend(backend) : Backend we have.
         '''
         if self.init_trainable is not None:  # If user has given the 'trainable' parameter.
             self.add_trainable(self.init_trainable)
         if self.init_pathway is not None:
             self.add_pathway(self.init_pathway)
 
         if backend.backend_name in self.prefered_backend:
             self._backend = backend
-
         else:
             raise ValueError(
                 "the backend %s is not supported by the learning rule %s" % (backend.backend_name, self.name))
         if self.optim_name is not None:
             self.build_optimizer()
         else:
             self.get_param()
@@ -195,14 +200,16 @@
                 for op in con._ops:
                     op.requires_grad = True
             for other in self.trainable_others.values():
                 for op in other._ops:
                     op.requires_grad = True
             for mod in self.trainable_modules.values():
                 mod.module.requires_grad_()
+                for op in mod._ops:
+                    op.requires_grad = True
 
             for node in self.pathway_nodes.values():
                 for op in node._ops:
                     op.requires_grad = True
             for group in self.pathway_groups.values():
                 for op in group._ops:
                     op.requires_grad = True
@@ -210,14 +217,75 @@
                 for op in con._ops:
                     op.requires_grad = True
             for other in self.pathway_others.values():
                 for op in other._ops:
                     op.requires_grad = True
             for mod in self.pathway_modules.values():
                 mod.module.requires_grad_()
+                for op in mod._ops:
+                    op.requires_grad = True
+
+
+        # add learner variables to the backend
+        self.dt = backend.dt
+        for (key, tau_var) in self._tau_constant_variables.items():
+            tau_var = np.exp(-self.dt / tau_var)
+            shape = ()
+            self.variable_to_backend(self._add_label(key), shape, value=tau_var)
+        for (key, tau_membrane_var) in self._tau_membrane_variables.items():
+            tau_membrane_var = self.dt/tau_membrane_var
+            shape = ()  # (1, neuron_num)
+            self.variable_to_backend(self._add_label(key), shape, value=tau_membrane_var)
+        for (key, var) in self._constant_variables.items():
+            if isinstance(var, np.ndarray):
+                if var.size > 1:
+                    var_shape = var.shape
+                    shape = (1, *var_shape)  # (1, shape)
+                else:
+                    shape = ()
+            elif isinstance(var, list):
+                if len(var) > 1:
+                    var_len = len(var)
+                    shape = (1, var_len)  # (1, shape)
+                else:
+                    shape = ()
+            else:
+                shape = ()
+            self.variable_to_backend(self._add_label(key), shape, value=var)
+        for (key, var) in self._variables.items():
+            if isinstance(var, np.ndarray):
+                if var.size > 1:
+                    var_shape = var.shape
+                    shape = (1, *var_shape)  # (1, shape)
+                else:
+                    shape = ()
+            elif isinstance(var, list):
+                if len(var) > 1:
+                    var_len = len(var)
+                    shape = (1, var_len)  # (1, shape)
+                else:
+                    shape = ()
+            else:
+                shape = ()
+            self.variable_to_backend(self._add_label(key), shape, value=var)
+
+        # build custom learning rules
+        if self.is_overridden(self.custom_rule):
+            self.custom_rule(backend)
+        if self.is_overridden(self.connection_rule):
+            for conn in self.trainable_connections.values():
+                self.connection_rule(conn, backend, 'trainable')
+            for conn in self.pathway_connections.values():
+                self.connection_rule(conn, backend, 'pathway')
+        if self.is_overridden(self.neuron_rule):
+            for neuron in self.trainable_groups.values():
+                self.neuron_rule(neuron, backend, 'trainable')
+            for neuron in self.pathway_groups.values():
+                self.neuron_rule(neuron, backend, 'pathway')
+
 
 
     def __new__(cls, trainable=None, pathway=None, algorithm=('STCA', 'STBP', 'RSTDP', '...'), **kwargs):
         if cls is not Learner:
             return super().__new__(cls)
 
         if algorithm == ('STCA', 'STBP', 'RSTDP', '...'):
@@ -277,14 +345,16 @@
             param.extend(mod.parameters)
 
         return param
 
     def get_varname(self, key):
         name = self.name + ':{' + key + '}'
         return name
+    def get_var_names(self):
+        return self._var_names
 
     def build_optimizer(self):
 
         param = self.get_param()
         self.optim = Learner.optim_dict[self.optim_name](param, self.optim_lr, **self.optim_para)
 
     def build_lr_schedule(self):
@@ -295,15 +365,15 @@
         if self.param_run_update:
             with torch.no_grad():
                 for key, value in self._backend._parameters_dict.items():
                     if key in self.training_param_name:
                         varialbe_value = self._backend._variables[key]
                         if varialbe_value is not value:
                             value.data = varialbe_value.data
-                            self._backend._variables[key] = value
+                            self._backend._variables[key] = value #Is this step needed?
 
         if self.optim is not None:
             self.optim.step()
 
     def optim_zero_grad(self):
 
         self.optim.zero_grad()
@@ -320,30 +390,31 @@
 
         if not issubclass(algorithm, Learner):
             raise ValueError(
                 ('Given algorithm of type %s does not seem to be a valid algorithm.' % str(type(algorithm))))
 
         Learner.learning_algorithms[name] = algorithm
 
-    @staticmethod
-    def connection_function(learner, input_vars=dict(), output_vars=dict(), new_vars_dict=dict(), execute_condition=['initial','iterative','end'], target=['trainable', 'pathway']):
-        pass
+    def custom_rule(self, backend: spaic.Backend):
+        return None
 
-    @staticmethod
-    def Assamble_function(learner, input_vars=dict(), output_vars=dict(), new_vars_dict=dict(), execute_condition=['initial','iterative','end'], target=['trainable', 'pathway']):
-        pass
+    def connection_rule(self, con : spaic.Connection, backend: spaic.Backend, obj_type='trainable'):
+        return None
 
 
-class SpikeProp(Learner):
+    def neuron_rule(self, neuron: spaic.NeuronGroup, backend: spaic.Backend, obj_type='trainable'):
+        return None
 
-    def __init__(self):
-        super(SpikeProp, self).__init__()
-        pass
 
-# Learner.register("spikeprop", SpikeProp)
+    def is_overridden(self, func):
+        if isinstance(self, Learner):
+            return False
+        super_func = getattr(super(type(self), self), func.__name__)
+        return super_func != func
+
 
 
 class ReSuMe(Learner):
 
     def __init__(self):
         super(ReSuMe, self).__init__()
         pass
```

### Comparing `SPAIC-0.6.1a0/spaic/Learning/RSTDP.py` & `SPAIC-0.6.2.0.0/spaic/Learning/RSTDP.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 @author: Yuan Mengwen
 @contact: mwyuan94@gmail.com
 @project: PyCharm
 @filename: RSTDP.py
 @time:2021/4/8 10:46
 @description:
 """
-from ..Network.BaseModule import Op
+from spaic.Network.BaseModule import Op
 from .Learner import Learner
 import numpy as np
 import torch
 
 class RSTDP(Learner):
     """
     Reward-modulated STDP. Adapted from `(Florian 2007)
@@ -197,42 +197,14 @@
                 reward = reward.transpose(1, 0)
                 reward = reward.repeat(1, eligibility_trace.shape[1])
             weight.add_(self.learning_rate * self.dt * reward * eligibility_trace)
         return weight
 
     def build(self, backend):
         super(RSTDPET, self).build(backend)
-        self.dt = backend.dt
-
-        for (key, tau_var) in self._tau_constant_variables.items():
-            tau_var = np.exp(-self.dt / tau_var)
-            shape = ()
-            self.variable_to_backend(key, shape, value=tau_var)
-
-        for (key, tau_membrane_var) in self._tau_membrane_variables.items():
-            tau_membrane_var = self.dt/tau_membrane_var
-            shape = ()  # (1, neuron_num)
-            self.variable_to_backend(key, shape, value=tau_membrane_var)
-
-        for (key, var) in self._constant_variables.items():
-            if isinstance(var, np.ndarray):
-                if var.size > 1:
-                    var_shape = var.shape
-                    shape = (1, *var_shape)  # (1, shape)
-                else:
-                    shape = ()
-            elif isinstance(var, list):
-                if len(var) > 1:
-                    var_len = len(var)
-                    shape = (1, var_len)  # (1, shape)
-                else:
-                    shape = ()
-            else:
-                shape = ()
-            self.variable_to_backend(key, shape, value=var)
 
         view_name = 'rstdpet_view_dim'
         view_dim_value = [-1]
         self.variable_to_backend(view_name, shape=None, value=view_dim_value, is_constant=True)
         reward_name = 'Output_Reward[updated]'
 
         # Traverse all trainable connections
@@ -285,7 +257,79 @@
             self.op_to_backend(eligibility_name, 'add', ['pre_post', 'post_pre'])
             self.op_to_backend('eligibility_trace_temp', 'var_mult', ['tau_e', eligibility_name + '[updated]'])
             self.op_to_backend(eligibility_trace_name, 'var_linear', 'tau_e_trace', eligibility_trace_name, 'eligibility_trace_temp')
 
             self.op_to_backend(None, self.weight_update, [weight_name, eligibility_trace_name, reward_name])
 
 Learner.register('rstdpet', RSTDPET)
+
+
+class RewardSwitchSTDP(Learner):
+    def __init__(self, trainable=None, **kwargs):
+        super(RewardSwitchSTDP, self).__init__(trainable=trainable, **kwargs)
+        self.trainable = trainable
+        self.prefered_backend = ['pytorch']
+        self.name = 'Reward_Switch_STDP'
+        self._constant_variables = dict()
+        self._constant_variables['Apost_pos'] = kwargs.get('Apost_pos', 5.0e-3)
+        self._constant_variables['Apre_pos'] = kwargs.get('Apre_pos', -4.0e-3)
+        self._constant_variables['Apost_neg'] = kwargs.get('Apost_neg', -5.0e-3)
+        self._constant_variables['Apre_neg'] = kwargs.get('Apre_neg', 4.0e-3)
+        self._constant_variables['pre_decay'] = kwargs.get('pre_decay', np.exp(-1/20.0))
+        post_decay = kwargs.get('post_decay', np.exp(-1/20.0))
+        self._constant_variables['post_decay'] = post_decay
+        self._constant_variables['homoestatic'] = kwargs.get('homoestatic', 1.0e-10)
+        m_rate = kwargs.get("m_rate", 20.0)
+        self._constant_variables['m_rate'] = m_rate*(1-post_decay)/(1000.0*post_decay)
+
+        self.w_min = kwargs.get('w_min', 0.0)
+        self.w_max = kwargs.get('w_max', 0.5)
+        self.w_norm = 1.2
+        self.w_mean = None
+        self.lr = kwargs.get('lr',0.1)
+        self.param_run_update = True
+        self.reward_name = kwargs.get('reward_name','Output_Reward[updated]')
+
+    def update(self, input, output, reward, input_trace, output_trace, pre_decay,
+               post_decay, Apost_pos, Apost_neg, Apre_pos, Apre_neg, m_rate, homoestatic, weight):
+        if self.w_mean is None:
+            self.w_mean = torch.mean(weight, dim=1, keepdim=True).detach()
+            self.aw_mean = torch.mean(self.w_mean)
+        if self.training:
+            input_trace = pre_decay * input_trace * input.le(0.0) + input
+            output_trace = post_decay * output_trace * output.le(0.0) + output
+            # with torch.no_grad():
+            #     self.w_mean = self.w_mean * self.aw_mean / torch.mean(self.w_mean)
+            Apost = reward.gt(0) * Apost_pos + reward.le(0) * Apost_neg
+            Apre = reward.gt(0) * Apre_pos + reward.le(0) * Apre_neg
+            pre_post = torch.matmul(output.permute(1, 0), Apost*input_trace)
+            post_pre = torch.matmul((Apre*output_trace).permute(1, 0), input)
+            dw = (pre_post + post_pre)/(1.0*input.shape[0]) # + torch.mean((m_rate-output_trace)*homoestatic,dim=0).unsqueeze(dim=1)
+
+            weight = weight + dw
+            weight = torch.clamp(weight, 0, 0.1)
+            return input_trace, output_trace, weight
+
+    def build(self, backend):
+        self._constant_variables['m_rate'] = self._constant_variables['m_rate']*backend.dt
+        self._constant_variables['homoestatic'] = self._constant_variables['homoestatic'] / self._constant_variables['m_rate']
+        super(RewardSwitchSTDP, self).build(backend)
+        self.dt = backend.dt
+        self.run_time = backend.runtime
+
+
+        for conn in self.trainable_connections.values():
+            preg = conn.pre
+            postg = conn.post
+            pre_name = conn.get_input_name(preg, postg)
+            post_name = conn.get_group_name(postg, 'O')
+            weight_name = conn.get_link_name(preg, postg, 'weight')
+
+            input_trace_name = conn.id + '_{input_trace}'
+            output_trace_name = conn.id + '_{output_trace[stay]}'
+            self.variable_to_backend(input_trace_name, backend._variables[pre_name].shape, value=0.0)
+            self.variable_to_backend(output_trace_name, backend._variables[post_name].shape, value=0.0)
+
+            self.op_to_backend([input_trace_name, output_trace_name, weight_name], self.update,
+                                   [pre_name, post_name, self.reward_name, input_trace_name, output_trace_name, 'pre_decay',
+                                    'post_decay', 'Apost_pos', 'Apost_neg', 'Apre_pos', 'Apre_neg', 'm_rate', 'homoestatic', weight_name])
+Learner.register('switch_rstdp', RewardSwitchSTDP)
```

### Comparing `SPAIC-0.6.1a0/spaic/Learning/STBP_Learner.py` & `SPAIC-0.6.2.0.0/spaic/Learning/STBP_Learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def build(self, backend):
         '''
             Build the backend, realize the algorithm of STBP model.
             Args：
                 backend: The backend we used to compute.
         '''
         super(STBP, self).build(backend)
-        self.device = backend.device
+        self.device = backend.device0
         if backend.backend_name == 'pytorch':
             import torch
             import math
             class ActFun(torch.autograd.Function):
                 """
                 Approximate firing func.
                 """
@@ -74,14 +74,15 @@
                 @staticmethod
                 def backward(
                         ctx,
                         grad_output
                 ):
                     input, = ctx.saved_tensors
                     grad_input = grad_output.clone()
+                    ctx.alpha = ctx.alpha.to(input)
                     temp = torch.exp(-(input - ctx.thresh) ** 2 / (2 * ctx.alpha)) \
                            / (2 * math.pi * ctx.alpha)
                     result = grad_input * temp.type_as(input)
                     return result, None, None
 
 
             self.firing_func = ActFun()
```

### Comparing `SPAIC-0.6.1a0/spaic/Learning/STCA_Learner.py` & `SPAIC-0.6.2.0.0/spaic/Learning/STCA_Learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     @staticmethod
     def backward(
             ctx,
             grad_output
     ):
         input, = ctx.saved_tensors
         grad_input = grad_output.clone()
+        ctx.alpha = ctx.alpha.to(input)
         temp = abs(input - ctx.thresh) < ctx.alpha  # 根据STCA，采用了sign函数
         result = grad_input * temp.type_as(input)
         return result, None, None
 
 act_fun = ActFun()
 def firing_func(x, v_th, alpha):
     return act_fun.apply(x, v_th, alpha)
@@ -89,15 +90,15 @@
             Build the backend, realize the algorithm of STCA model.
 
             Args：
                 backend: The backend we used to compute.
 
         '''
         super(STCA, self).build(backend)
-        self.device = backend.device
+        self.device = backend.device0
         if backend.backend_name == 'pytorch':
             import torch
             class ActFun(torch.autograd.Function):
                 """
                 Approximate firing func.
                 """
                 @staticmethod
```

### Comparing `SPAIC-0.6.1a0/spaic/Learning/STDP_Learner.py` & `SPAIC-0.6.2.0.0/spaic/Learning/STDP_Learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         super(nearest_online_STDP, self).__init__(trainable=trainable)
 
         self.prefered_backend = ['pytorch']
         self.name = 'nearest_online_STDP'
         self._constant_variables = dict()
         self._constant_variables['Apost'] = kwargs.get('Apost', 1e-2)
         self._constant_variables['Apre'] = kwargs.get('Apre', 1e-4)
-        self._constant_variables['trace_decay'] = kwargs.get('trace_decay', np.exp(-1/20))
+        self._constant_variables['trace_pre'] = kwargs.get('trace_pre', np.exp(-1/20))
+        self._constant_variables['trace_post'] = kwargs.get('trace_post', np.exp(-1/20))
         self._constant_variables['spike'] = kwargs.get('spike', 1)
         self.lr = kwargs.get('lr', 0.01)
         self.w_norm = 78.4
         self.trainable = trainable
 
     def nearest_online_stdp_weightupdate(self, dw, weight):
         '''
@@ -58,25 +59,24 @@
                 weight: weight between pre and post neurongroup
 
             Returns:
                 Updated weight.
 
         '''
         with torch.no_grad():
+            # weight = weight + dw
             weight.add_(dw)
 
             # if self._backend.n_time_step < self.total_step:
             #     pass
             # else:
-                # for i in range(weight.shape[0]):
-                #     weight[i] = (weight[i] * self.w_norm) / torch.sum(torch.abs(weight[i]))
+            #     for i in range(weight.shape[0]):
+            #         weight[i] = (weight[i] * self.w_norm) / torch.sum(torch.abs(weight[i]))
 
             weight[...] = (self.w_norm * torch.div(weight, torch.sum(torch.abs(weight), 1, keepdim=True)))
-
-
             weight.clamp_(0.0, 1.0)
             return weight
 
 
     def build(self, backend):
 
         super(nearest_online_STDP, self).build(backend)
@@ -128,19 +128,19 @@
             # self.output_trace = output_trace_s
             #
             ##calculate dw, dw = Apost * (output_spike * input_trace) – Apre * (output_trace * input_spike)
             #
             # dw = self.Apost * torch.matmul(output_spike.permute(1, 0), input_trace_s) \
             #              - self.Apre * torch.matmul(output_trace_s.permute(1, 0), input_spike)  #
 
-            self.op_to_backend('input_trace_s', 'var_mult', [input_trace_name, 'trace_decay'])
+            self.op_to_backend('input_trace_s', 'var_mult', [input_trace_name, 'trace_pre'])
             self.op_to_backend('input_temp', 'minus', ['spike', pre_name])
             self.op_to_backend(input_trace_name, 'var_linear', ['input_temp', 'input_trace_s', pre_name])
 
-            self.op_to_backend('output_trace_s', 'var_mult', [output_trace_name, 'trace_decay'])
+            self.op_to_backend('output_trace_s', 'var_mult', [output_trace_name, 'trace_post'])
             self.op_to_backend('output_temp', 'minus', ['spike', post_name])
             self.op_to_backend(output_trace_name, 'var_linear', ['output_temp', 'output_trace_s', post_name])
 
             self.op_to_backend('pre_post_temp', 'mat_mult_pre', [post_name, input_trace_name+'[updated]'])
             self.op_to_backend('pre_post', 'var_mult', ['Apost', 'pre_post_temp'])
             self.op_to_backend('post_pre_temp', 'mat_mult_pre', [output_trace_name+'[updated]', pre_name])
             self.op_to_backend('post_pre', 'var_mult', ['Apre', 'post_pre_temp'])
@@ -258,14 +258,15 @@
             #
             # dw = self.Apost * torch.matmul(output_spike.permute(1, 0), input_trace_s) \
             #              - self.Apre * torch.matmul(output_trace_s.permute(1, 0), input_spike)  #
 
             self.op_to_backend('input_trace_temp', 'var_mult', [input_trace_name, 'trace_decay'])
             self.op_to_backend(input_trace_name, 'add', [pre_name, 'input_trace_temp'])
 
+
             self.op_to_backend('output_trace_temp', 'var_mult', [output_trace_name, 'trace_decay'])
             self.op_to_backend(output_trace_name, 'add', [post_name, 'output_trace_temp'])
 
             self.op_to_backend('pre_post_temp', 'mat_mult_pre', [post_name, input_trace_name+'[updated]'])
             self.op_to_backend('pre_post', 'var_mult', ['Apost', 'pre_post_temp'])
             self.op_to_backend('post_pre_temp', 'mat_mult_pre', [output_trace_name+'[updated]', pre_name])
             self.op_to_backend('post_pre', 'var_mult', ['Apre', 'post_pre_temp'])
@@ -305,19 +306,14 @@
             pre_post = torch.matmul(output.permute(1, 0), input_trace)
             post_pre = torch.matmul(output_trace.permute(1,0), input)
             dw = Apost*pre_post - Apre*post_pre
             with torch.no_grad():
                 self.w_mean = self.w_mean - 0.1*Apre * (
                             torch.mean(output_trace, 0) - torch.mean(output_trace)).unsqueeze(1)
                 self.w_mean = self.w_mean*self.aw_mean/torch.mean(self.w_mean)
-            with torch.no_grad():
-                self.w_mean = self.w_mean - 0.1 * Apre * (
-                        torch.mean(output_trace, 0) - torch.mean(output_trace)).unsqueeze(1)
-                self.w_mean = self.w_mean * self.aw_mean / torch.mean(self.w_mean)
-
             soft_clamp = (dw.lt(0)*torch.exp(-0.2/torch.clamp_min(weight-self.w_min, 1.0e-4))
                           + dw.gt(0)*torch.exp(-0.2/torch.clamp_min(self.w_max-weight, 1.0e-4))).detach()
             weight = weight*self.w_mean/(torch.clamp_min(torch.mean(weight, dim=1, keepdim=True), 1e-6)).detach() + dw*soft_clamp
         # mw = torch.mean(weight, dim=1)
         # print(torch.amax(mw), torch.amin(mw))
         return input_trace, output_trace, weight
```

### Comparing `SPAIC-0.6.1a0/spaic/Learning/SpikeProp_Learner.py` & `SPAIC-0.6.2.0.0/spaic/Learning/SpikeProp_Learner.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/Learning/Tempotron_Learner.py` & `SPAIC-0.6.2.0.0/spaic/Learning/Tempotron_Learner.py`

 * *Files identical despite different names*

```diff
@@ -196,15 +196,15 @@
         '''
             Build the simulator, realize the algorithm of Tempotron model.
             Args:
                 simulator: The simulator we used to compute.
         '''
 
         super(Tempotron, self).build(backend)
-        self.device = backend.device
+        self.device = backend.device0
         self._backend = backend
         self.sim_name = backend.backend_name
         self.dt = backend.dt
 
         if backend.backend_name == 'pytorch':
             import torch
```

### Comparing `SPAIC-0.6.1a0/spaic/Learning/__init__.py` & `SPAIC-0.6.2.0.0/spaic/Learning/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 @description: 
 """
 
 from .STCA_Learner import STCA
 from .STBP_Learner import STBP
 from .RSTDP import RSTDP, RSTDPET
 # from .PSD_Learner import PSD
-# from .TRUE_Learner import TRUE_SpikeProp
-# from .Rate_Modulation import Rate_Modulate
 
+from .Rate_Modulation import Rate_Modulate
+from .Backprop_RSTDP import Backprop_RSTDP
 
 from .STDP_Learner import nearest_online_STDP, full_online_STDP
 from .Conv_RSTDP import Conv2d_RSTDP
 from .Conv_STDP import Conv2d_STDP
 # from .Tempotron_stm import Tempotron_stm
 from .Tempotron_Learner import Tempotron
```

### Comparing `SPAIC-0.6.1a0/spaic/Library/Network_loader.py` & `SPAIC-0.6.2.0.0/spaic/Library/Network_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,27 @@
 @description:
 对已按格式储存网络的加载和重建
 """
 
 import yaml
 import json
 
-import spaic
+from spaic.Network.Network import Network
+from spaic.Network.Assembly import Assembly
+from spaic.Neuron.Neuron import NeuronGroup
+from spaic.Neuron.Node import Node, Decoder, Encoder, Action, Generator, Reward
+from spaic.Network.Topology import Connection
+from spaic.Backend.Backend import Backend
+from spaic.Backend.Torch_Backend import Torch_Backend
+from spaic.Learning.Learner import Learner
+from spaic.Network.Topology import Projection
+from spaic.Monitor.Monitor import Monitor, StateMonitor, SpikeMonitor
+from spaic.IO.Initializer import BaseInitializer
+from spaic.IO import Initializer as Initer
+
 import torch
 
 
 def network_load(filename=None, path=None, device='cpu', load_weight=True):
     '''
         The main function for getting the target filename and reloading the
             network.
@@ -76,15 +88,15 @@
 
     net = ReloadedNetwork(net_data=data, device=device, load_weight=load_weight)
 
     os.chdir(origin_path)
     return net
 
 
-class ReloadedNetwork(spaic.Network):
+class ReloadedNetwork(Network):
     '''
         The network rebuild from the yaml file.
 
         Args:
             net_data(dict) : The network information reloaded from yaml files.
             dataloader(dataloader) : The dataloader of input layer, since the
                 large scale of data, we will not save the data.
@@ -116,23 +128,18 @@
         super(ReloadedNetwork, self).__init__()
 
         self.device = device
         self.name = list(net_data)[0]
         self._backend_info = []
 
         self.load_net(net_data)
-        if backend is None:
-            backend = spaic.Torch_Backend(device)
 
-        self.set_backend(backend)
-        self.set_backend_data_type()
+        self.load_backend(backend, device=device, load_weight=load_weight, data_type=data_type)
+
         # self._learner = Learner(algorithm='STCA', lr=0.5, trainable=self)
-        self.build()
-        if load_weight:
-            self.load_backend(device)
 
         del self._backend_info
 
     def load_net(self, data):
         '''
             The function for load the whole network, main function of this class.
 
@@ -178,15 +185,15 @@
 
                     break
             else:
                 self.add_assembly(name=list(g)[0], assembly=self.load_assembly(list(g)[0], para))
 
 
     def load_assembly(self, name, assembly: list):
-        target = spaic.Assembly(name=name)
+        target = Assembly(name=name)
         for g in assembly:
             para = g[list(g)[0]]
             if para.get('_class_label') == '<neg>':
                 lay_name = para.get('name')
                 target.add_assembly(name=lay_name,
                                   assembly=self.load_layer(para))
             elif para.get('_class_label') == '<nod>':
@@ -213,66 +220,69 @@
             Return：
                 NeuronGroup with need parameters.
 
         '''
         # layer.pop('_class_label')
         # parameters = self.trans_para(layer.get('parameters'))
         parameters = layer.get('parameters')
-        return_neuron = spaic.NeuronGroup(
+        return_neuron = NeuronGroup(
             num= layer.get('num', 100),
             shape= layer.get('shape', [100]),
             neuron_type     = layer.get('type', 'non_type'),
             neuron_position = layer.get('position', 'x, y, z'),
             model= layer.get('model_name', 'clif'),
             name            = layer.get('name'),
             **parameters
         )
         return_neuron.id = layer.get('id', None)
         return return_neuron
 
-    @staticmethod
-    def load_connection(pnet, con: dict):
+    def load_connection(self, pnet, con: dict):
         '''
             The function for load connections,
 
             Args:
                 con(dict): Data contains the parameters of connections.
 
             Return:
                 Connection with needed parameters.
 
         '''
-        # con.pop('_class_label')
 
-        # if con['pre'] in net._groups.keys() and \
-        #         con['post'] in net._groups.keys():
-        #     con['pre']  = net._groups[con['pre']]
-        #     con['post'] = net._groups[con['post']]
-        # else:
-        #     print("Trans_error")
-        #     print(net._groups.keys())
         if pnet._class_label == '<prj>':
             for pretarget in pnet.pre.get_groups():
                 if con['pre'] == pretarget.id:
                     con['pre'] = pretarget
             for posttarget in pnet.post.get_groups():
                 if con['post'] == posttarget.id:
                     con['post'] = posttarget
         else:
             for target in pnet.get_groups():
                 if con['pre'] == target.id:
                     con['pre'] = target
                 if con['post'] == target.id:
                     con['post'] = target
 
+        for con_tar in ['pre', 'post']:
+            if isinstance(con[con_tar], str):
+                con[con_tar] = self.get_elements()[con[con_tar]] if con[con_tar] in self.get_elements().keys() else None
+
         assert not isinstance(con['pre'], str)
         assert not isinstance(con['post'], str)
 
+        if 'bias' in con['parameters'].keys():
+            bias = con['parameters']['bias']
+            if isinstance(con['parameters']['bias'], dict):
+                if 'method' in con['parameters']['bias'].keys():
+                    method = bias.get('method')
+                    con['parameters']['bias'] = Initer.__dict__[method](**bias.get('para'))
+
+
         # con.pop('weight_path')
-        return_conn = spaic.Connection(
+        return_conn = Connection(
             pre              = con.get('pre'),
             post             = con.get('post'),
             name             = con.get('name'),
             link_type        = con.get('link_type', 'full'),
             syn_type         = con.get('synapse_type', ['basic_synapse']),
             max_delay        = con.get('max_delay', 0),
             sparse_with_mask = con.get('sparse_with_mask', False),
@@ -301,15 +311,15 @@
         else:
             print("Trans_error")
             print(self._groups.keys())
 
         assert not isinstance(prj['pre'], str)
         assert not isinstance(prj['post'], str)
 
-        this_prj = spaic.Projection(
+        this_prj = Projection(
             pre                  = prj.get('pre'),
             post                 = prj.get('post'),
             name                 = prj.get('name'),
             link_type            = prj.get('link_type', 'full'),
             # policies             = prj.get('policies', []),
             ConnectionParameters = prj.get('ConnectionParameters'),
         )
@@ -319,15 +329,15 @@
                 this_prj.add_connection(
                     con=self.load_connection(pnet=this_prj, con=value),
                     name=key,
                 )
 
 
         # prj['policies'] = []
-        # from spaic.Network.ConnectPolicy import IndexConnectPolicy, ExcludedTypePolicy, IncludedTypePolicy
+        # from Network.ConnectPolicy import IndexConnectPolicy, ExcludedTypePolicy, IncludedTypePolicy
         # policy_dict = {'Included_policy': IncludedTypePolicy,
         #                'Excluded_policy': ExcludedTypePolicy}
         #
         # for ply in prj['_policies']:
         #     if ply['name'] == 'Index_policy':
         #         prj['policies'].append(IndexConnectPolicy(pre_indexs=ply['pre_indexs'],
         #                                                   post_indexs=ply['post_indexs'],
@@ -348,18 +358,18 @@
                 node(dict): Data contains the parameters of nodes.
 
             Return:
                 Node of input or output layer, contains needed parameters.
 
         '''
 
-        Node_dict = {'decoder': spaic.Decoder, 'action': spaic.Action, 'reward': spaic.Reward,
-                     'generator': spaic.Generator, 'encoder': spaic.Encoder}
+        Node_dict = {'<decoder>': Decoder, '<action>': Action, '<reward>': Reward,
+                     '<generator>': Generator, '<encoder>': Encoder}
 
-        if node.get('kind') == 'decoder':
+        if node.get('kind') == '<decoder>':
             return_node = Node_dict[node.get('kind')](
                 num             = node.get('num'),
                 dec_target      = self._groups.get(node.get('dec_target', None), None),
                 dt              = node.get('dt', 0.1),
                 # time            = node.get('time'),
                 coding_method   = node.get('coding_method', 'poisson'),
                 coding_var_name = node.get('coding_var_name', 'O'),
@@ -377,44 +387,44 @@
                 coding_var_name = node.get('coding_var_name', 'O'),
                 node_type       = node.get('type', None),
                 **node.get('coding_param')
             )
         return_node.id = node.get('id', None)
         return return_node
 
-    def load_backend(self, device):
+    def load_backend(self, backend=None, device=None, load_weight=False, data_type=None):
         '''
             The function for load backend parameters.
 
         '''
 
-        # key_parameters_dict = ['_variables', '_parameters_dict', '_InitVariables_dict']
-        key_parameters_dict = ['_parameters_dict']
         key_parameters_list = ['dt', 'runtime', 'time', 'n_time_step']
         typical = ['_graph_var_dicts']
 
-
         import torch
-        # import os
 
+        if backend is None:
+            backend = Torch_Backend(device)
+        self.set_backend(backend)
+        self.set_backend_data_type(data_type=data_type)
         if self._backend_info:
-            # self._backend.data_type
             for key in key_parameters_list:
                 self._backend.__dict__[key] = self._backend_info[key]
+        self.build()
 
-            # for key in key_parameters_dict:
+        if load_weight:
             path = self._backend_info['_parameters_dict']
-            data = torch.load(path)
+            data = torch.load(path, map_location=self._backend.device0)
             for key, value in data.items():
                 # print(key, 'value:', value)
-                self._backend._parameters_dict[key] = value.to(device)
-            # self._backend.data_type = value.dtype
-        # #
-        # for key, value in self._backend.__dict__['_parameters_dict'].items():
-        #     self._backend.__dict__['_variables'][key] = value  # 这些变量的 requires_grad应该都是True
+                if key in self._backend._parameters_dict.keys():
+                    target_device = self._backend._parameters_dict[key].device
+                else:
+                    target_device = self._backend.device0
+                self._backend._parameters_dict[key] = value.to(target_device)
 
         return
 
     def set_backend_data_type(self, data_type=None):
         import torch
         supported_data_type = {'torch.float64': torch.float64,
                                'torch.float32': torch.float32,
@@ -426,43 +436,45 @@
                                'torch.bool': torch.bool,
                                'torch.uint8': torch.uint8}
         if data_type:
             self._backend.data_type = data_type
         else:
             if self._backend_info:
                 self._backend.data_type = supported_data_type[self._backend_info['data_type']]
+            else:
+                self._backend.data_type = supported_data_type['torch.float32']
 
     def load_learner(self, learner: dict):
         '''
             The function for load learners' parameters.
 
         '''
-        if '<net>' in learner['trainable']:  ## If self in net, use the whole net as the trainable traget.
+        if '<net>' in learner['trainable']:  ## If self in net, use the whole net as the trainable target.
             learner.pop('trainable')
-            builded_learner = spaic.Learner(
+            builded_learner = Learner(
                 algorithm = learner.get('algorithm'),
                 trainable = self,
                 **learner.get('parameters')
             )
         else:
             trainable_list = []
             for trains in learner['trainable']:
                 if trains in self._groups:
                     trainable_list.append(self._groups[trains])
                 elif trains in self._connections:
                     trainable_list.append(self._connections[trains])
             learner.pop('trainable')
             if learner.get('parameters'):
-                builded_learner = spaic.Learner(
+                builded_learner = Learner(
                     trainable = trainable_list,
                     algorithm = learner.get('algorithm'),
                     **learner.get('parameters')
                     )
             else:
-                builded_learner = spaic.Learner(
+                builded_learner = Learner(
                     trainable = trainable_list,
                     algorithm = learner.get('algorithm')
                 )
         if learner.get('optim_name', None):
             builded_learner.set_optimizer(optim_name=learner.get('optim_name'),
                                       optim_lr=learner.get('optim_lr'),
                                       **learner.get('optim_para'))
@@ -477,16 +489,16 @@
         Used to add monitors to the model according to the
 
         Args:
             monitor: a dict that contains monitors' information.
 
 
         '''
-        monitor_dict = {'StateMonitor': spaic.StateMonitor,
-                        'SpikeMonitor': spaic.SpikeMonitor}
+        monitor_dict = {'StateMonitor': StateMonitor,
+                        'SpikeMonitor': SpikeMonitor}
 
         for name, mon in monitor.items():
             for target in self.get_groups():
                 if mon['target'] == target.id:
                     mon['target'] = target
                     break
             for target in self.get_connections():
@@ -504,9 +516,9 @@
                                  index=mon['index']))
 
     def trans_para(self, para):
         if isinstance(para, dict):
             for key, value in para.items():
                 para[key] = self.trans_para(value)
         else:
-            para = torch.tensor(para, dtype=torch.float32, device=self.device)
+            para = torch.tensor(para, dtype=torch.float32, device=self.device[0])
         return para
```

### Comparing `SPAIC-0.6.1a0/spaic/Library/Network_saver.py` & `SPAIC-0.6.2.0.0/spaic/Library/Network_saver.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 @contact: mxzhangice@gmail.com
 
 @description:
 对既定格式网络的存储
 """
 
 import os
-from ..Network.Assembly import Assembly
-from ..Neuron.Neuron import NeuronGroup
-from ..Neuron.Node import Node
-from ..Network.Topology import Connection
-from ..Backend.Backend import Backend
-from ..Network.Topology import Projection
-from ..Monitor.Monitor import Monitor
+from spaic.Network.Assembly import Assembly
+from spaic.Neuron.Neuron import NeuronGroup
+from spaic.Neuron.Node import Node
+from spaic.Network.Topology import Connection
+from spaic.Backend.Backend import Backend
+from spaic.Network.Topology import Projection
+from spaic.Monitor.Monitor import Monitor
+from spaic.IO.Initializer import BaseInitializer
+from spaic.IO import Initializer as Initer
 
 import time
 
 def network_save(Net: Assembly, filename=None, path=None,
                  trans_format='json', combine=False, save=True, save_weight=True):
     '''
         Save network to files.
@@ -325,20 +327,23 @@
                 'unit_connections', '_var_names', '_supers', '_backend']
     # **link_parameters
 
     for key, para in connection.__dict__.items():
         if key in name_needed:
             para_dict[key] = para.id
         elif key in needed:
+            d_para = para
             if key == 'parameters':
-                if 'weight' in para.keys():
-                    del para['weight']
-            para_dict[key] = check_var_type(para)
+                if 'weight' in d_para.keys():
+                    del d_para['weight']
+                if 'bias' in d_para.keys():
+                    d_para['bias'] = trans_bias(d_para['bias'])
+            para_dict[key] = check_var_type(d_para)
     if combine:     # 是否需要在文件中存储weight
-        para_dict['weight'] = check_var_type(connection.weight)
+        para_dict['weight'] = check_var_type(connection.weight.value)
 
     para_dict['_class_label'] = '<con>'
     result_dict[connection.name] = para_dict
 
     return result_dict
 
 
@@ -380,14 +385,15 @@
         if save:
             save_path = sim_path + '/' + key + '.pt'
             data = backend.__dict__[key]
             torch.save(data, save_path)
             result_dict[key] = './parameters/' + key + '.pt'
         else:
             result_dict = backend._parameter_dict
+            # pass
             # raise ValueError("Wrong save choosen, since parameters can be get from network"
             #                  "unneeded to use network_save function.")
 
     for key in key_parameters_list:
         result_dict[key] = backend.__dict__[key]
 
     result_dict['data_type'] = str(backend.__dict__['data_type'])
@@ -462,14 +468,16 @@
     except:
         if isinstance(var, torch.Tensor):
             return var.detach().cpu().numpy().tolist()
         if isinstance(var, dict):
             for key, value in var.items():
                 var[key] = check_var_type(value)
             return var
+        if isinstance(var, str):
+            return var
         try:
             var_list = var.tolist()
             return var_list
         except:
             raise TypeError('Please check type of parameters, we only support tensor or python build-in types.')
         # if len(var) >= 2:
         #     res_list = var.tolist()
@@ -494,15 +502,24 @@
     #     for key, value in var.items():
     #         var[key] = check_var_type(value)
     #     return var
     # else:
     #     return var
 
 
-
-# def
+def trans_bias(para: dict):
+    if isinstance(para, BaseInitializer):
+        n_para = dict()
+        for key in Initer.__all__:
+            if Initer.__dict__[key] == para.__class__:
+                n_para['method'] = key
+                break
+        n_para['para'] = para.__dict__
+        return n_para
+    else:
+        return para
```

### Comparing `SPAIC-0.6.1a0/spaic/Library/STCA_music_network.py` & `SPAIC-0.6.2.0.0/spaic/Library/STCA_music_network.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/Monitor/Monitor.py` & `SPAIC-0.6.2.0.0/spaic/Monitor/Monitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 @filename: Monitor
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 
 @description:
 定义神经集群放电以及神经元状态量、连接状态量的仿真记录模块
 """
-from ..Network.Assembly import BaseModule, Assembly
-from ..Network.Connections import Connection
-from ..Backend.Backend import Backend
+from spaic.Network.Assembly import BaseModule, Assembly
+from spaic.Network.Connections import Connection
+from spaic.Learning.Learner import Learner
+from spaic.Backend.Backend import Backend
 import numpy as np
 import torch
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.image import AxesImage
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
@@ -26,14 +27,17 @@
         super().__init__()
         if isinstance(target, Assembly):
             self.target = target
             self.target_type = 'Assembly'
         elif isinstance(target, Connection):
             self.target = target
             self.target_type = 'Connection'
+        elif isinstance(target, Learner):
+            self.target = target
+            self.target_type = 'Learner'
         elif target == None:
             self.target = None
             self.target_type = None
         else:
             raise ValueError("The target does not belong to types that can be watched (Assembly, Connection).")
 
         self.var_name = '{'+var_name+'}'
@@ -47,15 +51,15 @@
         self._times = []
         self.dt = dt
         self.is_recording = True
         self.new_record = True
 
     def check_var_name(self, var_name):
         '''
-        Check if variable is in the traget model, and add the target id label to the variable name.
+        Check if variable is in the target model, and add the target id label to the variable name.
 
         Parameters
         ----------
         var_name : original variable name
 
         Returns : modified variable name
         -------
@@ -181,15 +185,17 @@
         Returns
         -------
 
         '''
         if self.is_recording is False:
             return
 
-        if int(10000 * self.backend.time / self.dt) % 10000 == 0:
+        from decimal import Decimal
+        acttime = Decimal(self.backend.time/ self.dt).quantize(Decimal(str(min(self.dt, 0.1))), rounding="ROUND_HALF_UP")
+        if int(10000 * float(acttime)) % 10000 == 0:
             record_value = variables[self.var_name]
             if self.get_grad:
                 variables[self.var_name].retain_grad()
             if self.index == 'full':
                 self._records.append(record_value)
                 self._times.append(self.backend.time)
             else:
@@ -212,55 +218,65 @@
 
     def _spike_transform(self):
         batch_size = self.backend.get_batch_size()
         if len(self._records) > self._transform_len:
             self._transform_len = len(self._records)
             self._spk_index = []
             self._spk_times = []
+            # self._spk_p = []
             if isinstance(self._records[0], torch.Tensor):
                 step = len(self._records)
-                rec_spikes = torch.stack(self._records, dim=-1).cpu().detach()
+                # for i,x in enumerate(self._records):
+                #     self._records[i] = x.cpu()
+                rec_spikes = torch.stack(self._records, dim=-1).detach()
                 if '{[2]' in self.var_name:
                     for ii in range(batch_size):
-                        rec_spikes_i = rec_spikes[ii,0,...].bool().reshape(-1)
+                        rec_spikes_i = rec_spikes[ii,0,...].bool().reshape(-1).cpu()
                         rec_spikes_t = rec_spikes[ii,1,...].reshape(-1)
                         num = int(rec_spikes_i.size(0)/step)
                         time_seq = torch.tensor(self._times).unsqueeze(dim=0).expand(num, -1).reshape(-1)
                         indx_seq = torch.arange(0, num).unsqueeze(dim=1).expand(-1, step).reshape(-1)
                         time_seq = (torch.masked_select(time_seq - rec_spikes_t, rec_spikes_i) ).numpy()
                         indx_seq = torch.masked_select(indx_seq, rec_spikes_i).numpy()
                         self._spk_index.append(indx_seq)
                         self._spk_times.append(time_seq)
+
                 else:
                     for ii in range(batch_size):
                         if rec_spikes.dtype.is_complex:
-                            rec_spikes_i = (rec_spikes[ii, ...].imag.bool()*rec_spikes[ii, ...].real.gt(0.5)).reshape(-1)
+                            rec_spikes_i = (rec_spikes[ii, ...].imag.bool()*rec_spikes[ii, ...].real.gt(0.0)).reshape(-1).cpu()
                         else:
-                            rec_spikes_i = rec_spikes[ii,...].bool().reshape(-1)
+                            rec_spikes_i = rec_spikes[ii,...].bool().reshape(-1).cpu()
 
                         num = int(rec_spikes_i.size(0)/step)
                         time_seq = torch.tensor(self._times).unsqueeze(dim=0).expand(num, -1).reshape(-1)
                         indx_seq = torch.arange(0, num).unsqueeze(dim=1).expand(-1, step).reshape(-1)
                         time_seq = torch.masked_select(time_seq, rec_spikes_i).numpy()
                         indx_seq = torch.masked_select(indx_seq, rec_spikes_i).numpy()
                         self._spk_index.append(indx_seq)
                         self._spk_times.append(time_seq)
+                        # self._spk_p.append(torch.masked_select(rec_spikes[ii, ...].real.reshape(-1).cpu(), rec_spikes_i).numpy())
 
 
     @property
     def spk_times(self):
         self._spike_transform()
         return self._spk_times
 
     @property
     def spk_index(self):
         self._spike_transform()
         return self._spk_index
 
     @property
+    # def spk_p(self):
+    #     self._spike_transform()
+    #     return self._spk_p
+
+    @property
     def spk_grad(self):
         pass
         return None
 
     @property
     def time_spk_rate(self):
         if isinstance(self._records[0], torch.Tensor):
@@ -352,14 +368,15 @@
     def init_record(self):
         '''
         Inite record of new trial
         Returns:
 
         '''
         self.new_record = True
+        self._last_step_time = 0
         if len(self._records) > 0:
             if self.nbatch is True:
                 if isinstance(self._records[0], torch.Tensor):
                     self._nbatch_records.append(torch.stack(self._records, dim=-1).cpu().detach().numpy())
                 else:
                     self._nbatch_records.append(np.stack(self._records, axis=-1))
                 self._nbatch_times.append(self._times)
@@ -374,27 +391,31 @@
                     self._nbatch_times = self._nbatch_times[-self.nbatch:]
 
 
             self._records = []
             self._times = []
 
 
+
     def update_step(self, variables):
         '''
         Recoding the variable values of the current step.
 
         Returns
         -------
 
         '''
         if self.is_recording is False:
             return
 
         # only data in variable_dict can be recorded now
-        if int(10000 * self.backend.time / self.dt) % 10000 == 0:
+        from decimal import Decimal
+        acttime = Decimal(self.backend.time/ self.dt).quantize(Decimal(str(min(self.dt, 0.1))), rounding="ROUND_HALF_UP")
+        if int(10000 * float(acttime)) % 10000 == 0:
+
             record_value = variables[self.var_name]
             if self.get_grad:
                 var = variables[self.var_name]
                 if var.requires_grad is True:
                     var.retain_grad()
             if self.index == 'full':
                 self._records.append(record_value)
@@ -413,14 +434,18 @@
                         record_value = np.array(record_value)
                         record_value = np.moveaxis(record_value, 0, -1)
                         indexed_value = record_value[tuple(self.index)]
                         indexed_value = np.moveaxis(indexed_value, -1, 0)
                     self._records.append(indexed_value)
                     self._times.append(self.backend.time)
 
+        else:
+            print(self.backend.time)
+        self._last_step_time = self.backend.time
+
 
     @property
     def nbatch_values(self):
         if self.new_record:
             self._nbatch_records_ = self._nbatch_records + [torch.stack(self._records, dim=-1).cpu().detach().numpy()]
             self._nbatch_times_ = self._nbatch_times + [self._times]
             self.new_record = False
@@ -434,14 +459,16 @@
             self.new_record = False
         return np.array([np.stack(times, axis=-1) for times in self._nbatch_times_])
 
     @property
     def values(self):
         # return np.concatenate(self._records)
         if isinstance(self._records[0], torch.Tensor):
+            # for i,x in enumerate(self._records):
+            #     self._records[i] = x.cpu()
             return torch.stack(self._records, dim=-1).cpu().detach().numpy()
         else:
             return np.stack(self._records, axis=-1)
 
     @property
     def tensor_values(self):
         assert isinstance(self._records[0], torch.Tensor)
@@ -469,15 +496,15 @@
         else:
             return np.stack(self._times, axis=-1)
 
 
     def plot_weight(self, **kwargs):
         neuron_id = kwargs.get('neuron_id')
         time_id = kwargs.get('time_id')
-        batch_id = kwargs.get('batch_id')
+        batch_id = kwargs.get('batch_id', None)
         new_shape = kwargs.get('new_shape')
         reshape = kwargs.get('reshape')
         axes = kwargs.get('Axes', None)
         ims = kwargs.get('AxesImage', None)
         n_sqrt = kwargs.get('n_sqrt', None)
         side = kwargs.get('side', None)
         figsize = kwargs.get('figsize', (5, 5))
@@ -490,18 +517,22 @@
             value = self.values[:, :, time_id]
             # value = self.simulator._variables[
             #     'autoname1<net>_connection1<con>:autoname1<net>_layer1<neg><-autoname1<net>_input<nod>:{weight}']
             # value = value.cpu().detach().numpy()
 
             if reshape:
 
+                # value = value.reshape(2, 5, side, side)
+                #
+                # value = value.transpose(0, 2, 1, 3)
+                # value = value.reshape(2*side, 5*side)
                 value = value.reshape(n_sqrt, n_sqrt, side, side)
 
                 value = value.transpose(0, 2, 1, 3)
-                value = value.reshape(n_sqrt*side, n_sqrt*side)
+                value = value.reshape(n_sqrt * side, n_sqrt * side)
                 square_weights = value
 
             else:
                 square_weights = value
 
         else:
             value = self.nbatch_values[batch_id, :, time_id, :]
```

### Comparing `SPAIC-0.6.1a0/spaic/Network/Assembly.py` & `SPAIC-0.6.2.0.0/spaic/Network/Assembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 @description:
 """
 import spaic
 
 from collections import OrderedDict
-from ..Network.BaseModule import BaseModule, VariableAgent
+from spaic.Network.BaseModule import BaseModule, VariableAgent
 from abc import ABC, abstractmethod
 from torch import nn
 from typing import List
 import inspect
 
 
 # class ContextMetaClass(type):
@@ -90,14 +90,16 @@
         self._backend: spaic.Backend = None
         self._groups: OrderedDict[str, Assembly] = OrderedDict()
         self._connections: OrderedDict[str, spaic.Connection] = OrderedDict()
         self._projections: OrderedDict[str, spaic.Projection] = OrderedDict()
         self._supers = list()
         self._input_connections = list()
         self._output_connections = list()
+        self._input_modules = list()
+        self._output_modules = list()
         self.num = 0
         self.position = None
         self.model_name = None
         # _var_names 和 _var_dict移动到了BaseModule 作为网络各模块的通用属性
         # self._var_names = []
         # self._var_dict = dict()
         self.context_enterpoint = 0
@@ -228,16 +230,16 @@
         Examples:
 
             >>> TestAsb = Assembly() # assuming contains neurongroups and network structure
             >>> TestAsb.add_connection(name='con1', connection=Connection(self.layer1, self.layer2, link_type='full'))
 
         """
         if self._backend: self._backend.builded = False
-        assert connection.pre in self.get_groups(), 'pre %s is not in the group' % connection.pre.name
-        assert connection.post in self.get_groups(), 'post %s is not in the group' % connection.post.name
+        # assert connection.pre in self.get_groups(), 'pre %s is not in the group' % connection.pre.name
+        # assert connection.post in self.get_groups(), 'post %s is not in the group' % connection.post.name
         if name in self._connections:
             if connection is self._connections[name]:
                 raise ValueError(" connection is already in the assembly's connection list")
             else:
                 raise ValueError("duplicated name for the connection")
         else:
             # self._connections[name] = connection
@@ -510,15 +512,15 @@
         if self._groups and recursive:
             all_groups = []
             for g in self._groups.values():
                 all_groups.extend(g.get_groups(recursive))
             return all_groups
         elif self._groups and not recursive:
             return list(self._groups.values())
-        elif self._class_label == '<asb>':
+        elif self._class_label == '<asb>' or self._class_label == '<net>':
             return []
         else:
             return [self]
 
     def get_leveled_groups(self):
         """
         Get list of all sup groups in leveled order, such as [ [self], [subgroups], [subgroup of subgroups], ...]
@@ -621,27 +623,45 @@
         Args:
             recursive(bool): flag to decide if member connections of the member assemblies should be returned.
 
         Returns:
             List of Connections
         """
         if not recursive:
-            return self._connections.values()
+            return list(self._connections.values())
         else:
             all_assmblies = self.get_assemblies(recursive=2)
-            connections = set()
-            connections.update(self._connections.values())
+            connections = list()
+            connections = self.update_connection(connections, self._connections)
+            # connections.update(self._connections.values())
             for asb in all_assmblies:
                 if asb is self:
-                    connections.update(asb.get_connections(recursive=False))
+                    # connections.update(asb.get_connections(recursive=False))
+                    connections = self.update_connection(connections, asb.get_connections(recursive=False))
                 else:
-                    connections.update(asb.get_connections(recursive=True))
+                    # connections.update(asb.get_connections(recursive=True))
+                    connections = self.update_connection(connections, asb.get_connections(recursive=True))
             for proj in self._projections.values():
-                connections.update(proj.get_connections(recursive=True))
+                # connections.update(proj.get_connections(recursive=True))
+                connections = self.update_connection(connections, proj.get_connections(recursive=True))
             return connections
+    def update_connection(self, container, connections):
+        assert isinstance(container, list)
+        if isinstance(connections, OrderedDict):
+            for con in connections.values():
+                if con not in container:
+                    container.append(con)
+        elif isinstance(connections, list):
+            for con in connections:
+                if con not in container:
+                    container.append(con)
+        else:
+            raise ValueError("connections type not right")
+        return container
+
 
     def get_var_names(self):
         """
         Get a list of variable names the assembly member contains.
 
         """
         return self._var_names
@@ -749,14 +769,23 @@
         if presynaptic:
             if connection_obj not in self._output_connections:
                 self._output_connections.append(connection_obj)
         else:
             if connection_obj not in self._input_connections:
                 self._input_connections.append(connection_obj)
 
+    def register_module(self, module_obj, pre):
+        if pre:
+            if module_obj not in self._output_modules:
+                self._output_modules.append(module_obj)
+        else:
+            if module_obj not in self._input_modules:
+                self._input_modules.append(module_obj)
+
+
     def structure_copy(self, name=None):
         """
         Copy the structure of this assembly with new members
         Args:
             name: name of the new Assembly
 
         Returns:
@@ -842,16 +871,16 @@
         spaic.global_assembly_context_list.pop()
         spaic.global_assembly_context_omit_start = self.context_enterpoint
         spaic.global_assembly_context_omit_end = endpoint_num
         # keys = list(globals().keys())
         # print(keys)
 
     def __setattr__(self, name, value):
-        from ..Network.Topology import Connection
-        from ..Network.Topology import Projection
+        from spaic.Network.Topology import Connection
+        from spaic.Network.Topology import Projection
         super(Assembly, self).__setattr__(name, value)
         if (self.__class__ is spaic.NeuronGroup) or (issubclass(self.__class__, spaic.Node)):
             # If class is NeuronGroup or the subclass of Node, do not add other object to it.
             return
 
         if isinstance(value, Assembly):
             if self._backend: self._backend.builded = False
```

### Comparing `SPAIC-0.6.1a0/spaic/Network/ConnectPolicy.py` & `SPAIC-0.6.2.0.0/spaic/Network/ConnectPolicy.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/Network/Connections.py` & `SPAIC-0.6.2.0.0/spaic/Network/Topology.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1043 +1,1081 @@
-# -*- coding:  utf-8 -*-
+# -*- coding: utf-8 -*-
 """
-Created on 2020/8/5
+Created on 2022/1/18
 @project: SPAIC
-@filename: Connection
+@filename: Topology
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 
-@description:
-定义神经集群间的连接，包括记录神经元集群、连接的突触前、突触后神经元编号、连接形式（全连接、稀疏连接、卷积）、权值、延迟 以及连接产生函数、重连接函数等。
+@description: 
 """
-from ..Network.Topology import Connection
-from ..Network.Assembly import Assembly
-import numpy as np
-import scipy.sparse as sp
-import torch
-from ..IO.Initializer import BaseInitializer
-import random
 
-class FullConnection(Connection):
 
-    '''
-    each neuron in the first layer is connected to each neuron in the second layer.
+from spaic.Network.BaseModule import BaseModule
+from spaic.Network.Assembly import Assembly
+# from spaic.Network.Synapse import Flatten_synapse
+from spaic.IO.Initializer import BaseInitializer
+from spaic.Network.BaseModule import VariableAgent, Op
+from spaic.Backend.Backend import Backend
+from abc import abstractmethod
+from typing import List
+import numpy as np
+from abc import ABC
+from spaic.utils.memory import get_cpu_mem,get_object_size
 
-    Args:
-        pre(Assembly): The assembly which needs to be connected
-        post(Assembly): The assembly which needs to connect the pre
-        link_type(str): full
+class Projection(BaseModule):
     '''
+    Class for projection between assemblies, which contain multiple connections between sub neurongroups
+    '''
+    _class_label = '<prj>'
+    _con_count = 0
 
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O', post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(FullConnection, self).__init__(pre=pre, post=post, name=name,
-                                             link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                             sparse_with_mask=sparse_with_mask,
-                                             pre_var_name=pre_var_name, post_var_name=post_var_name, syn_kwargs=syn_kwargs, **kwargs)
-        weight = kwargs.get('weight', None)
-        self.w_std = kwargs.get('w_std', 0.05)
-        self.w_mean = kwargs.get('w_mean', 0.005)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        self.is_parameter = kwargs.get('is_parameter', True)
-        self.is_sparse = kwargs.get('is_sparse', False)
-
-        bias = kwargs.get('bias', None)
-        if bias is None:
-            self.bias_flag = False
-        else:
-            self.bias_flag = True
-            if isinstance(bias, BaseInitializer):
-                self.b_init, self.b_init_param = self.decode_initializer(bias)
-                self.bias_value = np.empty(self.post_num)
-
-            else:
-                assert (bias.size == self.post_num), f"The size of the given bias {bias.shape} does not correspond" \
-                                                         f" to the size of post_num {self.post_num} "
-                self.bias_value = bias
-
-            self._variables['bias[link]'] = self.bias_value
-
-        if weight is None:
-            # Connection weight
-            self.weight = self.w_std*np.random.randn(*self.shape) + self.w_mean
-        else:
-            if isinstance(weight, BaseInitializer):
-                self.w_init, self.w_init_param = self.decode_initializer(weight)
-                self.weight = np.empty(self.shape)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-
-        self._variables['weight[link]'] = self.weight
-
-
-        self.Isyn_bn = kwargs.get('Isyn_bn', False)
-        if self.Isyn_bn is True:
-            self.Is = []
-            self.beta_ave = kwargs.get('beta_ave', 0.99)
-            self.beta_std = kwargs.get('beta_std', 0.999)
-            self.beta_bn = kwargs.get('beta_bn', 0.001)
-            self.targ_ave = kwargs.get('targ_ave', 1.5)
-            self.targ_std = kwargs.get('targ_std', 2.0)
-            self.running_ave = self.targ_ave
-            self.running_std = self.targ_std
-            self.running_bias = 0.0
-            self.running_scale = 1.0
-
-            self._operations.append([None, self.update_ave, 'V'+'[post]'])
-            self._init_operations.append(['weight[link]', self.update_bn, [post_var_name+'[post]', 'weight[link]']])
-
-        # construct unit connection information by policies,
-        # construct in __init__ is potentially bad, as network structure may change before build. should add new function
-        # self.connection_inforamtion = ConnectInformation(self.pre, self.post)
-        # self.connection_inforamtion.expand_connection()
-        # for p in self._policies:
-        #     self.connection_inforamtion = self.connection_inforamtion & p.generate_connection(self.pre, self.post)
-
-    def update_ave(self, Isyn):
-        with torch.no_grad():
-            if Isyn.dtype.is_complex:
-                self.Is.append(Isyn.imag.detach())
-            else:
-                self.Is.append(Isyn.detach())
-
-    def update_bn(self, Isyn, weight):
-        if self.training:
-            weight.register_hook(self.norm_hook)
-            with torch.no_grad():
-                if len(self.Is) > 1:
-                    Is = torch.cat(self.Is, dim=0)
-                    mean_rate = torch.mean(Is, dim=0)
-                    std = torch.std(Is, dim=0)
-                    self.running_ave = self.beta_ave*self.running_ave + (1-self.beta_ave)*mean_rate
-                    self.running_std = self.beta_std*self.running_std + (1-self.beta_std)*std
-
-                    d_bias = (self.targ_ave - self.running_ave)*torch.sigmoid(20.0*(self.targ_ave - self.running_ave)*(self.running_ave-mean_rate))
-                    self.running_bias = self.running_bias + self.beta_bn*d_bias
-                    d_scale = torch.exp((self.targ_std - self.running_std)) - 1.0
-                    self.running_scale = self.running_scale + self.beta_bn*d_scale
-                    self.Is = []
-                    self.weight_change = True
-                else:
-                    self.weight_change = False
-                    self.running_scale = torch.ones_like(torch.mean(Isyn.real, dim=0))
-                    self.running_bias = torch.zeros_like(torch.mean(Isyn.real, dim=0))
-        else:
-            self.Is = []
-
-        if self.weight_change:
-            weight = self.running_scale.unsqueeze(-1) * weight + self.running_bias.unsqueeze(-1)
-            if weight.requires_grad:
-                weight.retain_grad()
-
-
-        return weight
-    def norm_hook(self, grad):
-        mean_grad = torch.mean(grad, dim=1, keepdim=True)
-        return grad - mean_grad
-
-    def condition_check(self, pre_group, post_group):
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-        pass
-
-Connection.register('full', FullConnection)
-Connection.register('full_connection', FullConnection)
-
-class one_to_one_sparse(Connection):
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O', post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(one_to_one_sparse, self).__init__(pre=pre, post=post, name=name,
-                                                link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                                sparse_with_mask=sparse_with_mask,
-                                                pre_var_name=pre_var_name, post_var_name=post_var_name, syn_kwargs=syn_kwargs, **kwargs)
-        try:
-            assert self.pre_num == self.post_num
-        except AssertionError:
+    def __init__(self, pre: Assembly, post: Assembly, policies=[], link_type=None, ConnectionParameters=None,
+                 name=None):
+        super(Projection, self).__init__()
+        assert isinstance(pre, Assembly)
+        assert isinstance(post, Assembly)
+        self.name = name
+        self.super = None
+        self.abstract_level = 0
+        self._backend: Backend = None
+        self.pre = pre
+        self.post = post
+        self._connections = dict()
+        self._projections = dict()
+
+        if (pre.id is not None) and (post.id is not None):
+            self.key = pre.id + "->" + post.id
+        else:
+            self.key = 'default' + str(Projection._con_count)
+        Projection._con_count += 1
+        self._leaf_connections = dict()
+
+        if isinstance(ConnectionParameters, dict):
+            self.ConnectionParameters = ConnectionParameters
+        else:
+            self.ConnectionParameters = dict()
+        if pre._is_terminal and post._is_terminal:
+            self.is_unit = True
+        else:
+            self.is_unit = False
+
+        self._policies = policies
+        if self._policies:
+            assert link_type is not None
+        if isinstance(self._policies, ConnectPolicy):
+            self._policies = [self._policies]
+        self.link_type = link_type
+        self._supers = []
+
+    def __setattr__(self, name, value):
+        super(Projection, self).__setattr__(name, value)
+        if name == 'super':
+            return
+        if isinstance(value, Connection):
+            if self._backend: self._backend.builded = False
+            self._connections[name] = value
+            # self._leaf_connections[value.key] = value
+            value.set_name(name)
+            value.add_super(self)
+        elif isinstance(value, Projection):
+            if self._backend: self._backend.builded = False
+            self._projections[name] = value
+            # self._leaf_connections[value.key] = value
+            value.set_name(name)
+            value.add_super(self)
+
+    def homologous(self, other):
+        if (other.pre is self.pre) and (other.post is self.post):
+            return True
+        else:
+            return False
+
+    def is_empty(self):
+        if self.is_unit:
+            return False
+        elif len(self._connections) + len(self._projections) + len(self._leaf_connections) == 0:
+            return True
+        else:
+            return False
+
+    def __and__(self, other):
+        if not self.homologous(other):
+            raise ValueError("can't do & operation for nonhomologous connections")
+        if self.is_empty():
+            new_connect = self
+        elif other.is_empty():
+            new_connect = other
+        else:
+            new_connect = Projection(self.pre, self.post)
+            # unit connections
+            key1 = set(self._connections.keys())
+            key2 = set(other._connections.keys())
+            unite_keys = key1.intersection(key2)
+            for key in unite_keys:
+                new_connect._connections[key] = self._connections[key]
+                new_connect._connections[key].super = new_connect
+
+            # assb connections
+            key1 = set(self._projections.keys())
+            key2 = set(other._projections.keys())
+            unite_keys = key1.intersection(key2)
+            for key in unite_keys:
+                new_connect._projections[key] = self._projections[key] & other._projections[key]
+                new_connect._projections[key].super = new_connect
+
+            # leaf_connections
+            key1 = set(self._leaf_connections.keys())
+            key2 = set(other._leaf_connections.keys())
+            unite_keys = key1.intersection(key2)
+            for key in unite_keys:
+                new_connect._leaf_connections[key] = self._leaf_connections[key] & other._leaf_connections[key]
+
+        return new_connect
+
+    def add_connection(self, con, name=None):
+        assert isinstance(con, Projection)
+        con.super = self
+        key = con.key
+        if not (con.pre in self.pre and con.post in self.post):
             raise ValueError(
-                'One to One connection must be defined in two groups with the same size, but the pre_num %s is not equal to the post_num %s.' % (
-                self.pre_num, self.post_num))
-        weight = kwargs.get('weight', None)
-        self.w_mean = kwargs.get('w_mean', 0.05)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        self.is_parameter = kwargs.get('is_parameter', False)
-        self.is_sparse = kwargs.get('is_sparse', True)
-
-        if weight is None:
-            # Connection weight
-            self.weight = self.w_mean * np.eye(*self.shape)
-        else:
-            if isinstance(weight, BaseInitializer):
-                raise ValueError('Sparse implementation of one_to_one_sparse connection do not support the %s '
-                                 'initialization method. You can pass a numpy matrix whose diagonal is not zero.',
-                                 self.w_init)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-        self._variables['weight[link]'] = self.weight
-
-        bias = kwargs.get('bias', None)
-        if bias is None:
-            self.bias_flag = False
-        else:
-            self.bias_flag = True
-            if isinstance(bias, BaseInitializer):
-                self.b_init, self.b_init_param = self.decode_initializer(bias)
-                self.bias_value = np.empty(self.post_num)
+                "the sub connection is not belong to this connection group (pre and post is not a member of the connected Assemblies)")
 
-            else:
-                assert (bias.size == self.post_num), f"The size of the given bias {bias.shape} does not correspond" \
-                                                         f" to the size of post_num {self.post_num} "
-                self.bias_value = bias
-
-            self._variables['bias[link]'] = self.bias_value
-
-
-    def condition_check(self, pre_group, post_group):
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-        pass
-
-Connection.register('one_to_one_sparse', one_to_one_sparse)
-
-
-class one_to_one_mask(Connection):
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=True, pre_var_name='O', post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(one_to_one_mask, self).__init__(pre=pre, post=post, name=name,
-                                              link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                              sparse_with_mask=sparse_with_mask, pre_var_name=pre_var_name,
-                                              post_var_name=post_var_name, syn_kwargs=syn_kwargs, **kwargs)
-        try:
-            assert self.pre_num == self.post_num
-        except AssertionError:
-            raise ValueError('One to One connection must be defined in two groups with the same size, but '
-                             'the pre_num %s is not equal to the post_num %s.' % (self.pre_num, self.post_num))
-        weight = kwargs.get('weight', None)
-        self.w_mean = kwargs.get('w_mean', 0.05)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        # self.init = kwargs.get('init', None)
-        self.is_parameter = kwargs.get('is_parameter', True)
-        self.is_sparse = kwargs.get('is_sparse', False)
-        # self._variables = dict()
-
-        if weight is None:
-            # Connection weight
-            self.weight = self.w_mean * np.eye(*self.shape)
-        else:
-            if isinstance(weight, BaseInitializer):
-                raise ValueError('Dense implementation of one_to_one_mask connection do not support the %s '
-                                 'initialization method. You can pass a numpy matrix whose diagonal is not zero.', self.w_init)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-
-        self._variables['weight[link]'] = self.weight
-
-        bias = kwargs.get('bias', None)
-        if bias is None:
-            self.bias_flag = False
-        else:
-            self.bias_flag = True
-            if isinstance(bias, BaseInitializer):
-                self.b_init, self.b_init_param = self.decode_initializer(bias)
-                self.bias_value = np.empty(self.post_num)
-
-            else:
-                assert (bias.size == self.post_num), f"The size of the given bias {bias.shape} does not correspond" \
-                                                         f" to the size of post_num {self.post_num} "
-                self.bias_value = bias
+        con.set_name(name)
+        if con.is_unit:
+            self.__setattr__(name, con)
+            # self._connections[key] = con
+        else:
+            self._projections[key] = con
+
+    def add_leaf_connection(self, con):
+        assert isinstance(con, Projection)
+        con.super = self
+        key = con.key
+        if not (con.pre in self.pre and con.post in self.post):
+            raise ValueError("the sub connection is not belong to this connection group (pre and post is not a member of the connected Assemblies)")
+        con.set_name(None)
+        self._leaf_connections[key] = con
+
+    def del_connection(self):
+        if self.super is not None:
+            if self.key in self.super._connections:
+                self.super._connections.pop(self.key)
+            if self.key in self.super._projections:
+                self.super._projections.pop(self.key)
+            if self.key in self.super._leaf_connections:
+                self.super._leaf_connections.pop(self.key)
+
+            top_leaf = self.top._leaf_connections
+            if self.key in top_leaf:
+                top_leaf.pop(self.key)
+            if self.super.is_empty():
+                self.super.del_connection()
+            self.super = None
+        else:
+            self.is_unit = False
+
+    def expand_connection(self, to_level=-1):
+        assert isinstance(to_level, int), ValueError("level is not int")
+        if not bool(self._leaf_connections):
+            self._leaf_connections[self.key] = self
+        if self.is_unit:
+            return self._leaf_connections.values()
+        else:
+            new_leaf_connections = dict()
+            assb_connections = self._leaf_connections.values()
+            while (len(assb_connections) > 0):
+                if to_level >= 0 and to_level <= self.abstract_level:
+                    break
+                self.abstract_level += 1
+                new_assb_connections = []
+                for con in assb_connections:
+                    if con.is_unit:
+                        new_leaf_connections[con.key] = con
+                    else:
+                        pre_groups = con.pre.get_groups(recursive=False)
+                        post_groups = con.post.get_groups(recursive=False)
+                        for pre in pre_groups:
+                            for post in post_groups:
+                                new_con = Projection(pre, post)
+                                # con.add_connection(new_con)
+                                if new_con.is_unit:
+                                    new_leaf_connections[new_con.key] = new_con
+                                else:
+                                    new_assb_connections.append(new_con)
+
+                assb_connections = new_assb_connections
+
+            for con in assb_connections:
+                # 对于超过abstract_level的connection，都认为是leaf_connection
+                new_leaf_connections[con.key] = con
+
+            # self._leaf_connections = new_leaf_connections
+            self._leaf_connections.clear()
+            for key, con in new_leaf_connections.items():
+                self.add_leaf_connection(con)
+
+            return list(new_leaf_connections.values())
+
+    def assembly_linked(self, assembly):
+        if (assembly is self.pre) or (assembly is self.post):
+            return True
+        else:
+            return False
+
+    def replace_assembly(self, old_assembly, new_assembly):
+        if old_assembly is self.pre:
+            self.pre = new_assembly
+        elif old_assembly is self.post:
+            self.post = new_assembly
+        else:
+            raise ValueError("the old_assembly is not in the connnection")
+
+    def add_super(self, assembly):
+        assert isinstance(assembly, Assembly) or isinstance(assembly,
+                                                            Projection), "the super is not Assembly or Projection"
+        self._supers.append(assembly)
+
+    def del_super(self, assembly):
+        assert assembly in self._supers, "the assembly is not in supers"
+        self._supers.remove(assembly)
+
+    def get_connections(self, recursive=True):
+        """
+            Get the Connections in this assembly
+        Args:
+            recursive(bool): flag to decide if member connections of the member assemblies should be returned.
 
-            self._variables['bias[link]'] = self.bias_value
+        Returns:
+            List of Connections
+        """
+        if not recursive:
+            return self._connections.values()
+        else:
+            connections = list(self._connections.values())
+            for proj in self.sub_projections:
+                connections.extend(proj.get_connections(recursive=False))
+            return connections
+
+    @property
+    def top(self):
+        if self.super is None:
+            return self
+        else:
+            return self.super.top
+
+    @property
+    def sub_connections(self):
+        if self.is_unit:
+            raise ValueError("no sub_connections for unit connections")
+        else:
+            sub_connections = []
+            sub_connections.extend(self._connections.values())
+            return sub_connections
+
+    @property
+    def sub_projections(self):
+        if self.is_unit:
+            raise ValueError("no sub assb_connections for unit connections")
+        else:
+            return list(self._projections.values())
+
+    @property
+    def all_connections(self):
+        if self.is_unit:
+            return [self]
+        else:
+            unit_connections = []
+            unit_connections.extend(self._connections.values())
+            for con in self._projections.values():
+                unit_connections.extend(con.all_connections)
+            return unit_connections
+
+    @property
+    def all_projections(self):
+        if self.is_unit:
+            raise ValueError("no sub_connections for unit connections")
+        else:
+            assb_connections = []
+            assb_connections.extend(self._projections.values())
+            for con in self._projections.values():
+                assb_connections.extend(con.all_projections)
+            return assb_connections
+
+    @property
+    def leaf_connections(self):
+        return list(self._leaf_connections.values())
+
+    def get_str(self, level):
+
+        # TODO: add str of subconnections
+        level_space = "" + '-' * level
+        repr_str = level_space + "|name:{}, type:{}, ".format(self.name, type(self).__name__)
+        repr_str += "pre:{}, ".format(self.pre.name)
+        repr_str += "post:{}\n ".format(self.post.name)
+        level += 1
+        for c in self._projections.values():
+            repr_str += c.get_str(level)
+        for c in self._connections.values():
+            repr_str += c.get_str(level)
+        return repr_str
+
+    def train(self, mode=True):
+        self.training = mode
+        for p in self._projections.values():
+            p.train(mode)
+        for c in self._connections.values():
+            c.training = mode
+
+    def build(self, backend=None):
+        self._backend = backend
+
+        # clear previous builded connections
+        if backend.builded == True:
+            for super_asb in self._supers:
+                for con in self._connections:
+                    super_asb.del_connection(con)
+        for sub_proj in self._projections.values():
+            sub_proj.build(backend)
+        # if not policy is not given then it does not have connection policy (no default policy)
+        if not self._policies:
+            return
+        connection_inforamtion = None
+        for p in self._policies:
+            if connection_inforamtion is None:
+                connection_inforamtion = p.generate_connection(self.pre, self.post)
+            else:
+                connection_inforamtion = connection_inforamtion & p.generate_connection(self.pre,
+                                                                                        self.post)
+
+        self._connections = connection_inforamtion._connections
+        self._projections = connection_inforamtion._projections
+        self._leaf_connections = connection_inforamtion._leaf_connections
+        all_connections = dict()
+        all_connections.update(self._connections)
+        all_connections.update(self._leaf_connections)
+        new_connections = dict()
+        auto_con_num = 0
+        for key, con in all_connections.items():
+            assert con.is_unit
+            if con.link_type is not None:
+                link_type = con.link_type
+                con_name = con.name
+                con_kwargs = con.con_kwargs
+                con_kwargs.update(self.ConnectionParameters)
+                syn_kwargs = con.syn_kwargs
+            else:
+                assert self.link_type is not None
+                link_type = self.link_type
+                con_name = 'auto_con' + str(auto_con_num)
+                auto_con_num += 1
+                con_kwargs = self.ConnectionParameters
+                syn_kwargs = None
+
+            new_connections[key] = Connection(pre=con.pre, post=con.post,
+                                              name=con_name, link_type=link_type, syn_kwargs=syn_kwargs, **con_kwargs)
+            new_connections[key].add_super(self)
+        self._connections = new_connections
 
-    def condition_check(self, pre_group, post_group):
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-        pass
-Connection.register('one_to_one', one_to_one_mask)
 
-class conv_connect(Connection):
 
+class SynapseModel(ABC):
     '''
-    do the convolution connection.
-
-    Args:
-        pre(Assembly): the assembly which needs to be connected
-        post(Assembly): the assembly which needs to connect the pre
-        link_type(str): Conv
-    Methods:
-        unit_connect: define the basic connection information and add them to the connection_information.
-        condition_check: check whether the pre_group.type is equal to the post_group.type, only if they are equal, return flag=Ture.
-
+    op -> (return_name, operation_name, input_name1, input_name2...)
     '''
 
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['conv'], max_delay=0, sparse_with_mask=False, pre_var_name='O', post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(conv_connect, self).__init__(pre=pre, post=post, name=name,
-                                           link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                           sparse_with_mask=sparse_with_mask,
-                                           pre_var_name=pre_var_name, post_var_name=post_var_name, syn_kwargs=syn_kwargs, **kwargs)
-        self.out_channels = kwargs.get('out_channels', None)
-        self.in_channels = kwargs.get('in_channels', None)
-        self.kernel_size = kwargs.get('kernel_size', [3, 3])
-        self.w_std = kwargs.get('w_std', 0.05)
-        self.w_mean = kwargs.get('w_mean', 0.05)
-        weight = kwargs.get('weight', None)
+    #: A dictionary mapping synapse model names to `Model` objects
+    synapse_models = dict()
 
-        self.is_parameter = kwargs.get('is_parameter', True)
-        self.is_sparse = kwargs.get('is_sparse', False)
-        self.mask = kwargs.get('mask', None)
-        self.stride = kwargs.get('stride', 1)
-        self.padding = kwargs.get('padding', 0)
-        self.dilation = kwargs.get('dilation', 1)
-        self.groups = kwargs.get('groups', 1)
-
-        if isinstance(self.kernel_size, int):
-            self.kernel_size = [self.kernel_size] * 2
-        if isinstance(self.stride, int):
-            self.stride = [self.stride] * 2
-        if isinstance(self.padding, int):
-            self.padding = [self.padding] * 2
-        # self._variables = dict()
-        self._constant_variables['stride[pre]'] = self.stride
-        self._constant_variables['padding[pre]'] = self.padding
-        self._constant_variables['dilation[pre]'] = self.dilation
-        self._constant_variables['groups[pre]'] = self.groups
-
-        if self.in_channels is None:
-            from spaic.Neuron.Encoders import NullEncoder
-            if len(self.pre.shape) == 1:
-                raise ValueError('The shape %s of pre seems to be a flattened value. '
-                                 'Give the correct shape with structure [channel, height, width] in the NeuronGroup '
-                                 'class with the neuron_shape parameter' % self.pre.shape)
-            elif isinstance(self.pre, NullEncoder):
-                self.in_channels = self.pre.shape[2]
+    def __init__(self, conn, **kwargs):
+        super(SynapseModel, self).__init__()
+        self.name = 'none'
+        self._syn_operations = []
+        self._syn_variables = dict()
+        self._syn_constant_variables = dict()
+        self._syn_tau_variables = dict()
+        if conn is not None:
+            updated_input = conn.updated_input
+            if updated_input:
+                self.input_name = conn.pre_var_name + '[input][updated]'
             else:
-                self.in_channels = self.pre.shape[0]
+                self.input_name = conn.pre_var_name + '[input]'
 
-        if self.out_channels is None:
-            if len(self.post.shape) == 1:
-                raise ValueError('The shape %s of post seems to be a flattened value.  '
-                                 'Give the correct shape with structure [channel, height, width] in the NeuronGroup '
-                                 'class with the neuron_shape parameter' % self.post.shape)
-            else:
-                self.out_channels = self.post.shape[0]
+    @staticmethod
+    def register(name, model):
+        '''
+        Register a synapse model. Registered synapse models can be referred to
+        # via their name.
+        Parameters
+        ----------
+        name : str
+            A short name for the state updater (e.g. `'basic'`)
+        model : `SynapseModel`
+            The synapse model object, e.g. an `Basic_synapse`.
+        '''
 
-        self.shape = (self.out_channels, self.in_channels, self.kernel_size[0], self.kernel_size[1])
+        # only deal with lower case names
+        name = name.lower()
+        if name in SynapseModel.synapse_models:
+            raise ValueError(('A synapse_model with the name "%s" has already been registered') % name)
 
-        if weight is None:
-            # Connection weight
-            self.weight = self.w_std * np.random.randn(*self.shape) + self.w_mean
-        else:
-            if isinstance(weight, BaseInitializer):
-                self.w_init, self.w_init_param = self.decode_initializer(weight)
-                self.weight = np.empty(self.shape)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-
-        self._variables['weight[link]'] = self.weight
-
-        bias = kwargs.get('bias', None)
-        if bias is None:
-            self.bias_flag = False
-        else:
-            self.bias_flag = True
-            if isinstance(bias, BaseInitializer):
-                self.b_init, self.b_init_param = self.decode_initializer(bias)
-                # import math
-                # bound = math.sqrt(1 / (self.in_channels * self.kernel_size[0] * self.kernel_size[1]))
-                # self.bias_value = np.random.uniform(-bound, bound, self.out_channels)
-                self.bias_value = np.empty(self.out_channels)
+        if not issubclass(model, SynapseModel):
+            raise ValueError(('Given model of type %s does not seem to be a valid SynapseModel.' % str(type(model))))
 
-            else:
-                assert (bias.size == self.out_channels), f"The size of the given bias {bias.shape} does not correspond" \
-                                                     f" to the size of output_channels {self.out_channels} "
-                self.bias_value = bias
-
-            self._variables['bias[link]'] = self.bias_value
-
-        Hin = self.pre.shape[-2]
-        Win = self.pre.shape[-1]
-
-        pool_Flag = False
-        if 'avgpool' in self.synapse_name:
-            pool_Flag = True
-            self.pool_index = self.synapse_name.index('avgpool')
-
-        if 'maxpool' in self.synapse_name:
-            pool_Flag = True
-            self.pool_index = self.synapse_name.index('maxpool')
-
-        self.conv_index = self.synapse_name.index('conv')
-
-        # if self.pool is not None:  # 池化
-        if pool_Flag:
-            self.pool_only = False
-            self.pool_kernel_size = kwargs.get('pool_kernel_size', [2, 2])
-            self.pool_stride = kwargs.get('pool_stride', 2)
-            self.pool_padding = kwargs.get('pool_padding', 0)
-            if isinstance(self.pool_kernel_size, int):
-                self.pool_kernel_size = [self.pool_kernel_size] * 2
-            if isinstance(self.pool_stride, int):
-                self.pool_stride = [self.pool_stride] * 2
-            if isinstance(self.pool_padding, int):
-                self.pool_padding = [self.pool_padding] * 2
-
-            self._constant_variables['pool_kernel_size[pre]'] = self.pool_kernel_size
-            self._constant_variables['pool_stride[pre]'] = self.pool_stride
-            self._constant_variables['pool_padding[pre]'] = self.pool_padding
-
-            if self.pool_index < self.conv_index:
-                # pooling before conv
-                self.pool_before = True
-                Ho = int((Hin + 2 * self.pool_padding[0] - self.pool_kernel_size[0]) / self.pool_stride[0] + 1)
-                Wo = int((Win + 2 * self.pool_padding[1] - self.pool_kernel_size[1]) / self.pool_stride[1] + 1)
-                Ho = int((Ho + 2 * self.padding[0] - self.kernel_size[0]) / self.stride[0] + 1)
-                Wo = int((Wo + 2 * self.padding[1] - self.kernel_size[1]) / self.stride[1] + 1)
-            else:
-                # conv before pooling
-                self.pool_before = False
-                Ho = int((Hin + 2 * self.padding[0] - self.kernel_size[0]) / self.stride[0] + 1)  # Ho = (Hin + 2 * padding[0] - kernel_size[0]) / stride[0] + 1
-                Wo = int((Win + 2 * self.padding[1] - self.kernel_size[1]) / self.stride[1] + 1)  # Wo = (Win + 2 * padding[0] - kernel_size[1]) / stride[0] + 1
-                # Ho = int(Ho / self.pool_kernel_size[0])
-                # Wo = int(Wo / self.pool_kernel_size[1])
-                Ho = int((Ho + 2 * self.pool_padding[0] - self.pool_kernel_size[0]) / self.pool_stride[0] + 1)  # Ho = (Hin + 2 * padding[0] - kernel_size[0]) / stride[0] + 1
-                Wo = int((Wo + 2 * self.pool_padding[1] - self.pool_kernel_size[1]) / self.pool_stride[1] + 1)
-        else:
-            # without pooling
-            Ho = int((Hin + 2 * self.padding[0] - self.kernel_size[0]) / self.stride[0] + 1)
-            Wo = int((Win + 2 * self.padding[1] - self.kernel_size[1]) / self.stride[1] + 1)
-
-        post_num = int(Ho * Wo * self.out_channels)
-
-        if self.post.num == None:
-            self.post.num = post_num
-            self.post.shape = (self.out_channels, Ho, Wo)
-
-        if self.post.num != None:
-            if self.post.num != post_num:
-                raise ValueError(
-                    "The post_group num is not equal to the output num, cannot achieve the conv connection, "
-                    "the output num is %d * %d * %d " % (self.out_channels, Ho, Wo))
-            else:
-                self.post.shape = (self.out_channels, Ho, Wo)
+        SynapseModel.synapse_models[name] = model
+        model.name = name
 
-    def condition_check(self, pre_group, post_group):
+    @staticmethod
+    def apply_model(model_name):
         '''
-        check whether the pre_group.type is equal to the post_group.type, only if they are equal, return flag=Ture.
-
-        Args:
-            pre_group(Groups): the neuron group which need to be connected in the pre.
-            post_group(Groups): the neuron group which need to connect the pre_group in the post.
-
-        Returns: flag
-
+        Parameters
+        ----------
+        model_name : str
+        Returns
+        -------
         '''
+        model_name = model_name.lower()
+        if model_name not in SynapseModel.synapse_models:
+            raise ValueError(('Given synapse model name is not in the model list'))
+        else:
+            return SynapseModel.synapse_models[model_name]
 
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-Connection.register('conv', conv_connect)
-Connection.register('conv_connection', conv_connect)
-
-class pool_connect(Connection):
 
+class Connection(Projection):
     '''
-    do the pooling operation on spiking trains.
-
+    Base class for all kinds of connections, including full connection, sparse connection, conv connection,....
+    Ten connection methods are provided, as shown below (key: class):
+        'full', FullConnection
+        'one_to_one_sparse', one_to_one_sparse
+        'one_to_one', one_to_one_mask
+        'conv', conv_connect
+        'sparse_connection_sparse', sparse_connect_sparse
+        'sparse_connection', sparse_connect_mask
+        'random_connection_sparse', random_connect_sparse
+        'random_connection', random_connect_mask
     Args:
-        pre(Assembly): the assembly which needs to be connected
-        post(Assembly): the assembly which needs to connect the pre
-        link_type(str): Conv
+        pre(Assembly): the assembly which needs to be connected.
+        post(Assembly): the assembly which needs to connect the pre.
+        link_type(str): the type for connection: full, sparse, conv...
+
+    Attributes:
+        pre_group(groups): the neuron group which need to be connected in the pre.
+        post_group(groups): the neuron group which need to connect with pre_group neuron.
+        _var_names(list): a list contain variable names.
+
     Methods:
-        unit_connect: define the basic connection information and add them to the connection_information.
+        __new__: before build a new connection, do some checks.
+        get_var_names: get variable names.
+        register: register a connection class.
+        build: add the connection variable, variable name and opperation to the backend.
+        get_str:
         condition_check: check whether the pre_group.type is equal to the post_group.type, only if they are equal, return flag=Ture.
-
-    '''
-
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['maxpool'], max_delay=0, sparse_with_mask=False, pre_var_name='O', post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(pool_connect, self).__init__(pre=pre, post=post, name=name,
-                                           link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                           sparse_with_mask=sparse_with_mask,
-                                           pre_var_name=pre_var_name, post_var_name=post_var_name, syn_kwargs=syn_kwargs, **kwargs)
-
-        self.pool_kernel_size = kwargs.get('pool_kernel_size', [2, 2])
-        self.pool_stride = kwargs.get('pool_stride', 2)
-        self.pool_padding = kwargs.get('pool_padding', 0)
-        if isinstance(self.pool_kernel_size, int):
-            self.pool_kernel_size = [self.pool_kernel_size] * 2
-        if isinstance(self.pool_stride, int):
-            self.pool_stride = [self.pool_stride] * 2
-        if isinstance(self.pool_padding, int):
-            self.pool_padding = [self.pool_padding] * 2
-
-        self._constant_variables['pool_kernel_size[pre]'] = self.pool_kernel_size
-        self._constant_variables['pool_stride[pre]'] = self.pool_stride
-        self._constant_variables['pool_padding[pre]'] = self.pool_padding
-        self.pool_only = True
-
-
-    def condition_check(self, pre_group, post_group):
-        '''
-        check whether the pre_group.type is equal to the post_group.type, only if they are equal, return flag=Ture.
-
-        Args:
-            pre_group(Groups): the neuron group which need to be connected in the pre.
-            post_group(Groups): the neuron group which need to connect the pre_group in the post.
-
-        Returns: flag
+        connect: connect the preg with postg.
+        get_weight_name: give a name for each connection weight.
+        get_post_name: give a name for each post group.
+        get_input_name: give a name for each input group.
+
+    Examples:
+        when building the network:
+        self.connection1 = spaic.Connection(self.input, self.layer1, link_type='full')
 
         '''
 
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-
-Connection.register('pool', pool_connect)
-Connection.register('pool_connection', pool_connect)
-
-
-class sparse_connect_sparse(Connection):
-
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O',
-                 post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(sparse_connect_sparse, self).__init__(pre=pre, post=post, name=name,
-                                                    link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                                    sparse_with_mask=sparse_with_mask,
-                                                    pre_var_name=pre_var_name, post_var_name=post_var_name,
-                                                    syn_kwargs=syn_kwargs, **kwargs)
-        weight = kwargs.get('weight', None)
-        self.w_std = kwargs.get('w_std', 0.05)
-        self.density = kwargs.get('density', 0.1)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        # self.init = kwargs.get('init', None)
-        self.is_parameter = kwargs.get('is_parameter', False)
-        self.is_sparse = kwargs.get('is_sparse', True)
-        # self._variables = dict()
-
-        if weight is None:
-            # Connection weight
-            sparse_matrix = self.w_std * sp.rand(*self.shape, density=self.density, format='csr')
-            self.weight = sparse_matrix.toarray()
-        else:
-            if isinstance(weight, BaseInitializer):
-                self.w_init, self.w_init_param = self.decode_initializer(weight)
-                if self.w_init == 'sparse':
-                    self.weight = np.empty(self.shape)
-                else:
-                    raise ValueError('Sparse implementation of sparse_connection_sparse connection do not support '
-                                     'the %s initialization method', self.w_init)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-
-        self._variables['weight[link]'] = self.weight
-
-        bias = kwargs.get('bias', None)
-        if bias is None:
-            self.bias_flag = False
-        else:
-            self.bias_flag = True
-            if isinstance(bias, BaseInitializer):
-                self.b_init, self.b_init_param = self.decode_initializer(bias)
-                self.bias_value = np.empty(self.post_num)
-
-            else:
-                assert (bias.size == self.post_num), f"The size of the given bias {bias.shape} does not correspond" \
-                                                         f" to the size of post_num {self.post_num} "
-                self.bias_value = bias
-
-            self._variables['bias[link]'] = self.bias_value
+    _connection_subclasses = dict()
+    _class_label = '<con>'
 
-    def condition_check(self, pre_group, post_group):
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-        pass
-Connection.register('sparse_sparse', sparse_connect_sparse)
-Connection.register('sparse_connection_sparse', sparse_connect_sparse)
-
-
-class sparse_connect_mask(Connection):
-
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O',
-                 post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(sparse_connect_mask, self).__init__(pre=pre, post=post, name=name,
-                                                  link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                                  sparse_with_mask=sparse_with_mask,
-                                                  pre_var_name=pre_var_name, post_var_name=post_var_name,
-                                                  syn_kwargs=syn_kwargs, **kwargs)
-        weight = kwargs.get('weight', None)
-        self.w_std = kwargs.get('w_std', 0.05)
-        self.w_mean = kwargs.get('w_mean', 0.005)
-        self.density = kwargs.get('density', 0.1)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        # self.init = kwargs.get('init', None)
+    def __init__(self, pre: Assembly, post: Assembly, name=None,
+                 link_type=('full', 'sparse_connection', 'conv', '...'),
+                 syn_type=None, max_delay=0, sparse_with_mask=False, pre_var_name='O', post_var_name='Isyn',
+                 syn_kwargs=None, prefer_device=None, **kwargs):
+
+        super(Connection, self).__init__(pre, post)
+        # self.param_init = kwargs.get('param_init', None)
+        self.con_kwargs = kwargs
         self.is_parameter = kwargs.get('is_parameter', True)
         self.is_sparse = kwargs.get('is_sparse', False)
-        # self._variables = dict()
+        self.weight_quantization = kwargs.get('weight_quantization', False)
+        if syn_kwargs is None:
+            self.syn_kwargs = dict()
+        else:
+            self.syn_kwargs = syn_kwargs
+        # assert pre._is_terminal
+        # assert post._is_terminal
+        self.prefer_device = prefer_device
+        self.pre = pre  # .get_assemblies()
+        self.post = post  # .get_assemblies()
+        self.pre_var_name = pre_var_name
+        self.post_var_name = post_var_name
+
+        self.pre_num = pre.num
+        self.post_num = post.num
+        # self.link_num = self.pre_num * self.post_num
+        self.shape = (self.post_num, self.pre_num)
+
+        self.pre_groups = None  # pre.get_groups()
+        self.post_groups = None  # post.get_groups()
+        self.pre_assemblies = None
+        self.post_assemblies = None
+        self.connection_information = None
+        self.mask_info: List[(tuple, tuple)] = list()  # (var_code, op_code)
+
+        self.link_type = link_type
+        self.max_delay = max_delay
+        self.min_delay = kwargs.get('min_delay', 1.0)
+        self.sparse_with_mask = sparse_with_mask
+        self._var_names = list()
+        self._var_dict = dict()
+        self._supers = list()
+        self._link_var_codes = list()
+        # self._policies = policies
+        self._variables = dict()
+        self._operations = list()
+        self._init_operations = list()
+        # self._link_op_codes = list()
+        self.w_init = None
+        self.b_init = None
+        self.w_init_param = dict()
+        self.b_init_param = dict()
+
+        self.parameters = kwargs
+        # self.bias = kwargs.get('bias', False)
+
+        # self.updated_input = kwargs.get('updated_input', True)
+        self.weight_norm = kwargs.get('weight_norm', False)
+
+        self.w_max = None
+        self.w_min = None
+
+        self.set_name(name)
+        self.running_var = None
+        self.running_mean = None
+        self.decay = 0.9
+        self._variables = dict()
+        self._constant_variables = dict()
+
+        self.flatten = kwargs.get('flatten', False)
 
-        if weight is None:
-            # Connection weight
-            # sparse_matrix = self.w_std * sp.rand(*self.shape, density=self.density, format='csr')
-            # self.weight = sparse_matrix.toarray()
-            # self.weight[self.weight.nonzero()] = self.weight[self.weight.nonzero()] + self.w_mean
-            self.weight = self.w_std * np.random.rand(*self.shape) + self.w_mean
-            sparse_mask = np.less(np.random.rand(*self.shape), self.density)
-            self.weight = np.multiply(self.weight, sparse_mask)
-        else:
-            if isinstance(weight, BaseInitializer):
-                raise ValueError('Dense implementation of sparse_connection_mask do not support the %s initialization'
-                                 ' method', self.w_init)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-
-        self._variables['weight[link]'] = self.weight
-
-        bias = kwargs.get('bias', None)
-        if bias is None:
-            self.bias_flag = False
-        else:
-            self.bias_flag = True
-            if isinstance(bias, BaseInitializer):
-                self.b_init, self.b_init_param = self.decode_initializer(bias)
-                self.bias_value = np.empty(self.post_num)
+        # if len(syn_type) == 0:
+        #     raise ValueError('Please set the param syn_type, you can set it as \'basic\'')
 
-            else:
-                assert (bias.size == self.post_num), f"The size of the given bias {bias.shape} does not correspond" \
-                                                         f" to the size of post_num {self.post_num} "
-                self.bias_value = bias
-
-            self._variables['bias[link]'] = self.bias_value
-
-    def condition_check(self, pre_group, post_group):
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-        pass
-Connection.register('sparse', sparse_connect_mask)
-Connection.register('sparse_connection', sparse_connect_mask)
-
-
-class random_connect_sparse(Connection):
-
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O',
-                 post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(random_connect_sparse, self).__init__(pre=pre, post=post, name=name,
-                                                    link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                                    sparse_with_mask=sparse_with_mask,
-                                                    pre_var_name=pre_var_name, post_var_name=post_var_name,
-                                                    syn_kwargs=syn_kwargs, **kwargs)
-        weight = kwargs.get('weight', None)
-        self.probability = kwargs.get('probability', 0.1)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        # self.init = kwargs.get('init', None)
-        self.is_parameter = kwargs.get('is_parameter', False)
-        self.is_sparse = kwargs.get('is_sparse', True)
-        # self._variables = dict()
-
-        if weight is None:
-            # Link_parameters
-            prob_weight = np.random.rand(*self.shape)
-            diag_index = np.arange(min([self.pre_num, self.post_num]))
-            prob_weight[diag_index, diag_index] = 1
-            index = (prob_weight < self.probability)
-            # Connection weight
-            self.weight = np.zeros(self.shape)
-            self.weight[index] = prob_weight[index]
-        else:
-            if isinstance(weight, BaseInitializer):
-                self.w_init, self.w_init_param = self.decode_initializer(weight)
-                if self.w_init == 'sparse':
-                    self.weight = np.empty(self.shape)
-                else:
-                    raise ValueError('Sparse implementation of random_connect_sparse connection do not support '
-                                     'the %s initialization method', self.w_init)
-                self.weight = np.random.randn(*self.shape)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-
-        self._variables['weight[link]'] = self.weight
-
-        bias = kwargs.get('bias', None)
-        if bias is None:
-            self.bias_flag = False
-        else:
-            self.bias_flag = True
-            if isinstance(bias, BaseInitializer):
-                self.b_init, self.b_init_param = self.decode_initializer(bias)
-                self.bias_value = np.empty(self.post_num)
+        if isinstance(syn_type, list):
+            self.synapse_type = syn_type
+        else:
+            self.synapse_type = [syn_type]
+        self.synapse_name = []
+        self.synapse_class = []
 
+        for i in range(len(self.synapse_type)):
+            if isinstance(self.synapse_type[i], str):
+                self.synapse_class.append(SynapseModel.apply_model(self.synapse_type[i]))
+                self.synapse_name.append(self.synapse_type[i])  # self.model -> self.model_name
+                self.synapse = []
             else:
-                assert (bias.size == self.post_num), f"The size of the given bias {bias.shape} does not correspond" \
-                                                         f" to the size of post_num {self.post_num} "
-                self.bias_value = bias
+                raise ValueError("only support set synapse model with string")
 
-            self._variables['bias[link]'] = self.bias_value
+    def __new__(cls, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
+                syn_type=None, max_delay=0, sparse_with_mask=False, pre_var_name='O', post_var_name='Isyn',
+                syn_kwargs=None, **kwargs):
+        if cls is not Connection:
+            return super().__new__(cls)
 
-    def condition_check(self, pre_group, post_group):
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-        pass
-Connection.register('random_connection_sparse', random_connect_sparse)
+        if link_type in cls._connection_subclasses:
+            return cls._connection_subclasses[link_type](pre, post, name, link_type, syn_type,
+                                                         max_delay, sparse_with_mask, pre_var_name, post_var_name,
+                                                         syn_kwargs, **kwargs)
 
+        else:
+            raise ValueError("No connection type: %s in Connection classes" % link_type)
 
+    def get_var_names(self):
+        return self._var_names
 
-class random_connect_mask(Connection):
-
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O',
-                 post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(random_connect_mask, self).__init__(pre=pre, post=post, name=name,
-                                                  link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                                  sparse_with_mask=sparse_with_mask,
-                                                  pre_var_name=pre_var_name, post_var_name=post_var_name,
-                                                  syn_kwargs=syn_kwargs, **kwargs)
-        weight = kwargs.get('weight', None)
-        self.probability = kwargs.get('probability', 0.1)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        # self.init = kwargs.get('init', None)
-        self.is_parameter = kwargs.get('is_parameter', True)
-        self.is_sparse = kwargs.get('is_sparse', False)
-        # self._variables = dict()
-
-        if weight is None:
-            # Link_parameters
-            prob_weight = np.random.rand(*self.shape)
-            diag_index = np.arange(min([self.pre_num, self.post_num]))
-            prob_weight[diag_index, diag_index] = 1
-            index = (prob_weight < self.probability)
-            # Connection weight
-            self.weight = np.zeros(self.shape)
-            self.weight[index] = prob_weight[index]
-        else:
-            if isinstance(weight, BaseInitializer):
-                raise ValueError(
-                    'Dense implementation of random_connect_mask do not support the %s initialization method',
-                    self.w_init)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-
-        self._variables['weight[link]'] = self.weight
-
-        bias = kwargs.get('bias', None)
-        if bias is None:
-            self.bias_flag = False
-        else:
-            self.bias_flag = True
-            if isinstance(bias, BaseInitializer):
-                self.b_init, self.b_init_param = self.decode_initializer(bias)
-                self.bias_value = np.empty(self.post_num)
+    @staticmethod
+    def register(name, connection_class):
+        '''
+        Register a connection class. Registered connection classes can be referred to
+        # via their name.
+        Parameters
+        ----------
+        name : str
+            A short name for the state updater (e.g. `'full'`)
+        connection_class :
+            The subclass of Connection object, e.g. an `FullConnection`, 'ConvConnection'.
+        '''
 
-            else:
-                assert (bias.size == self.post_num), f"The size of the given bias {bias.shape} does not correspond" \
-                                                         f" to the size of post_num {self.post_num} "
-                self.bias_value = bias
+        # only deal with lower case names
+        name = name.lower()
+        if name in Connection._connection_subclasses:
+            raise ValueError(('A connection class with the name "%s" has already been registered') % name)
 
-            self._variables['bias[link]'] = self.bias_value
+        if not issubclass(connection_class, Connection):
+            raise ValueError(
+                ('Given model of type %s does not seem to be a valid ConnectionModel.' % str(type(connection_class))))
 
-    def condition_check(self, pre_group, post_group):
-        flag = False
-        pre_type = pre_group.type
-        post_type = post_group.type
-        if pre_type == post_type:
-            flag = True
-        return flag
-        pass
-Connection.register('random', random_connect_mask)
-Connection.register('random_connection', random_connect_mask)
+        Connection._connection_subclasses[name] = connection_class
 
+    def assembly_linked(self, assembly):
+        if (assembly is self.pre) or (assembly is self.post):
+            return True
+        else:
+            return False
 
-class NullConnection(Connection):
+    def replace_assembly(self, old_assembly, new_assembly):
+        if old_assembly is self.pre:
+            self.pre = new_assembly
+        elif old_assembly is self.post:
+            self.post = new_assembly
+        else:
+            raise ValueError("the old_assembly is not in the connnection")
 
-    '''
-    each neuron in the first layer is connected to each neuron in the second layer.
+    def add_super(self, assembly):
+        assert isinstance(assembly, Assembly) or isinstance(assembly, Projection), "the super is not Assembly"
+        self._supers.append(assembly)
 
-    Args:
-        pre(Assembly): The assembly which needs to be connected
-        post(Assembly): The assembly which needs to connect the pre
-        link_type(str): full
+    def del_super(self, assembly):
+        assert assembly in self._supers, "the assembly is not in supers"
+        self._supers.remove(assembly)
 
-    Methods:
-        unit_connect: define the basic connection information and add them to the connection_information.
-        condition_check: check whether the pre_group.type is equal to the post_group.type, only if they are equal, return flag=Ture.
+    def set_id(self):
+        if len(self._supers) == 0:
+            self.id = self.name + self.__class__._class_label
+        else:
+            super_ids = []
+            for super in self._supers:
+                if super.id is not None:
+                    super_ids.append(super.id)
+                else:
+                    super_ids.append(super.set_id())
 
-    '''
+            self.id = self.name + self.__class__._class_label
+            if len(super_ids) == 1:
+                self.id = super_ids[0] + '_' + self.id
+            else:
+                pre_id = '/'
+                for prefix in super_ids:
+                    pre_id += prefix + ','
+                pre_id += '/'
+                self.id = pre_id + '_' + self.id
+        return self.id
+
+    def get_str(self, level):
+
+        level_space = "" + '-' * level
+        repr_str = level_space + "|name:{}, type:{}, ".format(self.name, type(self).__name__)
+        repr_str += "pre:{}, ".format(self.pre.name)
+        repr_str += "post:{}\n ".format(self.post.name)
+        # for c in self._connections.values():
+        #     repr_str += c.get_str(level)
+        return repr_str
+
+    def set_delay(self, pre_group, post_group):
+        # TODO: add to unit_connections information after it changed to List[dict]
+
+        if self.max_delay > 0:
+            # print("set delay")
+            # pre_num = pre_group.num
+            # post_num = post_group.num
+            # shape = (post_num, pre_num)
+            delay_input_name, delay_output_name = self.get_delay_input_output(pre_group, post_group)
+
+            # add delay container
+            delay_queue = self._backend.add_delay(delay_input_name, self.max_delay)
+            delay_name = self.get_link_name(pre_group, post_group, 'delay')
+            # ONLY FOR TEST  ===============================
+            ini_delay = (self.max_delay-self.min_delay) * np.random.rand(*self.shape) + self.min_delay
+            # ==============================================
+            self.variable_to_backend(delay_name, self.shape, ini_delay, True)
+            self.variable_to_backend(delay_output_name, (1, *self.shape), 0)
+
+            # add delay index
+            self._backend.register_standalone(Op(delay_output_name, delay_queue.select, [delay_name] ,owner=self))
+
+            # add inital to transform initial delay_output
+            # self.init_op_to_backend(delay_output_name, delay_queue.transform_delay_output,
+            #                                [delay_input_name, delay_name])
+
+        else:
+            return
+
+    def clamp_weight(self, weight):
+        if not weight.is_sparse:
+            if (self.w_max is not None) and (self.w_min is not None):
+                self._backend.clamp_(weight, self.w_min, self.w_max)
+            elif self.w_max is not None:
+                self._backend.clamp_max_(weight, self.w_max)
+            elif self.w_min is not None:
+                self._backend.clamp_min_(weight, self.w_min)
+    def quantize_weight(self, weight):
+        return np.round(np.clip(weight + 2 ** 7, 0, 2 ** 8)) - 2 ** 7
+
+    def _add_label(self, var_name: str):
+        if '[pre]' in var_name:
+            var_name = var_name.replace("[pre]", "")
+            var_name = self.get_group_name(self.pre, var_name)
+        elif '[link]' in var_name:
+            var_name = var_name.replace("[link]", "")
+            var_name = self.get_link_name(self.pre, self.post, var_name)
+        elif '[post]' in var_name:
+            var_name = var_name.replace("[post]", "")
+            var_name = self.get_group_name(self.post, var_name)
+        elif '[input]' in var_name:
+            tmp_var_name = var_name.replace("[input]", "")
+            var_name = self.get_input_name(self.pre, self.post)
+            if tmp_var_name not in var_name:
+                raise ValueError(" the var_name tagged as [input] is not pre_var_name of the connection")
+        elif var_name[0] == '[' and var_name[-1] == ']':
+            var_name = var_name
+        else:
+            var_name = self.get_name(var_name)
+        return var_name
+
+    def add_conn_label(self, var_name: str):
+        if isinstance(var_name, str):
+            if '[updated]' in var_name:
+                var_name = var_name.replace("[updated]", "")
+                name = self._add_label(var_name)
+                return name + '[updated]'
+            else:
+                name = self._add_label(var_name)
+                return name
+
+        elif isinstance(var_name, list) or isinstance(var_name, tuple):
+            var_names = []
+            for name in var_name:
+                if isinstance(name, str):
+                    if '[updated]' in name:
+                        name = name.replace("[updated]", "")
+                        name = self._add_label(name)
+                        name = name + '[updated]'
+                    else:
+                        name = self._add_label(name)
+                    var_names.append(name)
+            return var_names
+
+    @property
+    def dt(self):
+        return self._backend.dt
+
+    def decode_syn_op(self, syn_ops, synapse_name, op_len):
+        if len(synapse_name) > 1:
+            for i in range(1, op_len):
+                pre_op_return_name = syn_ops[i-1][0]
+                post_op_first_input = syn_ops[i][2]
+                if '[updated]' in post_op_first_input:
+                    post_op_first_input = post_op_first_input.replace('[updated]', '')
+                if post_op_first_input == pre_op_return_name:
+                    temp_name = synapse_name[i-1]+'_' + str(i-1)
+                    syn_ops[i-1][0] = temp_name
+                    syn_ops[i][2] = temp_name
+        return syn_ops
+
+    def decode_initializer(self, initial):
+        init_name = initial.__class__.__name__
+        init_param = initial.__dict__
+        return init_name, init_param
 
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O',
-                 post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(NullConnection, self).__init__(pre=pre, post=post, name=name,
-                                             link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                             sparse_with_mask=sparse_with_mask,
-                                             pre_var_name=pre_var_name, post_var_name=post_var_name,
-                                             syn_kwargs=syn_kwargs, **kwargs)
+    def build(self, backend):
+        '''
+        add the connection variable, variable name and operation to the backend.
+        '''
 
-        pass
+        self._backend = backend
+        # Add weight
+        self.assigned_weight = False
+        self.assigned_bias = False
+        prefer_device=self.prefer_device if self.prefer_device != None else None
+
+        self.set_delay(self.pre, self.post)
 
-Connection.register('null', NullConnection)
 
-class Spike_to_Mass(Connection):
-    '''
-    Connect pre of spiking neurons to post of Neural Mass model
-    '''
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O',
-                 post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(Spike_to_Mass, self).__init__(pre=pre, post=post, name=name,
-                                            link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                            sparse_with_mask=sparse_with_mask,
-                                            pre_var_name=pre_var_name, post_var_name=post_var_name,
-                                            syn_kwargs=syn_kwargs, **kwargs)
-        weight = kwargs.get('weight', None)
-        bias = kwargs.get('bias', None)
-        self.tau_syn = kwargs.get('tau_syn', 6.0)
-        self.w_std = kwargs.get('w_std', 0.05)
-        self.w_mean = kwargs.get('w_mean', 0.005)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        self.is_parameter = kwargs.get('is_parameter', True)
-        self.shape = (post.num, 1)
-        self.synapse_class = []
+        for (key, value) in self._variables.items():
+            var_name = self.add_conn_label(key)
+            if isinstance(value, np.ndarray):
+                if value.size > 1:
+                    shape = value.shape
+                else:
+                    shape = ()
+            elif hasattr(value, '__iter__'):
+                value = np.array(value)
+                if value.size > 1:
+                    shape = value.shape
+                else:
+                    shape = ()
+            else:
+                shape = ()
 
+            if 'weight' in key:
+                if self.assigned_weight is False:
+                    self.assigned_weight = True
+                else:
+                    raise ValueError("connection have multiple weight variable")
+                if self.weight_quantization:
+                    value = self.quantize_weight(value)
+                self.weight = self.variable_to_backend(name=var_name, shape=self.shape, value=value, is_parameter=self.is_parameter,
+                                         is_sparse=self.is_sparse, init=self.w_init, init_param=self.w_init_param, prefer_device=prefer_device)  # (var_name, shape, value, is_parameter, is_sparse, init)
+            elif 'bias' in key:
+                if self.assigned_bias is False:
+                    self.assigned_bias = True
+                else:
+                    raise ValueError("connection have multiple bias variable")
+                self.bias = self.variable_to_backend(name=var_name, shape=value.shape, value=value, is_parameter=self.is_parameter,
+                                         init=self.b_init, init_param=self.b_init_param, prefer_device=prefer_device)
+            elif hasattr(value, 'requires_grad'):
+                self.variable_to_backend(var_name, shape=value.shape, value=value, is_parameter=value.requires_grad,
+                                         prefer_device=prefer_device)
+            else:
+                self.variable_to_backend(var_name, shape, value=value, prefer_device=prefer_device)
+            # self._var_names.append(var_name)
+            # self._var_dict[var_name] = VariableAgent(backend, var_name)
+
+        for (key, value) in self._constant_variables.items():
+            var_name = self.add_conn_label(key)
+            self.variable_to_backend(name=var_name, shape=None, value=value, is_constant=True, prefer_device=prefer_device)
+
+        weight_name = self.get_link_name(self.pre, self.post, 'weight')
+        if self.sparse_with_mask:
+            mask = (self.weight != 0)
+            mask_name = self.get_link_name(self.pre, self.post, 'mask')
+            self.variable_to_backend(mask_name, self.shape, mask, prefer_device=prefer_device)
+            self.init_op_to_backend(weight_name, self.mask_operation, [weight_name, mask_name], prefer_device)
+            # del self.sparse_with_mask
+
+        # del self.weight
+        if (self.w_min is not None) or (self.w_max is not None):
+            self.init_op_to_backend(None, self.clamp_weight, [weight_name], prefer_device)
+
+        # TODO: 这里input 和 output的 name 默认没有加label,同时都加上conn的label是不是过于局限了？
+        for op in self._operations:
+            addcode_op = Op(owner=self)
+            addcode_op.func_name = op[1]
+            addcode_op.output = self.add_conn_label(op[0])
+            if len(op) > 3:  # 为了解决历史的单一list格式的问题
+                addcode_op.input = self.add_conn_label(op[2:])
+            else:
+                addcode_op.input = self.add_conn_label(op[2])
+            addcode_op.place = prefer_device
+            # if len(op) > 3:
+            #     addcode_op[2] = addcode_op[2:]
+            #     addcode_op = addcode_op[:3]
+            backend.add_operation(addcode_op)
+
+        for op in self._init_operations:
+            addcode_op = []
+            for ind, name in enumerate(op):
+                if ind != 1:
+                    addcode_op.append(self.add_conn_label(op[ind]))
+                else:
+                    addcode_op.append(op[ind])
+            if len(op) > 3:
+                addcode_op[2] = addcode_op[2:]
+                addcode_op = addcode_op[:3]
+
+            self.init_op_to_backend(addcode_op[0], addcode_op[1], addcode_op[2], self.prefer_device)
+
+        # the initialzation of synapse with forward_build kwarg can be read
+        if backend.forward_build:
+            self.updated_input = True
+        else:
+            self.updated_input = False
+        syn_ops = []
+        for i in range(len(self.synapse_class)):
+            if self.synapse_class[i] is not None:
+                self.synapse.append(self.synapse_class[i](self, **self.syn_kwargs))
+
+            for (key, value) in self.synapse[i]._syn_variables.items():
+                key = self.add_conn_label(key)
+                self.variable_to_backend(key, value.shape, value=value)
+
+            for (key, value) in self.synapse[i]._syn_constant_variables.items():
+                key = self.add_conn_label(key)
+                self.variable_to_backend(key, shape=None, value=value, is_constant=True)
+            dt = backend.dt
+            for (key, value) in self.synapse[i]._syn_tau_variables.items():
+                key = self.add_conn_label(key)
+                tau_value = np.exp(-dt / value)
+                # 暂时只考虑scalar值
+                self.variable_to_backend(key, shape=[1, ], value=tau_value)
+            for op in self.synapse[i]._syn_operations:
+                syn_ops.append(op)
+
+        #toDO: make sure synapse with multiple ops
+        # if 'basic' in self.synapse_name:
+        syn_ops = self.decode_syn_op(syn_ops, self.synapse_name, len(syn_ops))
+
+        for sop in syn_ops:
+            addcode_op = Op(owner=self)
+            addcode_op.func_name = sop[1]
+            addcode_op.output = self.add_conn_label(sop[0])
+            if len(sop) > 3:  # 为了解决历史的单一list格式的问题
+                addcode_op.input = self.add_conn_label(sop[2:])
+            else:
+                addcode_op.input = self.add_conn_label(sop[2])
+            addcode_op.place = prefer_device
+            backend.add_operation(addcode_op)
 
-        if weight is None:
-            # Connection weight
-            self.weight = self.w_std * np.random.randn(*self.shape) + self.w_mean
-        else:
-            if isinstance(weight, BaseInitializer):
-                self.w_init, self.w_init_param = self.decode_initializer(weight)
-                self.weight = np.empty(self.shape)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
+    @abstractmethod
+    def condition_check(self, pre_group, post_group):
+        NotImplemented()
 
-        self._variables['weight[link]'] = self.weight
-        self._variables['beta[link]'] = np.exp(-0.1/self.tau_syn)
-        self._variables['rate[link]'] = 0.0
-        self._operations.append(['rate[link]', self.spike_to_rate, [pre_var_name+'[pre]', 'rate[link]', 'beta[link]']])
-        self._operations.append([self.post_var_name+'[post]', 'mat_mult_weight', 'rate[link][updated]', 'weight[link]'])
+    def mask_operation(self, weight, mask):
+        return weight * mask
 
+    def get_name(self, suffix_name: str):
+        '''
 
-    def spike_to_rate(self, spikes, last_rate, beta):
-        rate = beta*last_rate + torch.mean(spikes, dim=1, keepdim=True)
-        return rate
+        Args:
+            pre_group(Assembly): the neuron group which needs to be connected
+            post_group(Assembly): the neuron group which needs to connect with the pre_group
+            suffix_name(str): represents the name of the object you want to retrieve, such as 'weight'
+        Returns:
+            name(str)
+        '''
 
-Connection.register('spike2mass', Spike_to_Mass)
+        name = self.id + ':' + '{' + suffix_name + '}'
+        return name
 
-class Mass_to_Spike(Connection):
-    '''
-    Connect pre of spiking neurons to post of Neural Mass model
-    '''
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O',
-                 post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(Mass_to_Spike, self).__init__(pre=pre, post=post, name=name,
-                                            link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                            sparse_with_mask=sparse_with_mask,
-                                            pre_var_name=pre_var_name, post_var_name=post_var_name,
-                                            syn_kwargs=syn_kwargs, **kwargs)
-        weight = kwargs.get('weight', None)
-        bias = kwargs.get('bias', None)
-        self.tau_syn = kwargs.get('tau_syn', 6.0)
-        self.w_std = kwargs.get('w_std', 0.05)
-        self.w_mean = kwargs.get('w_mean', 0.005)
-        self.w_max = kwargs.get('w_max', None)
-        self.w_min = kwargs.get('w_min', None)
-        self.is_parameter = kwargs.get('is_parameter', True)
-        self.shape = (post.num, pre.num)
-        self.synapse_class = []
-        self.unit_conversion = kwargs.get('unit_conversion', 1.0)
+    def get_link_name(self, pre_group: Assembly, post_group: Assembly, suffix_name: str):
+        '''
 
+        Args:
+            pre_group(Assembly): the neuron group which needs to be connected
+            post_group(Assembly): the neuron group which needs to connect with the pre_group
+            suffix_name(str): represents the name of the object you want to retrieve, such as 'weight'
+        Returns:
+            name(str)
+        '''
 
-        if weight is None:
-            # Connection weight
-            self.weight = self.w_std * np.random.randn(*self.shape) + self.w_mean
-        else:
-            if isinstance(weight, BaseInitializer):
-                self.w_init, self.w_init_param = self.decode_initializer(weight)
-                self.weight = np.empty(self.shape)
-            else:
-                assert (weight.shape == self.shape), f"The size of the given weight {weight.shape} does not correspond" \
-                                                     f" to the size of synaptic matrix {self.shape} "
-                self.weight = weight
-
-        self._variables['weight[link]'] = self.weight
-        self._variables['beta[link]'] = np.exp(-0.1/self.tau_syn)
-        self._variables['rate[link]'] = 0.0
-
-        self._operations.append([post_var_name+'[post]', self.rate_to_Isyn, [pre_var_name+'[pre]', 'weight[link]']])
-
-
-
-    def rate_to_Isyn(self, rate, weight):
-        rate = rate.view(rate.shape[0], 1, self.pre.num).expand(rate.shape[0],
-                                                                self.post.num, self.pre.num)
-        spikes = torch.rand_like(rate).le(rate * self.unit_conversion * self.dt).type(self._backend.data_type)
-        Isyn = torch.sum(spikes*weight, dim=-1)
-        return Isyn
-Connection.register('mass2spike', Mass_to_Spike)
-
-class DistDepd_connect(Connection):
-
-    def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connection', 'conv', '...'),
-                 syn_type=['basic'], max_delay=0, sparse_with_mask=False, pre_var_name='O',
-                 post_var_name='Isyn', syn_kwargs=None, **kwargs):
-        super(DistDepd_connect, self).__init__(pre=pre, post=post, name=name,
-                                               link_type=link_type, syn_type=syn_type, max_delay=max_delay,
-                                               sparse_with_mask=sparse_with_mask,
-                                               pre_var_name=pre_var_name, post_var_name=post_var_name,
-                                               syn_kwargs=syn_kwargs, **kwargs)
-        self.distance_weight_function = kwargs.get('distance_weight_function', None)
-        self.zero_self = kwargs.get('zero_self', False)
-        if self.distance_weight_function is None:
-            self.distance_weight_function = self.default_dist_weight_function
-        self.dist_function = kwargs.get('dist_function', 'euclidean')
-        if self.dist_function == 'euclidean':
-            self.dist_function = self.euclidean_dist_function
-        elif self.dist_function == 'circular':
-            self.dist_function = self.circular_dist_function
-
-        self.dist_a = kwargs.get('dist_a', 0.2)
-        self.dist_b = kwargs.get('dist_b', 0.4)
-        self.w_amp = kwargs.get('w_amp', -0.1)
-        self.pos_range = kwargs.get('pos_range', 1.0)
-        self.p = kwargs.get('p', 1.0)
-
-        # building the weight
-        pre_num = pre.num
-        post_num = post.num
-        assert len(pre.position) > 0
-        assert len(post.position) > 0
-
-        post_pos = np.expand_dims(post.position, axis=1)
-        pre_pos = np.expand_dims(pre.position, axis=0)
-        weight = self.distance_weight_function(self.dist_function(pre_pos, post_pos))
-        if self.p < 1.0:
-            rand_mask = torch.rand_like(weight).lt(self.p)
-            weight = weight*rand_mask
-        self._variables['weight[link]'] = weight
+        name = self.id + ':' + post_group.id + '<-' + pre_group.id + ':' + '{' + suffix_name + '}'
+        return name
 
+    def get_group_name(self, group: Assembly, suffix_name: str):
+        '''
+        Args:
+            group(Assembly): the neuron group which needs to be connected
+            suffix_name(str): represents the name of the object you want to retrieve, such as 'O'
 
+        Returns:
+            name(str)
+        '''
+        name = group.id + ':' + '{' + suffix_name + '}'
+        return name
 
+    # def get_post_name(self, post_group: Assembly, suffix_name: str):
+    #     '''
+    #     Args:
+    #         post_group(Assembly): the neuron group which needs to connect with the pre_group
+    #         suffix_name(str): represents the name of the object you want to retrieve, such as 'maxpool_kernel_size'
+    #
+    #     Returns:
+    #         name(str)
+    #     '''
+    #     name = post_group.id + ':' + '{' + suffix_name + '}'
+    #     return name
+
+    # def get_mask_name(self, pre_group: Assembly, post_group: Assembly):
+    #     name = self.id + ':' + post_group.id + '<-' + pre_group.id + ':' + '{mask}'
+    #     return name
+    #
+    # def get_delay_name(self, pre_group: Assembly, post_group: Assembly):
+    #     name = self.id + ':' + post_group.id + '<-' + pre_group.id + ':' + '{delay}'
+    #     return name
+
+    # 这两个特例应该要留着
+    def get_delay_input_output(self, pre_group: Assembly, post_group: Assembly):
+        input_name = pre_group.id + ':' + '{' + self.pre_var_name + '}'
+        output_name = self.id + ':' + post_group.id + '<-' + pre_group.id + ':' + '{' + self.pre_var_name + '}'
+        return input_name, output_name
 
+    def get_input_name(self, pre_group: Assembly, post_group: Assembly):
+        '''
+        Give a name for input group's output spikes,  the name consists of two parts: pre_group.id + ':' + '{0}
+        Args:
+            pre_group(Assembly): The neuron group which need to connect with post_group neuron.
+            post_group(Assembly): the neuron group which needs to connect with the pre_group
+        Returns:
+            name(str)
+        '''
+        if self.max_delay > 0:
+            name = self.id + ':' + post_group.id + '<-' + pre_group.id + ':' + '{' + self.pre_var_name + '}'
+        else:
+            name = pre_group.id + ':' + '{' + self.pre_var_name + '}'
+        return name
 
-    def unit_connect(self, pre_group, post_group):
-        # The number of neurons in neuron group
-        pre_num = pre_group.num
-        post_num = post_group.num
-        assert len(pre_group.position) > 0
-        assert len(post_group.position) > 0
-        link_num = pre_num * post_num
-        shape = (post_num, pre_num)
-        weight = np.zeros(shape)
-        post_pos = np.expand_dims(post_group.position,  axis=1)
-        pre_pos = np.expand_dims(pre_group.position, axis=0)
-        weight = self.distance_weight_function(self.dist_function(pre_pos, post_pos))
-        # from matplotlib import pyplot as plt
-        # plt.imshow(weight)
-        # plt.show()
-
-        # The name for backend variables
-        input_name = self.get_input_name(pre_group, post_group)
-        weight_name = self.get_weight_name(pre_group, post_group)
-        target_name = self.get_target_name(post_group)
-
-        # The backend variable
-        var_code = (weight_name, shape, weight, True, False) # (var_name, shape, value, is_parameter, is_sparse, init)
-        op_code = [target_name, 'mat_mult', input_name, weight_name]
-        connection_information = (pre_group, post_group, link_num, var_code, op_code)
-        self.unit_connections.append(connection_information)
-
-    def circular_dist_function(self, pre_pos, post_pos):
-        if not isinstance(pre_pos, torch.Tensor):
-            pre_pos = torch.tensor(pre_pos)
-        if not  isinstance(post_pos, torch.Tensor):
-            post_pos = torch.tensor(post_pos)
-
-        z = torch.maximum(pre_pos, post_pos)
-        k = torch.minimum(pre_pos, post_pos)
-        dist = torch.minimum(z - k, self.pos_range + k - z)
-        dist = torch.norm(dist, p=2, dim=-1)
-        return dist
-
-    def euclidean_dist_function(self, pre_pos, post_pos):
-        if isinstance(pre_pos, torch.Tensor) and isinstance(post_pos, torch.Tensor):
-            diff = pre_pos - post_pos
-        else:
-            diff = torch.tensor(pre_pos-post_pos)
-        dist = torch.norm(diff, p=2, dim=-1)
-        return dist
-
-    def default_dist_weight_function(self, dist):
-        weights = self.w_amp * (torch.exp(-dist / self.dist_a)/self.dist_a - 0.5*torch.exp(-dist / self.dist_b)/self.dist_b)
-        if self.zero_self:
-            weights = weights * (dist!=0).type(self._backend.data_type)
-        # import matplotlib.pyplot as plt
-        # plt.imshow(weights, aspect='auto')
-        # plt.show()
-        return weights
-Connection.register('dist_depd', DistDepd_connect)
-
-# class reconnect(Connection):
-#     def __init__(self, pre, post, name=None, link_type=('full', 'sparse_connect', 'conv', '...'), policies=[],
-#                  max_delay=0, sparse_with_mask=False, pre_var_name='O', post_var_name='Isyn', syn_kwargs=None, **kwargs):
-#         super(reconnect, self).__init__(pre=pre, post=post, name=name, link_type=link_type,
-#                                              policies=policies, max_delay=max_delay, sparse_with_mask=sparse_with_mask, pre_var_name=pre_var_name, post_var_name=post_var_name,syn_kwargs=syn_kwargs, **kwargs)
-#     def unit_connect(self, pre_group, post_group):
-#         pass
-#
-#     def condition_check(self, pre_group, post_group):
-#         pass
+    def get_target_output_name(self, output_group: Assembly):
+        name = output_group.id + ':' + '{' + self.pre_var_name + '}'
+        return name
+
+    # def Chemistry_Isyn(self):
+    #     """
+    #     Chemistry current synapse
+    #     I = tauP*I + WgtSum
+    #     """
+    #     I = self.get_post_name(self.post, 'I')
+    #     WgtSum = self.get_post_name(self.post, 'WgtSum')
+    #     tauP = self.get_post_name(self.post, 'tauP')
+    #     # I = self.get_I_ele_name(self.post)
+    #     # WgtSum = self.get_target_name(self.post)
+    #     # tauP = self.post.id + ':' + '{tauP}'
+    #     self._syn_variables[I] = 0
+    #     self._syn_variables[WgtSum] = 0
+    #     self._syn_tau_constant_variables[tauP] = self.tau_p
+    #
+    #     self._syn_operations.append([I, 'var_linear', tauP, I, WgtSum])
+
+    # def Electrical_synapse(self):
+    #     """
+    #     Electrical synapse
+    #     WgtSum = weight *（V(l-1) - V(l)）
+    #     """
+    #     V_post = self.get_post_name(self.post, 'V')
+    #     V_pre = self.get_pre_name(self.post, 'V')
+    #     Vtemp1_post = self.get_link_name(self.pre, self.post, 'Vtemp')
+    #     I_post = self.get_post_name(self.post, 'I')
+    #     weight = self.get_link_name(self.pre, self.post, 'weight')
+    #     Vtemp1_pre = self.get_link_name(self.post, self.pre, 'Vtemp')
+    #     I_pre = self.get_pre_name(self.post, 'I_ele')
+    #     # V_post = self.get_V_name(self.post)
+    #     # V_pre = self.get_V_name(self.pre)
+    #     # Vtemp1_post = self.get_Vtemp_name(self.pre, self.post)
+    #     # I_post = self.get_I_ele_name(self.post)
+    #     # weight = self.get_weight_name(self.pre, self.post)
+    #     # Vtemp1_pre = self.get_Vtemp_name(self.post, self.pre)
+    #     # I_pre = self.get_I_ele_name(self.pre)
+    #
+    #     self._syn_variables[Vtemp1_post] = 0
+    #     self._syn_variables[I_post] = 0
+    #     self._syn_variables[Vtemp1_pre] = 0
+    #     self._syn_variables[I_pre] = 0
+    #     self._syn_operations.append([Vtemp1_post, 'minus', V_pre, V_post])
+    #     self._syn_operations.append([I_post, 'var_mult', weight, Vtemp1_post + '[updated]'])
+    #     self._syn_operations.append([Vtemp1_pre, 'minus', V_post, V_pre])
+    #     self._syn_operations.append([I_pre, 'var_mult', weight, Vtemp1_pre + '[updated]'])
+
+
+class ConnectPolicy():
+
+    def __init__(self, level=-1):
+        super(ConnectPolicy, self).__init__()
+        self.level = level
+        self.policies = [self, ]
+
+    @abstractmethod
+    def checked_connection(self, new_connection: Projection):
+        NotImplementedError()
+
+    def extend_policy(self, policies):
+        self.policies.extend(policies)
+
+    def __and__(self, other):
+        self.extend_policy(other.policies)
+        return self
+
+    def generate_connection(self, pre: Assembly, post: Assembly):
+
+        candidates = []
+        for p in self.policies:
+            candidates.append(p.checked_connection(Projection(pre, post)))
+        res = candidates[-1]
+        candidates.pop()
+        for con in candidates:
+            res = res & con
+        return res
```

### Comparing `SPAIC-0.6.1a0/spaic/Network/Construct.py` & `SPAIC-0.6.2.0.0/spaic/Network/Construct.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @project: SPAIC
 @filename: WithBuildFuncs
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 
 @description: 
 """
-from ..Network.Assembly import Assembly
+from spaic.Network.Assembly import Assembly
 import spaic
 
 # ================= Assembly Functions used in with ==========================
 
 def add_assembly(name, assembly):
     context = spaic.global_assembly_context_list
     assert len(context) >0, "use global assembly build functions outside of the 'with' context"
```

### Comparing `SPAIC-0.6.1a0/spaic/Network/DelayQueue.py` & `SPAIC-0.6.2.0.0/spaic/Network/DelayQueue.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,25 +72,26 @@
         NotImplementedError()
 
 
 class TorchDelayQueue(DelayQueue):
 
     def __init__(self,var_name, max_len, backend):
         super(TorchDelayQueue, self).__init__(var_name, max_len, backend)
-        self.device = backend.device
+        self.device = backend.device0
         self._backend = backend
 
 
 
-    def initial(self, var=None):
+    def initial(self, var=None, batch_size=1):
         self.count = 0
         # self.queue = None #torch.zeros(queue_shape, device=self.device)
-        self.var_shape = var.shape
-        queue_shape = [self.max_len] + list(self.var_shape)
-        self.queue = torch.zeros(queue_shape, device=self.device)
+        self.var_shape = list(var.shape)
+        self.var_shape[0] = batch_size
+        queue_shape = [self.max_len] + self.var_shape
+        self.queue = torch.zeros(queue_shape, device=self.device, dtype=var.dtype)
 
     def transform_delay_output(self, input, delay):
         if input.dim() == 2:
             output = input.unsqueeze(-1).expand(-1, -1, delay.shape[0])
         else:
             output = input.unsqueeze(-1).expand(-1, -1, -1, delay.shape[0])
         return output
@@ -98,37 +99,47 @@
 
     def push(self, input):
         # if self.queue is None:
         #     self.var_shape = input.shape
         #     queue_shape = [self.max_len] + list(self.var_shape)
         #     self.queue = torch.zeros(queue_shape, device=self.device)
 
-        self.queue[self.count, ...] = input
+        if input.requires_grad:
+            self.queue = torch.cat([self.queue[:self.count], input.unsqueeze(0), self.queue[self.count + 1:]], dim=0)
+        else:
+            self.queue[self.count, ...] = input
+
         self.count += 1
         self.count = self.count % self.max_len
 
         return input
 
 
     def select(self, delay: torch.Tensor):
         # Only for one-dim neurongroup for now
         delay = delay.clip(0, self.max_len*self.dt)
         if self.queue.dim() == delay.dim()+1:
-            delay = delay.unsqueeze(1).expand(-1, self.var_shape[0], -1)
+            delay = delay.unsqueeze(1).expand(-1, self.var_shape[0], -1)  # (post_num, batch)
             ind = (delay/self.dt).long()
             ind = torch.fmod(self.max_len-ind + self.count, self.max_len)
-            output = torch.gather(self.queue, 0, ind).permute(1,2,0)
+            output = torch.gather(self.queue, 0, ind).permute(1, 0, 2)
 
         elif self.queue.dim() == delay.dim()+2:
             delay = delay.unsqueeze(1).unsqueeze(1).expand(-1,self.var_shape[0], 2, -1)
             ind = (delay / self.dt).long()
             ind = torch.fmod(self.max_len-ind + self.count+1, self.max_len)
             output = torch.gather(self.queue, 0, ind)
             output[:, :, 1, :] -= (delay - ind*self.dt)[:, :, 1, :]/10.0
-            output = output.permute(1,2,3,0)
+            output = output.permute(1, 0, 2, 3)
+        elif self.queue.dim() == delay.dim():
+            delay = delay.expand(-1, self.var_shape[0], -1)
+            ind = (delay / self.dt).long()
+            ind = torch.fmod(self.max_len - ind + self.count, self.max_len)
+            output = torch.gather(self.queue, 0, ind).permute(1, 0, 2)
+
 
         return output
 
 
 DelayQueue.register('pytorch', TorchDelayQueue)
```

### Comparing `SPAIC-0.6.1a0/spaic/Network/Network.py` & `SPAIC-0.6.2.0.0/spaic/Network/Network.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,47 +11,60 @@
 执行过程：网络定义->网络生成->网络仿真与学习
 """
 from spaic.Network.Assembly import Assembly
 # from spaic.Network.Topology import Connection
 from collections import OrderedDict
 from warnings import warn
 import spaic
-# from ..Backend.Backend import Op
+from spaic.utils.memory import get_tens_mem
+from multiprocessing.pool import ThreadPool as Pool
+
+try:
+    import torch
+except:
+    pass
 
-class Network(Assembly):
 
+class Network(Assembly):
     _class_label = '<net>'
+
     def __init__(self, name=None):
 
         super(Network, self).__init__(name=name)
         self._monitors = OrderedDict()
         self._learners = OrderedDict()
         self._pipline = None
         self._backend: spaic.Backend = None
+        self._forward_build = False
         pass
 
     # --------- Frontend code ----------
-    def set_backend(self, backend=None, device='cpu'):
+    def set_backend(self, backend=None, device='cpu', partition=False):
+        if isinstance(device, str):
+            device = [device]
         if backend is None:
             self._backend = spaic.Torch_Backend(device)
+            self._backend.partition = partition
         elif isinstance(backend, spaic.Backend):
             self._backend = backend
         elif isinstance(backend, str):
-            if backend == 'torch' or backend =='pytorch':
+            if backend == 'torch' or backend == 'pytorch':
                 self._backend = spaic.Torch_Backend(device)
+                self._backend.partition = partition
             elif backend == 'tensorflow':
                 self._backend = spaic.Tensorflow_Backend(device)
 
-    def set_backend_dt(self, dt=0.1):
+    def set_backend_dt(self, dt=0.1, partition=False):
         if self._backend is None:
             warn("have not set backend, default pytorch backend is set automatically")
             self._backend = spaic.Torch_Backend('cpu')
             self._backend.dt = dt
         else:
             self._backend.dt = dt
+            self._backend.partition = partition
 
     def set_random_seed(self, seed):
         if isinstance(self._backend, spaic.Torch_Backend):
             import torch
             torch.random.manual_seed(int(seed))
             if self._backend.device == 'cuda':
                 torch.cuda.manual_seed(int(seed))
@@ -64,151 +77,189 @@
 
     def add_learner(self, name, learner):
         assert isinstance(learner, spaic.Learner)
         self.__setattr__(name, learner)
 
     # TODO: 这里的setattr是否有必要要，是否可以全部放到Assembly里？
     def __setattr__(self, name, value):
-        from ..Monitor.Monitor import Monitor
-        from ..Learning.Learner import Learner
+        from spaic.Monitor.Monitor import Monitor
+        from spaic.Learning.Learner import Learner
         super(Network, self).__setattr__(name, value)
         if isinstance(value, Monitor):
             self._monitors[name] = value
 
         elif isinstance(value, Learner):
             self._learners[name] = value
 
     # ---------  backend code  ----------
 
-    def build(self, backend=None, strategy=0):
+    def build(self, backend=None, strategy=0, full_enable_grad=None, device=None):
+        if full_enable_grad is not None:
+            self.enable_full_grad(full_enable_grad)
         if self._backend is None:
             if backend is not None:
-                self.set_backend(backend)
+                if device is not None:
+                    self.set_backend(backend, device)
+                else:
+                    self.set_backend(backend)
             else:
-                self.set_backend()
+                if device is not None:
+                    self.set_backend(device=device)
+                else:
+                    self.set_backend()
 
         self._backend.clear_step()
 
         # build 试运行时，假设一个runtime
         if self._backend.runtime is None:
-            self._backend.runtime = 10*self._backend.dt
+            self._backend.runtime = 10 * self._backend.dt
 
         all_groups = self.get_groups()
         for asb in all_groups:
             asb.set_id()
 
         self.build_projections(self._backend)
 
         all_connections = self.get_connections()
 
+        # for debug
+        con_debug = False
+        con_syn_count = 0
 
         for con in all_connections:
             con.set_id()
 
-            #----根据连接，对每个神经元建立input_connection和output_connection
+            # ----根据连接，对每个神经元建立input_connection和output_connection
             con.pre.register_connection(con, True)
             con.post.register_connection(con, False)
 
-
         if strategy == 1:
             # 采取单纯的从头递归地build，一旦出现环路会陷入死循环，可以避开固有延迟的问题,
             # Use directly build strategy to avoid inherent delay. But cannot be used on models with loop, will fall in an endless loop.
             # Unfortunately,
             self.forward_build(all_groups, all_connections)
+            self._backend.forward_build = True
         # elif strategy == 2:
         #     # 采取策略性构建，但是目前存在两个问题：
         #     #   1. 网络中存在Assembly块时会出现bug，尚未修复
         #     #   2. Connection所使用的input_spike为上一步的，需要添加[updated]，目前暂不使用所以未添加
         #     #   该构建方式可以较大程度上避开固有延迟的问题
         #     self.strategy_build(self.get_groups(False))
         else:
             # 原本的构建方式，首先构建连接，每个连接都是用上一轮神经元的输出脉冲，从而存在固有延迟的问题
             # 但是可以避开环路的问题。
-            for connection in all_connections:
-                connection.build(self._backend)
+            self._backend.forward_build = False
+            def build_fn(module):
+                # if con_debug:
+                #     con_syn_count += torch.count_nonzero(connection.weight.value).item()
+                module.build(self._backend)
+
+            # for connection in all_connections:
+            #     connection.build(self._backend)
+            #     if con_debug:
+            #         import torch
+            #         con_syn_count += torch.count_nonzero(connection.weight.value).item()
+
+            # for group in all_groups:
+            #     group.build(self._backend)    
+            pool = Pool(4)
+            pool.map(build_fn, all_connections)
+            pool.close()
+            pool.join()
+            pool = Pool(4)
+            pool.map(build_fn, all_groups)
+            pool.close()
+            pool.join()
 
-            for group in all_groups:
-                group.build(self._backend)
+        for learner in self._learners.values():
+            learner.set_id()
+            learner.build(self._backend)
 
         for monitor in self._monitors.values():
             monitor.build(self._backend)
 
-        for learner in self._learners.values():
-            learner.build(self._backend)
-
         self._backend.build_graph()
         # self._backend.build()
         self._backend.builded = True
-
-
+        # if con_debug:
+        #     print("Connection synapses count:%d"%con_syn_count)
 
         # for group in all_groups:
         #     if hasattr(group, 'index'):
         #         group.index = 0
 
         pass
 
     def forward_build(self, all_groups=None, all_connections=None):
         builded_groups = []
         builded_connections = []
-        for group in all_groups:
-            # if '_node_sub_class' in dir(group):
-            #     if group._node_sub_class == '<encoder>' or (group._node_sub_class) == '<generator>':
-            if (group._class_label == '<nod>') and ('predict' not in dir(group)):
-                group.build(self._backend)
-                builded_groups.append(group)
-                all_groups.remove(group)
-        break_tag = 0
-        crash_tag = 100
-        while all_groups or all_connections:
-            old_all_connections = all_connections.copy()
-            old_all_groups = all_groups.copy()
-            if break_tag > crash_tag:
-                raise Warning('May be stuck in an infinite building loop.')
-                keep_build = str(input('continue?(Y or N)'))
-                if keep_build.lower() == 'y':
-                    break_tag = 0
-                    crash_tag += 100
-                    continue
-                break
-            for conn in old_all_connections:
-                if conn.pre_assembly in builded_groups: # 如果连接的突触前神经元已经build，则可以build
-                    conn.build(self._backend)
-                    builded_connections.append(conn)
-                    all_connections.remove(conn)
-                    break_tag = 0
-                    continue
-            break_tag += 1
-            for group in old_all_groups:
-                can_build = 1
-                if not all_connections:
+        nod_groups = []
+        for group in all_groups.copy():
+            if group._class_label == '<nod>':
+                if (group._node_sub_class == '<encoder>') or (group._node_sub_class == '<generator>'):
                     group.build(self._backend)
                     builded_groups.append(group)
                     all_groups.remove(group)
-                    break_tag = 0
-                    continue
+                    for conn in group._output_connections:
+                        self.deep_forward_build(conn, all_groups, all_connections, builded_groups, builded_connections)
+                    for module in group._output_modules:
+                        self.deep_forward_build(module, all_groups, all_connections, builded_groups,
+                                                builded_connections)
                 else:
-                    for conn in all_connections:
-                        if group == conn.post_assembly:
-                            can_build = 0
-                            break
-                    if can_build:
-                        group.build(self._backend)
-                        builded_groups.append(group)
-                        all_groups.remove(group)
-                        break_tag = 0
-                        continue
-            break_tag += 1
-    #
+                    all_groups.remove(group)
+                    nod_groups.append(group)
+
+        while all_groups or all_connections:
+            for group in all_groups:
+                self.deep_forward_build(group, all_groups, all_connections, builded_groups, builded_connections)
+            for conn in all_connections:
+                self.deep_forward_build(conn, all_groups, all_connections, builded_groups, builded_connections)
+
+        for group in nod_groups:
+            group.build(self._backend)
+            builded_groups.append(group)
+
+    def deep_forward_build(self, target, all_groups, all_connections, builded_groups, builded_connections):
+        if (target in builded_groups) or (target in builded_connections):
+            return
+        if target._class_label == '<con>':
+            pre = [target.pre]
+            post = [target.post]
+        elif target._class_label == '<neg>':
+            pre = target._input_connections + target._input_modules
+            post = target._output_connections + target._output_modules
+        elif target._class_label == '<mod>':
+            pre = target.input_targets.copy()
+            post = target.output_targets.copy()
+        else:
+            raise ValueError("Deep forward build Error, unsupported class label.")
+
+        for pr in pre:
+            if (pr in all_groups) or (pr in all_connections):
+                return
+
+        target.build(self._backend)
+        if target._class_label == '<con>':
+            builded_connections.append(target)
+            all_connections.remove(target)
+        elif (target._class_label == '<neg>') or (target._class_label == '<mod>'):
+            builded_groups.append(target)
+            all_groups.remove(target)
+
+        for po in post:
+            self.deep_forward_build(po, all_groups, all_connections, builded_groups, builded_connections)
+
+        return
+
     # def strategy_build(self, all_groups=None):
     #     builded_groups = []
     #     unbuild_groups = {}
     #     output_groups = []
     #     level = 0
-    #     from ..Neuron.Node import Encoder, Decoder, Generator
+    #     from spaic.Neuron.Node import Encoder, Decoder, Generator
     #     # ===================从input开始按深度构建计算图==============
     #     for group in all_groups:
     #         if isinstance(group, Encoder) or isinstance(group, Generator):
     #             # 如果是input节点，则开始深度构建计算图
     #             group.build(self._backend)
     #             builded_groups.append(group)
     #             # all_groups.remove(group)
@@ -306,27 +357,36 @@
         self._backend.initial_continue_step()
         self._backend.update_time_steps()
 
     def reset(self, ):
         if self._backend.builded is True:
             self._backend.initial_step()
 
+    def enable_full_grad(self, requires_grad=True):
+        self._backend.full_enable_grad = requires_grad
+
     def init_run(self):
         self._backend.initial_step()
 
     def add_monitor(self, name, monitor):
         from spaic.Monitor.Monitor import Monitor
         assert isinstance(monitor, Monitor), "Type Error, it is not monitor"
         assert monitor not in self._monitors.values(), "monitor %s is already added" % (name)
         assert name not in self._monitors.keys(), "monitor with name: %s have the same name with an already exists monitor" % (
             name)
 
         self.__setattr__(name, monitor)
         # self._monitors[name] = monitor
 
+    def get_elements(self):
+        element_dict = dict()
+        for element in self.get_groups():
+            element_dict[element.id] = element
+        return element_dict
+
     def save_state(self, filename=None, direct=None, save=True, hdf5=False):
         """
         Save weights in memory or on hard disk.
 
         Args:
             filename: The name of saved file.
             direct: Target direction for saving state.
@@ -396,23 +456,25 @@
                 self.set_backend('torch', device=device)
             else:
                 self.set_backend('torch')
         if self._backend.builded is False:
             self.build()
         if self._backend.device != device:
             import warnings
-            warnings.warn('Backend device setting is '+self._backend.device+'. Backend device selection is priority.')
-            device = self._backend.device
+            warnings.warn(
+                'Backend device setting is ' + str(self._backend.device) + '. Backend device selection is priority.')
+            # device = self._backend.device
         if state:
             import torch
             if isinstance(state, dict) or isinstance(state, torch.Tensor):
                 for key, para in state.items():
                     backend_key = self._backend.check_key(key, self._backend._parameters_dict)
-                    if key:
-                        self._backend._parameters_dict[backend_key] = para.to(device)
+                    if backend_key:
+                        target_device = self._backend._parameters_dict[backend_key].device
+                        self._backend._parameters_dict[backend_key] = para.to(target_device)
 
                 # if self._backend.device
                 return
             else:
                 raise ValueError("Given state has wrong type")
 
         if direct:
@@ -431,32 +493,31 @@
         origin_path = os.getcwd()
         try:
             os.chdir(path)
         except:
             raise ValueError('Wrong Path.')
 
         if '_parameters_dict.pt' in os.listdir('./'):
-            data = torch.load('./_parameters_dict.pt')
+            data = torch.load('./_parameters_dict.pt', map_location=self._backend.device0)
             for key, para in data.items():
                 backend_key = self._backend.check_key(key, self._backend._parameters_dict)
                 if backend_key:
-                    self._backend._parameters_dict[backend_key] = para.to(device)
+                    target_device = self._backend._parameters_dict[backend_key].device
+                    self._backend._parameters_dict[backend_key] = para.to(target_device)
             if 'module_dict.pt' in os.listdir('./'):
-                module_data = torch.load('./module_dict.pt')
+                module_data = torch.load('./module_dict.pt', map_location=self._backend.device0)
                 for group in self.get_groups():
                     if isinstance(group, spaic.Module):
                         target_key = self._backend.check_key(group.id, module_data)
                         group.load_state_dict(module_data[target_key])
         else:
             for file in os.listdir('./'):
                 if file.endswith('.hdf5'):
                     import h5py
                     with h5py.File(direct, 'r') as f:
                         for key, para in f.items():
                             backend_key = self._backend.check_key(key, self._backend._parameters_dict)
                             if key:
-                                self._backend._parameters_dict[backend_key] = para.to(device)
+                                target_device = self._backend._parameters_dict[backend_key].device
+                                self._backend._parameters_dict[backend_key] = para.to(target_device)
         os.chdir(origin_path)
         return
-
-
-
```

### Comparing `SPAIC-0.6.1a0/spaic/Neuron/Actions.py` & `SPAIC-0.6.2.0.0/spaic/Neuron/Actions.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/Neuron/Decoders.py` & `SPAIC-0.6.2.0.0/spaic/Neuron/Decoders.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         #     index = spikes_list[i].index(max_value[i])
         #     predict_labels.append(index)
         return pop_spikes
 
     def torch_coding(self, record, target, device):
         # the shape of record is (time_step, batch_size, n_neurons)
         if '[2]' in self.coding_var_name:
-            pop_spikes = record[:,:,0,:].mean(0).to(device=device)
+            pop_spikes = record[:,:,0,:].sum(0).to(device=device)
         else:
-            spike_rate = record.mean(0).to(device=device)
+            spike_rate = record.sum(0).to(device=device)
             pop_num = int(self.num / self.pop_size)
             pop_spikes_temp = (
                 [
                     spike_rate[:, (i * self.pop_size): (i * self.pop_size) + self.pop_size].sum(dim=1)
                     for i in range(pop_num)
                 ]
             )
@@ -282,69 +282,61 @@
         return out
 
 Decoder.register('voltage_sum', Voltage_Sum)
 
 class Complex_Count(Decoder):
     def __init__(self, num=None, dec_target=None, dt=None, coding_method=('poisson', 'spike_counts', '...'), coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
         super(Complex_Count, self).__init__(num, dec_target, dt, coding_method, coding_var_name, node_type, **kwargs)
-
+        self.tlen = None
     def torch_coding(self, record: torch.Tensor, target, device):
         assert record.dtype.is_complex
-        tlen = record.shape[0]
-        time_array = torch.arange(0, tlen, device=device, dtype=torch.float)
-        # count = record.real
-        count = record.imag.gt(0)*record.real
-        t = time_array.view(-1,1,1)
-        out = torch.sum(count*torch.exp(-2.0*(t-record.imag)/tlen), dim=0) + 1.0e-6
-        rate = torch.sum(count, dim=0)/self._backend.time
-        return out, rate
+        if self.tlen is None:
+            self.tlen = record.shape[0]*1.0
+        time_array = torch.arange(0, self.tlen, device=device, dtype=torch.float).view(-1,1,1)
+        spk = record.real.gt(0.0)
+        # for gradient test
+        sum_spk = torch.cumsum(spk, dim=0)
+        spk = spk*sum_spk.lt(5)
+
+        # count = record.imag.gt(0)
+        out = torch.sum(spk*(-(time_array-record.imag)/self.tlen), dim=0) + 1.0e-6
+        # out = torch.sum(count, dim=0) + 1.0e-6
+        # rate = torch.sum(count, dim=0)/self._backend.time
+        return out
 
 Decoder.register('complex_count', Complex_Count)
 
 
 class Complex_Phase(Decoder):
     def __init__(self, num=None, dec_target=None, dt=None, coding_method=('poisson', 'spike_counts', '...'), coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
         super(Complex_Phase, self).__init__(num, dec_target, dt, coding_method, coding_var_name, node_type, **kwargs)
         self.trange = kwargs.get('trange',2.0)
         self.period = kwargs.get('period', 20.0)
-        class TransClamp(torch.autograd.Function):
-            @staticmethod
-            def forward(ctx, x, min=None, max=None):
-                return torch.clamp(x, min, max)
-
-            @staticmethod
-            def backward(ctx, grad_outputs):
-                return grad_outputs, None, None
-        self.clamp = TransClamp.apply
-
-
+        # class TransClamp(torch.autograd.Function):
+        #     @staticmethod
+        #     def forward(ctx, x, min=None, max=None):
+        #         return torch.clamp(x, min, max)
+        #
+        #     @staticmethod
+        #     def backward(ctx, grad_outputs):
+        #         return grad_outputs, None, None
+        # self.clamp = TransClamp.apply
 
 
 
 
     def torch_coding(self,  record: torch.Tensor, target, device):
+        assert record.dtype.is_complex
+        # record.shape = (time, batch, num)
         tlen = record.shape[0]
-        time_array = self.dt * torch.arange(0, tlen, device=device, dtype=torch.float)
-        spk = record.real.gt(0.0)
-        count = torch.cumsum(spk, dim=0)
-        spk_count = (spk*count + 1.0e6*(1-spk.to(torch.float))).detach()
-        sort_spk_count, sort_spk_index = torch.sort(spk_count, dim=0)
-        sort_spk = torch.gather(spk, dim=0, index=sort_spk_index)
-
-        rate = torch.sum(spk, dim=0) / self._backend.time
-
-        time = time_array.view(-1,1,1) - record.imag
-        sort_time = torch.gather(time, dim=0, index=sort_spk_index)
-        sort_time_aim = sort_time
-        sort_time_target = torch.amin(sort_time, dim=-1, keepdim=True).detach()
-        sort_time_diff = torch.exp((sort_time_target-sort_time_aim)/self.trange)*sort_spk
-        out_time_score = torch.sum(sort_time_diff, dim=0) + 1.0e-4 + rate
-        # (0.9 ** sort_spk_count) *
-
-        return out_time_score, rate
+        reference = torch.mean(record.abs(), dim=-1, keepdim=True)
+        reference = torch.softmax(reference, dim=0)*self.dt
+        phase = record.real/(record.abs()+1.0)
+        phase = torch.sum(phase*reference, dim=0)
+        return phase
 
     def torch_coding2(self, record, target, device):
         import torch.nn.functional as F
         tlen = record.shape[0]
         batch_size = record.shape[1]
         out_num = record.shape[2]
         kernel_range = int(self.period / self.dt)
@@ -360,17 +352,73 @@
                             .view(batch_size, out_num, tlen), dim=1, keepdim=True)
         x = x.view(batch_size, out_num, tlen)
         out_phase = torch.sum(conv_i*x.real.detach() + conv_t*x.imag*self.dt, dim=-1)
 
         return out_phase, conv_i
 
 
-
 Decoder.register('complex_phase', Complex_Phase)
 
+class Complex_Latency(Decoder):
+    def __init__(self, num=None, dec_target=None, dt=None, coding_method=('poisson', 'spike_counts', '...'), coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
+        super(Complex_Latency, self).__init__(num, dec_target, dt, coding_method, coding_var_name, node_type, **kwargs)
+        self.tlen = None
+
+    def torch_coding(self,  record: torch.Tensor, target, device):
+        assert record.dtype.is_complex
+        # if self.tlen is None:
+        self.tlen = record.shape[0]
+        time_array = torch.arange(0, self.tlen, device=device, dtype=torch.float).view(-1,1,1)
+        spk = record.real.gt(0)
+        spk_time = (self.tlen-(time_array - record.imag))*spk
+        spk_time = torch.exp(1*(spk_time-torch.amax(spk_time, dim=(0,2), keepdim=True).detach())/self.tlen)
+        spk_rate = record.real
+        spk_weight = torch.exp(-torch.cumsum(record.real.detach(),dim=0)/5.0)
+        weighted_spk_time = torch.sum(spk_weight*spk_rate*spk_time*spk,dim=0)
+        return weighted_spk_time
+
+Decoder.register('complex_latency', Complex_Latency)
+
+class Complex_TimingDistance(Decoder):
+    def __init__(self, num=None, dec_target=None, dt=None, coding_method=('poisson', 'spike_counts', '...'), coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
+        super(Complex_TimingDistance, self).__init__(num, dec_target, dt, coding_method, coding_var_name, node_type, **kwargs)
+        from matplotlib import pyplot as plt
+        self.tlen = None
+        self.filter_time = kwargs.get("filter_time", 10.0)
+
+
+    def build(self, backend):
+        super(Complex_TimingDistance, self).build(backend)
+        tdt = 6.0*self.dt/(1.0*self.filter_time)
+        tt = torch.arange(0, 6.0+tdt, tdt)
+        self.rate_filter = (torch.exp(-(tt - 2) ** 2)).view(1, 1, -1)
+        self.d_rate_filter = (0.5*(tt-2)*torch.exp(-(tt - 1) ** 2)).view(1, 1, -1)*tdt*0.01
+
+
+    def torch_coding(self, record: torch.Tensor, target: torch.Tensor , device: str):
+        from torch.nn.functional import mse_loss
+        # record shape (time, batch, neuron)
+        # target shape (batch, neuron, time)
+        assert record.dtype.is_complex
+        n_time, n_batch, n_neuron = record.shape
+        self.rate_filter = self.rate_filter.to(device)
+        self.d_rate_filter = self.d_rate_filter.to(device)
+        target = target.view(-1, 1, n_time)
+        record = record.permute(1,2,0).view(-1, 1, n_time)
+
+        target_rate = torch.conv1d(target, self.rate_filter, padding='same')
+        record_rate = torch.conv1d(record.real, self.rate_filter, padding='same') - torch.conv1d(record.imag, self.d_rate_filter, padding='same')
+        rate_loss = mse_loss(record_rate, target_rate)
+        return rate_loss, record_rate, target_rate
+
+Decoder.register('complex_timing_distance', Complex_TimingDistance)
+
+
+
+
 class Complex_Trajectory(Decoder):
 
     def __init__(self, num=None, dec_target=None, dt=None, coding_method=('poisson', 'spike_counts', '...'), coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
         super(Complex_Trajectory, self).__init__(num, dec_target, dt, coding_method, coding_var_name, node_type, **kwargs)
         self.tau_d = kwargs.get('tau_d', 20.0+20*torch.rand(num).view(1,-1))
         self.tau_r = kwargs.get('tau_r', 10.0+50*torch.rand(num).view(1,-1))
         self.group_num = kwargs.get('group_num', 1)
```

### Comparing `SPAIC-0.6.1a0/spaic/Neuron/Encoders.py` & `SPAIC-0.6.2.0.0/spaic/Neuron/Encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,25 +89,26 @@
                 spk_shape = [self.time_step, self.num]
                 spike_values = torch.sparse.FloatTensor(indexes, values, size=spk_shape).to_dense()
                 spike_dts = torch.sparse.FloatTensor(indexes, delta_times, size=spk_shape).to_dense()
                 all_spikes.append(torch.stack([spike_values, spike_dts], dim=1))
             spikes = torch.stack(all_spikes, dim=1)
 
         else:
-            for i in range(source.shape[0]):
+            for i in range(len(source)):
                 spiking_times, neuron_ids = source[i]
 
                 assert (spiking_times >= 0).all(), "Inputs must be non-negative"
                 spike_index = spiking_times / self.dt
                 spike_index = spike_index #.squeeze(-1)
                 # neuron_ids = np.float32(neuron_ids) #.squeeze(-1)
-                indexes = [spike_index, neuron_ids]
-                if source.__class__.__name__ == 'ndarray':
-                    indexes = torch.tensor(indexes, device=device, dtype=torch.long)
-                    indexes[0] = torch.clamp_max(indexes[0], self.time_step-1)
+                indexes = np.array([spike_index, neuron_ids])
+                # if indexes.__class__.__name__ == 'ndarray':
+                indexes = torch.tensor(indexes, device=device, dtype=torch.long)
+                indexes[0] = torch.clamp_max(indexes[0], self.time_step-1)
+
 
 
                 spk_shape = [self.time_step, self.num]
 
                 # mapping the spike times into [0,1] matrix.
                 indexes = indexes.to(dtype=torch.long)
                 values = torch.ones(spike_index.shape, device=device)
@@ -154,47 +155,55 @@
     """
     def __init__(self, shape=None, num=None, dec_target=None, dt=None, coding_method='poisson',
                  coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
         super(PoissonEncoding, self).__init__(shape, num, dec_target, dt, coding_method, coding_var_name, node_type, **kwargs)
         self.unit_conversion = kwargs.get('unit_conversion', 1.0)
         self.single_test = kwargs.get("single_test", False)
         self.end_time = kwargs.get("end_time", None)
+        self.start_time = kwargs.get("start_time", None)
 
     def numpy_coding(self, source, device):
         # assert (source >= 0).all(), "Inputs must be non-negative"
         shape = list(source.shape)
         spk_shape = [self.time_step] + shape
         spikes = np.random.rand(*spk_shape).__le__(source * self.dt).astype(float)
         return spikes
 
 
     def torch_coding(self, source, device):
         # assert (source >= 0).all(), "Inputs must be non-negative"
+        # device = device[0] if isinstance(device, list) else device
         if source.__class__.__name__ == 'ndarray':
             source = torch.tensor(source, device=device, dtype=self._backend.data_type)
-        self.device = device
+        # self.device = device
         self.source = source
 
         if self.single_test:
-            spikes = torch.rand([self.time_step, 1, self.shape[-1]], device=device).le(source * self.unit_conversion * self.dt)
+            spikes = torch.rand([self.time_step+1, 1, self.shape[-1]], device=device).le(source * self.unit_conversion * self.dt)
             return spikes.type(self._backend.data_type)
         else:
             return None
 
 
     def next_stage(self):
         if self.new_input:
             self.get_input()
             self.new_input = False
+            self.shape[0] = self.source.shape[0]
+
 
-        # self.index += 1
-        if self.end_time is not None and self.time > self.end_time:
-            return torch.zeros(self.source.shape, device=self.device).type(self._backend.data_type)
+        self.index += 1
+        if self.end_time is not None and self.index > self.end_time/self.dt:
+            return torch.zeros(self.shape, device=self.device)
+        elif self.start_time is not None and self.index < self.start_time/self.dt:
+            return torch.zeros(self.shape, device=self.device)
+        elif self.single_test:
+            return self.all_spikes[self.index]
         else:
-            return torch.rand(self.source.shape, device=self.device).le(self.source * self.unit_conversion * self.dt).type(self._backend.data_type)
+            return torch.rand(self.shape, device=self.device).le(self.source * self.unit_conversion * self.dt).type(self._backend.data_type)
 
 
 Encoder.register('poisson', PoissonEncoding)
 
 class Latency(Encoder):
     """
         延迟编码，刺激强度越大，脉冲发放越早。刺激强度被归一化到[0, 1]。
@@ -203,35 +212,39 @@
         dt: time step
     """
 
     def __init__(self, shape=None, num=None, dec_target=None, dt=None, coding_method=('poisson', 'spike_counts', '...'),
                  coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
         super(Latency, self).__init__(shape, num, dec_target, dt, coding_method, coding_var_name, node_type, **kwargs)
         self.max_scale = kwargs.get("max_scale", None)
+        self.cut_off = kwargs.get('cut_off', False)
 
     def torch_coding(self, source, device):
         assert (source >= 0).all(), "Inputs must be non-negative"
         if self.max_scale is None:
             max_scale = self.time_step - 1.0
         else:
-            max_scale = self.max_scale/self.dt
+            max_scale = self.max_scale*(self.time_step - 1.0)
 
         if source.__class__.__name__ == 'ndarray':
             source = torch.tensor(source, device=device, dtype=self._backend.data_type)
         shape = list(source.shape)
         spk_shape = [self.time_step] + shape
 
         # Create spike times in order of decreasing intensity.
         min_value = 1.0e-10
         source_temp = (source - torch.min(source)) / (torch.max(source) - torch.min(source) + min_value)
         spike_index = max_scale*(1-source_temp)
         spike_index = spike_index.reshape([1] + shape).to(device=device, dtype=torch.long)
         spikes = torch.zeros(spk_shape, device=device)
         spike_src = torch.ones_like(spike_index, device=device, dtype=self._backend.data_type)
         spikes.scatter_(dim=0, index=spike_index, src=spike_src)
+        if self.cut_off:
+            min_mask = source.gt(0.05*torch.max(source, dim=-1, keepdim=True)[0])
+            spikes = spikes*min_mask
         return spikes
 Encoder.register('latency', Latency)
 
 class Relative_Latency(Encoder):
     '''
         相对延迟编码，在一个样本中，其相对强度越大，放电越靠前
     '''
```

### Comparing `SPAIC-0.6.1a0/spaic/Neuron/Generators.py` & `SPAIC-0.6.2.0.0/spaic/Neuron/Generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,23 +62,24 @@
         #     end_time_step = int(self.end_time/self.dt)
         #     spikes[end_time_step:, ...] = 0.0
         return None
 
     def next_stage(self):
         if self.new_input:
             self.get_input()
+            self.shape[0] = self.inp_source.shape[0]
             self.new_input = False
 
         if (self.start_time is None or self.start_time< self.index*self.dt) \
             and (self.end_time is None or self.end_time> self.index*self.dt):
-            spikes = self.weight*torch.rand(self.shape, device=self._backend.device).le(
+            spikes = self.weight*torch.rand(self.shape, device=self._backend.device[0]).le(
                 self.inp_source*self.unit_conversion)
             return spikes.type(self._backend.data_type)
         else:
-            return torch.zeros(0).type(self._backend.data_type)
+            return torch.zeros(self.shape, dtype=self._backend.data_type, device=self._backend.device)
 
 Generator.register('poisson_generator', Poisson_Generator)
 
 class Poisson_Generator2(Generator):
     """
         泊松生成器，根据输入脉冲速率生成。
         Generate a poisson spike train according input rate.
```

### Comparing `SPAIC-0.6.1a0/spaic/Neuron/Module.py` & `SPAIC-0.6.2.0.0/spaic/Neuron/Module.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,39 +8,46 @@
 
 @description:
 wrap around deep learning module such as a cnn network lstm cell
 """
 import torch
 
 import spaic
-from ..Network.Assembly import Assembly
-from ..Network.BaseModule import Op
+from spaic.Network.Assembly import Assembly
+from spaic.Network.BaseModule import Op
 
 class Module(Assembly):
     _class_label = '<mod>'
 
-    def __init__(self, module=None, name=None, input_targets=[], input_var_names=['O[updated]'], output_tragets=None, output_var_names=['Isyn'], module_backend='pytorch'):
+    def __init__(self, module=None, name=None, input_targets=[], input_var_names=['O[updated]'], output_targets=None, output_var_names=['Isyn'], module_backend='pytorch'):
         super(Module, self).__init__(name)
         self.module: torch.nn.Module = module
         if isinstance(input_targets, list):
             self.input_targets = input_targets
         else:
             self.input_targets = [input_targets]
         if isinstance(input_var_names, list):
             self.input_var_names = input_var_names
         else:
             self.input_var_names = [input_var_names]
-        if isinstance(output_tragets, list):
-            self.output_traget = output_tragets
+
+        if isinstance(output_targets, list):
+            self.output_targets = output_targets
         else:
-            self.output_traget = [output_tragets]
+            self.output_targets = [output_targets]
         if isinstance(output_var_names, list):
             self.output_var_names = output_var_names
         else:
             self.output_var_names = [output_var_names]
+
+        for in_targ in self.input_targets:
+            in_targ.register_module(self, True)
+        for out_targ in self.output_targets:
+            out_targ.register_module(self, False)
+
         self.module_backend = module_backend
 
 
     def standalone_run(self, *args):
         return self.module(*args)
 
     def init_variable(self, var_names=None, var_shapes=None, var_value_dict=None):
@@ -79,24 +86,24 @@
         var_len = len(self._var_names)
         for ii in range(var_len):
             key = self.id + ":" + "{" + self._var_names[ii] + "}"
             shape = (1, *self._var_shapes[ii])
             self.variable_to_backend(key, shape, self._var_values[ii])
 
         # add standalone operation
-        output_var_name = self.output_traget[0].id + ":" + "{" + self.output_var_names[0] + "}"
+        output_var_name = self.output_targets[0].id + ":" + "{" + self.output_var_names[0] + "}"
         self._var_names.append(output_var_name)
         input_var_names = []
         for input_target, input_name in zip(self.input_targets, self.input_var_names):
             input_var_name = input_target.id + ":" + "{" + input_name + "}"
             self._var_names.append(input_var_name)
             input_var_names.append(input_var_name)
 
         backend.register_standalone(Op(output_var_name, self.standalone_run, input_var_names, owner=self))
-        self.module.to(backend.device)
+        self.module.to(backend.device0)
 
 
 
     @property
     def parameters(self):
 
         return self.module.parameters()  # .state_dict()
```

### Comparing `SPAIC-0.6.1a0/spaic/Neuron/Neuron.py` & `SPAIC-0.6.2.0.0/spaic/Neuron/Neuron.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,51 +8,54 @@
 
 @description:
 定义神经集群和神经元模型。
 神经元集群保存神经元数目、神经元编号、类型、模型、模型参数、神经元位置等信息，参与网络构建
 """
 # print('__file__={0:<35} | __name__={1:<20} | __package__={2:<20}'.format(__file__,__name__,str(__package__)))
 import numpy as np
-from ..Network import Assembly
+from spaic.Network import Assembly
 from abc import ABC, abstractmethod
 from collections import OrderedDict
-from ..Network.BaseModule import VariableAgent, Op
+from spaic.Network.BaseModule import VariableAgent, Op
+from spaic.IO.Initializer import uniform
 import re
-import torch
 
-# from brian2 import *
 
+# from brian2 import *
 
 class NeuronGroup(Assembly):
     '''Class for a group of neurons.
     '''
 
     _class_label = '<neg>'
     _is_terminal = True
     def __init__(self, num=None,
                  model=None,
                  shape=None,
                  neuron_type=('excitatory', 'inhibitory', 'pyramidal', '...'),
-                 neuron_position=('x, y, z' or 'x, y'),
+                 neuron_position='x, y, z',
                  name=None,
+                 parameter_variables: list = None,
+                 varible_ranges: dict = None,
+                 prefer_device=None,
                  **kwargs
                  ):
         super(NeuronGroup, self).__init__(name=name)
         self.set_num_shape(num=num, shape=shape)
         self.outlayer = kwargs.get("outlayer", False)
 
         # self.model = model
         if neuron_type == ('excitatory', 'inhibitory', 'pyramidal', '...'):
             self.type = ['nontype']
         elif isinstance(neuron_type, list):
             self.type = neuron_type
         else:
             self.type = [neuron_type]
 
-        if neuron_position == ('x, y, z' or 'x, y'):
+        if neuron_position == 'x, y, z':
             self.position = []
         else:
             neuron_position = np.array(neuron_position)
             assert neuron_position.shape[0] == num, " Neuron_position not equal to neuron number"
             self.position = neuron_position
 
         self.parameters = kwargs
@@ -62,18 +65,31 @@
             self.model = None
         elif isinstance(model, NeuronModel):
             self.model = model
             self.model_class = None
             self.model_name = 'custom_model'
         else:
             raise ValueError("only support set neuron model with string or NeuronModel class constructed by @custom_model()")
+        # variables that can be trained
+        if parameter_variables is None:
+            self._parameter_var_names = []
+        else:
+            assert isinstance(parameter_variables, list)
+            self._parameter_var_names = parameter_variables
+        # variables that needs clamp
+        if varible_ranges is None:
+            self._variablel_ranges = dict()
+        else:
+            assert isinstance(varible_ranges, dict)
+            self._variablel_ranges = varible_ranges
         self._var_names = list()
         self._var_dict = dict()
         self._operations = OrderedDict()
         self._init_operations = OrderedDict()
+        self.prefer_device = prefer_device
 
 
     def set_num_shape(self, num, shape):
         self.num = num
         self.shape = shape
         if self.shape is not None:
             num = np.prod(self.shape)
@@ -88,93 +104,120 @@
 
     def set_parameter(self):
         pass
 
     def get_model(self):
         return self.model
 
-    def _add_label(self, key):
-        if isinstance(key, str):
-            if key == '[dt]':
-                return key
-            elif '[updated]' in key:
-                return self.id + ':' + '{' + key.replace('[updated]', "") + '}' + '[updated]'
-            else:
-                return self.id + ':' + '{' + key + '}'
-        elif isinstance(key, VariableAgent):
-            return key.var_name
-        else:
-            raise ValueError(" the key data type is not supported for add_label")
 
     def add_neuron_label(self, key: str):
         if isinstance(key, str) or isinstance(key, VariableAgent):
             return self._add_label(key)
         elif isinstance(key, list) or isinstance(key, tuple):
             keys = []
             for k in key:
                 keys.append(self._add_label(k))
             return keys
 
+    def add_variable_kwargs(self, key):
+        t_kwargs = dict()
+        if key in self._parameter_var_names:
+            t_kwargs['is_parameter'] = True
+        if key in self._variablel_ranges:
+            min, max = self._variablel_ranges[key]
+            if min is not None:
+                assert isinstance(min, float)
+                t_kwargs['min'] = min
+            if max is not None:
+                assert isinstance(max, float)
+                t_kwargs['max'] = max
+        return t_kwargs
+
     def build(self, backend):
         '''
         Parameters
         ----------
         backend : Backend.Backend
         Returns
         -------
         '''
         self._backend = backend
-        batch_size = self._backend.get_batch_size()
+        prefer_device=self.prefer_device if self.prefer_device != None else None
+        # batch_size = self._backend.get_batch_size()
         # if(self.parameters is not None):
         #     self.model = self.model_class(**self.model_parameters)
         # else:
         #     self.model = self.model_class()
         if self.model_class is not None:
             if 'dt' not in self.parameters:
                 self.parameters['dt'] = self._backend.dt
+            self.parameters['neuron_num'] = self.num
             self.model = self.model_class(**self.parameters)
 
 
         dt = backend.dt
         for (key, tau_var) in self.model._tau_variables.items():
+            t_kwargs = self.add_variable_kwargs(key)
             key = self.add_neuron_label(key)
             tau_var = np.exp(-dt / tau_var)
             # shape = ()
             if tau_var.size > 1:
                 shape = tau_var.shape
                 assert tau_var.size == self.num, "The number of tau should equal the number of neurons."
             else:
                 shape = ()
 
-            self.variable_to_backend(key, shape, value=tau_var)
+            self.variable_to_backend(key, shape, value=tau_var, prefer_device=prefer_device,  **t_kwargs)
 
         for (key, membrane_tau_var) in self.model._membrane_variables.items():
+            t_kwargs = self.add_variable_kwargs(key)
             key = self.add_neuron_label(key)
             # TODO: 计划把membrane tau反过来了变成membrane_tau/dt，需要把用的模型也改一下
             membrane_tau_var = dt/membrane_tau_var
             shape = (1, *self.shape)  # (1, neuron_num)
-            self.variable_to_backend(key, shape, value=membrane_tau_var)
+            self.variable_to_backend(key, shape, value=membrane_tau_var, prefer_device=prefer_device, **t_kwargs)
 
 
         for (key, var) in self.model._variables.items():
             # add the rule to extend new dimension before shape (for slif model)
+            t_kwargs = self.add_variable_kwargs(key)
             extend_tag = re.search("\[\d*\]", key)
             if extend_tag is not None:
                 extend_tag = int(key[extend_tag.start() + 1:extend_tag.end() - 1])
             key = self.add_neuron_label(key)
 
+
             if extend_tag is not None:
                 shape = (1, extend_tag, *self.shape)
             else:
                 shape = (1, *self.shape)  # (batch_size, shape)
-            self.variable_to_backend(key, shape, value=var)
+            if hasattr(var, 'shape') and len(var.shape) > 0:
+                # adding more dimensions after the neuron shape, assuming neuron'shape in var.shape is 1
+                if len(var.shape) > len(shape):
+                    var_shape = list(var.shape)
+                    for i, s in enumerate(shape):
+                        if s != var_shape[i]:
+                            assert var_shape[i] == 1
+                            var_shape[i] = shape[i]
+                    var = var.expand(var_shape)
+                    shape = var.shape
+
+                elif var.shape[0] > 1 and var.shape[0]==shape[1]:
+                    # for batch dim
+                    var = var.unsqueeze(dim=0)
+
+
+            self.variable_to_backend(key, shape, value=var, prefer_device=prefer_device, **t_kwargs)
 
         for (key, var) in self.model._parameter_variables.items():
-            key = self.add_neuron_label(key)
+            t_kwargs = self.add_variable_kwargs(key)
+            t_kwargs['is_parameter'] = True
 
+            key = self.add_neuron_label(key)
+            # is pararmeter by default?
             if isinstance(var, np.ndarray):
                 if var.size > 1:
                     shape = var.shape
                     # assert var.size == self.num, "The number of tau should equal the number of neurons."
                 else:
                     shape = ()
             elif isinstance(var, torch.Tensor):
@@ -185,58 +228,44 @@
                     shape = var.shape
                     assert var.size == self.num, "The number of tau should equal the number of neurons."
                 else:
                     shape = ()
             else:
                 shape = ()
 
-            self.variable_to_backend(key, shape, value=var)
+            self.variable_to_backend(key, shape, value=var, prefer_device=prefer_device, **t_kwargs)
 
         for (key, var) in self.model._constant_variables.items():
             key = self.add_neuron_label(key)
-
-            # if isinstance(var, np.ndarray):
-            #     if var.size > 1:
-            #         shape = var.shape
-            #     else:
-            #         shape = ()
-            # elif isinstance(var, torch.Tensor):
-            #     shape = var.shape
-            # elif hasattr(var, '__iter__'):
-            #     var = np.array(var)
-            #     if var.size > 1:
-            #         shape = var.shape
-            #     else:
-            #         shape = ()
-            # else:
             shape = None
 
-            self.variable_to_backend(key, shape, value=var, is_constant=True)
+            self.variable_to_backend(key, shape, value=var, is_constant=True, prefer_device=prefer_device)
 
         op_count = 0
         for op in self.model._operations:
             addcode_op = Op(owner=self)
             if isinstance(op[1], str):
-                # op_name = str(op_count) + ':' + op[1]
                 op_name = f'{op_count}:{op[1]}'
-                addcode_op.func = op[1]
+                addcode_op.func_name = op[1]
                 addcode_op.output = self.add_neuron_label(op[0])
                 if len(op) > 3:  # 为了解决历史的单一list格式的问题
                     addcode_op.input = self.add_neuron_label(op[2:])
                 else:
                     addcode_op.input = self.add_neuron_label(op[2])
+                addcode_op.place = prefer_device
                 backend.add_operation(addcode_op)
             else:
                 op_name = f'{op_count}:custom_function'
-                addcode_op.func = op[1]
+                addcode_op.func_name = op[1]
                 addcode_op.output = self.add_neuron_label(op[0])
                 if len(op) > 3:  # 为了解决历史的单一list格式的问题
                     addcode_op.input = self.add_neuron_label(op[2:])
                 else:
                     addcode_op.input = self.add_neuron_label(op[2])
+                addcode_op.place = prefer_device
                 backend.register_standalone(addcode_op)
             op_count += 1
 
             self._operations[op_name] = addcode_op
 
         for op in self.model._init_operations:
             addcode_op = []
@@ -245,30 +274,30 @@
                     addcode_op.append(self.add_neuron_label(value))
                 else:
                     addcode_op.append(value)
             if len(op) > 3:
                 addcode_op[2] = addcode_op[2:]
                 addcode_op = addcode_op[:3]
             op_count += 1
-            self.init_op_to_backend(addcode_op[0], addcode_op[1], addcode_op[2])
+            self.init_op_to_backend(addcode_op[0], addcode_op[1], addcode_op[2], prefer_device)
             op_name = str(op_count) + ':' + 'custom_initial_function'
             self._init_operations[op_name] = addcode_op
 
 
 
         if self.model_name == "slif" or self.model_name == 'selif':
             self.model.build((1, *self.shape), backend)
             self.model.outlayer = self.outlayer
             update_code = self.model.update_op_code
             intital_code = self.model.initial_op_code
-            self.init_op_to_backend(intital_code[0], intital_code[1], intital_code[2])
+            self.init_op_to_backend(intital_code[0], intital_code[1], intital_code[2], prefer_device)
             backend.register_standalone(Op(self.add_neuron_label(update_code[0]), update_code[1],
-                                          [self.add_neuron_label(update_code[2])], owner=self))
-            backend.register_standalone(Op(self.add_neuron_label('V'), self.model.return_V, [], owner=self))
-            backend.register_standalone(Op(self.add_neuron_label('S'), self.model.return_S, [], owner=self))
+                                          [self.add_neuron_label(update_code[2])], prefer_device, owner=self))
+            backend.register_standalone(Op(self.add_neuron_label('V'), self.model.return_V, [], prefer_device, owner=self))
+            backend.register_standalone(Op(self.add_neuron_label('S'), self.model.return_S, [], prefer_device, owner=self))
 
 
     @staticmethod
     def custom_model(input_vars, output_vars, new_vars_dict, equation_type=('iterative','euler_iterative','exp_euler_iterative','ode'), backend='torch', custom_function_name='custom', base_model=None, add_threshold=True):
         '''
         Examples:
             @NeuronGroup.custom_model(input_vars=['M', 'S', 'WgtSum'], output_vars=['V', 'M', 'S'],
@@ -340,14 +369,16 @@
             model._operations.append(op_code)
             if add_threshold == True:
                 model._operations.append(('O', 'threshold', 'V[updated]', 'Vth'))
             return model
         return model_function
 
 
+
+
 class NeuronModel(ABC):
     '''
     op -> (return_name, operation_name, input_name1, input_name2...)
     '''
 
     #: A dictionary mapping neuron model names to `Model` objects
     neuron_models = dict()
@@ -463,18 +494,16 @@
         self._operations.append(('S', 'var_linear', 'tauQ', 'S', 'I[updated]'))
         self._operations.append(('PSP', 'minus', 'M[updated]', 'S[updated]'))
         self._operations.append(('V', 'minus', 'PSP', 'E'))
         self._operations.append(('O', 'threshold', 'V[updated]', 'Vth'))
         self._operations.append(('Resetting', 'var_mult', 'Vth', 'O[updated]'))
         self._operations.append(('E', 'var_linear', 'tauM', 'E', 'Resetting'))
 
-
 NeuronModel.register("clif", CLIFModel)
 
-
 class AdaptiveCLIFModel(NeuronModel):
     """
     Current LIF 3-kernel model:
     V(t) = M(t) − S(t) − E(t)
     I^n[t] = V0 * Isyn^n[t-1] #sum(w * O^(n-1)[t])
     M^n[t] = betaM * M^n[t-1] + I^n[t-1]
     S^n[t] = betaS * S^n[t-1] + I^n[t-1]
@@ -498,40 +527,40 @@
         self._variables['O'] = 0.0
         self._variables['V'] = 0.0
         self._variables['Isyn'] = 0.0
 
         self._tau_variables['tauM'] = np.asarray(kwargs.get('tau_m', 20.0))  # self.neuron_parameters['tau_m']
         self._tau_variables['tauP'] = np.asarray(kwargs.get('tau_p', 12.0))  # self.neuron_parameters['tau_p']
         self._tau_variables['tauQ'] = np.asarray(kwargs.get('tau_q', 8.0))  # self.neuron_parameters['tau_q']
+        self._tau_variables['tauA'] = np.asarray(kwargs.get('tau_a', 2000.0))  # self.neuron_parameters['tau_q']
 
         beta = self._tau_variables['tauP'] / self._tau_variables['tauQ']
         V0 = (1 / (beta - 1)) * (beta ** (beta / (beta - 1)))
         self._parameter_variables['V0'] = V0
 
-        self._constant_variables['Vth0'] = kwargs.get('v_th', 1.0)
-        self._variables['Vth1'] = 0.0
+        self._constant_variables['Vth'] = kwargs.get('v_th', 1.0)
+        self._variables['Vth1[stay]'] = 0 #uniform(0, 1.0)
+        self._variables['beta_adaptive'] = kwargs.get('beta_adaptive', 0.1)
 
         # self._operations.append(('I_che', 'var_mult', 'V0', 'WgtSum[updated]'))
         # self._operations.append(('I', 'add', 'I_che[updated]', 'I_ele'))
 
-        self._operations.append(('Vth1', 'var_linear', 'tauP', 'Vth1', 'O'))
-        self._operations.append(('Vth', 'add', 'Vth1[updated]', 'Vth0'))
+        self._operations.append(('Vth1[stay]', 'var_linear', 'tauA', 'Vth1[stay]', 'O'))
+        # self._operations.append(('Vth', 'add', 'Vth1[stay][updated]', 'Vth0'))
         self._operations.append(('I', 'var_mult', 'V0', 'Isyn[updated]'))
         self._operations.append(('M', 'var_linear', 'tauP', 'M', 'I[updated]'))
         self._operations.append(('S', 'var_linear', 'tauQ', 'S', 'I[updated]'))
         self._operations.append(('PSP', 'minus', 'M[updated]', 'S[updated]'))
-        self._operations.append(('V', 'minus', 'PSP', 'E'))
+        self._operations.append(('EE', 'var_linear', 'beta_adaptive', 'Vth1[stay][updated]', 'E'))
+        self._operations.append(('V', 'minus', 'PSP', 'EE'))
         self._operations.append(('O', 'threshold', 'V[updated]', 'Vth'))
         self._operations.append(('Resetting', 'var_mult', 'Vth', 'O[updated]'))
         self._operations.append(('E', 'var_linear', 'tauM', 'E', 'Resetting'))
 
-
 NeuronModel.register("aclif", AdaptiveCLIFModel)
-
-
 class IFModel(NeuronModel):
     """
     IF model:
     V(t) = V(t-1) * (1 - O(t-1)) + Isyn[t] - ConstantDecay
 
     O^n[t] = spike_func(V^n[t-1])
     """
@@ -550,36 +579,539 @@
 
         self._operations.append(('Vtemp', 'add', 'V', 'Isyn[updated]'))
         self._operations.append(('Vtemp1', 'minus', 'Vtemp', 'ConstantDecay'))
         self._operations.append(('O', 'threshold', 'Vtemp1', 'Vth'))
         self._operations.append(('Resetting', 'var_mult', 'Vtemp1', 'O[updated]'))
         self._operations.append(('V', 'minus', 'Vtemp1', 'Resetting'))
 
-
 NeuronModel.register("if", IFModel)
 
-
 class NullModel(NeuronModel):
     """
     return 'O'
     """
 
     def __init__(self, **kwargs):
         super(NullModel, self).__init__()
         # self.neuron_parameters['ConstantDecay'] = kwargs.get('ConstantDecay', 0.0)
         # self.neuron_parameters['v_th'] = kwargs.get('v_th', 1.0)
         self._variables['Isyn'] = 0.0
         self._variables['O'] = 0.0
 
         self._operations.append(('O', 'assign', 'Isyn[updated]'))
 
-
 NeuronModel.register("null", NullModel)
 
 
+
+import torch
+
+
+class QLIFModel(NeuronModel):
+    """
+    LIF neuron model for Q-Backprop learning
+
+    E[t] = beta_m*E[t-1] + Vth*O[t-1]
+    V[t] = WgtSum(PSP[t]) - E[t]
+    O[t] = spike_function(V[t])
+
+
+    # Q for non-spiking
+    Mp[t] = beta_m*Mp[t-1] + WpSum[t]
+    Sp[t] = beta_s*Sp[t-1] + WpSum[t]
+    P[t] = Mp[t] - Sp[t]
+
+    # Q for spiking
+    Mq[t] = beta_m*Mq[t-1] + WqSum[t]
+    Sq[t] = beta_s*Sq[t-1] + WqSum[t]
+    Q[t] = Mq[t] - Sq[t]
+
+    R[t] = ~O[t]*beta_s*R[t-1] + O[t]
+    F[t] = 1 - R[t]
+    QP[t] = Q[t] - P[t]
+    BQ[t] = R[t]*Q[t] + F[t]*P[t]
+
+    TP[t] = R[t]*P[t] + F[t]*Reward - P[t-1]
+    TQ[t] = F[t]*Q[t] + R[t]*Reward - Q[t-1]
+    """
+
+    # WgtSum(BQ_post[t - 1]) / WgtSum)
+    def __init__(self, **kwargs):
+        super(QLIFModel, self).__init__()
+        self._tau_variables['Beta_m'] = kwargs.get('tau_m', 20.0)
+        self._tau_variables['Beta_s'] = kwargs.get('tau_s', 8.0)
+        self._parameter_variables['Vth'] = kwargs.get('v_th', 1.0)
+        self._constant_variables['One'] = 1.0
+
+        self._variables['E'] = 0.0
+        self._variables['O'] = 0.0
+        self._variables['V'] = 0.0
+        self._variables['P'] = 0.0
+        self._variables['Mp'] = 0.0
+        self._variables['Sp'] = 0.0
+        self._variables['Q'] = 0.0
+        self._variables['Mq'] = 0.0
+        self._variables['Sq'] = 0.0
+        self._variables['R'] = 0.0
+        self._variables['F'] = 0.0
+        self._variables['QP'] = 0.0
+        self._variables['BQ'] = 0.0
+        self._variables['TP'] = 0.0
+        self._variables['TQ'] = 0.0
+        self._variables['PSP'] = 0.0
+        self._variables['WpSum'] = 0.0
+        self._variables['WqSum'] = 0.0
+        self._variables['Reward'] = 0.0
+
+        self._operations.append(('Resetting', 'var_mult', 'Vth', 'O'))
+        self._operations.append(('E', 'var_linear', 'Beta_m', 'E', 'Resetting'))
+        self._operations.append(('SumPSP', 'reduce_sum', 'PSP'))
+        self._operations.append(('V', 'minus', 'SumPSP', 'E[updated]'))
+        self._operations.append(('Mp', 'var_linear', 'Beta_m', 'Mp', 'WpSum'))
+        self._operations.append(('Sp', 'var_linear', 'Beta_s', 'Sp', 'WpSum'))
+        self._operations.append(('P', 'minus', 'Mp[updated]', 'Sp[updated]'))
+        self._operations.append(('Mq', 'var_linear', 'Beta_m', 'Mq', 'WpSum'))
+        self._operations.append(('Sq', 'var_linear', 'Beta_s', 'Sq', 'WpSum'))
+        self._operations.append(('Q', 'minus', 'Mq[updated]', 'Sq[updated]'))
+        self._operations.append(('RTmp', 'var_mult', 'Beta_s', 'R'))
+        self._operations.append(('', 'var_linear', 'Beta_s', 'R'))
+
+
+
+NeuronModel.register("qlif", QLIFModel)
+
+
+class SELIFModel(NeuronModel):  #Exponential Model
+    """
+    SpikeProp LIF 3-kernel model:
+
+
+    V[t] = WgtSum[t-1] - E[t-1]
+    I[t] = spike_func(V[t])
+    M[t] = betaM * M[t-1] + I[t]
+    S[t] = betaS * S[t-1] + I[t]
+    E[t] = betaM * E[t-1] + Vth * I[t]
+    O[t] = M[t] − S[t]
+    """
+
+    def __init__(self,
+                 tau_m=12.0,
+                 tau_p=6.0,
+                 tau_q=2.0,
+                 tau_r=16.0,
+                 v_th=1.0,
+                 v_reset=2.0,
+                 outlayer=False,
+                 **kwargs
+                 ):
+        super(SELIFModel, self).__init__()
+        from spaic.Learning.TRUE_Learner import TRUE_SpikeProp
+        # initial value for state variables
+        self._variables['[2]O'] = 0.0
+        self._variables['V'] = 0.0
+        self._variables['dV'] = 0.0
+        self._variables['S'] = 0.0
+        self._variables['WgtSum'] = 0.0
+        self.tau_m = tau_m
+        self.tau_e = tau_p
+        self.tau_s = tau_q
+        self.tau_r = tau_r
+        self.v_th = v_th
+        self.v_reset = 1.0 * v_th
+        self.outlayer = outlayer
+
+        self.beta = tau_p / tau_q
+        self.V0 = (1 / (self.beta - 1)) * (self.beta ** (self.beta / (self.beta - 1)))
+        # self.delat_m = self.tau_m/(self.tau_m-self.tau_s)
+        # self.delat_s = self.tau_s/(self.tau_m-self.tau_s)
+        # self.delat_ms = self.tau_m*self.tau_s/(self.tau_m-self.tau_s)
+
+        self.update_op_code = ('[2]O', self.update, 'WgtSum[updated]')  # 'WgtSum[updated]'
+
+        self.return_op_code = (None, self.return_V, [])
+
+        self.initial_op_code = (None, self.initial, [])
+
+        '''
+            V(t) = M(t) − S(t) − E(t)
+            I^n[t] = V0 * WgtSum^n[t-1] #sum(w * O^(n-1)[t])
+            M^n[t] = betaM * M^n[t-1] + I^n[t-1]
+            S^n[t] = betaS * S^n[t-1] + I^n[t-1]
+            E^n[t] = betaM * E^n[t-1] + Vth * O^n[t-1]
+
+            O^n[t] = spike_func(V^n[t-1])
+        '''
+
+    def attach_learner(self, learner):
+        self.learner = learner
+
+    def build(self, shape, backend):
+        self.dt = backend.dt
+        self.M_initial = torch.zeros(shape, device=backend.device)
+        self.S_initial = torch.zeros(shape, device=backend.device)
+        self.R_initial = torch.zeros(shape, device=backend.device)
+        self.V_initial = torch.zeros(shape, device=backend.device)
+        self.beta_m = np.exp(-backend.dt / self.tau_m)
+        self.beta_s = np.exp(-backend.dt / self.tau_s)
+        self.beta_e = np.exp(-backend.dt / self.tau_e)
+        self.beta_r = np.exp(-backend.dt / self.tau_r)
+        self.running_var = None
+        self.running_mean = None
+        self.decay = 0.9999
+        self.initial()
+        self.rec_E = []
+
+    def initial(self):
+        self.M = self.M_initial
+        self.S = self.S_initial
+        self.R = self.R_initial
+        self.V = self.V_initial
+        self.O = None
+        self.rec_E = []
+
+    def norm_hook(self, grad):
+        if self.running_var is None:
+            self.running_var = torch.norm(grad, dim=0) * 0
+            self.running_mean = torch.mean(grad, dim=0) * 0
+        else:
+            self.running_var = self.decay * self.running_var + (1 - self.decay) * torch.norm(grad, dim=0)
+            self.running_mean = self.decay * self.running_mean + (1 - self.decay) * torch.mean(grad, dim=0)
+        return (grad - self.running_mean) / (1.0e-10 + self.running_var)
+
+    def update(self, WgtSum):
+        # with torch.no_grad():
+        #     self.dV = self.E / self.tau_m +self.S / self.tau_s - self.M / self.tau_m
+        I = self.V0 * WgtSum
+        # WgtSum.register_hook(self.norm_hook)
+
+        if I.dim() == self.M.dim() + 1:
+            Ii = I[:, 0, ...]
+            I0 = I[:, 1, ...]
+            self.M = self.beta_e * self.M + (Ii - I0 / self.tau_e)
+            self.S = self.beta_s * self.S + (Ii - I0 / self.tau_s)
+        else:
+            self.M = self.beta_e * self.M + I
+            self.S = self.beta_s * self.S + I
+
+        if self.O is not None:
+            Oi = self.O[:, 0, ...] #+ 0.9*self.O[:, 0, ...].detach()  # *self.O[:, 0, ...].gt(0.0)
+            Ot = self.O[:, 1, ...] #+ 0.9*self.O[:, 1, ...].detach()
+        else:
+            Oi = 0.0
+            Ot = 0.0
+
+
+        # expv = torch.clamp_max(torch.exp(2.5 * self.V)-1, 12)
+        expv = 2.0*torch.pow(torch.clamp(self.V,-10,self.v_th), 2.0)
+        self.R = self.beta_r*self.R + (1-self.beta_r)*self.V + 10.0*(Oi-Ot/self.tau_r)
+        self.dV = (expv - self.V + (self.M - self.S) + 0.5-0.5*self.R) / self.tau_m
+        # with torch.no_grad():
+        #     self.ddV = (self.dV * (0.2 * expv - 1) + self.S / self.tau_s - self.M / self.tau_e) / self.tau_m
+        #     self.dV2 = self.dV + self.ddV * self.dt
+        self.V = self.V + self.dV * self.dt - self.v_reset*(Oi-Ot/self.tau_m)# + self.ddV * self.dt ** 2 / 2.0
+        # self.P = self.M + self.S
+
+
+        self.O = self.learner.threshold(self.V, self.dV, self.v_th)
+        #
+        # self.rec_E.append(self.Vmax)
+        # if (I is not None) and (I.requires_grad == True):
+        #     I.retain_grad()
+        #     self.rec_E.append(I)
+
+        return self.O
+
+    def return_V(self):
+        return self.V
+
+    def return_M(self):
+        return self.M
+
+    def return_S(self):
+        return self.S
+
+    def return_dV(self):
+        return self.dV
+
+    @property
+    def E_values(self):
+        return torch.stack(self.rec_E, dim=-1).cpu().detach().numpy()
+
+    @property
+    def E_grads(self):
+        grads = []
+        for v in self.rec_E:
+            if v.grad is not None:
+                grads.append(v.grad.cpu().numpy())
+            else:
+                grads.append(torch.zeros_like(v).cpu().numpy())
+        grads = np.stack(grads[1:], axis=-1)
+        return grads
+NeuronModel.register("selif", SELIFModel)
+
+class SLIFModel(NeuronModel):
+    """
+    SpikeProp LIF 3-kernel model:
+
+
+    V[t] = WgtSum[t-1] - E[t-1]
+    I[t] = spike_func(V[t])
+    M[t] = betaM * M[t-1] + I[t]
+    S[t] = betaS * S[t-1] + I[t]
+    E[t] = betaM * E[t-1] + Vth * I[t]
+    O[t] = M[t] − S[t]
+    """
+
+    def __init__(self,
+                 tau_m=20.0,
+                 tau_p=20.0,
+                 tau_q=8.0,
+                 v_th=1.0,
+                 v_reset=2.0,
+                 outlayer=False,
+                 ):
+        super(SLIFModel, self).__init__()
+        from spaic.Learning.TRUE_Learner import TRUE_SpikeProp
+        # initial value for state variables
+        self._variables['[2]O'] = 0.0
+        self._variables['V'] = 0.0
+        self._variables['dV'] = 0.0
+        self._variables['S'] = 0.0
+        self._variables['Isyn'] = 0.0
+        self.tau_m = tau_m
+        self.tau_e = tau_p
+        self.tau_s = tau_q
+        self.v_th = v_th
+        self.v_reset = 5.0 * v_th
+        self.outlayer = outlayer
+
+        self.beta = tau_m / tau_q
+        self.V0 = (1 / (self.beta - 1)) * (self.beta ** (self.beta / (self.beta - 1)))
+        # self.delat_m = self.tau_m/(self.tau_m-self.tau_s)
+        # self.delat_s = self.tau_s/(self.tau_m-self.tau_s)
+        # self.delat_ms = self.tau_m*self.tau_s/(self.tau_m-self.tau_s)
+
+        self.update_op_code = ('[2]O', self.update, 'Isyn[updated]')  # 'WgtSum[updated]'
+
+        self.return_op_code = (None, self.return_V, [])
+
+        self.initial_op_code = (None, self.initial, [])
+
+        '''
+            V(t) = M(t) − S(t) − E(t)
+            I^n[t] = V0 * WgtSum^n[t-1] #sum(w * O^(n-1)[t])
+            M^n[t] = betaM * M^n[t-1] + I^n[t-1]
+            S^n[t] = betaS * S^n[t-1] + I^n[t-1]
+            E^n[t] = betaM * E^n[t-1] + Vth * O^n[t-1]
+
+            O^n[t] = spike_func(V^n[t-1])
+        '''
+
+    def attach_learner(self, learner):
+        self.learner = learner
+
+    def build(self, shape, backend):
+        self.dt = backend.dt
+        self.M_initial = torch.zeros(shape, device=backend.device)
+        self.S_initial = torch.zeros(shape, device=backend.device)
+        self.E_initial = torch.zeros(shape, device=backend.device)
+        self.V_initial = torch.zeros(shape, device=backend.device)
+        self.O_initial = torch.zeros((1,2,1), device=backend.device)
+        self.beta_m = np.exp(-backend.dt / self.tau_m)
+        self.beta_s = np.exp(-backend.dt / self.tau_s)
+        self.beta_e = np.exp(-backend.dt / self.tau_e)
+        self.deta_m = (1 - self.dt/(2*self.tau_m))/self.tau_m
+        self.deta_s = (1 - self.dt/(2*self.tau_s))/self.tau_s
+        self.running_var = None
+        self.running_mean = None
+        self.decay = 0.9999
+        self.initial()
+        self.rec_E = []
+
+    def initial(self):
+        self.M = self.M_initial
+        self.S = self.S_initial
+        self.E = self.E_initial
+        self.V = self.V_initial
+        self.O = None
+        self.rec_E = []
+
+    def norm_hook(self, grad):
+        if self.running_var is None:
+            self.running_var = torch.norm(grad, dim=0) * 0
+            self.running_mean = torch.mean(grad, dim=0) * 0
+        else:
+            self.running_var = self.decay * self.running_var + (1 - self.decay) * torch.norm(grad, dim=0)
+            self.running_mean = self.decay * self.running_mean + (1 - self.decay) * torch.mean(grad, dim=0)
+        return (grad - self.running_mean) / (1.0e-10 + self.running_var)
+
+    def update(self, WgtSum):
+        # with torch.no_grad():
+        #     self.dV = self.E / self.tau_m +self.S / self.tau_s - self.M / self.tau_m
+        I = self.V0 * WgtSum
+        # WgtSum.register_hook(self.norm_hook)
+        # Oi = self.O[:, 0, ...]
+        # Ot = self.O[:, 1, ...]
+        if self.O is not None:
+            Oi = 0.1*self.O[:, 0, ...] + 0.9*self.O[:, 0, ...].detach()
+            Ot = 0.1*self.O[:, 1, ...] + 0.9*self.O[:, 1, ...].detach()
+        else:
+            Oi = 0
+            Ot = 0
+
+        if I.dim() == self.M.dim() + 1:
+            Ii = I[:, 0, ...]
+            I0 = I[:, 1, ...]
+            self.M = self.beta_m * self.M + Ii - I0 / self.tau_m - self.v_reset*(Oi-Ot/self.tau_m)
+            self.S = self.beta_s * self.S + Ii - I0 / self.tau_s
+        else:
+            self.M = self.beta_m * self.M + I - self.v_reset*(Oi-Ot/self.tau_m)
+            self.S = self.beta_s * self.S + I
+
+
+
+
+        self.V = self.M - self.S
+        # self.P = self.M + self.S
+        self.dV = self.S*self.deta_s - self.M*self.deta_m
+
+        #
+        # if self.O is not None:
+        #     self.E = self.E*Oi.lt(1.0).float()# + (0.5*self.E.detach() - 0.5*self.E)*Oi.ge(1.0).float()
+        # MSbase = torch.clamp_min(self.M*self.tau_s/(self.S*self.tau_m+1.0e-20), 0)
+        # self.Vmax = self.M*MSbase**self.delat_s - self.S*MSbase**self.delat_m
+
+        self.O = self.learner.threshold(self.V, self.dV, self.v_th)
+        #
+        # self.rec_E.append(self.Vmax)
+        # if (I is not None) and (I.requires_grad == True):
+        #     I.retain_grad()
+        #     self.rec_E.append(I)
+
+        return self.O
+
+    def return_V(self):
+        return self.V
+
+    def return_M(self):
+        return self.M
+
+    def return_S(self):
+        return self.S
+
+    def return_dV(self):
+        return self.dV
+
+    @property
+    def E_values(self):
+        return torch.stack(self.rec_E, dim=-1).cpu().detach().numpy()
+
+    @property
+    def E_grads(self):
+        grads = []
+        for v in self.rec_E:
+            if v.grad is not None:
+                grads.append(v.grad.cpu().numpy())
+            else:
+                grads.append(torch.zeros_like(v).cpu().numpy())
+        grads = np.stack(grads[1:], axis=-1)
+        return grads
+# for ii in range(2):
+#     out.append(test.update(I))
+
+NeuronModel.register("slif", SLIFModel)
+
+
+class SELIFDebugModel(NeuronModel):
+
+    def __init__(self,
+                 tau_m=20.0, tau_p=20.0, tau_q=8.0, v_th=1.0,
+                 outlayer=False
+                 ):
+        super(SELIFDebugModel, self).__init__()
+        from spaic.Learning.TRUE_Learner import TRUE_SpikeProp
+        # initial value for state variables
+        self._variables['[2]O'] = 0.0
+        self._variables['V'] = 0.0
+        self._variables['dV'] = 0.0
+        self._variables['S'] = 0.0
+        self._variables['WgtSum'] = 0.0
+        self._variables['cumV'] = 0.0
+        self.tau_m = tau_m
+        self.tau_e = tau_p
+        self.tau_s = tau_q
+        self.v_th = v_th
+        self.v_reset = 5.0 * v_th
+        self.outlayer = outlayer
+
+        self.beta = tau_m / tau_q
+        self.V0 = (1 / (self.beta - 1)) * (self.beta ** (self.beta / (self.beta - 1)))
+
+
+        self.update_op_code = ('[2]O', self.update, 'WgtSum[updated]')  # 'WgtSum[updated]'
+        self.return_op_code = (None, self.return_V, [])
+        self.initial_op_code = (None, self.initial, [])
+
+    def attach_learner(self, learner):
+        self.learner = learner
+
+    def build(self, shape, backend):
+        self.dt = backend.dt
+        self.M_initial = torch.zeros(shape, device=backend.device)
+        self.S_initial = torch.zeros(shape, device=backend.device)
+        self.V_initial = torch.zeros(shape, device=backend.device)
+        self.beta_m = np.exp(-backend.dt / self.tau_m)
+        self.beta_s = np.exp(-backend.dt / self.tau_s)
+        self.beta_e = np.exp(-backend.dt / self.tau_e)
+        self.initial()
+        self.rec_E = []
+
+    def initial(self):
+        self.M = self.M_initial
+        self.S = self.S_initial
+        self.V = self.V_initial
+        self.cumV = self.V_initial
+        self.O = None
+        self.rec_E = []
+
+    def update(self, WgtSum):
+
+        I = self.V0 * WgtSum
+
+        if I.dim() == self.M.dim() + 1:
+            Ii = I[:, 0, ...]
+            I0 = I[:, 1, ...]
+            self.M = self.beta_e * self.M + (Ii - I0 / self.tau_e)
+            self.S = self.beta_s * self.S + (Ii - I0 / self.tau_s)
+        else:
+            self.M = self.beta_e * self.M + I
+            self.S = self.beta_s * self.S + I
+
+        if self.O is not None:
+            Oi = self.O[:, 0, ...] #+ 0.9*self.O[:, 0, ...].detach()  # *self.O[:, 0, ...].gt(0.0)
+            Ot = self.O[:, 1, ...] #+ 0.9*self.O[:, 1, ...].detach()
+        else:
+            Oi = 0.0
+            Ot = 0.0
+
+
+        # expv = torch.clamp_max(torch.exp(2.5 * self.V)-1, 12)
+        expv = 2.0*torch.pow(torch.clamp(self.V,-10,self.v_th), 2.0)
+        self.dV = (expv - self.V + (self.M - self.S)) / self.tau_m
+        self.V = self.V + self.dV * self.dt - self.v_reset*(Oi-Ot/self.tau_m)
+
+
+
+        self.O = self.learner.threshold(self.V, self.dV, self.v_th)
+
+        return self.O
+
+    def return_V(self):
+        return self.V
+
 class LIFModel(NeuronModel):
     """
     LIF model:
     # V(t) = tuaM * V^n[t-1] + Isyn[t]   # tauM: constant membrane time (tauM=RmCm)
     O^n[t] = spike_func(V^n[t-1])
     """
 
@@ -596,18 +1128,89 @@
 
         self._tau_variables['tauM'] = kwargs.get('tau_m', 8.0)
 
         self._operations.append(('Vtemp', 'var_linear', 'tauM', 'V', 'Isyn[updated]'))
         self._operations.append(('O', 'threshold', 'Vtemp', 'Vth'))
         self._operations.append(('V', 'reset', 'Vtemp',  'O[updated]'))
 
-
 NeuronModel.register("lif", LIFModel)
 
 
+class PLIFModel(NeuronModel):
+    """
+    LIF model:
+    # V(t) = tuaM * V^n[t-1] + Isyn[t]   # tauM: constant membrane time (tauM=RmCm)
+    O^n[t] = spike_func(V^n[t-1])
+    """
+
+    def __init__(self, **kwargs):
+        super(PLIFModel, self).__init__()
+        # initial value for state variables
+
+        # self.neuron_parameters['tau_m'] = kwargs.get('tau_m', 20.0)  # 20
+        # self.neuron_parameters['v_th'] = kwargs.get('v_th', 1)
+        # self.neuron_parameters['v_reset'] = kwargs.get('v_reset', 0.0)
+
+        self._variables['V'] = 0.0
+        self._variables['O'] = 0.0
+        self._variables['Isyn'] = 0.0
+        # self._variables['b'] = 0.0
+        # self._variables['I_che'] = 0.0
+        # self._variables['I_ele'] = 0.0
+        # self._variables['I'] = 0.0
+
+        self._parameter_variables['Vth'] = kwargs.get('v_th', 1)
+        self._constant_variables['Vreset'] = kwargs.get('v_reset', 0.0)
+
+
+        import math
+        tau = kwargs.get('tau_m', 2.0)  # dt/taum
+        tau = -math.log(tau - 1.)
+        self._tau_parameter_variables['tau'] = tau  # dt/taum
+
+        # self.mem = self.mem + ((inputs - self.mem) * self.w.sigmoid()) * self.dt
+        self._operations.append(('tau_temp', 'sigmoid', 'tau'))
+        self._operations.append(('Vtemp', 'minus', 'Isyn[updated]', 'V'))
+        self._operations.append(('Vtemp1', 'var_linear', 'tau_temp', 'Vtemp', 'V'))
+        # self._operations.append(('Vtemp', 'var_linear', 'tauM', 'V', 'Isyn[updated]'))
+        self._operations.append(('O', 'threshold', 'Vtemp1', 'Vth'))
+        self._operations.append(('V', 'reset', 'Vtemp1',  'O'))
+        # self._operations.append(('tau_temp', 'sigmoid', 'tau'))
+        # self._operations.append(('Vtemp', 'var_linear', 'tau_temp', 'V', 'Isyn[updated]'))
+        # self._operations.append(('O', 'threshold', 'Vtemp', 'Vth'))
+        # self._operations.append(('V', 'reset', 'Vtemp', 'O'))
+
+NeuronModel.register("plif", PLIFModel)
+
+
+# class linearDecayLIFModel(NeuronModel):
+#     """
+#     LIF model:
+#     # V(t) = tuaM * V^n[t-1] + Isyn[t]   # tauM: constant membrane time (tauM=RmCm)
+#     O^n[t] = spike_func(V^n[t-1])
+#     """
+#
+#     def __init__(self, **kwargs):
+#         super(ConstantDecayLIFModel, self).__init__()
+#         # initial value for state variables
+#         self._variables['V'] = 0.0
+#         self._variables['O'] = 0.0
+#         self._variables['Isyn'] = 0.0
+#
+#         self._parameter_variables['Vth'] = kwargs.get('v_th', 1)
+#         self._constant_variables['Vreset'] = kwargs.get('v_reset', 0.0)
+#         self._constant_variables['Vdecay'] = kwargs.get('v_decay', 1.0)
+#
+#         self._operations.append(('Vtemp', 'var_linear', 'tauM', 'V', 'Isyn[updated]'))
+#         self._operations.append(('O', 'threshold', 'Vtemp', 'Vth'))
+#         self._operations.append(('Resetting', 'var_mult', 'Vtemp', 'O[updated]'))
+#         self._operations.append(('V', 'minus', 'Vtemp', 'Resetting'))
+#
+# NeuronModel.register("constantdecaylif", ConstantDecayLIFModel)
+
 class ConstantCurrentLIFModel(NeuronModel):
     """
     ConstantCurrentLIF model:
     V(t) = V^n[t-1] + (dt/taum) * (Ureset-V^n[t-1]+I)  # tauM: constant membrane time (tauM=RmCm)  Isyn = I*Weight
     O^n[t] = spike_func(V^n[t-1])
     """
 
@@ -734,27 +1337,22 @@
 
 
 class IZHModel(NeuronModel):
     """
     IZH model:
 
     .. math::
-        V &= V + dt / tauM * (C1 * V * V + C2 * V + C3 - U + I) \\
-
-        V &= V + dt / tauM * (V * (C1 * V + C2) + C3 - U + I)  \\
-
-        U &= U + a. * (b. * V - U) \\
+        V = V + dt / tauM * (C1 * V * V + C2 * V + C3 - U + I)  # tauM=1 此处加tauM是为了添加op时和LIF模型保存一致 \\
+        V = V + dt / tauM * (V* (C1 * V + C2) + C3 - U + I)     # 由上式拆分而来 \\
+        U = U + a. * (b. * V - U) \\
 
-        O^n[t] &= spike\_func(V^n[t-1]) \\
+        O^n[t] = spike\_func(V^n[t-1])
 
-        if V &> Vth, \\
-
-        then V &= C,
-
-        U &= U + d
+        if V > Vth, \\
+        then V = C, U = U + d
 
     References:
         Izhikevich, E. M. (2003). Simple model of spiking neurons. IEEE Transactions on neural networks, 14(6), 1569-1572.
     """
 
     def __init__(self, **kwargs):
         super(IZHModel, self).__init__()
@@ -803,31 +1401,24 @@
 
 
 class aEIFModel(NeuronModel):
     """
     aEIF model:
 
     .. math::
-        V &= V + dt / tauM * (EL - V + EXP - U + I^n[t]) \\
-
-        U &= U + dt / tauW * (a * (V - EL) - U) \\
+        V = V + dt / tauM * (EL - V + EXP - U + I^n[t]) \\
+        U = U + dt / tauW * (a * (V - EL) - U) \\
+        EXP = delta\_t * delta\_t2 * exp(dv\_th/delta\_t2) \\
+        dv = V - EL \\
+        dv\_th = V - Vth
 
-        EXP &= delta\_t * delta\_t2 * exp(dv\_th/delta\_t2) \\
+        O^n[t] = spike\_func(V^n[t-1]) \\
 
-        dv &= V - EL \\
-
-        dv\_th &= V - Vth \\
-
-        O^n[t] &= spike\_func(V^n[t-1]) \\
-
-        If V &> 20: \\
-
-        then V &= EL,
-
-        U &= U + b
+        If V > 20: \\
+        then V = EL, U = U + b
 
     References:
         Brette, R., & Gerstner, W. (2005). Adaptive exponential integrate-and-fire model as an
         effective description of neuronal activity. Journal of neurophysiology, 94(5), 3637-3642.
     """
 
     def __init__(self, **kwargs):
@@ -892,36 +1483,28 @@
 NeuronModel.register("adex", aEIFModel)
 
 
 class GLIFModel(NeuronModel):
     """
     Current GLIF5 model:
 
-    .. math::
-
-        V &= V + dt / C * (I + I1 + I2 - (V - E\_L) / R)  \\
+        V = V + dt / C * (I + I1 + I2 - (V - E_L) / R)
+        Theta_s = Theta_s - dt * b_s * Theta_s
+        I_j = I_j - dt * k_j * I_j (j = 1,2)
+        Theta_v = Theta_v + dt * (a_v * (V - E_L) - b_v * Theta_v)
 
-        Theta\_s &= Theta\_s - dt * b\_s * Theta\_s \\
-
-        I\_j &= I\_j - dt * k\_j * I\_j (j = 1,2) \\
-
-        Theta\_v &= Theta\_v + dt * (a\_v * (V - E\_L) - b\_v * Theta\_v) \\
-
-        v\_th &= Theta\_v + Theta\_s + Theta\_inf \\
-
-        O &= spike\_func(V) \\
+        v_th = Theta_v + Theta_s + Theta_inf
+        O = spike_func(V)
 
         Reset function:
-        V &= E\_L + f\_v * (V - E\_L) - delta\_v \\
-
-        Theta\_s &= Theta\_s + delta\_Theta\_s \\
-
-        I\_j &= f\_j * I\_j + delta\_I\_j (j = 1, 2) \\
 
-        Theta\_v &= Theta\_v
+        V = E_L + f_v * (V - E_L) - delta_v
+        Theta_s = Theta_s + delta_Theta_s
+        I_j = f_j * I_j + delta_I_j (j = 1, 2)
+        Theta_v = Theta_v
 
     References:
         Teeter, C., Iyer, R., Menon, V., Gouwens, N., Feng, D., Berg, J., ... & Mihalas, S. (2018). Generalized leaky
         integrate-and-fire models classify multiple neuron types. Nature communications, 9(1), 1-15.
     """
 
     def __init__(self, **kwargs):
@@ -963,16 +1546,16 @@
         self._constant_variables['delta_I2'] = kwargs.get('delta_I2', 0.1)
 
         # I_j = I_j - dt * k_j * I_j
         self._operations.append(('I1temp', 'var_linear', 'k1', 'I1', 'I1'))
         self._operations.append(('I2temp', 'var_linear', 'k2', 'I2', 'I2'))
 
         # I_sum = I + I1 + I2
-        self._operations.append(('I_sum', 'add', 'I1temp', 'I2temp'))
-        self._operations.append(('I_sum', 'add', 'I_sum', 'Isyn[updated]'))
+        self._operations.append(('I_sum1', 'add', 'I1temp', 'I2temp'))
+        self._operations.append(('I_sum', 'add', 'I_sum1', 'Isyn[updated]'))
 
         # dv = V - E_L
         self._operations.append(('dv', 'minus', 'V', 'E_L'))
 
         # V_up = I + I1 + I2 - (V - E_L) / R
         self._operations.append(('V_up', 'var_linear', 'dv', 'R', 'I_sum'))
 
@@ -993,17 +1576,17 @@
         self._operations.append(('Theta', 'add', 'Theta_v[updated]', 'Theta_s_temp'))
         self._operations.append(('Vth', 'add', 'Theta', 'Theta_inf'))
 
         self._operations.append(('O', 'threshold', 'Vtemp', 'Vth[updated]'))
 
         # V = E_L + f_v * (V - E_L) - delta_v
         self._operations.append(('dv_reset', 'minus', 'Vtemp', 'E_L'))
-        self._operations.append(('Vreset', 'var_linear', 'f_v', 'dv_reset', 'E_L'))
-        self._operations.append(('Vreset', 'minus', 'Vreset', 'delta_v'))
-        self._operations.append(('Vreset', 'minus', 'Vreset', 'Vtemp'))
+        self._operations.append(('Vreset1', 'var_linear', 'f_v', 'dv_reset', 'E_L'))
+        self._operations.append(('Vreset2', 'minus', 'Vreset1', 'delta_v'))
+        self._operations.append(('Vreset', 'minus', 'Vreset2', 'Vtemp'))
 
         self._operations.append(('V', 'var_linear', 'Vreset', 'O[updated]', 'Vtemp'))
 
         # Theta_s = Theta_s + delta_Theta_s
         self._operations.append(('Theta_s', 'var_linear', 'delta_Theta_s', 'O[updated]', 'Theta_s_temp'))
 
         # I_j = f_j * I_j + delta_I_j (j = 1, 2)
@@ -1264,15 +1847,14 @@
         self._operations.append(('V', 'add', 'Resetting1', 'Resetting3'))
         self._operations.append(('Resetting_theta', 'var_mult', 'O[updated]', 'th_inc'))
         self._operations.append(('theta[stay]', 'add', 'theta_temp', 'Resetting_theta'))
 
 
 NeuronModel.register("lifstdp_ex", LIFSTDPEXModel)
 
-
 class ALIFSTDPEXModel(NeuronModel):
     """
     LIF model:
     V(t) = decay_v * (v - v_rest) + v_rest + I^n[t]
     I^n[t] = V0 * Isyn^n[t]  #V0 = 1
     theta(t) = decay_th * theta[t-1]
     if v >= (vth + theta) then s_out = 1; else s_out = 0;
@@ -1320,15 +1902,14 @@
         self._operations.append(('Resetting_theta1', 'var_mult', 'O[updated]', 'th_inc'))
         self._operations.append(('Resetting_theta', 'var_mult', 'Resetting_theta1', 'Vth_theta'))
         self._operations.append(('theta[stay]', 'add', 'theta_temp', 'Resetting_theta'))
 
 
 NeuronModel.register("alifstdp_ex", ALIFSTDPEXModel)
 
-
 class LIFSTDPIHModel(NeuronModel):
     """
     LIF model:
     V(t) = decay_v * (v - v_rest) + v_rest + I^n[t]
     I^n[t] = V0 * Isyn^n[t]  #V0 = 1
 
     Reset:
@@ -1436,34 +2017,55 @@
         self._operations.append(('U', 'var_linear', 'tau', 'dU', 'U'))
         self._operations.append(('O', 'relu', 'U[updated]'))
 
 
 NeuronModel.register("meanfield", MeanFieldModel)
 
 
+class SimpleRateModel(NeuronModel):
+    """
+    Rate model  "
+
+    U = U + dt/tau * (sigmoid(Iext + WgtSum) - U)
+    (WgtSum = weight*O_pre)
+    """
+    def __init__(self, **kwargs):
+        super(MeanFieldModel, self).__init__()
+        self._membrane_variables['tau'] = kwargs.get('tau', 1.0)
+
+        self._variables['Iext'] = 0.0
+        self._variables['WgtSum'] = 0.0
+        self._variables['U'] = 0.0
+
+        self._operations.append(('Isum', 'add', 'WgtSum', 'Iext'))
+        self._operations.append(('F', 'sigmoid', 'Isum'))
+        self._operations.append(('dU', 'minus', 'F', 'U'))
+        self._operations.append(('U', 'var_linear', 'tau', 'dU', 'U'))
+
+
 class Darwin_CLIF(NeuronModel):
     """
     I = I*P4 + Wgt_sum
     V = V*P0 + I + P1
     """
 
     def __init__(self, **kwargs):
         super(Darwin_CLIF, self).__init__()
         self.dt = kwargs.get('dt', 0.1)
         self.tau_m = kwargs.get('tau_m', 12.0)
         self.tau_s = kwargs.get('tau_s', 8.0)
         self.bias = kwargs.get('bias', 0.0)
         self.v_th = kwargs.get('v_th', 16384)
 
-        self._constant_variables['P0'] = np.round(np.exp(-self.dt / self.tau_m) * 2.0 ** 16) / 2.0 ** 16 #non-negative
-        self._constant_variables['P4'] = np.round(np.exp(-self.dt / self.tau_s) * 2.0 ** 16) / 2.0 ** 16 #non-negative
+        self._constant_variables['P0'] = np.round(np.exp(-self.dt / self.tau_m) * 2.0 ** 8) / 2.0 ** 8 #non-negative
+        self._constant_variables['P4'] = np.round(np.exp(-self.dt / self.tau_s) * 2.0 ** 8) / 2.0 ** 8 #non-negative
         self._constant_variables['P1'] = np.round(self.bias*2.0**15)/2.0*15
         self._constant_variables['Vth'] = self.v_th
 
-        self._variables['V'] = 0.0
+        self._variables['V'] = uniform(10000, 15000)
         self._variables['I'] = 0.0
         self._variables['O'] = 0.0
         self._variables['Isyn'] = 0.0 # named WgtSum in Darwin
 
         self._operations.append((['V', 'I', 'O'], self.update, ['V', 'I', 'Isyn', 'P0', 'P4', 'P1', 'Vth']))
 
     def update(self, V, I, Isyn, P0, P4, P1, Vth):
@@ -1473,17 +2075,92 @@
         V = V - V*O
         return V, I, O
 
     def quantize_16(self, x):
         x = torch.round(torch.clamp(x+2**15, 0, 2**16)) - 2**15
         return x
 
-
 NeuronModel.register("darwin_clif", Darwin_CLIF)
 
 
+class Darwin_ALIF(NeuronModel):
+    """
+    Adaptive threshold LIF
+    I = I*P4 + Wgt_sum
+    V = V*P0 + I + P1
+    Vth = Vth*P2 + C1
+    if spike:
+    Vth = Vth + C2
+    """
+
+    def __init__(self, **kwargs):
+        super(Darwin_ALIF, self).__init__()
+        self.dt = kwargs.get('dt', 0.1)
+        self.tau_m = kwargs.get('tau_m', 12.0)
+        self.tau_s = kwargs.get('tau_s', 8.0)
+        self.bias = kwargs.get('bias', 0.0)
+        self.v_th = kwargs.get('v_th', 16384)
+
+        self._constant_variables['P0'] = np.round(np.exp(-self.dt / self.tau_m) * 2.0 ** 8) / 2.0 ** 8  # non-negative
+        self._constant_variables['P4'] = np.round(np.exp(-self.dt / self.tau_s) * 2.0 ** 8) / 2.0 ** 8  # non-negative
+        self._constant_variables['P1'] = np.round(self.bias * 2.0 ** 15) / 2.0 * 15
+        self._constant_variables['P2'] = 0.999
+        self._constant_variables['C1'] = np.round(self.v_th*0.001)
+        self._constant_variables['C2'] = np.round(self.v_th*0.2)
+
+        self._variables['Vth'] = self.v_th
+        self._variables['V'] = uniform(-30000, 15000)
+        self._variables['I'] = 0.0
+        self._variables['O'] = 0.0
+        self._variables['Isyn'] = 0.0  # named WgtSum in Darwin
+
+        self._operations.append((['V', 'I', 'O', 'Vth'], self.update, ['V', 'I', 'Isyn', 'P0', 'P4', 'P1', 'Vth', 'P2', 'C1', 'C2']))
+
+    def update(self, V, I, Isyn, P0, P4, P1, Vth, P2, C1, C2):
+        I = self.quantize_16(I * P4 + Isyn)
+        V = self.quantize_16(V * P0 + I + P1)
+        O = (V > Vth).to(torch.float)
+        V = V - V * O
+        Vth = P2*Vth + C1 + O*C2
+        return V, I, O, Vth
+
+    def quantize_16(self, x):
+        x = torch.round(torch.clamp(x + 2 ** 15, 0, 2 ** 16)) - 2 ** 15
+        return x
+
+
+NeuronModel.register("darwin_alif", Darwin_ALIF)
+class Darwin_Random(NeuronModel):
+
+    def __init__(self, **kwargs):
+        super(Darwin_Random, self).__init__()
+        self.dt = kwargs.get('dt', 0.1)
+        self.tau_m = kwargs.get("tau_m", 10.0)
+        self.bias = kwargs.get('bias', 0.0)
+        self.std = kwargs.get('std', 0.0)
+        self.v_th = kwargs.get('v_th', 15000)
+
+        self._variables['V'] = uniform(10000, 15000)
+        self._variables['O'] = 0.0
+
+        self._constant_variables['P0'] = np.round(np.exp(-self.dt / self.tau_m) * 2.0 ** 16) / 2.0 ** 16  # non-negative
+        self._constant_variables['bias'] =  np.round(self.bias)
+        self._constant_variables['std'] = np.round(self.std)
+        self._constant_variables['Vth'] = self.v_th
+
+        self._operations.append((['V', 'O'], self.update, ['V', 'P0', 'bias', 'std', 'Vth']))
+
+    def update(self, V, P0, bias, std, Vth):
+        V = P0*V + torch.round(std*torch.rand_like(V)-std/2.0) + bias
+        O = (V > Vth).to(torch.float)
+        V = V - V * O
+        return V, O
+
+
+NeuronModel.register("darwin_random", Darwin_Random)
+
```

### Comparing `SPAIC-0.6.1a0/spaic/Neuron/Node.py` & `SPAIC-0.6.2.0.0/spaic/Neuron/Node.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 @filename: Node
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 
 @description:
 定义神经网络的输入输出接口
 """
-from ..Network.Assembly import Assembly
+from spaic.Network.Assembly import Assembly
 import torch
 import numpy as np
-from ..Backend.Backend import Op
+from spaic.Backend.Backend import Op
 class Node(Assembly):
     '''Base class for input encoder and output decoders.
     '''
     _class_label = '<nod>'
     _is_terminal = True
 
     def __init__(self, shape=None, num=None, dec_target=None, dt=None, coding_method=('poisson', 'spike_counts', '...'),
                  coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
         super(Node, self).__init__()
 
-        self._node_sub_class = None
         self._dt = dt
         self._time = kwargs.get('time', None)
         self.coding_var_name = coding_var_name
         position = kwargs.get('position', None)
         if position == None:
             self.position = []
         else:
@@ -38,15 +37,15 @@
         if coding_method == ('poisson', 'spike_counts', '...'):
             raise ValueError('Please specify the coding method such as poisson or spike_counts')
         else:
             self.coding_method = coding_method.lower()  # The name of coding method
 
         self.coding_var_name = coding_var_name
 
-        if coding_method == 'null':
+        if coding_method.lower() == 'null':
             self.is_encoded = True
         else:
             self.is_encoded = kwargs.get('is_encoded', False)
 
         # 单神经元多脉冲的语音数据集的shape包含脉冲时间以及发放神经元标签，所以不能通过np.prod(shape)获取num，最好还是外部输入num
         assert num is not None or shape is not None, "One of the shape and number must not be None"
         if num is None:
@@ -56,24 +55,24 @@
         else:
             self.num = num
 
         self.num = int(self.num)  # 统一数据格式为Python内置格式
 
         if shape is None:
             if self.is_encoded:
-                self.shape = (1, 1, self.num)
+                self.shape = [1, 1, self.num]
             else:
-                self.shape = (1, self.num)
+                self.shape = [1, self.num]
         else:
             if coding_method == 'mstb' or coding_method == 'sstb':
                 self.shape = (1, self.num)
             elif self.is_encoded:
-                self.shape = tuple([1, 1] + list(shape))
+                self.shape = [1, 1] + list(shape)
             else:
-                self.shape = tuple([1] + list(shape))
+                self.shape = [1] + list(shape)
 
         if node_type == ('excitatory', 'inhibitory', 'pyramidal', '...'):
             self.type = []
         elif isinstance(node_type, list):
             self.type = node_type
         else:
             self.type = [node_type]
@@ -142,44 +141,45 @@
             The subclass of coding object, e.g. an 'PoissonEncoding', 'Spike_Counts'.
         '''
 
         raise NotImplementedError
 
     def torch_coding(self, source: torch.Tensor, target: torch.Tensor , device: str) -> torch.Tensor:
         '''
-
         Args:
-            source (): It is input spike trains for encoding class and output spike trains for decoding class.
-            target (): It is None  for encodoing class and labels for decoding class.
-            device (): CPU or CUDA, this parameter is taken from backend
-
+            source : It is input spike trains for encoding class and output spike trains for decoding class.
+            target : It is None  for encodoing class and labels for decoding class.
+            device : CPU or CUDA, this parameter is taken from backend
         Returns:
-
         '''
+
         raise NotImplementedError
 
     def numpy_coding(self, source, target, device):
         raise NotImplementedError
 
     def tensorflow_coding(self, source, target, device):
         raise NotImplementedError
 
     def build(self, backend):
         self._backend = backend
-        raise NotImplementedError
+        self.data_type = backend.data_type
 
     def __call__(self, data=None):
 
         if isinstance(self, Encoder) or isinstance(self, Generator) or isinstance(self, Reward):
             if isinstance(data, np.ndarray):
                 self.source = data
                 batch_size = data.shape[0]
             elif isinstance(data, torch.Tensor):
                 self.source = data
                 batch_size = data.shape[0]
+            elif isinstance(data, list) and self.coding_method=="mstb":
+                self.source = data
+                batch_size = len(self.source)
             elif hasattr(data, '__iter__'):
                 self.source = np.array(data)
                 batch_size = self.source.shape[0]
             else:
                 self.source = np.array([data])
                 batch_size = 1
 
@@ -291,15 +291,15 @@
     def reset(self):
         # Called at the start of each epoch
         self.init_state()
 
     def build(self, backend):
         self._backend = backend
         self.sim_name = backend.backend_name
-        self.device = backend.device
+        self.device = backend.device0
 
         # if self.dt is None:
         #     self.dt = backend.dt
         if self.batch_size is not None:
             self._backend.set_batch_size(self.batch_size)
 
         # if self.sim_name == 'pytorch':
@@ -400,15 +400,15 @@
     def reset(self):
         # Called at the start of each epoch
         self.init_state()
 
     def build(self, backend):
         self._backend = backend
         self.sim_name = backend.backend_name
-        self.device = backend.device
+        self.device = backend.device0
         # if self.dt is None:
         #     self.dt = backend.dt
 
         output_name = self.dec_target.id + ':' + '{'+self.coding_var_name+'}'
         self.init_op_to_backend(None, self.init_state, [])
         backend.register_standalone(Op(None, self.get_output, [output_name], owner=self))
 
@@ -466,15 +466,16 @@
 
         Reward._coding_subclasses[name] = coding_class
 
     def init_state(self):
         self.index = 0
 
     # stand alone operation: get reward from output activities
-    def get_reward(self, output):
+    def get_reward(self, output=np.empty(0)):
+        self.device = self._backend.device0
         if (self.index % self.dec_sample_step) == 0:
             self.index = 0
             shape = list(output.shape)
             dec_shape = [self.dec_sample_step] + shape
             if type(output).__name__ == 'Tensor':
                 self.records = torch.zeros(dec_shape, device=self.device)
             else:
@@ -489,24 +490,26 @@
             else:
                 reward = self.numpy_coding(self.records, self.source, self.device)
         return reward
 
     def build(self, backend):
         self._backend = backend
         self.sim_name = backend.backend_name
-        self.device = backend.device
+        self.data_type = backend.data_type
+        self.device = backend.device0
         # if self.dt is None:
         #     self.dt = backend.dt
-
-        output_name = self.dec_target.id + ':' + '{'+self.coding_var_name+'}'
         self.init_op_to_backend(None, self.init_state, [])
         reward_name = 'Output_Reward'
-        self.variable_to_backend(reward_name, self.reward_shape, value=0.0) # shape还是要让具体的子类定义吧
-
-        backend.register_standalone(Op(reward_name, self.get_reward, [output_name], owner=self))
+        self.variable_to_backend(reward_name, self.reward_shape, value=0.0)  # shape还是要让具体的子类定义吧
+        if self.dec_target is not None:
+            output_name = self.dec_target.id + ':' + '{'+self.coding_var_name+'}'
+            backend.register_standalone(Op(reward_name, self.get_reward, [output_name], owner=self))
+        else:
+            backend.register_standalone(Op(reward_name, self.get_reward, [], owner=self))
 
 
 class Generator(Node):
     '''
         Two generator method are provided, as shown below (key: class):
         1. 'poisson_generator': Poisson_Generator,
         2. 'cosine_generator': Cosine_Generator
@@ -590,15 +593,15 @@
             self.new_input = False
         self.index += 1
         return self.all_spikes[self.index-1]
 
     def build(self, backend):
         self._backend = backend
         self.sim_name = backend.backend_name
-        self.device = backend.device
+        self.device = backend.device0
         # if self.dt is None:
         #     self.dt = backend.dt
 
         if self.sim_name == 'pytorch':
             singlestep_spikes = torch.zeros(self.shape, device=self.device)
         else:
             singlestep_spikes = np.zeros(self.shape)
@@ -689,14 +692,14 @@
             else:
                 self.action = self.numpy_coding(self.records, self.source, self.device)
         return 0
 
     def build(self, backend):
         self._backend = backend
         self.sim_name = backend.backend_name
-        self.device = backend.device
+        self.device = backend.device0
         # if self.dt is None:
         #     self.dt = backend.dt
 
         output_name = self.dec_target.id + ':' + '{'+self.coding_var_name+'}'
         self.init_op_to_backend(None, self.init_state, [])
         backend.register_standalone(Op(None, self.get_action, [output_name], owner=self))
```

### Comparing `SPAIC-0.6.1a0/spaic/Neuron/Rewards.py` & `SPAIC-0.6.2.0.0/spaic/Neuron/Rewards.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 
     def __init__(self,shape=None, num=None, dec_target=None, dt=None, coding_method=('poisson', 'spike_counts', '...'), coding_var_name='O', node_type=('excitatory', 'inhibitory', 'pyramidal', '...'), **kwargs):
         super(Environment_Reward, self).__init__(shape, num, dec_target, dt, coding_method, coding_var_name, node_type, **kwargs)
 
     def torch_coding(self, record, target, device):
         # the shape of record is (time_step, batch_size, n_neurons)
-        reward = torch.tensor(target, device=device)
+        reward = torch.tensor(target, device=device, dtype=self.data_type)
         return reward
 
 Reward.register('environment_reward', Environment_Reward)
 
 
 class Classifiy_Reward(Reward):
```

### Comparing `SPAIC-0.6.1a0/spaic/__init__.py` & `SPAIC-0.6.2.0.0/spaic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,48 @@
 @project: SPAIC
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 
 @description: 
 """
 
-VERSION = (0, 6, 1, 'a', 0)
+VERSION = (0, 6, 2, 0, 0)
 __version__ = '.'.join(map(lambda x: str(x), VERSION))
 
 # print('__file__={0:<35} | __name__={1:<20} | __package__={2:<20}'.format(__file__,__name__,str(__package__)))
 from .Network import Network, Connection, Assembly, Projection, Synapse
-from .Neuron import NeuronGroup
-
+from .Neuron import NeuronGroup, NeuronModel
 from .Neuron import Node, Encoders, Decoders, Generators, Rewards, Actions
 from .Neuron.Node import Encoder, Decoder, Generator, Reward, Action
 from .Neuron.Module import Module
-from .Network.BaseModule import BaseModule
+from .Network.BaseModule import BaseModule, Op
 from .Network.ConnectPolicy import ExcludedTypePolicy, IndexConnectPolicy, IncludedTypePolicy
 from .Backend.Backend import Backend
 from .Backend.Torch_Backend import Torch_Backend
 # from .Backend.Tensorflow_Backend import Tensorflow_Backend
 from .Monitor.Monitor import StateMonitor, SpikeMonitor
-# from .Learning.Rate_Modulation import Rate_Modulate
+from .Learning.Rate_Modulation import Rate_Modulate
 from .Learning.STCA_Learner import STCA
-# from .Learning.TRUE_Learner import TRUE_SpikeProp
-# from .Learning.BioHashSTDP_Learner import BioHash
+from .Learning.SurrogateBP_Learner import SurrogateBP
+
 from .Learning.Learner import Learner
-from .IO.Dataset import Dataset, CustomDataset, MNIST, FashionMNIST, OctMNIST, PathMNIST, MNISTVoices, cifar10, SHD, SSC
+from .IO.Dataset import Dataset, CustomDataset, MNIST, FashionMNIST, OctMNIST, PathMNIST, MNISTVoices, cifar10, SHD, SSC, \
+    DVS128Gesture
+from .IO.Initializer import BaseInitializer, uniform, normal, xavier_normal, xavier_uniform, kaiming_normal,\
+    kaiming_uniform, constant, sparse
 from .IO.Dataloader import Dataloader
 from .IO.Pipeline import RLPipeline, ReplayMemory
 from .IO.Environment import GymEnvironment
+import numpy as np
 
 from .Library import Network_loader, Network_saver
 
+
+
 # ============== Global variable block for network building ==================
 global_assembly_context_list = list()
 global_assembly_context_omit_start = 10000000000000000000000
 global_assembly_context_omit_end = -1
 global_assembly_init_count = 0
 global_module_name_count = 0
 debug_grad = dict()
+
```

### Comparing `SPAIC-0.6.1a0/spaic/utils/fftweight.py` & `SPAIC-0.6.2.0.0/spaic/utils/fftweight.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/utils/filters.py` & `SPAIC-0.6.2.0.0/spaic/utils/filters.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/utils/gtgram.py` & `SPAIC-0.6.2.0.0/spaic/utils/gtgram.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.1a0/spaic/utils/plot.py` & `SPAIC-0.6.2.0.0/spaic/utils/plot.py`

 * *Files identical despite different names*

