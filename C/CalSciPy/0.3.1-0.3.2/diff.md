# Comparing `tmp/CalSciPy-0.3.1.tar.gz` & `tmp/CalSciPy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.3.1.tar", last modified: Thu Jun  1 21:02:50 2023, max compression
+gzip compressed data, was "CalSciPy-0.3.2.tar", last modified: Thu Jun  1 22:56:41 2023, max compression
```

## Comparing `CalSciPy-0.3.1.tar` & `CalSciPy-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.179371 CalSciPy-0.3.1/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     4947 2023-06-01 21:02:50.177378 CalSciPy-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.3.1/README.md
--rw-rw-rw-   0        0        0     2303 2023-06-01 21:02:24.000000 CalSciPy-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 21:02:50.179371 CalSciPy-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.040372 CalSciPy-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.102371 CalSciPy-0.3.1/src/CalSciPy/
--rw-rw-rw-   0        0        0      368 2023-05-24 14:06:12.000000 CalSciPy-0.3.1/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    10702 2023-06-01 20:59:59.000000 CalSciPy-0.3.1/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3270 2023-05-24 14:25:43.000000 CalSciPy-0.3.1/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     9766 2023-05-24 14:18:29.000000 CalSciPy-0.3.1/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     4603 2023-05-24 14:11:21.000000 CalSciPy-0.3.1/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     8973 2023-05-24 14:26:47.000000 CalSciPy-0.3.1/src/CalSciPy/interactive_visuals.py
--rw-rw-rw-   0        0        0    10046 2023-06-01 20:59:59.000000 CalSciPy-0.3.1/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     8876 2023-05-26 15:07:57.000000 CalSciPy-0.3.1/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.3.1/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0    10311 2023-05-24 14:19:33.000000 CalSciPy-0.3.1/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.3.1/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.127371 CalSciPy-0.3.1/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4947 2023-06-01 21:02:49.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-06-01 21:02:50.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 21:02:49.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      376 2023-06-01 21:02:49.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-01 21:02:49.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.3.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.171370 CalSciPy-0.3.1/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.3.1/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.3.1/tests/test_bruker.py
--rw-rw-rw-   0        0        0      492 2023-05-24 14:14:23.000000 CalSciPy-0.3.1/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.3.1/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.3.1/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.3.1/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.3.1/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.3.1/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.496893 CalSciPy-0.3.2/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     4947 2023-06-01 22:56:41.493905 CalSciPy-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.3.2/README.md
+-rw-rw-rw-   0        0        0     2303 2023-06-01 22:55:46.000000 CalSciPy-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 22:56:41.496893 CalSciPy-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.328894 CalSciPy-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.399896 CalSciPy-0.3.2/src/CalSciPy/
+-rw-rw-rw-   0        0        0      358 2023-06-01 22:48:52.000000 CalSciPy-0.3.2/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    15266 2023-06-01 22:35:40.000000 CalSciPy-0.3.2/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3270 2023-05-24 14:25:43.000000 CalSciPy-0.3.2/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0     8422 2023-06-01 22:48:52.000000 CalSciPy-0.3.2/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     4000 2023-06-01 22:44:59.000000 CalSciPy-0.3.2/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     9700 2023-06-01 22:48:52.000000 CalSciPy-0.3.2/src/CalSciPy/interactive_visuals.py
+-rw-rw-rw-   0        0        0    10053 2023-06-01 22:34:13.000000 CalSciPy-0.3.2/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     8733 2023-06-01 22:39:17.000000 CalSciPy-0.3.2/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3109 2023-06-01 22:40:45.000000 CalSciPy-0.3.2/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0     9604 2023-06-01 22:44:01.000000 CalSciPy-0.3.2/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.3.2/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.428893 CalSciPy-0.3.2/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4947 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      376 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.3.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.485893 CalSciPy-0.3.2/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.3.2/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.3.2/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      492 2023-05-24 14:14:23.000000 CalSciPy-0.3.2/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.3.2/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.3.2/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.3.2/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.3.2/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.3.2/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.3.1/LICENSE` & `CalSciPy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/PKG-INFO` & `CalSciPy-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.3.1/README.md` & `CalSciPy-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/pyproject.toml` & `CalSciPy-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.3.1"
+version = "0.3.2"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy/bruker.py` & `CalSciPy-0.3.2/src/CalSciPy/bruker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,61 @@
 from __future__ import annotations
 from typing import Tuple, Optional, Union, List, Any
 from operator import eq
 from pathlib import Path
 from itertools import product
-
+from xml.etree import ElementTree
 
 import numpy as np
+import pandas as pd
 from prettytable import PrettyTable
 import cv2
 from PPVD.parsing import convert_permitted_types_to_required, find_num_unique_files_given_static_substring, \
     find_num_unique_files_containing_tag
+from PPVD.validation import validate_extension
 from tqdm import tqdm as tq
 
 
 from .misc import PatternMatching, calculate_frames_per_file, generate_blocks, generate_padded_filename
 from .io_tools import _load_single_tif, _save_single_tif
 
 
 """
-These functions have been incorporated into pyPrairieView and will likely be deprecated in the future and/or 
+These functions have been incorporated into pyPrairieView and will likely be deprecated in the future and/or
 pyPrairieView will absorbed into CalSciPy
 """
 
 
