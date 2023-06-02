# Comparing `tmp/neurodatagen-0.1.0a2.tar.gz` & `tmp/neurodatagen-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurodatagen-0.1.0a2.tar", last modified: Fri Jun  2 07:35:48 2023, max compression
+gzip compressed data, was "neurodatagen-0.1.0a3.tar", last modified: Fri Jun  2 08:07:00 2023, max compression
```

## Comparing `neurodatagen-0.1.0a2.tar` & `neurodatagen-0.1.0a3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 07:35:48.794580 neurodatagen-0.1.0a2/
--rw-r--r--   0 droumis    (502) staff       (20)     1514 2023-06-01 15:50:46.000000 neurodatagen-0.1.0a2/LICENSE.txt
--rw-r--r--   0 droumis    (502) staff       (20)      285 2023-06-02 07:35:48.794381 neurodatagen-0.1.0a2/PKG-INFO
--rw-r--r--   0 droumis    (502) staff       (20)       44 2023-06-01 15:51:01.000000 neurodatagen-0.1.0a2/README.md
-drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 07:35:48.789501 neurodatagen-0.1.0a2/neurodatagen/
--rw-r--r--   0 droumis    (502) staff       (20)        0 2023-05-19 09:15:20.000000 neurodatagen-0.1.0a2/neurodatagen/__init__.py
-drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 07:35:48.791661 neurodatagen-0.1.0a2/neurodatagen/eeg/
--rw-r--r--   0 droumis    (502) staff       (20)       50 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/eeg/__init__.py
--rw-r--r--   0 droumis    (502) staff       (20)     2172 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/eeg/gen_eeg.py
--rw-r--r--   0 droumis    (502) staff       (20)     2067 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/eeg/gen_eeg_mne.py
-drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 07:35:48.793292 neurodatagen-0.1.0a2/neurodatagen/ephys/
--rw-r--r--   0 droumis    (502) staff       (20)      114 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/ephys/__init__.py
--rw-r--r--   0 droumis    (502) staff       (20)     6740 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/ephys/gen_ephys.py
--rw-r--r--   0 droumis    (502) staff       (20)     2977 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/ephys/gen_spiketimes.py
--rw-r--r--   0 droumis    (502) staff       (20)     1477 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/ephys/gen_waveforms.py
--rw-r--r--   0 droumis    (502) staff       (20)      651 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/ephys/load_waveforms.py
-drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 07:35:48.793905 neurodatagen-0.1.0a2/neurodatagen/imaging/
--rw-r--r--   0 droumis    (502) staff       (20)       51 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/imaging/__init__.py
--rw-r--r--   0 droumis    (502) staff       (20)    18729 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a2/neurodatagen/imaging/gen_miniscope.py
-drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 07:35:48.790318 neurodatagen-0.1.0a2/neurodatagen.egg-info/
--rw-r--r--   0 droumis    (502) staff       (20)      285 2023-06-02 07:35:48.000000 neurodatagen-0.1.0a2/neurodatagen.egg-info/PKG-INFO
--rw-r--r--   0 droumis    (502) staff       (20)      538 2023-06-02 07:35:48.000000 neurodatagen-0.1.0a2/neurodatagen.egg-info/SOURCES.txt
--rw-r--r--   0 droumis    (502) staff       (20)        1 2023-06-02 07:35:48.000000 neurodatagen-0.1.0a2/neurodatagen.egg-info/dependency_links.txt
--rw-r--r--   0 droumis    (502) staff       (20)       13 2023-06-02 07:35:48.000000 neurodatagen-0.1.0a2/neurodatagen.egg-info/top_level.txt
--rw-r--r--   0 droumis    (502) staff       (20)      405 2023-06-02 07:29:56.000000 neurodatagen-0.1.0a2/pyproject.toml
--rw-r--r--   0 droumis    (502) staff       (20)       38 2023-06-02 07:35:48.794648 neurodatagen-0.1.0a2/setup.cfg
+drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 08:07:00.489724 neurodatagen-0.1.0a3/
+-rw-r--r--   0 droumis    (502) staff       (20)     1514 2023-06-01 15:50:46.000000 neurodatagen-0.1.0a3/LICENSE.txt
+-rw-r--r--   0 droumis    (502) staff       (20)      285 2023-06-02 08:07:00.489540 neurodatagen-0.1.0a3/PKG-INFO
+-rw-r--r--   0 droumis    (502) staff       (20)       44 2023-06-01 15:51:01.000000 neurodatagen-0.1.0a3/README.md
+drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 08:07:00.485740 neurodatagen-0.1.0a3/neurodatagen/
+-rw-r--r--   0 droumis    (502) staff       (20)        0 2023-05-19 09:15:20.000000 neurodatagen-0.1.0a3/neurodatagen/__init__.py
+drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 08:07:00.487392 neurodatagen-0.1.0a3/neurodatagen/eeg/
+-rw-r--r--   0 droumis    (502) staff       (20)       50 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/eeg/__init__.py
+-rw-r--r--   0 droumis    (502) staff       (20)     2172 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/eeg/gen_eeg.py
+-rw-r--r--   0 droumis    (502) staff       (20)     2067 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/eeg/gen_eeg_mne.py
+drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 08:07:00.488570 neurodatagen-0.1.0a3/neurodatagen/ephys/
+-rw-r--r--   0 droumis    (502) staff       (20)      114 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/ephys/__init__.py
+-rw-r--r--   0 droumis    (502) staff       (20)     6740 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/ephys/gen_ephys.py
+-rw-r--r--   0 droumis    (502) staff       (20)     2977 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/ephys/gen_spiketimes.py
+-rw-r--r--   0 droumis    (502) staff       (20)     1477 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/ephys/gen_waveforms.py
+-rw-r--r--   0 droumis    (502) staff       (20)      651 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/ephys/load_waveforms.py
+drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 08:07:00.489053 neurodatagen-0.1.0a3/neurodatagen/imaging/
+-rw-r--r--   0 droumis    (502) staff       (20)       51 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/imaging/__init__.py
+-rw-r--r--   0 droumis    (502) staff       (20)    18729 2023-06-01 10:15:40.000000 neurodatagen-0.1.0a3/neurodatagen/imaging/gen_miniscope.py
+drwxr-xr-x   0 droumis    (502) staff       (20)        0 2023-06-02 08:07:00.486487 neurodatagen-0.1.0a3/neurodatagen.egg-info/
+-rw-r--r--   0 droumis    (502) staff       (20)      285 2023-06-02 08:07:00.000000 neurodatagen-0.1.0a3/neurodatagen.egg-info/PKG-INFO
+-rw-r--r--   0 droumis    (502) staff       (20)      538 2023-06-02 08:07:00.000000 neurodatagen-0.1.0a3/neurodatagen.egg-info/SOURCES.txt
+-rw-r--r--   0 droumis    (502) staff       (20)        1 2023-06-02 08:07:00.000000 neurodatagen-0.1.0a3/neurodatagen.egg-info/dependency_links.txt
+-rw-r--r--   0 droumis    (502) staff       (20)       13 2023-06-02 08:07:00.000000 neurodatagen-0.1.0a3/neurodatagen.egg-info/top_level.txt
+-rw-r--r--   0 droumis    (502) staff       (20)      421 2023-06-02 08:05:41.000000 neurodatagen-0.1.0a3/pyproject.toml
+-rw-r--r--   0 droumis    (502) staff       (20)       38 2023-06-02 08:07:00.489795 neurodatagen-0.1.0a3/setup.cfg
```

### Comparing `neurodatagen-0.1.0a2/LICENSE.txt` & `neurodatagen-0.1.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurodatagen-0.1.0a2/neurodatagen/eeg/gen_eeg.py` & `neurodatagen-0.1.0a3/neurodatagen/eeg/gen_eeg.py`

 * *Files identical despite different names*

### Comparing `neurodatagen-0.1.0a2/neurodatagen/eeg/gen_eeg_mne.py` & `neurodatagen-0.1.0a3/neurodatagen/eeg/gen_eeg_mne.py`

 * *Files identical despite different names*

### Comparing `neurodatagen-0.1.0a2/neurodatagen/ephys/gen_ephys.py` & `neurodatagen-0.1.0a3/neurodatagen/ephys/gen_ephys.py`

 * *Files identical despite different names*

### Comparing `neurodatagen-0.1.0a2/neurodatagen/ephys/gen_spiketimes.py` & `neurodatagen-0.1.0a3/neurodatagen/ephys/gen_spiketimes.py`

 * *Files identical despite different names*

### Comparing `neurodatagen-0.1.0a2/neurodatagen/ephys/gen_waveforms.py` & `neurodatagen-0.1.0a3/neurodatagen/ephys/gen_waveforms.py`

 * *Files identical despite different names*

### Comparing `neurodatagen-0.1.0a2/neurodatagen/ephys/load_waveforms.py` & `neurodatagen-0.1.0a3/neurodatagen/ephys/load_waveforms.py`

 * *Files identical despite different names*

### Comparing `neurodatagen-0.1.0a2/neurodatagen/imaging/gen_miniscope.py` & `neurodatagen-0.1.0a3/neurodatagen/imaging/gen_miniscope.py`

 * *Files identical despite different names*

### Comparing `neurodatagen-0.1.0a2/neurodatagen.egg-info/SOURCES.txt` & `neurodatagen-0.1.0a3/neurodatagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

