# Comparing `tmp/start_ocr-0.0.2.tar.gz` & `tmp/start_ocr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_ocr-0.0.2.tar", max compression
+gzip compressed data, was "start_ocr-0.0.3.tar", max compression
```

## Comparing `start_ocr-0.0.2.tar` & `start_ocr-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      241 2023-06-02 03:24:39.015853 start_ocr-0.0.2/README.md
--rw-r--r--   0        0        0     1302 2023-06-02 03:42:00.581088 start_ocr-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      524 2023-06-02 01:57:39.835874 start_ocr-0.0.2/start_ocr/__init__.py
--rw-r--r--   0        0        0    11212 2023-06-02 03:10:52.468508 start_ocr-0.0.2/start_ocr/components.py
--rw-r--r--   0        0        0     3402 2023-06-02 01:18:37.671647 start_ocr-0.0.2/start_ocr/content.py
--rw-r--r--   0        0        0     2322 2023-06-01 09:16:30.897051 start_ocr-0.0.2/start_ocr/coordinates.py
--rw-r--r--   0        0        0      533 2023-06-02 01:13:39.519842 start_ocr-0.0.2/start_ocr/demo.py
--rw-r--r--   0        0        0     4140 2023-06-02 00:57:34.383161 start_ocr-0.0.2/start_ocr/fetch.py
--rw-r--r--   0        0        0     7338 2023-06-02 03:13:24.885710 start_ocr-0.0.2/start_ocr/slice.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 start_ocr-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-06-02 03:24:39.015853 start_ocr-0.0.3/README.md
+-rw-r--r--   0        0        0     1302 2023-06-02 09:07:04.515066 start_ocr-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      536 2023-06-02 09:05:39.809611 start_ocr-0.0.3/start_ocr/__init__.py
+-rw-r--r--   0        0        0    11204 2023-06-02 09:06:37.474212 start_ocr-0.0.3/start_ocr/components.py
+-rw-r--r--   0        0        0     5980 2023-06-02 07:11:34.030889 start_ocr-0.0.3/start_ocr/content.py
+-rw-r--r--   0        0        0     2322 2023-06-01 09:16:30.897051 start_ocr-0.0.3/start_ocr/coordinates.py
+-rw-r--r--   0        0        0      533 2023-06-02 01:13:39.519842 start_ocr-0.0.3/start_ocr/demo.py
+-rw-r--r--   0        0        0     4140 2023-06-02 06:47:30.613949 start_ocr-0.0.3/start_ocr/fetch.py
+-rw-r--r--   0        0        0     7326 2023-06-02 07:34:22.659838 start_ocr-0.0.3/start_ocr/slice.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 start_ocr-0.0.3/PKG-INFO
```

### Comparing `start_ocr-0.0.2/pyproject.toml` & `start_ocr-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "start-ocr"
 description = "Applying pdfplumber + opencv + pytesseract to extract content and metadata from formal PDF files."
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-ocr"
 documentation = "https://justmars.github.io/start-ocr"
 classifiers = [
   "Programming Language :: Python :: 3.11",
```

### Comparing `start_ocr-0.0.2/start_ocr/__init__.py` & `start_ocr-0.0.3/start_ocr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     footnote_lines,
     get_header_line,
     get_header_upper_right,
     get_page_end,
     get_page_num,
     page_width_lines,
 )
