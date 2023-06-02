# Comparing `tmp/SPAIC-0.6.2.0.0.tar.gz` & `tmp/SPAIC-0.6.2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPAIC-0.6.2.0.0.tar", last modified: Fri Jun  2 01:36:33 2023, max compression
+gzip compressed data, was "SPAIC-0.6.2.1.0.tar", last modified: Fri Jun  2 02:55:52 2023, max compression
```

## Comparing `SPAIC-0.6.2.0.0.tar` & `SPAIC-0.6.2.1.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.361873 SPAIC-0.6.2.0.0/
--rw-rw-r--   0 crj       (1000) crj       (1000)    11357 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/LICENSE
--rw-rw-r--   0 crj       (1000) crj       (1000)    13662 2023-06-02 01:36:33.361873 SPAIC-0.6.2.0.0/PKG-INFO
--rw-rw-r--   0 crj       (1000) crj       (1000)    12543 2022-12-09 10:34:18.000000 SPAIC-0.6.2.0.0/README.md
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.349874 SPAIC-0.6.2.0.0/SPAIC.egg-info/
--rw-rw-r--   0 crj       (1000) crj       (1000)    13662 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/PKG-INFO
--rw-rw-r--   0 crj       (1000) crj       (1000)     1901 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/SOURCES.txt
--rw-rw-r--   0 crj       (1000) crj       (1000)        1 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/dependency_links.txt
--rw-rw-r--   0 crj       (1000) crj       (1000)       53 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/requires.txt
--rw-rw-r--   0 crj       (1000) crj       (1000)        6 2023-06-02 01:36:33.000000 SPAIC-0.6.2.0.0/SPAIC.egg-info/top_level.txt
--rw-rw-r--   0 crj       (1000) crj       (1000)     1154 2023-06-02 01:36:33.361873 SPAIC-0.6.2.0.0/setup.cfg
--rw-rw-r--   0 crj       (1000) crj       (1000)      324 2022-12-09 10:34:18.000000 SPAIC-0.6.2.0.0/setup.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.349874 SPAIC-0.6.2.0.0/spaic/
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.353874 SPAIC-0.6.2.0.0/spaic/Backend/
--rw-rw-r--   0 crj       (1000) crj       (1000)    67350 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Backend/Backend.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      154 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Backend/Builder.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    29893 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Backend/Torch_Backend.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      135 2022-11-29 07:15:36.000000 SPAIC-0.6.2.0.0/spaic/Backend/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.353874 SPAIC-0.6.2.0.0/spaic/IO/
--rw-rw-r--   0 crj       (1000) crj       (1000)     6527 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/IO/Dataloader.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    67724 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/IO/Dataset.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5921 2022-09-19 07:10:34.000000 SPAIC-0.6.2.0.0/spaic/IO/Environment.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     4408 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/IO/Initializer.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     7072 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/IO/Pipeline.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      391 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/IO/SignalGenerator.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      136 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/IO/__init__.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5279 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/IO/sampler.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    32180 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/IO/utils.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.353874 SPAIC-0.6.2.0.0/spaic/Learning/
--rw-rw-r--   0 crj       (1000) crj       (1000)    15353 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Backprop_RSTDP.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     8763 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Conv_RSTDP.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     8553 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Conv_STDP.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     2076 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/FiniteDifference.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    16759 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    16941 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/RSTDP.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     3269 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Rate_Modulation.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     3545 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/STBP_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     4755 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/STCA_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    16506 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/STDP_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    10761 2023-06-02 01:33:47.000000 SPAIC-0.6.2.0.0/spaic/Learning/SpikeProp_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     2520 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/SurrogateBP_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    10620 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/Tempotron_Learner.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      571 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/__init__.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     7759 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Learning/surrogate.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/Library/
--rw-rw-r--   0 crj       (1000) crj       (1000)      357 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Library/Library.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    20447 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Library/Network_loader.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    17000 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Library/Network_saver.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      806 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Library/STCA_music_network.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      222 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Library/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/Monitor/
--rw-rw-r--   0 crj       (1000) crj       (1000)    20942 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Monitor/Monitor.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      158 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Monitor/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/Network/
--rw-rw-r--   0 crj       (1000) crj       (1000)    35207 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Assembly.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    11527 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/BaseModule.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    14325 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/Network/ConnectPolicy.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    85318 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Connections.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     3858 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Construct.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5442 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/DelayQueue.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    21572 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Network.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    24642 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Synapse.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    43003 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Network/Topology.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      316 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Network/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/Neuron/
--rw-rw-r--   0 crj       (1000) crj       (1000)     8145 2022-11-10 07:01:11.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Actions.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    23816 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Decoders.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    16388 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Encoders.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     8635 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Generators.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     3952 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Module.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    85703 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Neuron.py
--rw-rw-r--   0 crj       (1000) crj       (1000)    28015 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Node.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     6893 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/Neuron/Rewards.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      316 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/Neuron/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.357874 SPAIC-0.6.2.0.0/spaic/UI/
--rw-rw-r--   0 crj       (1000) crj       (1000)      676 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/UI/OnlineSpikePlot.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      309 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/UI/Visualization.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      134 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/UI/__init__.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     1946 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/__init__.py
-drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 01:36:33.361873 SPAIC-0.6.2.0.0/spaic/utils/
--rw-rw-r--   0 crj       (1000) crj       (1000)      876 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/utils/AnimateScatter.py
--rw-rw-r--   0 crj       (1000) crj       (1000)       24 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/utils/__init__.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5077 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/utils/fftweight.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     8291 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/utils/filters.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     2844 2022-08-16 07:05:57.000000 SPAIC-0.6.2.0.0/spaic/utils/gtgram.py
--rw-rw-r--   0 crj       (1000) crj       (1000)      631 2023-06-02 01:33:56.000000 SPAIC-0.6.2.0.0/spaic/utils/memory.py
--rw-rw-r--   0 crj       (1000) crj       (1000)     5010 2022-08-03 05:27:07.000000 SPAIC-0.6.2.0.0/spaic/utils/plot.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.716548 SPAIC-0.6.2.1.0/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    11357 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/LICENSE
+-rw-rw-r--   0 crj       (1000) crj       (1000)    13672 2023-06-02 02:55:52.716548 SPAIC-0.6.2.1.0/PKG-INFO
+-rw-rw-r--   0 crj       (1000) crj       (1000)    12553 2023-06-02 02:46:37.000000 SPAIC-0.6.2.1.0/README.md
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.704549 SPAIC-0.6.2.1.0/SPAIC.egg-info/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    13672 2023-06-02 02:55:52.000000 SPAIC-0.6.2.1.0/SPAIC.egg-info/PKG-INFO
+-rw-rw-r--   0 crj       (1000) crj       (1000)     1901 2023-06-02 02:55:52.000000 SPAIC-0.6.2.1.0/SPAIC.egg-info/SOURCES.txt
+-rw-rw-r--   0 crj       (1000) crj       (1000)        1 2023-06-02 02:55:52.000000 SPAIC-0.6.2.1.0/SPAIC.egg-info/dependency_links.txt
+-rw-rw-r--   0 crj       (1000) crj       (1000)       53 2023-06-02 02:55:52.000000 SPAIC-0.6.2.1.0/SPAIC.egg-info/requires.txt
+-rw-rw-r--   0 crj       (1000) crj       (1000)        6 2023-06-02 02:55:52.000000 SPAIC-0.6.2.1.0/SPAIC.egg-info/top_level.txt
+-rw-rw-r--   0 crj       (1000) crj       (1000)     1154 2023-06-02 02:55:52.720548 SPAIC-0.6.2.1.0/setup.cfg
+-rw-rw-r--   0 crj       (1000) crj       (1000)      324 2022-12-09 10:34:18.000000 SPAIC-0.6.2.1.0/setup.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.704549 SPAIC-0.6.2.1.0/spaic/
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.704549 SPAIC-0.6.2.1.0/spaic/Backend/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    67350 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Backend/Backend.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      154 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/Backend/Builder.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    29893 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Backend/Torch_Backend.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      135 2022-11-29 07:15:36.000000 SPAIC-0.6.2.1.0/spaic/Backend/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.708549 SPAIC-0.6.2.1.0/spaic/IO/
+-rw-rw-r--   0 crj       (1000) crj       (1000)     6527 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/IO/Dataloader.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    67724 2022-11-10 07:01:11.000000 SPAIC-0.6.2.1.0/spaic/IO/Dataset.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5921 2022-09-19 07:10:34.000000 SPAIC-0.6.2.1.0/spaic/IO/Environment.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     4408 2022-11-10 07:01:11.000000 SPAIC-0.6.2.1.0/spaic/IO/Initializer.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     7072 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/IO/Pipeline.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      391 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/IO/SignalGenerator.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      136 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/IO/__init__.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5279 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/IO/sampler.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    32180 2022-11-10 07:01:11.000000 SPAIC-0.6.2.1.0/spaic/IO/utils.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.712548 SPAIC-0.6.2.1.0/spaic/Learning/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    15353 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/Backprop_RSTDP.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8763 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/Conv_RSTDP.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8553 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/Conv_STDP.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     2076 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/FiniteDifference.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    16759 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    16941 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/RSTDP.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     3269 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/Rate_Modulation.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     3545 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/STBP_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     4755 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/STCA_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    16506 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/STDP_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    10761 2023-06-02 01:33:47.000000 SPAIC-0.6.2.1.0/spaic/Learning/SpikeProp_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     2520 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/SurrogateBP_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    10620 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/Tempotron_Learner.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      571 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/__init__.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     7759 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Learning/surrogate.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.712548 SPAIC-0.6.2.1.0/spaic/Library/
+-rw-rw-r--   0 crj       (1000) crj       (1000)      357 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Library/Library.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    20447 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Library/Network_loader.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    17000 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Library/Network_saver.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      806 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/Library/STCA_music_network.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      222 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/Library/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.712548 SPAIC-0.6.2.1.0/spaic/Monitor/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    20949 2023-06-02 02:46:37.000000 SPAIC-0.6.2.1.0/spaic/Monitor/Monitor.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      158 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/Monitor/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.712548 SPAIC-0.6.2.1.0/spaic/Network/
+-rw-rw-r--   0 crj       (1000) crj       (1000)    35207 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Network/Assembly.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    11527 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Network/BaseModule.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    14325 2022-11-10 07:01:11.000000 SPAIC-0.6.2.1.0/spaic/Network/ConnectPolicy.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    85318 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Network/Connections.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     3858 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Network/Construct.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5442 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Network/DelayQueue.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    21572 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Network/Network.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    24642 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Network/Synapse.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    43003 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Network/Topology.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      316 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/Network/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.716548 SPAIC-0.6.2.1.0/spaic/Neuron/
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8145 2022-11-10 07:01:11.000000 SPAIC-0.6.2.1.0/spaic/Neuron/Actions.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    23816 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Neuron/Decoders.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    16388 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Neuron/Encoders.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8635 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Neuron/Generators.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     3952 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Neuron/Module.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    85703 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Neuron/Neuron.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)    28015 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Neuron/Node.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     6893 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/Neuron/Rewards.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      316 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/Neuron/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.716548 SPAIC-0.6.2.1.0/spaic/UI/
+-rw-rw-r--   0 crj       (1000) crj       (1000)      676 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/UI/OnlineSpikePlot.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      309 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/UI/Visualization.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      134 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/UI/__init__.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     1946 2023-06-02 02:54:31.000000 SPAIC-0.6.2.1.0/spaic/__init__.py
+drwxrwxr-x   0 crj       (1000) crj       (1000)        0 2023-06-02 02:55:52.716548 SPAIC-0.6.2.1.0/spaic/utils/
+-rw-rw-r--   0 crj       (1000) crj       (1000)      876 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/utils/AnimateScatter.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)       24 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/utils/__init__.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5077 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/utils/fftweight.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     8291 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/utils/filters.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     2844 2022-08-16 07:05:57.000000 SPAIC-0.6.2.1.0/spaic/utils/gtgram.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)      631 2023-06-02 01:33:56.000000 SPAIC-0.6.2.1.0/spaic/utils/memory.py
+-rw-rw-r--   0 crj       (1000) crj       (1000)     5010 2022-08-03 05:27:07.000000 SPAIC-0.6.2.1.0/spaic/utils/plot.py
```

### Comparing `SPAIC-0.6.2.0.0/LICENSE` & `SPAIC-0.6.2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/PKG-INFO` & `SPAIC-0.6.2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPAIC
-Version: 0.6.2.0.0
+Version: 0.6.2.1.0
 Summary: The spaic platform simulation training platform is a network construction, forward simulation and learning training platform developed for spiking neural networks.
 Home-page: https://github.com/ZhejianglabNCRC/SPAIC/
 Author: zjlab
 Author-email: hongchf@zhejianglab.com
 Maintainer: hongchaofei
 Maintainer-email: hongchf@zhejianglab.com
 License: Apache-2.0 license