+def align_data(analog_data: pd.DataFrame, frame_times: pd.DataFrame, fill: bool = False) -> pd.DataFrame:
+    """
+    Synchronizes analog data & imaging frames using the timestamp of each frame. Option to generate a second column
+    in which the frame index is interpolated such that each analog sample matches with an associated frame.
+
+    :param analog_data: analog data
+    :param frame_times: frame timestamps
+    :param fill: whether to include an interpolated nearest-neighbor column so each sample has an associated frame
+    :returns: a dataframe containing time (index, ms) with aligned columns of voltage recordings/analog data and imaging frame
+    """
+    frame_times = frame_times.reindex(index=analog_data.index)
+
+    # Join frames & analog (deep copy to make sure not a view)
+    data = analog_data.copy(deep=True)
+    data = data.join(frame_times)
+
+    if fill:
+        frame_times_filled = frame_times.copy(deep=True)
+        frame_times_filled.columns = ["Imaging Frame (interpolated)"]
+        frame_times_filled.interpolate(method="nearest", inplace=True)
+        # forward fill the final frame
+        frame_times_filled.ffill(inplace=True)
+        data = data.join(frame_times_filled)
+
+    return data
+
+
 def generate_bruker_naming_convention(channel: int, plane: int, num_channels: int = 1, num_planes: int = 1) \
         -> str:
     """
     Generates the expected bruker naming convention for images collected with an arbitrary number of cycles & channels
 
     This function expects that the naming convention is _Cycle00000_Ch0_000000.ome.tiff where the channel is
     one-indexed. The 5-digit cycle id represents the frame if using multiplane imaging and the 6-digit tag represents
@@ -114,14 +143,51 @@
     channels = find_channels()
 
     # noinspection PyTypeChecker
     return channels, find_planes(), find_frames(), find_dimensions()[0], find_dimensions()[1]
     # apparently * on a return is illegal for python 3.7  # noqa
 
 
+@convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
+def extract_frame_times(filename: Union[str, Path]) -> pd.DataFrame:
+    """
+    Function to extract the relative frame times from a PrairieView imaging session's primary .xml file
+
+    :param: filename
+    :returns: dataframe containing time (index, ms) x imaging frame (*zero-indexed*)
+    """
+    tree = ElementTree.parse(filename)
+    root = tree.getroot()
+
+    # assert expected
+    # child_tags = [child.tag for child in root]
+    # expected_tags = ("SystemIDs", "PVStateShard", "Sequence")
+
+    # for tag_ in expected_tags:
+    #   assert (tag_ in child_tags), "XML follows unexpected structure"
+
+    # Since expected, let's grab frame sequence
+    sequence = root.find("Sequence")
+    # use set comprehension to avoid duplicates
+    relative_frame_times = {frame.attrib.get("relativeTime") for frame in sequence if "relativeTime" in frame.attrib}
+    # convert to float (appropriate type) & sort chronologically
+    relative_frame_times = sorted([float(frame) for frame in relative_frame_times])
+    frames = range(len(relative_frame_times))
+    # convert to same type as analog data to avoid people getting gotcha'd by pandas
+    frames = np.array(frames).astype(np.float64)
+    # convert to milliseconds, create new array to avoid people getting gotcha'd by pandas
+    frame_times = np.array(relative_frame_times) * 1000
+    # round to each millisecond
+    frame_times = np.round(frame_times).astype(np.int64)
+    # make index
+    frame_times = pd.Index(data=frame_times, name="Time (ms)")
+    # make dataframe
+    return pd.DataFrame(data=frames, index=frame_times, columns=["Imaging Frame"])
+
+
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def load_bruker_tifs(folder: Union[str, Path],
                      channel: Optional[int] = None, plane: Optional[int] = None) -> Tuple[np.ndarray]:  # noqa: C901
     """
     This function loads images collected and converted to .tif files by Bruker's Prairieview software.
     If multiple channels or multiple planes exist, each channel and plane combination is loaded to a separate
     numpy array. Identification of multiple channels / planes is dependent on :func:`determine_imaging_content`.
@@ -142,14 +208,33 @@
             images.append(_load_bruker_tif_stack(folder, channel_, plane_, num_channels, num_planes))
     else:
         images.append(_load_bruker_tif_stack(folder, channel, plane, num_channels, num_planes))
     return tuple(images)
 
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
+def load_voltage_recording(path: Union[str, Path]) -> pd.DataFrame:
+    """
+    Import bruker analog data from an imaging folder or individual file. By PrairieView naming conventions, these
+    | files contain "VoltageRecording" in the name.
+
+    :param path: folder or filename containing analog data
+    :returns: dataframe containing time (index, ms) x channel data
+    """
+    if "VoltageRecording" in path.name and path.is_file():
+        return _import_csv(path)
+    elif not path.is_file():
+        file = [file for file in path.glob("*.csv") if "VoltageRecording" in str(file)]
+        assert (len(file) == 1), "Too many files meeting parsing requirements"
+        return _import_csv(file)
+    else:
+        raise FileNotFoundError
+
+
+@convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def repackage_bruker_tifs(input_folder: Union[str, Path], output_folder: Union[str, Path],
                           channel: int = 0, plane: int = 0) -> None:
     """
     This function repackages a folder containing .tif files exported by Bruker's Prairieview software into a sequence
     of <4 GB .tif stacks. Note that parameters channel and plane are **zero-indexed**.
 
     :param input_folder: folder containing a sequence of single frame .tif files exported by Bruker's Prairieview
@@ -189,14 +274,31 @@
         images = [_verbose_load_single_tif(file, pbar) for file in files]
         images = np.concatenate(images, axis=0)
         _save_single_tif(output_folder.joinpath("images.tif"), images)
 
     pbar.close()
 
 
+@convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
+@validate_extension(required_extension=".csv", pos=0)
+def _import_csv(path: Union[str, Path]) -> pd.DataFrame:
+    """
+    Implementation function for loading csv files. Abstracted from the upper-level functions for cleaner logic.
+
+    :param path: filepath of .csv to import
+    :type path: str or Path
+    :return: dataframe containing time (index) x data [0:8]
+    :rtype: pandas.DataFrame
+    """
+    data = pd.read_csv(path, skipinitialspace=True)
+    data = data.set_index("Time(ms)")
+    data.sort_index(inplace=True)
+    return data
+
+
 def _load_bruker_tif_stack(input_folder: Path, channel: int, plane: int,
                            num_channels: int, num_planes: int) -> np.ndarray:
     """
     Implementation function to load a single bruker tif stack
 
     :param input_folder: folder containing tif stack
     :param channel: selected channel to load
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy/coloring.py` & `CalSciPy-0.3.2/src/CalSciPy/coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/src/CalSciPy/event_processing.py` & `CalSciPy-0.3.2/src/CalSciPy/event_processing.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,17 @@
 
 def calculate_firing_rates(spike_probability_matrix: np.ndarray, frame_rate: float = 30.0, in_place: bool = False) \
         -> np.ndarray:
     """
     Calculate firing rates
 
     :param spike_probability_matrix: matrix of n neuron x m samples where each element is the probability of a spike
-    :type spike_probability_matrix: numpy.ndarray
     :param frame_rate: frame rate of dataset
-    :type frame_rate: float = 30
     :param in_place: boolean indicating whether to perform calculation in-place
-    :type in_place: bool = False
-    :return: firing matrix of n neurons x m samples where each element is a binary indicating presence of spike event
-    :rtype: numpy.ndarray
+    :returns: firing matrix of n neurons x m samples where each element is a binary indicating presence of spike event
     """
     if in_place:
         firing_matrix = spike_probability_matrix
     else:
         firing_matrix = spike_probability_matrix.copy()
 
     firing_matrix *= frame_rate