-from .content import Content
+from .content import Collection, Content
 from .coordinates import CoordinatedImage
 from .demo import show_contours
 from .fetch import (
     get_img_from_page,
     get_page_and_img,
     get_pages_and_imgs,
     get_reverse_pages_and_imgs,
```

### Comparing `start_ocr-0.0.2/start_ocr/components.py` & `start_ocr-0.0.3/start_ocr/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .coordinates import CoordinatedImage
 from .slice import get_contours
 
 line_break = re.compile(r"\s*\n+\s*")
 
 paragraph_break = re.compile(r"\s{10,}(?=[A-Z])")
 
-footnote_nums = re.compile(r"\n\s+(?P<fn>\d+)(?=\s+[A-Z])")
+footnote_nums = re.compile(r"(\n\s+|^)(?P<fn>\d+)(?=\s+[A-Z])")
 
 
 class Bodyline(NamedTuple):
     """Each page may be divided into lines which, for our purposes,
     will refer to an arbitrary segmentation of text based on regex parameters.
 
     Field | Type | Description
@@ -262,16 +262,16 @@
     cv2.imwrite("temp/boxes.png", im)
     return results
 
 
 def footnote_lines(im: np.ndarray) -> list[CoordinatedImage]:
     """Filter short horizontal lines:
 
-    1. > width of 400 pixels
-    2. height of less than 44 pixels, using the test pdf, any larger than 44 pixels will make this include text as well.
+    1. > width of 300 pixels
+    2. height of less than 40 pixels, using the test pdf, any larger than 44 pixels will make this include text as well.
 
     The footer represents content below the main content. This is also
     called the annex of the page.
 
     This detects a short line in the lower half of the page that has at least a width
     of 400 pixels and a , indicating a narrow box
     (as dilated by openCV). Text found below this box represents the annex.
@@ -289,21 +289,21 @@
     contours = get_contours(
         im=im,
         rectangle_size=(30, 10),
         test_dilation=True,
         test_dilated_image="temp/dilated.png",
     )
     results = []
-    for c in contours:
-        x, y, w, h = cv2.boundingRect(c)
+    for contour in contours:
+        x, y, w, h = cv2.boundingRect(contour)
         filtering_criteria = [
             x < (im_w / 2),
             (x + w) < (im_w / 2),
-            (im_w / 2) > w > 400,
-            h < 50,
+            (im_w / 2) > w > 300,
+            h < 40,
         ]
         if all(filtering_criteria):
             obj = CoordinatedImage(im, x, y, w, h)
             obj.greenbox()
             results.append(obj)
     cv2.imwrite("temp/boxes.png", im)
     return results
@@ -330,18 +330,16 @@
         879
 
     Args:
         im (numpy.ndarray): the openCV image that may contain a footnote line
         page (Page): the pdfplumber.page.Page based on `im`
 
     Returns:
-        tuple[float, float | None]: The annex line's y-axis (if it exists) and
-            The page's end content line
+        tuple[float, float | None]: Annex line's y-axis (if it exists) and the page's end content line.
     """  # noqa: E501
-    im_h, _, _ = im.shape
-    lines = footnote_lines(im)
     y1 = PERCENT_OF_MAX_PAGE * page.height
-    if lines:
+    im_h, _, _ = im.shape
+    if lines := footnote_lines(im):
         fn_line_end = lines[0].y / im_h
         y0 = fn_line_end * page.height
         return y0, y1
     return y1, None
```

### Comparing `start_ocr-0.0.2/start_ocr/coordinates.py` & `start_ocr-0.0.3/start_ocr/coordinates.py`

 * *Files identical despite different names*

### Comparing `start_ocr-0.0.2/start_ocr/demo.py` & `start_ocr-0.0.3/start_ocr/demo.py`

 * *Files identical despite different names*

### Comparing `start_ocr-0.0.2/start_ocr/fetch.py` & `start_ocr-0.0.3/start_ocr/fetch.py`

 * *Files identical despite different names*

### Comparing `start_ocr-0.0.2/start_ocr/slice.py` & `start_ocr-0.0.3/start_ocr/slice.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from difflib import SequenceMatcher
 from typing import NamedTuple
 
 import cv2
-import numpy
+import numpy as np
 import pytesseract
 from pdfplumber._typing import T_bbox
 from pdfplumber.page import CroppedPage, Page
 
 
 def is_match_text(
-    sliced_im: numpy.ndarray,
+    sliced_im: np.ndarray,
     text_to_match: str,
     likelihood: float = 0.7,
 ) -> bool:
     """Test whether textual image in `sliced_im` resembles `text_to_match` by
     a `likelihood` percentage.
 
     Args:
-        sliced_im (numpy.ndarray): Slice of a larger image containing text
+        sliced_im (np.ndarray): Slice of a larger image containing text
         text_to_match (str): How to match the text slice in `im`
         likelihood (float): Allowed percentage expressed in decimals
 
     Returns:
         bool: Whether or not the `text_to_match` resembles `sliced_im`'s text.
     """
     upper_candidate = pytesseract.image_to_string(sliced_im).strip().upper()
     upper_matcher = text_to_match.upper()
     match = SequenceMatcher(None, a=upper_candidate, b=upper_matcher)
     return match.ratio() > likelihood
 
 
 def get_contours(
-    im: numpy.ndarray,
+    im: np.ndarray,
     rectangle_size: tuple[int, int],
     test_dilation: bool = False,
     test_dilated_image: str | None = "temp/dilated.png",
 ) -> list:
     """Using tiny `rectangle_size` of the format `(width, height)`, create a dilated version
     of the image `im`. The contours found are outputed by this function.
 
@@ -50,15 +50,15 @@
         >>> len(contours)
         15
         >>> contours = get_contours(im, (10,10))
         >>> len(contours) in [222,223]
         True
 
     Args:
-        im (numpy.ndarray): The opencv formatted image
+        im (np.ndarray): The opencv formatted image
         rectangle_size (tuple[int, int]): The width and height of the contours to make
         test_dilation (bool, optional): _description_. Defaults to False.
         test_dilated_image (str | None, optional): _description_. Defaults to "temp/dilated.png".
 
     Returns:
         list: The contours found based on the specified structuring element
 
@@ -72,15 +72,15 @@
         cv2.imwrite(test_dilated_image, dilate)
     cnts = cv2.findContours(dilate, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
     cnts = cnts[0] if len(cnts) == 2 else cnts[1]
     return sorted(cnts, key=lambda x: cv2.boundingRect(x)[1])
 
 
 def get_likelihood_centered_coordinates(
-    im: numpy.ndarray, text_to_match: str
+    im: np.ndarray, text_to_match: str
 ) -> tuple[int, int, int, int] | None:
     """With a image `im`, get all contours found in the center
     of the image and then for each of these matches, if they
     are text resembling `text_to_match`, extract the coordinates of
     such contours.
 
     Examples:
@@ -90,15 +90,15 @@
         >>> get_likelihood_centered_coordinates(im, 'Decision') # None found
         >>> res = get_likelihood_centered_coordinates(im, 'Memo')
         >>> isinstance(res, tuple)
         True
         >>> page.pdf.close()
 
     Args:
-        im (numpy.ndarray): The base image to look for text
+        im (np.ndarray): The base image to look for text
         text_to_match (str): The words that should match
 
     Returns:
         tuple[int, int, int, int] | None: (x, y, w, h) pixels representing
             `cv2.boundingRect`, if found.
     """  # noqa: E501
     _, im_w, _ = im.shape
```

### Comparing `start_ocr-0.0.2/PKG-INFO` & `start_ocr-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: start-ocr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Applying pdfplumber + opencv + pytesseract to extract content and metadata from formal PDF files.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