@@ -147,26 +147,26 @@
 ```python
 class ExampleNet(spaic.Network):
      def __init__(self):
         super(ExampleNet, self).__init__()
         
         
         # Create an input node and select the input encoding method
-        self.input = spaic.Node(dataloader, encoding='latency')
+        self.input = spaic.Encoder(dataloader, encoding='latency')
               
         # Establish neurongroups, select neuron types, and set neuron parameter values
         self.layer1 = spaic.NeuronGroup(100, model='clif')
         self.layer2 = spaic.NeuronGroup(10, model='clif')
         
         # Establish connections between Neurongroups
         self.connection1 = spaic.Connection(self.input, self.layer1, link_type='full')
         self.connection2 = spaic.Connection(self.layer1, self.layer2, link_type='full')
         
         # Create an output node and select the output decoding method
-        self.output = spaic.Node(decoding='spike_counts',target=self.layer2)
+        self.output = spaic.Decoder(decoding='spike_counts',target=self.layer2)
 
         # Establish a state detector, which can monitor the state of various objects
         self.monitor1 = spaic.StateMonitor(self.layer1, 'V')
 
         # Add the learning algorithm and select the network structure to be trained 
         self.learner1 = spaic.STCA(0.5, self)
         
@@ -183,27 +183,27 @@
 ```python
 # Initialize the object of the basic network class
 Net = spaic.Network()
 
 # Create a network structure by defining network components in with
 with Net:
     # Create an input node and select the input encoding method