@@ -31,96 +27,78 @@
 
 
 def calculate_mean_firing_rates(firing_matrix: np.ndarray) -> np.ndarray:
     """
     Calculate mean firing rate
 
     :param firing_matrix: matrix of n neuron x m samples where each element is either a spike or an
-        instantaneous firing rate
-    :type firing_matrix: numpy.ndarray
-    :return: 1-D vector of mean firing rates
-    :rtype: numpy.ndarray
+    | instantaneous firing rate
+    :returns: 1-D vector of mean firing rates
     """
     return np.nanmean(firing_matrix, axis=1)
 
 
 def collect_waveforms(traces: np.ndarray, event_indices: Iterable[Iterable[int]], pre: int = 150, post: int = 450) \
         -> Tuple[np.ndarray]:
     """
     Collect waveforms for each event
 
     :param traces: a matrix of M neurons x N samples
-    :type traces: numpy.ndarray
     :param event_indices: a list of events
-    :type event_indices: Iterable[Iterable[int]]
     :param pre: number of pre-event frames
-    :type pre: int
     :param post: number of post-event frames
-    :type post: int
-    :return: a matrix of M events x N samples
-    :rtype: Tuple[numpy.ndarray]
+    :returns: a matrix of M events x N samples
     """
     return tuple([_collect_waveforms(traces[neuron, :], event_indices[neuron], pre, post)
                   for neuron in range(traces.shape[0])])
 
 
 def convert_tau(tau: float, dt: float) -> float:
     """
     Converts a discrete tau to a continuous tau
 
     :param tau: decay constant
-    :type dt: float
     :param dt: time step (s)
-    :type dt: float
-    :return: continuous tau (s)
-    :rtype: float
+    :returns: continuous tau (s)
     """
     ctau = np.roots(np.hstack([1, -tau]))
     if ctau < 0:
         ctau = 0
     ctau = np.log(ctau) / dt
     return -1 / ctau
 
 
 def get_num_events(event_indices: Iterable[Iterable[int]]) -> np.ndarray:
     """
     Determines the number of events for each neuron in the event indices
 
     :param event_indices: An iterable of length M neurons containing a sequence with a duration for each event
-    :type event_indices: Iterable[Iterable[int]]
-    :return: A 1-D vector of length M neurons containing the number of events for each neuron
-    :rtype: numpy.ndarray
+    :returns: A 1-D vector of length M neurons containing the number of events for each neuron
     """
     return np.array([len(event_index) for event_index in event_indices])
 
 
 def get_inter_event_intervals(event_indices: Iterable[Iterable[int]], frame_rate: float = 30.0) -> Tuple[np.ndarray]:
     """
     Calculate the inter event intervals for each neuron in the event indices
 
     :param event_indices: An iterable of length M containing a sequence with a duration for each event
-    :type event_indices: Iterable[Iterable[int]]
     :param frame_rate: frame_rate for trace matrix
-    :type frame_rate: float
-    :return: An iterable of length M neurons containing the inter-event intervals for each event in the sequence
-    :rtype: Tuple[numpy.ndarray]
+    :returns: An iterable of length M neurons containing the inter-event intervals for each event in the sequence
     """
     return tuple([np.diff(events) / frame_rate for events in event_indices])
 
 
 def get_event_onset_intensities(traces: np.ndarray, event_indices: Iterable[Iterable[int]]) -> Tuple[np.ndarray]:
     """
     Retrieve the signal intensity at event onset for each neuron in the event indices
 
     :param traces: An M neuron by N sample matrix
-    :type traces: numpy.ndarray
     :param event_indices: An iterable of length M containing a sequence with a duration for each event
-    :type event_indices: Iterable[Iterable[int]]
-    :return: An iterable of length M neurons containing the onset intensities for each event in the sequence
-    :rtype: Tuple[numpy.ndarray]
+    :returns: An iterable of length M neurons containing the onset intensities for each event in the sequence
     """
     intensities = []
     for neuron in range(traces.shape[0]):
         intensities.append([traces[neuron, event] for event in event_indices[neuron]])
     return tuple(intensities)
 
 
