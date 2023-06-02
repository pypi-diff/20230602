# Comparing `tmp/start_ocr-0.0.1.tar.gz` & `tmp/start_ocr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_ocr-0.0.1.tar", max compression
+gzip compressed data, was "start_ocr-0.0.2.tar", max compression
```

## Comparing `start_ocr-0.0.1.tar` & `start_ocr-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      311 2023-06-01 15:56:16.241518 start_ocr-0.0.1/README.md
--rw-r--r--   0        0        0     1354 2023-06-01 12:13:29.516726 start_ocr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      435 2023-06-01 15:21:25.335655 start_ocr-0.0.1/start_ocr/__init__.py
--rw-r--r--   0        0        0     2322 2023-06-01 09:16:30.897051 start_ocr-0.0.1/start_ocr/coordinates.py
--rw-r--r--   0        0        0     3452 2023-06-01 12:52:33.494587 start_ocr-0.0.1/start_ocr/fetch.py
--rw-r--r--   0        0        0     3941 2023-06-01 15:52:38.259638 start_ocr-0.0.1/start_ocr/header.py
--rw-r--r--   0        0        0     4635 2023-06-01 12:55:47.408414 start_ocr-0.0.1/start_ocr/lines.py
--rw-r--r--   0        0        0     7279 2023-06-01 15:53:03.263479 start_ocr-0.0.1/start_ocr/slice.py
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 start_ocr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-06-02 03:24:39.015853 start_ocr-0.0.2/README.md
+-rw-r--r--   0        0        0     1302 2023-06-02 03:42:00.581088 start_ocr-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      524 2023-06-02 01:57:39.835874 start_ocr-0.0.2/start_ocr/__init__.py
+-rw-r--r--   0        0        0    11212 2023-06-02 03:10:52.468508 start_ocr-0.0.2/start_ocr/components.py
+-rw-r--r--   0        0        0     3402 2023-06-02 01:18:37.671647 start_ocr-0.0.2/start_ocr/content.py
+-rw-r--r--   0        0        0     2322 2023-06-01 09:16:30.897051 start_ocr-0.0.2/start_ocr/coordinates.py
+-rw-r--r--   0        0        0      533 2023-06-02 01:13:39.519842 start_ocr-0.0.2/start_ocr/demo.py
+-rw-r--r--   0        0        0     4140 2023-06-02 00:57:34.383161 start_ocr-0.0.2/start_ocr/fetch.py
+-rw-r--r--   0        0        0     7338 2023-06-02 03:13:24.885710 start_ocr-0.0.2/start_ocr/slice.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 start_ocr-0.0.2/PKG-INFO
```

### Comparing `start_ocr-0.0.1/pyproject.toml` & `start_ocr-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "start-ocr"
-description = "Integrating pdf-plumber and opencv"
-version = "0.0.1"
+description = "Applying pdfplumber + opencv + pytesseract to extract content and metadata from formal PDF files."
+version = "0.0.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
-repository = "https://github.com/justmars/start-code"
-documentation = "https://mv3.dev/start-code"
+repository = "https://github.com/justmars/start-ocr"
+documentation = "https://justmars.github.io/start-ocr"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
@@ -18,32 +18,28 @@
 python = "^3.11"
 python-dotenv = "^1.0"
 pdfplumber = "^0.9"
 opencv-python = "^4.7"
 pytesseract = "^0.3.10"
 
 [tool.poetry.group.dev.dependencies]
-rich = "^13.3"
 pytest = "^7.3"
 pytest-env = "^0.8.1"
 pytest-datadir = "^1.4"
-pytest-cov = "^2.12"
-pre-commit = "^2.21"
+pytest-cov = "^4.1"
+pre-commit = "^3.3"
 mkdocs = "^1.4"
 mkdocstrings = { extras = ["python"], version = "^0.22" }
 mkdocs-material = "^9.1"
 ipykernel = "^6.23"
 
 [tool.pytest.ini_options]
 env = ["MAGICK_HOME=/opt/homebrew/Cellar/imagemagick/7.1.1-10"]
 minversion = "7.3"