-    input1 = spaic.Node(dataloader, encoding='latency')
+    input = spaic.Encoder(dataloader, encoding='latency')
 
 
     # Establish neurongroups, select neuron types, and set neuron parameter values
     layer1 = spaic.NeuronGroup(100, model='clif')
     layer2 = spaic.NeuronGroup(10, model='clif')
 
     # Establish connections between Neurongroups
     connection1 = spaic.Connection(input1, layer1, link_type='full')
     connection2 = spaic.Connection(layer1, layer2, link_type='full')
 
     # Create an output node and select the output decoding method
-    output1 = spaic.Node(decoding='spike_counts',target=layer2)
+    output = spaic.Decoder(decoding='spike_counts',target=layer2)
 
     # Establish a state detector, which can monitor the state of various objects
     monitor1 = spaic.StateMonitor(layer1, 'V')
 
     # Add the learning algorithm and select the network structure to be trained 
     learner1 = spaic.STCA(0.5, Net)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SPAIC Version: 0.6.2.0.0 Summary: The spaic
+Metadata-Version: 2.1 Name: SPAIC Version: 0.6.2.1.0 Summary: The spaic
 platform simulation training platform is a network construction, forward
 simulation and learning training platform developed for spiking neural
 networks. Home-page: https://github.com/ZhejianglabNCRC/SPAIC/ Author: zjlab
 Author-email: hongchf@zhejianglab.com Maintainer: hongchaofei Maintainer-email:
 hongchf@zhejianglab.com License: Apache-2.0 license Project-URL: Documentation,
 https://spaic.readthedocs.io/ Project-URL: Source Code, https://github.com/
 ZhejianglabNCRC/SPAIC Project-URL: Issue Tracker, https://github.com/