@@ -128,25 +106,19 @@
                     force_nonneg: bool = True) \
         -> Tuple[List[int]]:
     """
     Identify event onset for each neuron using the smoothed, non-negative first-time derivative. The threshold for noise
     is considered 1/2th the standard deviation of the derivative.
 
     :param traces: An M neuron by N sample matrix
-    :type traces: numpy.ndarray
     :param timeout: timeout distance for peak finding (frames)
-    :type timeout: int
     :param frame_rate: frame rate / time step for trace matrix
-    :type frame_rate: float
     :param smooth: boolean indicating whether to smooth first-time derivative
-    :type smooth: bool = True
     :param force_nonneg: boolean indicating whether to enforce non-negativity constraint on first-time derivative
-    :type force_nonneg: bool = True
-    :return: An iterable where each element contains a sequence of frames identified as event onsets
-    :rtype: Tuple[List[int]]
+    :returns: An iterable where each element contains a sequence of frames identified as event onsets
     """
     delta = np.zeros_like(traces)
     delta[..., 1:] = np.diff(traces, axis=-1)
 
     if smooth:
         gaussian_filter1d(delta, sigma=frame_rate, output=delta)
 
@@ -164,19 +136,16 @@
 
 def normalize_firing_rates(firing_matrix: np.ndarray, in_place: bool = False) -> np.ndarray:
     """
     Normalize firing rates by scaling to a max of 1.0. Non-negativity constrained.
 
     :param firing_matrix: matrix of n neuron x m samples where each element is either a spike or an
         instantaneous firing rate
-    :type firing_matrix: numpy.ndarray
     :param in_place: boolean indicating whether to perform calculation in-place
-    :type in_place: bool = False
-    :return: normalized firing rate matrix of n neurons x m samples
-    :rtype: numpy.ndarray
+    :returns: normalized firing rate matrix of n neurons x m samples
     """
     if in_place:
         normalized_matrix = firing_matrix
     else:
         normalized_matrix = firing_matrix.copy()
 
     normalized_matrix /= np.nanmax(normalized_matrix, axis=0)
@@ -185,37 +154,29 @@
 
 
 def scale_waveforms(waveforms: Iterable[np.ndarray], scaler: Callable = StandardScaler) -> np.ndarray:
     """
     Scale waveforms for cross-neuron comparisons
 
     :param waveforms: An Iterable of M events by N samples matrices of waveforms
-    :type waveforms: numpy.ndarray
     :param scaler: sklearn preprocessing object
-    :type scaler: Callable
-    :return: An Iterable of M event by N samples scaled matrices of waveforms
-    :rtype: Iterable[numpy.ndarray]
+    :returns: An Iterable of M event by N samples scaled matrices of waveforms
     """
     return tuple([_scale_waveforms(waves, scaler) for waves in waveforms])
 
 
 def _collect_waveforms(trace: np.ndarray, event_index: Iterable[int], pre: int = 150, post: int = 450) -> np.ndarray:
     """
     Collect waveforms for each event
 
     :param trace: a fluorescent trace
-    :type trace: numpy.ndarray
     :param event_index: a list of events
-    :type event_index: Iterable[int]
     :param pre: number of pre-event frames
-    :type pre: int
     :param post: number of post-event frames
-    :type post: int
-    :return: a matrix of M events x N samples
-    :rtype: numpy.ndarray
+    :returns: a matrix of M events x N samples
     """
     waveforms = []  # Pre-allocate empty list. Not need to preallocate numpy array this is fine.
     frames_in_waveform = pre + post + 1
     total_frames = trace.shape[0]
     for event in event_index:
         if event - pre < 0:
             wv = trace[0: post + 1]
@@ -230,19 +191,16 @@
 
 
 def _scale_waveforms(waveforms: np.ndarray, scaler: Callable) -> np.ndarray:
     """
     Scale waveforms for cross-neuron comparisons
 
     :param waveforms: an M events by N samples matrix of waveforms
-    :type waveforms: numpy.ndarray
     :param scaler: sklearn preprocessing object
-    :type scaler: Callable
-    :return: an M events by N samples scaled matrix of waveforms
-    :rtype: numpy.ndarray
+    :returns: an M events by N samples scaled matrix of waveforms
     """
     waves = []  # Again this is fine, don't premature optimize
     for wave in range(waveforms.shape[0]):
         scaling = scaler()
         x = np.reshape(waveforms[wave, :], (-1, 1))
         waves.append(scaling.fit_transform(x))
     return np.transpose(np.hstack(waves))
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy/image_processing.py` & `CalSciPy-0.3.2/src/CalSciPy/image_processing.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,25 +20,19 @@
     blockwise with overlapping or non-overlapping blocks.
 
     Designed for use on arrays larger than the available memory capacity.
 
     Footprint is of the form np.ones((frames, y pixels, x pixels)) with the origin in the center
 
     :param images: images stack to be filtered
-    :type images: numpy.ndarray
     :param sigma: sigma for gaussian filter
-    :type sigma: Number or numpy.ndarray
     :param block_size: the size of each block. Must fit within memory
-    :type block_size: int = None
     :param block_buffer: the size of the overlapping region between block
-    :type block_buffer: int = 0
     :param in_place: whether to calculate in-place
-    :type in_place: bool = False
-    :return: images: numpy array (frames, y pixels, x pixels)
-    :rtype: numpy.ndarray
+    :returns: images: numpy array (frames, y pixels, x pixels)
     """
     if in_place:
         filtered_images = images
     else:
         filtered_images = images.copy()
 
     frames = filtered_images.shape[0]
@@ -63,25 +57,19 @@
     blockwise with overlapping or non-overlapping blocks.
 
     Designed for use on arrays larger than the available memory capacity.
 
     Footprint is of the form np.ones((frames, y pixels, x pixels)) with the origin in the center
 
     :param images: images stack to be filtered
-    :type images: numpy.ndarray
     :param mask: mask of the median filter
-    :type mask: numpy.ndarray = np.ones((3, 3, 3))
     :param block_size: the size of each block. Must fit within memory
-    :type block_size: int = None
     :param block_buffer: the size of the overlapping region between block
-    :type block_buffer: int = 0
     :param in_place: whether to calculate in-place
-    :type in_place: bool = False
-    :return: images: numpy array (frames, y pixels, x pixels)
-    :rtype: numpy.ndarray
+    :returns: images: numpy array (frames, y pixels, x pixels)
     """
 
     if in_place:
         filtered_images = images
     else:
         filtered_images = images.copy()
 