-addopts = "-ra -q --cov --doctest-modules"
-filterwarnings = [
-  "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
-]
+addopts = "-v -x -ra -q --cov --doctest-modules"
 testpaths = ["tests", "start_ocr"]
 
 [tool.ruff]
 ignore = ["F401", "F403"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
```

### Comparing `start_ocr-0.0.1/start_ocr/coordinates.py` & `start_ocr-0.0.2/start_ocr/coordinates.py`

 * *Files identical despite different names*

### Comparing `start_ocr-0.0.1/start_ocr/fetch.py` & `start_ocr-0.0.2/start_ocr/fetch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,112 +1,137 @@
 from collections.abc import Iterator
 from pathlib import Path
 
 import cv2
-import numpy
+import numpy as np
 import pdfplumber
+import pytesseract
 from pdfplumber.page import Page
 
 
-def get_img_from_page(page: Page) -> numpy.ndarray:
+def paged_text(page: Page) -> str:
+    """pdfplumber features an experimental setting `layout=True`.
+    Used here in tandem with another setting `keep_blank_chars` to monitor
+    line breaks.
+
+    Args:
+        page (Page): pdfplumber Page.
+
+    Returns:
+        str: text found from the page.
+    """
+    return page.extract_text(layout=True, keep_blank_chars=True).strip()
+
+
+def imaged_text(page: Page) -> str:
+    """Use pytesseract to extract text from the apge by first
+    converting the page to numpy format."""
+    img = get_img_from_page(page)
+    text = pytesseract.image_to_string(img)
+    return text.strip()
+
+
+def get_img_from_page(page: Page) -> np.ndarray:
     """Converts a `pdfplumber.Page` to an OpenCV formatted image file.
 
     Args:
         page (Page): pdfplumber.Page
 
     Returns:
-        numpy.ndarray: OpenCV format.
+        np.ndarray: OpenCV format.
     """
     obj = page.to_image(resolution=300).original
-    return cv2.cvtColor(numpy.array(obj), cv2.COLOR_RGB2BGR)
+    im = np.array(obj)
+    img = cv2.cvtColor(im, cv2.COLOR_RGB2BGR)
+    return img
 
 
-def get_page_and_img(pdfpath: str | Path, index: int) -> tuple[Page, numpy.ndarray]:
+def get_page_and_img(pdfpath: str | Path, index: int) -> tuple[Page, np.ndarray]:
     """Each page of a PDF file, can be opened and cropped via `pdfplumber`.
     To parse, it's necessary to convert the pdf to an `opencv` compatible-image format
-    (i.e. `numpy.ndarray`). This function converts a `Path` object into a pair of objects:
+    (i.e. `np.ndarray`). This function converts a `Path` object into a pair of objects:
 
     1. the first part is a `pdfplumber.Page`
-    2. the second part is an openCV image, i.e. `numpy.ndarray`
+    2. the second part is an openCV image, i.e. `np.ndarray`
 
     Examples:
-        >>> import numpy
-        >>> page, im = get_page_and_img(Path().cwd() / "tests" / "data" / "test.pdf", 0) # 0 marks the first page
+        >>> page, im = get_page_and_img(Path().cwd() / "tests" / "data" / "lorem_ipsum.pdf", 0) # 0 marks the first page
         >>> page.page_number # the first page
         1
         >>> isinstance(page, Page)
         True
-        >>> isinstance(im, numpy.ndarray)
+        >>> isinstance(im, np.ndarray)
         True
         >>> page.pdf.close()
 
     Args:
         pdfpath (str | Path): Path to the PDF file.
         index (int): Zero-based index that determines the page number.
 
     Returns:
-        tuple[Page, numpy.ndarray]: Page identified by `index`  with image of the
-            page  (in numpy format) that can be manipulated.
+        tuple[Page, np.ndarray]: Page identified by `index`  with image of the
+            page  (in np format) that can be manipulated.
     """  # noqa: E501
     with pdfplumber.open(pdfpath) as pdf:
         page = pdf.pages[index]
         img = get_img_from_page(page)
         return page, img
 
 
 def get_pages_and_imgs(
     pdfpath: str | Path,
-) -> Iterator[tuple[Page, numpy.ndarray]]:
+) -> Iterator[tuple[Page, np.ndarray]]:
     """Get page and images in sequential order.
 
     Examples:
-        >>> results = get_pages_and_imgs(Path().cwd() / "tests" / "data" / "test.pdf")
+        >>> results = get_pages_and_imgs(Path().cwd() / "tests" / "data" / "lorem_ipsum.pdf")
         >>> result = next(results)
         >>> type(result)
         <class 'tuple'>
         >>> isinstance(result[0], Page)
         True
         >>> result[0].page_number == 1 # first
         True
 
     Args:
         pdfpath (Page | Path): Path to the PDF file.
 
     Yields:
-        Iterator[tuple[Page, numpy.ndarray]]: Pages with respective images
-    """
+        Iterator[tuple[Page, np.ndarray]]: Pages with respective images
+    """  # noqa: E501
     with pdfplumber.open(pdfpath) as pdf:
         index = 0
         while index < len(pdf.pages):
             page = pdf.pages[index]
             yield page, get_img_from_page(page)
             index += 1
 
 
 def get_reverse_pages_and_imgs(
     pdfpath: str | Path,
-) -> Iterator[tuple[Page, numpy.ndarray]]:
+) -> Iterator[tuple[Page, np.ndarray]]:
     """Start from end page to get to first page to determine terminal values.
 
     Examples:
-        >>> x = Path().cwd() / "tests" / "data" / "test.pdf"
+        >>> x = Path().cwd() / "tests" / "data" / "lorem_ipsum.pdf"
+        >>> num_pages = pdfplumber.open(x).pages
         >>> results = get_reverse_pages_and_imgs(x)
         >>> result = next(results)
         >>> type(result)
         <class 'tuple'>
         >>> isinstance(result[0], Page)
         True
-        >>> result[0].page_number == len(pdfplumber.open(x).pages) # last first
+        >>> result[0].page_number == len(num_pages) # last page is first
         True
 
     Args:
         pdfpath (Page | Path): Path to the PDF file.
 
     Yields:
-        Iterator[tuple[Page, numpy.ndarray]]: Pages with respective images
+        Iterator[tuple[Page, np.ndarray]]: Pages with respective images
     """  # noqa: E501
     with pdfplumber.open(pdfpath) as pdf:
         index = len(pdf.pages) - 1
         while index >= 0:
             page = pdf.pages[index]
             yield page, get_img_from_page(page)
             index -= 1
```

### Comparing `start_ocr-0.0.1/start_ocr/slice.py` & `start_ocr-0.0.2/start_ocr/slice.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,21 +41,21 @@
 
     If `test_dilation` is `True`, a file will be created in the path represented in `test_dilated_image`
     to illustrate what the "diluted" image looks like.
 
     Examples:
         >>> from pathlib import Path
         >>> from start_ocr.fetch import get_page_and_img
-        >>> page, im = get_page_and_img(Path().cwd() / "tests" / "data" / "test.pdf", 0)
+        >>> page, im = get_page_and_img(Path().cwd() / "tests" / "data" / "lorem_ipsum.pdf", 0)
         >>> contours = get_contours(im, (50,50))
         >>> len(contours)
-        12
+        15
         >>> contours = get_contours(im, (10,10))
-        >>> len(contours)
-        285
+        >>> len(contours) in [222,223]
+        True
 
     Args:
         im (numpy.ndarray): The opencv formatted image
         rectangle_size (tuple[int, int]): The width and height of the contours to make
         test_dilation (bool, optional): _description_. Defaults to False.
         test_dilated_image (str | None, optional): _description_. Defaults to "temp/dilated.png".
 
@@ -82,29 +82,29 @@
     of the image and then for each of these matches, if they
     are text resembling `text_to_match`, extract the coordinates of
     such contours.
 
     Examples:
         >>> from pathlib import Path
         >>> from start_ocr.fetch import get_page_and_img
-        >>> page, im = get_page_and_img(Path().cwd() / "tests" / "data" / "test.pdf", 0)
+        >>> page, im = get_page_and_img(Path().cwd() / "tests" / "data" / "lorem_ipsum.pdf", 0)
         >>> get_likelihood_centered_coordinates(im, 'Decision') # None found
-        >>> res = get_likelihood_centered_coordinates(im, 'Resolution')
+        >>> res = get_likelihood_centered_coordinates(im, 'Memo')
         >>> isinstance(res, tuple)
         True
         >>> page.pdf.close()
 
     Args:
         im (numpy.ndarray): The base image to look for text
         text_to_match (str): The words that should match
 
     Returns:
         tuple[int, int, int, int] | None: (x, y, w, h) pixels representing
             `cv2.boundingRect`, if found.
-    """
+    """  # noqa: E501
     _, im_w, _ = im.shape
     for cnt in get_contours(im, (50, 50)):
         x, y, w, h = cv2.boundingRect(cnt)
         x0_mid_left = (1 * im_w) / 4 < x
         endpoint_on_right = x + w > im_w / 2
         short_width = w > 200
         if all([x0_mid_left, endpoint_on_right, short_width]):
@@ -138,22 +138,22 @@
     x0: float | int
     x1: float | int
     y0: float | int
     y1: float | int
 
     @property
     def slice(self) -> CroppedPage:
-        """Unlike slicing from an image based on a `numpy.ndarray`, a page cut
+        """Unlike slicing from an image based on a `np.ndarray`, a page cut
         implies a page derived from `pdfplumber`. The former is based on pixels;
         the latter on points.
 
         Examples:
             >>> from pathlib import Path
             >>> from start_ocr.fetch import get_page_and_img
-            >>> page, im = get_page_and_img(Path().cwd() / "tests" / "data" / "test.pdf", 0) # page 1
+            >>> page, im = get_page_and_img(Path().cwd() / "tests" / "data" / "lorem_ipsum.pdf", 0) # page 1
             >>> page.height
             936
             >>> cutpage = PageCut(page=page, x0=100, x1=200, y0=100, y1=200).slice
             >>> cutpage.height
             100
             >>> page.pdf.close()
 
@@ -169,20 +169,20 @@
         to generate page width and thus force preset margins. The `y0`
         and `y1` fields determine how to slice the page.
 
         Examples:
             >>> import pdfplumber
             >>> from pathlib import Path
             >>> from start_ocr.fetch import get_img_from_page
-            >>> pdf = pdfplumber.open(Path().cwd() / "tests" / "data" / "test.pdf")
-            >>> page = pdf.pages[0] # page 1
+            >>> pdf = pdfplumber.open(Path().cwd() / "tests" / "data" / "lorem_ipsum.pdf")
+            >>> page = pdf.pages[1] # page 2
             >>> im = get_img_from_page(page)
             >>> crop = PageCut.set(page, y0=0, y1=page.height * 0.1)
             >>> crop.extract_text()
-            'Indicator 1 xyzabc123'
+            'ALorem IpsumDocument 2 June1,2023'
             >>> pdf.close()
 
         Args:
             page (Page): pdfplumber Page object
             y0 (float | int): Top y-axis
             y1 (float | int): Bottom y-axis
```