@@ -108,37 +108,37 @@
 loaded ## Network model construction The model can be built in two ways: first,
 like Pytorch's module class inheritance, which is built in the _init_ function,
 and second, like Nengo's with statement. In addition, the existing model
 structure in the model algorithm library can also be introduced into the
 modeling process ### Modeling Method 1: Class Inheritance Form ```python class
 ExampleNet(spaic.Network): def __init__(self): super(ExampleNet, self).__init__
 () # Create an input node and select the input encoding method self.input =
-spaic.Node(dataloader, encoding='latency') # Establish neurongroups, select
+spaic.Encoder(dataloader, encoding='latency') # Establish neurongroups, select
 neuron types, and set neuron parameter values self.layer1 = spaic.NeuronGroup
 (100, model='clif') self.layer2 = spaic.NeuronGroup(10, model='clif') #
 Establish connections between Neurongroups self.connection1 = spaic.Connection
 (self.input, self.layer1, link_type='full') self.connection2 = spaic.Connection
 (self.layer1, self.layer2, link_type='full') # Create an output node and select
-the output decoding method self.output = spaic.Node
+the output decoding method self.output = spaic.Decoder
 (decoding='spike_counts',target=self.layer2) # Establish a state detector,
 which can monitor the state of various objects self.monitor1 =
 spaic.StateMonitor(self.layer1, 'V') # Add the learning algorithm and select
 the network structure to be trained self.learner1 = spaic.STCA(0.5, self) # Add
 optimization algorithm self.optim = spaic.Adam(lr=0.01, schedule='StepLR',
 maxstep=1000) # Initialize the ExampleNet network object Net = ExampleNet() ```
 ### Modeling method 2: Using "with" ```python # Initialize the object of the
 basic network class Net = spaic.Network() # Create a network structure by
 defining network components in with with Net: # Create an input node and select