@@ -102,29 +90,23 @@
 
 @wrap_cupy_block
 def _gaussian_filter(images: cupy.ndarray, sigma: Union[Number, np.ndarray]) -> np.ndarray:
     """
     Implementation function of gaussian filter
 
     :param images: images to be filtered
-    :type images: cupy.ndarray
     :param sigma: sigma for filter
-    :type sigma: Number or numpy.ndarray
-    :return: filtered numpy array
-    :rtype: numpy.ndarray
+    :returns: filtered numpy array
     """
     return cupyx.scipy.ndimage.gaussian_filter(images, sigma=sigma)
 
 
 @wrap_cupy_block
 def _median_filter(images: cupy.ndarray, mask: np.ndarray) -> np.ndarray:
     """
     Implementation function of median filter
 
     :param images: images to be filtered
-    :type images: cupy.ndarray
     :param mask: mask for filtering
-    :type mask: numpy.ndarray
-    :return: filtered numpy array
-    :rtype: numpy.ndarray
+    :returns: filtered numpy array
     """
     return cupyx.scipy.ndimage.median_filter(images, footprint=mask)
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy/interactive_visuals.py` & `CalSciPy-0.3.2/src/CalSciPy/interactive_visuals.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 matplotlib.use('Qt5Agg')
 from matplotlib import pyplot as plt   # noqa: E402
 from matplotlib.widgets import Slider  # noqa: E402
 import seaborn as sns  # noqa: F401, E402
 
 
 def interactive_traces(traces: np.ndarray, frame_rate: float, **kwargs) -> None:
+    """
+    Function to interactive compare traces. Press Up/Down to switch neurons
+
+    :param traces: primary traces
+    :param frame_rate: frame rate
+    :returns: interactive figure
+    """
     _num_neurons, _num_frames = traces.shape
 
     _line_width = kwargs.get("lw", 3)
     _alpha = kwargs.get("alpha", 0.95)
 
     x = np.arange(0, (_num_frames * (1 / frame_rate)), 1 / frame_rate, dtype=np.float64)
 
@@ -89,14 +96,22 @@
                 fig.canvas.draw()
 
     fig.canvas.mpl_connect('key_press_event', on_key)
     plt.show()
 
 
 def interactive_traces_overlay(traces: np.ndarray, traces2: np.ndarray, frame_rate: float, **kwargs) -> None:
+    """
+    Function to interactive compare traces with an overlay trace (e.g., noise). Press Up/Down to switch neurons
+
+    :param traces: primary traces
+    :param traces2: secondary trace
+    :param frame_rate: frame_rate
+    :returns: interactive figure
+    """
     _num_neurons, _num_frames = traces.shape
 
     _line_width = kwargs.get("lw", 3)
     _alpha = kwargs.get("alpha", 0.95)
 
     x = np.arange(0, (_num_frames * (1 / frame_rate)), 1 / frame_rate, dtype=np.float64)
 
@@ -175,14 +190,22 @@
                 fig.canvas.draw()
 
     fig.canvas.mpl_connect('key_press_event', on_key)
     plt.show()
 
 
 def interactive_traces_compare(traces: np.ndarray, traces2: np.ndarray, frame_rate: float, **kwargs) -> None:
+    """
+    Function to interactively compare two sets of traces. Press Up/Down to switch neurons
+
+    :param traces: primary traces
+    :param traces2: secondary trace
+    :param frame_rate: frame_rate
+    :returns: interactive figure
+    """
     _num_neurons, _num_frames = traces.shape
 
     _line_width = kwargs.get("lw", 3)
     _alpha = kwargs.get("alpha", 0.95)
 
     x = np.arange(0, (_num_frames * (1 / frame_rate)), 1 / frame_rate, dtype=np.float64)
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy/io_tools.py` & `CalSciPy-0.3.2/src/CalSciPy/io_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,16 @@
     Save images to language-agnostic binary format. Ideal for optimal read/write speeds and highly-robust to corruption.
     However, the downside is that the images and their metadata are split into two separate files. Images are saved with
     the *.bin* extension, while metadata is saved with extension *.json*. If for some reason you lose the metadata, you
     can still load the binary if you know three of the following: number of frames, y-pixels, x-pixels, and the
     datatype. The datatype is almost always unsigned 16-bit (:class:`numpy.uint16`) for all modern imaging
     systems--even if they are collected at 12 or 13-bit.
 
-    :param path: path to save images to. The path stem is considered the filename if it doesn't have any extension. If no filename is provided then the default filename is *binary_video*.
+    :param path: path to save images to. The path stem is considered the filename if it doesn't have any extension. If
+    | no filename is provided then the default filename is *binary_video*.
     :param images: images to save (frames, y-pixels, x-pixels)
     :returns: 0 if successful
     """
     # parse the desired path
     if path.is_file():
         name = Path.name
         file_path = Path(path.parents)
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy/misc.py` & `CalSciPy-0.3.2/src/CalSciPy/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,53 +2,45 @@
 from typing import Iterable, Iterator, Any, Callable
 from collections import deque
 from pathlib import Path
 from numbers import Number
 from functools import wraps
 
 import numpy as np
+from tqdm import tqdm
 
 try:
     import cupy
 except ModuleNotFoundError:
     pass
 
 
 def calculate_frames_per_file(y_pixels: int, x_pixels: int, bit_depth: np.dtype = np.uint16, size_cap: Number = 3.9) \
         -> int:
     """
     Estimates the number of image frames to allocate to each file given some maximum size.
 
     :param y_pixels: number of y_pixels in image
-    :type y_pixels: int
     :param x_pixels: number of x_pixels in image
-    :type x_pixels: int
     :param bit_depth: bit-depth / type of image elements