-the input encoding method input1 = spaic.Node(dataloader, encoding='latency') #
-Establish neurongroups, select neuron types, and set neuron parameter values
+the input encoding method input = spaic.Encoder(dataloader, encoding='latency')
+# Establish neurongroups, select neuron types, and set neuron parameter values
 layer1 = spaic.NeuronGroup(100, model='clif') layer2 = spaic.NeuronGroup(10,
 model='clif') # Establish connections between Neurongroups connection1 =
 spaic.Connection(input1, layer1, link_type='full') connection2 =
 spaic.Connection(layer1, layer2, link_type='full') # Create an output node and
-select the output decoding method output1 = spaic.Node
+select the output decoding method output = spaic.Decoder
 (decoding='spike_counts',target=layer2) # Establish a state detector, which can
 monitor the state of various objects monitor1 = spaic.StateMonitor(layer1, 'V')
 # Add the learning algorithm and select the network structure to be trained
 learner1 = spaic.STCA(0.5, Net) # Add optimization algorithm optim = spaic.Adam
 (lr=0.01, schedule='StepLR', maxstep=1000) ``` ### Modeling method 3: importing
 a model library model and modifying it with functions ```python from
 spaic.Library import ExampleNet Net = ExampleNet() # neuron parameters
```

### Comparing `SPAIC-0.6.2.0.0/README.md` & `SPAIC-0.6.2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -122,26 +122,26 @@
 ```python
 class ExampleNet(spaic.Network):
      def __init__(self):
         super(ExampleNet, self).__init__()
         
         
         # Create an input node and select the input encoding method
-        self.input = spaic.Node(dataloader, encoding='latency')
+        self.input = spaic.Encoder(dataloader, encoding='latency')
               
         # Establish neurongroups, select neuron types, and set neuron parameter values
         self.layer1 = spaic.NeuronGroup(100, model='clif')
         self.layer2 = spaic.NeuronGroup(10, model='clif')
         
         # Establish connections between Neurongroups
         self.connection1 = spaic.Connection(self.input, self.layer1, link_type='full')
         self.connection2 = spaic.Connection(self.layer1, self.layer2, link_type='full')
         
         # Create an output node and select the output decoding method
-        self.output = spaic.Node(decoding='spike_counts',target=self.layer2)
+        self.output = spaic.Decoder(decoding='spike_counts',target=self.layer2)
 
         # Establish a state detector, which can monitor the state of various objects
         self.monitor1 = spaic.StateMonitor(self.layer1, 'V')
 
         # Add the learning algorithm and select the network structure to be trained 
         self.learner1 = spaic.STCA(0.5, self)
         
@@ -158,27 +158,27 @@
 ```python
 # Initialize the object of the basic network class
 Net = spaic.Network()
 
 # Create a network structure by defining network components in with
 with Net:
     # Create an input node and select the input encoding method
-    input1 = spaic.Node(dataloader, encoding='latency')
+    input = spaic.Encoder(dataloader, encoding='latency')
 
 
     # Establish neurongroups, select neuron types, and set neuron parameter values
     layer1 = spaic.NeuronGroup(100, model='clif')
     layer2 = spaic.NeuronGroup(10, model='clif')
 
     # Establish connections between Neurongroups
     connection1 = spaic.Connection(input1, layer1, link_type='full')
     connection2 = spaic.Connection(layer1, layer2, link_type='full')
 
     # Create an output node and select the output decoding method
-    output1 = spaic.Node(decoding='spike_counts',target=layer2)
+    output = spaic.Decoder(decoding='spike_counts',target=layer2)
 
     # Establish a state detector, which can monitor the state of various objects
     monitor1 = spaic.StateMonitor(layer1, 'V')
 
     # Add the learning algorithm and select the network structure to be trained 
     learner1 = spaic.STCA(0.5, Net)
```

### Comparing `SPAIC-0.6.2.0.0/SPAIC.egg-info/PKG-INFO` & `SPAIC-0.6.2.1.0/SPAIC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPAIC
-Version: 0.6.2.0.0
+Version: 0.6.2.1.0
 Summary: The spaic platform simulation training platform is a network construction, forward simulation and learning training platform developed for spiking neural networks.
 Home-page: https://github.com/ZhejianglabNCRC/SPAIC/
 Author: zjlab
 Author-email: hongchf@zhejianglab.com
 Maintainer: hongchaofei
 Maintainer-email: hongchf@zhejianglab.com
 License: Apache-2.0 license
@@ -147,26 +147,26 @@
 ```python
 class ExampleNet(spaic.Network):
      def __init__(self):
         super(ExampleNet, self).__init__()
         
         
         # Create an input node and select the input encoding method
-        self.input = spaic.Node(dataloader, encoding='latency')
+        self.input = spaic.Encoder(dataloader, encoding='latency')
               
         # Establish neurongroups, select neuron types, and set neuron parameter values
         self.layer1 = spaic.NeuronGroup(100, model='clif')
         self.layer2 = spaic.NeuronGroup(10, model='clif')
         
         # Establish connections between Neurongroups
         self.connection1 = spaic.Connection(self.input, self.layer1, link_type='full')
         self.connection2 = spaic.Connection(self.layer1, self.layer2, link_type='full')
         
         # Create an output node and select the output decoding method
-        self.output = spaic.Node(decoding='spike_counts',target=self.layer2)
+        self.output = spaic.Decoder(decoding='spike_counts',target=self.layer2)
 
         # Establish a state detector, which can monitor the state of various objects
         self.monitor1 = spaic.StateMonitor(self.layer1, 'V')
 
         # Add the learning algorithm and select the network structure to be trained 
         self.learner1 = spaic.STCA(0.5, self)
         
@@ -183,27 +183,27 @@
 ```python
 # Initialize the object of the basic network class
 Net = spaic.Network()
 
 # Create a network structure by defining network components in with
 with Net:
     # Create an input node and select the input encoding method
-    input1 = spaic.Node(dataloader, encoding='latency')
+    input = spaic.Encoder(dataloader, encoding='latency')
 
 
     # Establish neurongroups, select neuron types, and set neuron parameter values
     layer1 = spaic.NeuronGroup(100, model='clif')
     layer2 = spaic.NeuronGroup(10, model='clif')
 
     # Establish connections between Neurongroups
     connection1 = spaic.Connection(input1, layer1, link_type='full')
     connection2 = spaic.Connection(layer1, layer2, link_type='full')
 
     # Create an output node and select the output decoding method
-    output1 = spaic.Node(decoding='spike_counts',target=layer2)
+    output = spaic.Decoder(decoding='spike_counts',target=layer2)
 
     # Establish a state detector, which can monitor the state of various objects
     monitor1 = spaic.StateMonitor(layer1, 'V')
 
     # Add the learning algorithm and select the network structure to be trained 
     learner1 = spaic.STCA(0.5, Net)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SPAIC Version: 0.6.2.0.0 Summary: The spaic
+Metadata-Version: 2.1 Name: SPAIC Version: 0.6.2.1.0 Summary: The spaic
 platform simulation training platform is a network construction, forward
 simulation and learning training platform developed for spiking neural
 networks. Home-page: https://github.com/ZhejianglabNCRC/SPAIC/ Author: zjlab
 Author-email: hongchf@zhejianglab.com Maintainer: hongchaofei Maintainer-email:
 hongchf@zhejianglab.com License: Apache-2.0 license Project-URL: Documentation,
 https://spaic.readthedocs.io/ Project-URL: Source Code, https://github.com/
 ZhejianglabNCRC/SPAIC Project-URL: Issue Tracker, https://github.com/
@@ -108,37 +108,37 @@
 loaded ## Network model construction The model can be built in two ways: first,
 like Pytorch's module class inheritance, which is built in the _init_ function,
 and second, like Nengo's with statement. In addition, the existing model
 structure in the model algorithm library can also be introduced into the
 modeling process ### Modeling Method 1: Class Inheritance Form ```python class
 ExampleNet(spaic.Network): def __init__(self): super(ExampleNet, self).__init__
 () # Create an input node and select the input encoding method self.input =
-spaic.Node(dataloader, encoding='latency') # Establish neurongroups, select
+spaic.Encoder(dataloader, encoding='latency') # Establish neurongroups, select
 neuron types, and set neuron parameter values self.layer1 = spaic.NeuronGroup
 (100, model='clif') self.layer2 = spaic.NeuronGroup(10, model='clif') #
 Establish connections between Neurongroups self.connection1 = spaic.Connection
 (self.input, self.layer1, link_type='full') self.connection2 = spaic.Connection
 (self.layer1, self.layer2, link_type='full') # Create an output node and select
-the output decoding method self.output = spaic.Node
+the output decoding method self.output = spaic.Decoder
 (decoding='spike_counts',target=self.layer2) # Establish a state detector,
 which can monitor the state of various objects self.monitor1 =
 spaic.StateMonitor(self.layer1, 'V') # Add the learning algorithm and select
 the network structure to be trained self.learner1 = spaic.STCA(0.5, self) # Add
 optimization algorithm self.optim = spaic.Adam(lr=0.01, schedule='StepLR',
 maxstep=1000) # Initialize the ExampleNet network object Net = ExampleNet() ```
 ### Modeling method 2: Using "with" ```python # Initialize the object of the
 basic network class Net = spaic.Network() # Create a network structure by
 defining network components in with with Net: # Create an input node and select