-    :type bit_depth: numpy.dtype = numpy.uint16
     :param size_cap: maximum file size
-    :type size_cap: float = 3.9
-    :return: the maximum number of frames to allocate for each file
-    :rtype: int
+    :returns: the maximum number of frames to allocate for each file
     """
     single_frame_size = np.ones((y_pixels, x_pixels), dtype=bit_depth).nbytes * 1e-9
     return size_cap // single_frame_size
 
 
 def generate_blocks(sequence: Iterable, block_size: int, block_buffer: int = 0) -> Iterator:
     """
     Returns a generator of some arbitrary iterable sequence that yields m blocks with overlapping regions of size n
 
     :param sequence: Sequence to be split into overlapping blocks
-    :type sequence: Iterable
     :param block_size: size of blocks
-    :type block_size: int
     :param block_buffer: size of overlap between blocks
-    :type block_buffer: int
-    :return: generator yielding m blocks with overlapping regions of size n
-    :rtype: Iterator
+    :returns: generator yielding m blocks with overlapping regions of size n
     """
     if block_size <= 1:
         raise ValueError("Block size must be > 1")
     if block_buffer >= block_size:
         raise AssertionError("Block buffer must be smaller than the size of the block.")
     if block_size >= len(sequence):
         raise AssertionError("Block must be smaller than iterable sequence")
@@ -78,14 +70,22 @@
             else:
                 yield tuple(block)[-idx:]  # if we don't have a full block, we must ensure the number of repeats is
                 # equal to block buffer
             raise StopIteration
 
 
 def generate_overlapping_blocks(sequence: Iterable, block_size: int, block_buffer: int) -> Iterator:
+    """
+    Returns a generator of some arbitrary iterable sequence that yields m blocks with overlapping regions of size n
+
+    :param sequence: Sequence to be split into overlapping blocks
+    :param block_size: size of blocks
+    :param block_buffer: size of overlap between blocks
+    :returns: generator yielding m blocks with overlapping regions of size n
+    """
     if block_size <= 1:
         raise ValueError("Block size must be > 1")
     if block_buffer >= block_size:
         raise AssertionError("Block buffer must be smaller than the size of the block.")
     if block_size >= len(sequence):
         raise AssertionError("Block must be smaller than iterable sequence")
 
@@ -124,25 +124,19 @@
 def generate_padded_filename(output_folder: Path, index: int, base: str = "images", digits: int = 2,
                              ext: str = ".tif") -> Path:
     """
     Generates a pathlib Path whose name is defined as '{base}_{index}{ext}' where index is zero-padded if it
     is not equal to the number of digits
 
     :param output_folder: folder that will contain file
-    :type output_folder: pathlib.Path
     :param index: index of file
-    :type index: int
     :param base: base tag of file
-    :type base: str = "images"
     :param digits: number of digits for representing index
-    :type digits: int
     :param ext: file extension
-    :type ext: str
-    :return: generated filename
-    :rtype: pathlib.Path
+    :returns: generated filename
     """
     index = str(index)
 
     if len(index) > digits:
         raise ValueError("Index is larger than allocated number of digits in representation")
 
     while len(index) < digits:
@@ -152,17 +146,15 @@
 
 
 def wrap_cupy_block(cupy_function: Callable) -> Callable:
     """
     Wraps a cupy function such that incoming numpy arrays are converting to cupy arrays and swapped back on return
 
     :param cupy_function: any cupy function that accepts numpy arrays
-    :type cupy_function: Callable
     :return: wrapped function
-    :rtype: Callable
     """
     @wraps(cupy_function)
     def decorator(*args, **kwargs) -> Callable:
         args = list(args)
         if isinstance(args[0], np.ndarray):
             args[0] = cupy.asarray(args[0])
         args = tuple(args)
@@ -176,15 +168,14 @@
         Manual implementation of pattern matching for python < 3.10
 
         Not the most extensible or robust right now, but she works well for the
         current implementations.
 
 
         :param value: value or iterator of values of interest
-        :type value: Any
         """
         self.value = value
         self.comparison_expressions = comparison_expressions
 
     def __enter__(self):
         return self
 
@@ -192,24 +183,22 @@
         return False
 
     def __call__(self, cases: Any):
         """
         Magic call for comparing some case with some value using some comparison operator
 
         :param cases: case/s for comparison
-        :type: Any
-        :return: whether the case/s are matched by the value/s
-        :rtype: bool
+        :returns: whether the case/s are matched by the value/s
         """
         for value, comparator, case in zip(self.value, self.comparison_expressions, cases):
             if not comparator(value, case):
                 return False
         return True
-        
-        
+
+
 def sliding_window(sequence: np.ndarray, window_length: int, function: Callable, *args, **kwargs) -> np.ndarray:
     window_gen = generate_sliding_window(range(sequence.shape[-1]), window_length, 1)
     values = []
     sequence_length = sequence.shape[-1] - window_length + 2
     pbar = tqdm(total=sequence_length, desc="Calculating baselines...")
     try:
         for step in window_gen:
@@ -228,20 +217,19 @@
 
     for _ in range(window_length):
         window.append(next(iterable))
 
     while True:
         try:
             yield tuple(window)
-            for idx in range(step_size):
+            for idx in range(step_size):  # noqa: B007
                 window.append(next(iterable))
 
         except StopIteration:
             # noinspection PyUnboundLocalVariable
             if idx == 0:
                 pass
             elif idx == step_size:
                 pass
             else:
                 yield tuple(window)
             raise StopIteration