-the input encoding method input1 = spaic.Node(dataloader, encoding='latency') #
-Establish neurongroups, select neuron types, and set neuron parameter values
+the input encoding method input = spaic.Encoder(dataloader, encoding='latency')
+# Establish neurongroups, select neuron types, and set neuron parameter values
 layer1 = spaic.NeuronGroup(100, model='clif') layer2 = spaic.NeuronGroup(10,
 model='clif') # Establish connections between Neurongroups connection1 =
 spaic.Connection(input1, layer1, link_type='full') connection2 =
 spaic.Connection(layer1, layer2, link_type='full') # Create an output node and
-select the output decoding method output1 = spaic.Node
+select the output decoding method output = spaic.Decoder
 (decoding='spike_counts',target=layer2) # Establish a state detector, which can
 monitor the state of various objects monitor1 = spaic.StateMonitor(layer1, 'V')
 # Add the learning algorithm and select the network structure to be trained
 learner1 = spaic.STCA(0.5, Net) # Add optimization algorithm optim = spaic.Adam
 (lr=0.01, schedule='StepLR', maxstep=1000) ``` ### Modeling method 3: importing
 a model library model and modifying it with functions ```python from
 spaic.Library import ExampleNet Net = ExampleNet() # neuron parameters
```

### Comparing `SPAIC-0.6.2.0.0/SPAIC.egg-info/SOURCES.txt` & `SPAIC-0.6.2.1.0/SPAIC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/setup.cfg` & `SPAIC-0.6.2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Backend/Backend.py` & `SPAIC-0.6.2.1.0/spaic/Backend/Backend.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Backend/Torch_Backend.py` & `SPAIC-0.6.2.1.0/spaic/Backend/Torch_Backend.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/IO/Dataloader.py` & `SPAIC-0.6.2.1.0/spaic/IO/Dataloader.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/IO/Dataset.py` & `SPAIC-0.6.2.1.0/spaic/IO/Dataset.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/IO/Environment.py` & `SPAIC-0.6.2.1.0/spaic/IO/Environment.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/IO/Initializer.py` & `SPAIC-0.6.2.1.0/spaic/IO/Initializer.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/IO/Pipeline.py` & `SPAIC-0.6.2.1.0/spaic/IO/Pipeline.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/IO/sampler.py` & `SPAIC-0.6.2.1.0/spaic/IO/sampler.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/IO/utils.py` & `SPAIC-0.6.2.1.0/spaic/IO/utils.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/Backprop_RSTDP.py` & `SPAIC-0.6.2.1.0/spaic/Learning/Backprop_RSTDP.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/Conv_RSTDP.py` & `SPAIC-0.6.2.1.0/spaic/Learning/Conv_RSTDP.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/Conv_STDP.py` & `SPAIC-0.6.2.1.0/spaic/Learning/Conv_STDP.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/FiniteDifference.py` & `SPAIC-0.6.2.1.0/spaic/Learning/FiniteDifference.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/Learner.py` & `SPAIC-0.6.2.1.0/spaic/Learning/Learner.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/RSTDP.py` & `SPAIC-0.6.2.1.0/spaic/Learning/RSTDP.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/Rate_Modulation.py` & `SPAIC-0.6.2.1.0/spaic/Learning/Rate_Modulation.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/STBP_Learner.py` & `SPAIC-0.6.2.1.0/spaic/Learning/STBP_Learner.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/STCA_Learner.py` & `SPAIC-0.6.2.1.0/spaic/Learning/STCA_Learner.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/STDP_Learner.py` & `SPAIC-0.6.2.1.0/spaic/Learning/STDP_Learner.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/SpikeProp_Learner.py` & `SPAIC-0.6.2.1.0/spaic/Learning/SpikeProp_Learner.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/SurrogateBP_Learner.py` & `SPAIC-0.6.2.1.0/spaic/Learning/SurrogateBP_Learner.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/Tempotron_Learner.py` & `SPAIC-0.6.2.1.0/spaic/Learning/Tempotron_Learner.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/__init__.py` & `SPAIC-0.6.2.1.0/spaic/Learning/__init__.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Learning/surrogate.py` & `SPAIC-0.6.2.1.0/spaic/Learning/surrogate.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Library/Network_loader.py` & `SPAIC-0.6.2.1.0/spaic/Library/Network_loader.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Library/Network_saver.py` & `SPAIC-0.6.2.1.0/spaic/Library/Network_saver.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Library/STCA_music_network.py` & `SPAIC-0.6.2.1.0/spaic/Library/STCA_music_network.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Monitor/Monitor.py` & `SPAIC-0.6.2.1.0/spaic/Monitor/Monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             if self.get_grad:
                 variables[self.var_name].retain_grad()
             if self.index == 'full':
                 self._records.append(record_value)
                 self._times.append(self.backend.time)
             else:
                 if len(self.index) == record_value.ndim:
-                    self._records.append(record_value[self.index])
+                    self._records.append(record_value[tuple(self.index)])
                     self._times.append(self.backend.time)
                 else:
                     assert len(self.index) == record_value.ndim -1
                     if self.backend.backend_name == 'pytorch':
                         record_value = torch.movedim(record_value, 0, -1)
                         indexed_value = record_value[tuple(self.index)]
                         indexed_value = torch.movedim(indexed_value, -1, 0)
```

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/Assembly.py` & `SPAIC-0.6.2.1.0/spaic/Network/Assembly.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/BaseModule.py` & `SPAIC-0.6.2.1.0/spaic/Network/BaseModule.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/ConnectPolicy.py` & `SPAIC-0.6.2.1.0/spaic/Network/ConnectPolicy.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/Connections.py` & `SPAIC-0.6.2.1.0/spaic/Network/Connections.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/Construct.py` & `SPAIC-0.6.2.1.0/spaic/Network/Construct.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/DelayQueue.py` & `SPAIC-0.6.2.1.0/spaic/Network/DelayQueue.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/Network.py` & `SPAIC-0.6.2.1.0/spaic/Network/Network.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/Synapse.py` & `SPAIC-0.6.2.1.0/spaic/Network/Synapse.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Network/Topology.py` & `SPAIC-0.6.2.1.0/spaic/Network/Topology.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Neuron/Actions.py` & `SPAIC-0.6.2.1.0/spaic/Neuron/Actions.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Neuron/Decoders.py` & `SPAIC-0.6.2.1.0/spaic/Neuron/Decoders.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Neuron/Encoders.py` & `SPAIC-0.6.2.1.0/spaic/Neuron/Encoders.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Neuron/Generators.py` & `SPAIC-0.6.2.1.0/spaic/Neuron/Generators.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Neuron/Module.py` & `SPAIC-0.6.2.1.0/spaic/Neuron/Module.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Neuron/Neuron.py` & `SPAIC-0.6.2.1.0/spaic/Neuron/Neuron.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Neuron/Node.py` & `SPAIC-0.6.2.1.0/spaic/Neuron/Node.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/Neuron/Rewards.py` & `SPAIC-0.6.2.1.0/spaic/Neuron/Rewards.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/UI/OnlineSpikePlot.py` & `SPAIC-0.6.2.1.0/spaic/UI/OnlineSpikePlot.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/__init__.py` & `SPAIC-0.6.2.1.0/spaic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @project: SPAIC
 @author: Hong Chaofei
 @contact: hongchf@gmail.com
 
 @description: 
 """
 
-VERSION = (0, 6, 2, 0, 0)
+VERSION = (0, 6, 2, 1, 0)
 __version__ = '.'.join(map(lambda x: str(x), VERSION))
 
 # print('__file__={0:<35} | __name__={1:<20} | __package__={2:<20}'.format(__file__,__name__,str(__package__)))
 from .Network import Network, Connection, Assembly, Projection, Synapse
 from .Neuron import NeuronGroup, NeuronModel
 from .Neuron import Node, Encoders, Decoders, Generators, Rewards, Actions
 from .Neuron.Node import Encoder, Decoder, Generator, Reward, Action
```

### Comparing `SPAIC-0.6.2.0.0/spaic/utils/AnimateScatter.py` & `SPAIC-0.6.2.1.0/spaic/utils/AnimateScatter.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/utils/fftweight.py` & `SPAIC-0.6.2.1.0/spaic/utils/fftweight.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/utils/filters.py` & `SPAIC-0.6.2.1.0/spaic/utils/filters.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/utils/gtgram.py` & `SPAIC-0.6.2.1.0/spaic/utils/gtgram.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/utils/memory.py` & `SPAIC-0.6.2.1.0/spaic/utils/memory.py`

 * *Files identical despite different names*

### Comparing `SPAIC-0.6.2.0.0/spaic/utils/plot.py` & `SPAIC-0.6.2.1.0/spaic/utils/plot.py`

 * *Files identical despite different names*