-
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy/reorganization.py` & `CalSciPy-0.3.2/src/CalSciPy/reorganization.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 
 
 def generate_raster(event_frames: Iterable[Iterable[int]], total_frames: Optional[int] = None) -> np.ndarray:
     """
     Generate raster from an iterable of iterables containing the spike or event times for each neuron
 
     :param event_frames: iterable containing an iterable identifying the event frames for each neuron
-    :type event_frames: Iterable[Iterable[int]]
     :param total_frames: total number of frames
-    :type total_frames: Optional[int] = None
-    :return: event matrix of neurons x total frames
-    :rtype: numpy.ndarray
+    :returns: event matrix of neurons x total frames
     """
 
     if not total_frames:  # if total frames not provided we estimate by finding the very last event
         total_frames = np.max([event for events in event_frames for event in events]) + 1  # + 1 to account for 0-index
     _neurons = len(event_frames)
     event_matrix = np.full((_neurons, total_frames), 0, dtype=np.int32)
 
@@ -31,51 +28,43 @@
 @validate_matrix(pos=0)
 @validate_evenly_divisible(numerator=0, denominator=1, axis=1)
 def generate_tensor(traces_as_matrix: np.ndarray, chunk_size: int) -> np.ndarray:
     """
     Generates a tensor given chunk / trial indices
 
     :param traces_as_matrix: traces in matrix form (neurons x frames)
-    :type traces_as_matrix: numpy.ndarray
     :param chunk_size: size of each chunk
-    :type chunk_size: int
-    :return: traces_as_tensor
-    :rtype: numpy.ndarray
+    :returns: traces as a tensor of trial x neurons x frames
     """
     return np.stack(np.hsplit(traces_as_matrix, traces_as_matrix.shape[1] // chunk_size), axis=0)
 
 
 @validate_tensor(pos=0)
 def merge_tensor(traces_as_tensor: np.ndarray) -> np.ndarray:
     """
     Concatenate multiple trials or tiffs into single matrix:
 
 
-    :param traces_as_tensor: chunk (trial, tiff, etc) x neurons x frames
-    :type traces_as_tensor: numpy.ndarray
-    :return: traces in matrix form
-    :rtype: numpy.ndarray
+    :param traces_as_tensor: chunk (trial, tif, etc) x neurons x frames
+    :returns: traces in matrix form (neurons x frames)
     """
     return np.hstack(traces_as_tensor)
 
 
 @validate_numpy_type(required_dtype="object", pos=0)
 def merge_factorized_matrices(factorized_traces: np.ndarray, component: int = 0) -> np.ndarray:
     """
     Concatenate a neuron x chunk or trial array in which each element is a component x frame factorization of the
     original trace:
 
 
-    :param factorized_traces: neurons x chunks (trial, tiff, etc) containing the neuron's trace factorized
+    :param factorized_traces: neurons x chunks (trial, tif, etc) containing the neuron's trace factorized
         into several components
-    :type factorized_traces: numpy.ndarray
     :param component: specific component to extract
-    :type component: int
-    :return: traces of specific component in matrix form
-    :rtype: numpy.ndarray
+    :returns: traces of specific component in matrix form
     """
     _neurons, _trials = factorized_traces.shape
     _frames = np.concatenate(factorized_traces[0], axis=1)[0, :].shape[0]
     traces_as_matrix = np.full((_neurons, _frames), 0, dtype=factorized_traces.dtype)  # pre-allocated
 
     # Merge Here - could be done more efficiently but not priority
     for _neuron in range(_neurons):
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy/trace_processing.py` & `CalSciPy-0.3.2/src/CalSciPy/trace_processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from __future__ import annotations
+from typing import Optional
+
 import numpy as np
 from scipy.signal import firwin, filtfilt
-from typing import Optional
 from numba import njit
 from tqdm import tqdm
 
 
 def calculate_dfof(traces: np.ndarray, frame_rate: float = 30.0, in_place: bool = False,
                    offset: float = 0.0, external_reference: Optional[np.ndarray] = None) \
         -> np.ndarray:
+    # noinspection GrazieInspection
     """
-    Calculates Δf/f0 (fold fluorescence over baseline). Baseline is defined as the 5th percentile of the signal
-    after a 1Hz low-pass filter using a Hamming window. Baseline can be calculated using an external reference using the
-    raw argument or adjusted by using the offset argument. Supports in-place calculation (off by default).
-
-    :param traces: matrix of traces in the form of neurons x frames
-    :type traces: numpy.ndarray
-    :param frame_rate: frame rate of dataset
-    :type frame_rate: float = 30.0
-    :param in_place: boolean indicating whether to perform calculation in-place
-    :type in_place: bool = False
-    :param offset: offset added to baseline; useful if traces are non-negative
-    :type offset: float = 0.0
-    :param external_reference: secondary dataset used to calculate baseline; useful if traces have been factorized
-    :type external_reference: numpy.ndarray = None
-    :return: Δf/f0 matrix of n neurons x m samples
-    :rtype: numpy.ndarray
-    """
+        Calculates Δf/f0 (fold fluorescence over baseline). Baseline is defined as the 5th percentile of the signal
+        after a 1Hz low-pass filter using a Hamming window. Baseline can be calculated using an external reference
+        | using the raw argument or adjusted by using the offset argument. Supports in-place calculation
+        | (off by default).
+
+        :param traces: matrix of traces in the form of neurons x frames
+        :param frame_rate: frame rate of dataset
+        :param in_place: boolean indicating whether to perform calculation in-place
+        :param offset: offset added to baseline; useful if traces are non-negative
+        :param external_reference: secondary dataset used to calculate baseline; useful if traces have been factorized
+        :return: Δf/f0 matrix of n neurons x m samples
+        """
     if in_place:
         dfof = traces
     else:
         dfof = traces.copy()
 
     taps = 30  # More taps mean higher frequency resolution, which in turn means narrower filters and/or steeper
     # roll‐offs.
@@ -76,33 +73,27 @@
     Calculates a frame-rate independent standardized noise as defined as:
         | :math:`v = \\frac{\sigma \\frac{\Delta F}F}\sqrt{f}`
 
     It is robust against outliers and approximates the standard deviation of Δf/f0 baseline fluctuations.
     For comparison, the more exquisite of the Allen Brain Institute's public datasets are approximately 1*%Hz^(-1/2)
 
     :param fold_fluorescence_over_baseline: fold fluorescence over baseline (i.e., Δf/f0)
-    :type fold_fluorescence_over_baseline: numpy.ndarray
     :param frame_rate: frame rate of dataset
-    :type frame_rate: float = 30
-    :return: standardized noise (units are  1*%Hz^(-1/2) ) for each neuron
-    :rtype: numpy.ndarray
+    :returns: standardized noise (units are  1*%Hz^(-1/2) ) for each neuron
     """
     return 100.0 * np.median(np.abs(np.diff(fold_fluorescence_over_baseline, axis=1)), axis=1) / np.sqrt(frame_rate)
 
 
 def detrend_polynomial(traces: np.ndarray, in_place: bool = False) -> np.ndarray:
     """
     Detrend traces using a fourth-order polynomial
 
     :param traces: matrix of traces in the form of neurons x frames
-    :type traces: numpy.ndarray
     :param in_place: boolean indicating whether to perform calculation in-place
-    :type in_place: bool = False
-    :return: detrended traces
-    :rtype: numpy.ndarray
+    :returns: detrended traces
     """
     [_neurons, _samples] = traces.shape
     _samples_vector = np.arange(_samples)
 
     if in_place:
         detrended_matrix = traces
     else:
@@ -123,36 +114,27 @@
     The parameter `kappa` controls the level of smoothing ("diffusion") as a function of the derivative of the trace
     (or "gradient" in the case of 2D images where this algorithm is often used). This function is known as the
     diffusion coefficient. When the derivative for some portion of the trace is low, the algorithm will encourage
     smoothing to reduce noise. If the derivative is large like during a burst of activity, the algorithm will discourage
     smoothing to maintain its structure. Here, the argument `kappa` is multiplied by the dynamic range to generate the
     true kappa.
 
-    represents the percentile used to calculate the true
-    kappa
-
     The diffusion coefficient implemented here is e^(-(derivative/kappa)^2).
 
     Perona-Malik diffusion is an iterative process. The parameter `gamma` controls the rate of diffusion, while
     parameter `iters` sets the number of iterations to perform.
 
     This implementation is currently situated to handle 1-D vectors because it gives us some performance benefits.
 
     :param traces: matrix of M neurons by N samples
-    :type traces: numpy.ndarray
     :param iters: number of iterations
-    :type iters: int = 25
     :param kappa: used to calculate the true kappa, where true kappa = kappa * dynamic range. range 0-1
-    :type kappa: Number = 15
     :param gamma: rate of diffusion for each iter. range 0-1
-    :type gamma: float = 0.25
     :param in_place: whether to calculate in-place
-    :type in_place: bool = False
-    :return: smoothed traces
-    :rtype: numpy.ndarray
+    :returns: smoothed traces
     """
 
     assert (0 < iters), "iters must be at least 1"
     assert (0 <= kappa <= 1), "kappa must satisfy 0 <= kappa <= 1"
     assert (0 <= gamma <= 1), "gamma must satisfy 0 <= gamma <= 1"
 
     if in_place:
@@ -178,37 +160,28 @@
     The parameter `kappa` controls the level of smoothing ("diffusion") as a function of the derivative of the trace
     (or "gradient" in the case of 2D images where this algorithm is often used). This function is known as the
     diffusion coefficient. When the derivative for some portion of the trace is low, the algorithm will encourage
     smoothing to reduce noise. If the derivative is large like during a burst of activity, the algorithm will discourage
     smoothing to maintain its structure. Here, the argument `kappa` is multiplied by the dynamic range to generate the
     true kappa.
 
-    represents the percentile used to calculate the true
-    kappa
-
     The diffusion coefficient implemented here is e^(-(derivative/kappa)^2). If the diffusion coefficient was a
     scalar instead of a function of the derivative the algorithm would be equivalent to standard gaussian smoothing.
 
     Perona-Malik diffusion is an iterative process. The parameter `gamma` controls the rate of diffusion, while
     parameter `iters` sets the number of iterations to perform.
 
     This implementation is currently situated to handle 1-D vectors because it gives us some performance benefits.
 
     :param trace: trace for a single neuron (i.e., vector)
-    :type trace: numpy.ndarray
     :param iters: number of iterations
-    :type iters: int = 25
     :param kappa: used to calculate the true kappa, where true kappa = kappa * dynamic range. range 0-1
-    :type kappa: Number = 15
     :param gamma: rate of diffusion for each iter. range 0-1
-    :type gamma: float = 0.25
     :param in_place: whether to calculate in-place
-    :type in_place: bool = False
-    :return: smoothed traces
-    :rtype: numpy.ndarray
+    :returns: smoothed traces
     """
 
     if in_place:
         smoothed_trace = trace
     else:
         smoothed_trace = trace.copy()
 
@@ -225,8 +198,15 @@
         smoothed_trace += (gamma * diffusion)
 
     return smoothed_trace
 
 
 @njit
 def _diffusion_coefficient(derivative: np.ndarray, kappa: float) -> np.ndarray:
+    """
+    Diffusion coefficient
+
+    :param derivative: derivative
+    :param kappa: kappa
+    :returns: value
+    """
     return np.exp(-((derivative / kappa)**2.0))
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.3.2/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.3.1/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.3.2/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/tests/test_a_install.py` & `CalSciPy-0.3.2/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/tests/test_bruker.py` & `CalSciPy-0.3.2/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/tests/test_event_processing.py` & `CalSciPy-0.3.2/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/tests/test_io_tools.py` & `CalSciPy-0.3.2/tests/test_io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/tests/test_misc.py` & `CalSciPy-0.3.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/tests/test_reorganization.py` & `CalSciPy-0.3.2/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.1/tests/test_trace_processing.py` & `CalSciPy-0.3.2/tests/test_trace_processing.py`

 * *Files identical despite different names*

