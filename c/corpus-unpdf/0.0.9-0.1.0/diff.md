# Comparing `tmp/corpus_unpdf-0.0.9.tar.gz` & `tmp/corpus_unpdf-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_unpdf-0.0.9.tar", max compression
+gzip compressed data, was "corpus_unpdf-0.1.0.tar", max compression
```

## Comparing `corpus_unpdf-0.0.9.tar` & `corpus_unpdf-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,7 @@
--rw-r--r--   0        0        0      558 2023-01-29 10:58:37.331283 corpus_unpdf-0.0.9/README.md
--rw-r--r--   0        0        0      147 2023-02-08 10:35:44.239354 corpus_unpdf-0.0.9/corpus_unpdf/__init__.py
--rw-r--r--   0        0        0     8248 2023-02-08 10:38:58.744061 corpus_unpdf-0.0.9/corpus_unpdf/decision.py
--rw-r--r--   0        0        0      692 2023-02-08 10:35:44.240275 corpus_unpdf-0.0.9/corpus_unpdf/src/__init__.py
--rw-r--r--   0        0        0      238 2023-02-08 10:35:44.246425 corpus_unpdf-0.0.9/corpus_unpdf/src/common/__init__.py
--rw-r--r--   0        0        0     3289 2023-02-05 03:14:11.840252 corpus_unpdf-0.0.9/corpus_unpdf/src/common/fetch.py
--rw-r--r--   0        0        0     6926 2023-02-08 09:39:22.727966 corpus_unpdf-0.0.9/corpus_unpdf/src/common/slice.py
--rw-r--r--   0        0        0     2374 2023-02-05 03:14:11.840515 corpus_unpdf-0.0.9/corpus_unpdf/src/content_ender.py
--rw-r--r--   0        0        0     7355 2023-02-08 10:35:44.248195 corpus_unpdf-0.0.9/corpus_unpdf/src/content_markers.py
--rw-r--r--   0        0        0     2348 2023-02-05 03:14:11.840730 corpus_unpdf-0.0.9/corpus_unpdf/src/content_starter.py
--rw-r--r--   0        0        0    10050 2023-02-08 10:37:26.329567 corpus_unpdf-0.0.9/corpus_unpdf/src/decision_objects.py
--rw-r--r--   0        0        0     2641 2023-02-05 03:14:11.840800 corpus_unpdf-0.0.9/corpus_unpdf/src/page_footer.py
--rw-r--r--   0        0        0     4116 2023-02-07 03:40:55.897530 corpus_unpdf-0.0.9/corpus_unpdf/src/page_header.py
--rw-r--r--   0        0        0     1764 2023-02-08 10:11:01.339293 corpus_unpdf-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 corpus_unpdf-0.0.9/setup.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 corpus_unpdf-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-01-29 10:58:37.331283 corpus_unpdf-0.1.0/README.md
+-rw-r--r--   0        0        0       79 2023-06-02 12:29:01.353163 corpus_unpdf-0.1.0/corpus_unpdf/__init__.py
+-rw-r--r--   0        0        0     5736 2023-06-02 12:22:59.509075 corpus_unpdf-0.1.0/corpus_unpdf/_markers.py
+-rw-r--r--   0        0        0     6248 2023-06-02 09:15:41.415245 corpus_unpdf-0.1.0/corpus_unpdf/_positions.py
+-rw-r--r--   0        0        0     6537 2023-06-02 12:55:08.623296 corpus_unpdf-0.1.0/corpus_unpdf/main.py
+-rw-r--r--   0        0        0     1398 2023-06-02 09:08:46.331365 corpus_unpdf-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 corpus_unpdf-0.1.0/PKG-INFO
```

### Comparing `corpus_unpdf-0.0.9/README.md` & `corpus_unpdf-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `corpus_unpdf-0.0.9/corpus_unpdf/decision.py` & `corpus_unpdf-0.1.0/corpus_unpdf/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,227 +1,158 @@
-from collections.abc import Iterator
+import logging
+from dataclasses import dataclass
 from pathlib import Path
-from typing import NamedTuple
+from typing import Self
 
 import pdfplumber
-from loguru import logger
 from pdfplumber.page import Page
 from pdfplumber.pdf import PDF
+from start_ocr import Content
+from start_ocr.content import Collection
 
-from .src import (
-    Decision,
-    DecisionPage,
-    Opinion,
+from ._markers import (
+    FrontpageMeta,
     PositionCourtComposition,
     PositionDecisionCategoryWriter,
     PositionNotice,
-    PositionOpinion,
-    get_end_page_pos,
-    get_start_page_pos,
 )
+from ._positions import PositionMeta
 
+logger = logging.getLogger(__name__)
 
-class DecisionMeta(NamedTuple):
-    """Metadata required to create a [decision][decision-document].
 
-    Field | Type | Description
-    --:|:--:|:--
-    `start_index` | int | The zero-based integer `x`, i.e. get specific `pdfplumber.pages[x]`
-    `start_page_num` | int | The 1-based integer to describe human-readable page number
-    `start_indicator` | [PositionDecisionCategoryWriter][decision-category-writer] or [PositionNotice][notice] | Marking the [start of content proper][start-of-content]
-    `writer` | str | When [PositionDecisionCategoryWriter][decision-category-writer]  is selected, the writer found underneath the category
-    `notice` | bool | Will be marked `True`, if [PositionNotice][notice] is selected; default is `False`.
-    `pages` | list[[DecisionPage][decision-pages]] | A list of pages having material content
+@dataclass
+class SeparateOpinionPages(Collection):
+    """Handles content and metadata of separate opinions, i.e. the concurring, dissenting opinions to a [main
+    opinion][mainopinionpages] of a _Decision_ or _Resolution_.
+
+    Given a PDF file, can use `SeparateOpinionPages.set(<path-to-pdf)` to extract _content pages (only)_ of the file. The fields of this data structure inherits from `start_ocr`'s `Collection`.
+    """  # noqa: E501
+
+    ...
+
+    @classmethod
+    def set(cls, path: Path):
+        """Limited extraction: only interested in content unlike decisions where metadata is relevant. Also assumes first page will always be the logical start.
+
+        Examples:
+            >>> x = Path().cwd() / "tests" / "data" / "opinion.pdf"
+            >>> opinion = SeparateOpinionPages.set(x)
+            >>> len(opinion.pages) # total page count
+            10
+            >>> from start_ocr import Bodyline, Footnote, Content
+            >>> isinstance(opinion.pages[0], Content) # first page
+            True
+            >>> isinstance(opinion.segments[0], Bodyline)
+            True
+            >>> isinstance(opinion.footnotes[0], Footnote)
+            True
+        """  # noqa: E501
+        first_page = Collection.preliminary_page(path)  # uses the sample execution
+        return Collection.make(path, preliminary_page=first_page)
+
+
+@dataclass
+class MainOpinionPages(Collection, FrontpageMeta):
+    """The main opinion of a _Decision_ or _Resolution_, specifically its front and last pages, is formatted differenly from [separate opinions][separateopinionpages]. The following metadata are required to be parsed:
+
+    1. [Composition][court-composition], i.e. whether _En Banc_ or by divison.
+    2. [Category][decision-category-writer], i.e. whether a _Decision_ or a _Resolution_.
+    2. [Writer][decision-category-writer], i.e. who penned the main opinion.
+    3. [Notice][notice], i.e. whether it is of a particular category of decisions.
+
+    Given a PDF file, can use `MainOpinionPages.set(<path-to-pdf)` to extract content pages _and the above metadata_ of the file. The fields of this data structure inherits from `start_ocr`'s `Collection` with a custom `FrontpageMeta`.
     """  # noqa: E501
 
-    start_index: int
-    start_page_num: int
-    start_indicator: PositionDecisionCategoryWriter | PositionNotice
-    end_page_num: int
-    end_page_pos: float | int
+    ...
+
+    @classmethod
+    def set(cls, path: Path) -> Self:
+        """From a _*.pdf_ file found in `path`, extract relevant metadata to generate a decision having content pages. Each of which will contain a body and, likely, an annex for footnotes.
+
+        Examples:
+            >>> x = Path().cwd() / "tests" / "data" / "decision.pdf"
+            >>> decision = MainOpinionPages.set(x)
+            >>> decision.category
+            <DecisionCategoryChoices.RESO: 'Resolution'>
+            >>> decision.composition
+            <CourtCompositionChoices.DIV2: 'Second Division'>
+            >>> decision.writer
+            'CARPIO. J.:'
+            >>> len(decision.pages) # total page count
+            5
+            >>> from start_ocr import Bodyline, Footnote, Content
+            >>> isinstance(decision.pages[0], Content) # first page
+            True
+            >>> isinstance(decision.segments[0], Bodyline)
+            True
+            >>> isinstance(decision.footnotes[0], Footnote)
+            True
+            >>> len(decision.footnotes) # TODO: limited number detected; should be 15
+            10
+        """  # noqa: E501
+        pos = PositionMeta.prep(path)
+        with pdfplumber.open(path) as pdf:
+            caso = cls._init(pdf=pdf, pos=pos)  # all pages
+            caso._limit_pages(pages=pdf.pages, pos=pos)  # limited pages
+            caso.join_segments()
+            caso.join_annexes()
+            return caso
 
     @classmethod
-    def prep(cls, path: Path):
-        if not (starter := get_start_page_pos(path)):
-            raise Exception("Could not detect start of content.")
-
-        index, start_indicator = starter
-        if not start_indicator:
-            raise Exception("Could not detect start indicator.")
-
-        ender = get_end_page_pos(path)
-        if not ender:
-            raise Exception("Could not detect end of content.")
-        end_page_num, end_page_pos = ender
-
-        return cls(
-            start_index=index,
-            start_page_num=index + 1,
-            start_indicator=start_indicator,
-            end_page_num=end_page_num,
-            end_page_pos=end_page_pos,
-        )
-
-    def init(self, pdf: PDF) -> Decision:
-        """Add the metadata of a [Decision][decision-document] and extract the first
-        page of the content proper which may not necessarily be page 1.
+    def _init(cls, pdf: PDF, pos: PositionMeta) -> Self:
+        """Extract first page of the content proper which may not necessarily be page 1.
+
+        Args:
+            pdf (PDF): The `pdfplumber`-formatted PDF
+            pos (PositionMeta): Contains true start and end position / pages
 
         Returns:
-            Decision: A Decision instance, if all elements match.
+            Self: MainOpinionPages instance.
         """
-        logger.debug(f"Initialize {self=}")
-        composition = PositionCourtComposition.from_pdf(pdf).element
-        start_page = pdf.pages[self.start_index]
-        if isinstance(self.start_indicator, PositionNotice):
-            return Decision(
-                composition=composition,
+        start_page = pdf.pages[pos.start_index]
+        if isinstance(pos.start_indicator, PositionNotice):
+            return cls(
+                composition=PositionCourtComposition.from_pdf(pdf).element,
                 notice=True,
                 pages=[
-                    DecisionPage.set(
+                    Content.set(
                         page=start_page,
-                        start_y=self.start_indicator.position_pct_height
+                        start_y=pos.start_indicator.position_pct_height
                         * start_page.height,
                     )
                 ],
             )
-        elif isinstance(self.start_indicator, PositionDecisionCategoryWriter):
-            return Decision(
-                composition=composition,
-                category=self.start_indicator.element,
-                writer=self.start_indicator.writer,
+        elif isinstance(pos.start_indicator, PositionDecisionCategoryWriter):
+            return cls(
+                composition=PositionCourtComposition.from_pdf(pdf).element,
+                category=pos.start_indicator.element,
+                writer=pos.start_indicator.writer,
                 pages=[
-                    DecisionPage.set(
+                    Content.set(
                         page=start_page,
-                        start_y=self.start_indicator.writer_pct_height
+                        start_y=pos.start_indicator.writer_pct_height
                         * start_page.height,
                     )
                 ],
             )
         raise Exception("Unexpected initialization of decision.")
 
-    def add(self, pages: list[Page]) -> Iterator[DecisionPage]:
+    def _limit_pages(self, pages: list[Page], pos: PositionMeta):
+        """Only add pages included in the `pos` metadata when generating the Decision collection."""  # noqa: E501
         for nxt in pages:
-            if nxt.page_number <= self.start_page_num:
+            if nxt.page_number <= pos.start_page_num:
                 continue
-            if nxt.page_number == self.end_page_num:
+
+            if nxt.page_number == pos.end_page_num:
                 logger.debug(f"Finalize {nxt.page_number=}.")
-                if page_valid := DecisionPage.set(
-                    page=nxt, end_y=self.end_page_pos
-                ):
-                    yield page_valid
+                if page_valid := Content.set(page=nxt, end_y=pos.end_page_pos):
+                    self.pages.append(page_valid)
                 else:
                     logger.warning("Detected blank page.")
                 break
             else:
                 logger.debug(f"Initialize {nxt.page_number=}.")
-                if page_valid := DecisionPage.set(page=nxt):
-                    yield page_valid
+                if page_valid := Content.set(page=nxt):
+                    self.pages.append(page_valid)
                 else:
                     logger.warning("Detected blank page.")
-
-
-def construct(obj: Decision | Opinion):
-    for page in obj.pages:
-        obj.body += f"\n\n\n\n{page.body_text}"
-        obj.segments.extend(page.segments)
-        if page.annex_text:
-            obj.annex += f"\n\n\n\n{page.annex_text}"
-            obj.footnotes.extend(page.footnotes)
-    return obj
-
-
-def get_decision(path: Path) -> Decision:
-    """From a _*.pdf_ file found in `path`, extract relevant [metadata][decisionmeta]
-    to generate a [decision][decision-document] having [pages][decision-pages].
-    Each of which will contain a body and, likely, an annex for footnotes.
-
-    Examples:
-        >>> from pathlib import Path
-        >>> x = Path().cwd() / "tests" / "data" / "decision.pdf"
-        >>> decision = get_decision(x)
-        >>> decision.category
-        <DecisionCategoryChoices.RESO: 'Resolution'>
-        >>> decision.composition
-        <CourtCompositionChoices.DIV2: 'Second Division'>
-        >>> decision.writer
-        'CARPIO. J.:'
-        >>> len(decision.pages) # total page count
-        5
-        >>> isinstance(decision.pages[0], DecisionPage) # first page
-        True
-        >>> from corpus_unpdf.src import Footnote, Bodyline
-        >>> isinstance(decision.segments[0], Bodyline)
-        True
-        >>> isinstance(decision.footnotes[0], Footnote)
-        True
-        >>> len(decision.footnotes) # TODO: limited number detected; should be 15
-        7
-
-    Args:
-        path (Path): Path to the pdf file.
-
-    Returns:
-        Self: Instance of a Decision with pages populated
-    """  # noqa: E501
-    meta = DecisionMeta.prep(path)
-    with pdfplumber.open(path) as pdf:
-        # create all the pages of the decision
-        caso = meta.init(pdf=pdf)
-        content_pages = meta.add(pages=pdf.pages)
-        caso.pages.extend(content_pages)
-        # construct full decision
-        obj = construct(caso)
-        if isinstance(obj, Decision):
-            return obj
-        raise Exception("Bad construction of Decision.")
-
-
-def get_opinion(path: Path) -> Opinion:
-    """From a _*.pdf_ file found in `path`, extract relevant opinion metadata
-    to generate an [opinion][opinion-document] having [pages][decision-pages].
-    Each of which will contain a body and, likely, an annex for footnotes.
-
-    Examples:
-        >>> from pathlib import Path
-        >>> x = Path().cwd() / "tests" / "data" / "opinion.pdf"
-        >>> opinion = get_opinion(x)
-        >>> opinion.writer
-        'HERNANDO, J.:'
-        >>> opinion.label
-        'DISSENTING OPINION'
-        >>> len(opinion.pages) # total page count
-        28
-        >>> isinstance(opinion.pages[0], DecisionPage) # first page
-        True
-        >>> from corpus_unpdf.src import Footnote, Bodyline
-        >>> isinstance(opinion.segments[0], Bodyline)
-        True
-        >>> isinstance(opinion.footnotes[0], Footnote)
-        True
-        >>> len(opinion.footnotes)
-        49
-
-    Args:
-        path (Path): Path to the pdf file.
-
-    Returns:
-        Self: Instance of an Opinion with pages populated
-    """  # noqa: E501
-    with pdfplumber.open(path) as pdf:
-        meta = PositionOpinion.from_pdf(pdf)
-        # initialize the opinion
-        start_page = pdf.pages[0]
-        start_y = meta.writer_pct_height * start_page.height
-        opinion = Opinion(
-            label=meta.label,
-            writer=meta.writer,
-            pages=[DecisionPage.set(page=start_page, start_y=start_y)],
-        )
-        # create all the pages of the opinion
-        for page in pdf.pages[1:]:
-            if page_valid := DecisionPage.set(page=page):
-                opinion.pages.append(page_valid)
-        # construct full opinion
-        obj = construct(opinion)
-        if isinstance(obj, Opinion):
-            return obj
-        raise Exception("Bad construction of Opinion.")
```

### Comparing `corpus_unpdf-0.0.9/corpus_unpdf/src/content_markers.py` & `corpus_unpdf-0.1.0/corpus_unpdf/_markers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,75 @@
+from dataclasses import dataclass
 from enum import Enum
 from typing import NamedTuple, Self
 
-import cv2
-import numpy
+import numpy as np
 import pytesseract
+from pdfplumber.page import CroppedPage
 from pdfplumber.pdf import PDF
-
-from .common import (
-    get_contours,
-    get_img_from_page,
-    get_likelihood_centered_coordinates,
-)
+from start_ocr import get_img_from_page, get_likelihood_centered_coordinates
 
 
 class NoticeChoices(Enum):
     NOTICE = "Notice"
 
 
 class PositionNotice(NamedTuple):
-    """When present, signifies that this was issued by authority of the Court.
+    """When present, signifies issuance by authority of the Court.
 
     Field | Type | Description
     --:|:--:|:--
     `element` | NoticeChoices | Only a single choice (for now)
     `coordinates` | tuple[int, int, int, int] | The opencv rectangle found in the page where the notice is found
     `position_pct_height` | float | The `y` + height `h` of the `coordinates` over the `im_h` image height; used so the pdfplumber can utilize its cropping mechanism.
     """  # noqa: E501
 
     element: NoticeChoices
     coordinates: tuple[int, int, int, int]
     position_pct_height: float
 
     @classmethod
-    def extract(cls, im: numpy.ndarray) -> Self | None:
+    def extract(cls, im: np.ndarray) -> Self | None:
         im_h, _, _ = im.shape
         for member in NoticeChoices:
             if xywh := get_likelihood_centered_coordinates(im, member.value):
                 y, h = xywh[1], xywh[3]
                 return cls(
                     element=member,
                     coordinates=xywh,
                     position_pct_height=(y + h) / im_h,
                 )
         return None
 
 
 class CourtCompositionChoices(Enum):
-    """How the Supreme Court sits. At present, this includes four
-    options: en banc + 3 divisions. Might need to add cases for _special_ divisions.
-    """
+    """How Philippine Supreme Court sits. At present, this includes four options: en banc + 3 divisions. TODO: Might need to add cases for _special_ divisions."""  # noqa: E501
 
     ENBANC = "En Banc"
     DIV1 = "First Division"
     DIV2 = "Second Division"
     DIV3 = "Third Division"
 
 
 class PositionCourtComposition(NamedTuple):
-    """Should be present as the top centered element in the first page
-    of the pdf of the Decision.
+    """Should be present as top centered element in the first page of a Decision PDF file.
 
     Field | Type | Description
     --:|:--:|:--
     `element` | [CourtCompositionChoices][composition-choices] | Presently four choices
     `coordinates` | tuple[int, int, int, int] | The opencv rectangle found in the page where the composition is found
     `composition_pct_height` | float | The `y` + height `h` of the `coordinates` over the `im_h` image height; used so the pdfplumber can utilize its cropping mechanism.
     """  # noqa: E501
 
     element: CourtCompositionChoices
     coordinates: tuple[int, int, int, int]
     composition_pct_height: float
 
     @classmethod
-    def extract(cls, im: numpy.ndarray) -> Self | None:
+    def extract(cls, im: np.ndarray) -> Self | None:
         im_h, _, _ = im.shape
         for member in CourtCompositionChoices:
             if xywh := get_likelihood_centered_coordinates(im, member.value):
                 y, h = xywh[1], xywh[3]
                 return cls(
                     element=member,
                     coordinates=xywh,
@@ -98,34 +91,33 @@
     a decision or a resolution."""
 
     CASO = "Decision"
     RESO = "Resolution"
 
 
 class PositionDecisionCategoryWriter(NamedTuple):
-    """Should be present as the top centered element in the first page
-    of the pdf of the Decision.
+    """Should be present as top centered element in the first page of a Decision PDF file.
 
     Field | Type | Description
     --:|:--:|:--
     `element` | [DecisionCategoryChoices][category-choices] | Presently four choices
     `coordinates` | tuple[int, int, int, int] | The opencv rectangle found in the page where the `composition` element is found
     `writer` | str | The string found indicating the name of the writer
     `category_pct_height` | float | The `y` + height `h` of the `coordinates` over the `im_h` image height; used so the pdfplumber can utilize its cropping mechanism.
-    `writer_pct_height` | float | The writer's coordinates are found below the category coordinates. This can then be used to signify the anchoring [start of the document][start-of-content].
+    `writer_pct_height` | float | The writer's coordinates are found below the category coordinates. This can then be used to signify the anchoring start of the document.
     """  # noqa: E501
 
     element: DecisionCategoryChoices
     coordinates: tuple[int, int, int, int]
     writer: str
     category_pct_height: float
     writer_pct_height: float
 
     @classmethod
-    def extract(cls, im: numpy.ndarray) -> Self | None:
+    def extract(cls, im: np.ndarray) -> Self | None:
         im_h, _, _ = im.shape
         for member in DecisionCategoryChoices:
             if xywh := get_likelihood_centered_coordinates(im, member.value):
                 _, y, _, h = xywh
                 y0, y1 = y + h, y + 270
                 writer_box = im[y0:y1]
                 writer = pytesseract.image_to_string(writer_box).strip()
@@ -135,58 +127,25 @@
                     writer=writer,
                     category_pct_height=y / im_h,
                     writer_pct_height=y1 / im_h,
                 )
         return None
 
 
-class PositionOpinion(NamedTuple):
-    """Should be present as the top centered element in the first page
-    of the pdf of the Opinion.
-
-    Field | Type | Description
-    --:|:--:|:--
-    `label` | str | Should be a phase including the word 'Opinion'
-    `writer` | str | The string found indicating the name of the writer
-    `coordinates` | tuple[int, int, int, int] | The opencv rectangle found in the page where the `label` is found
-    `opinion_pct_height` | float | The `y` + height `h` of the `coordinates` over the `im_h` image height; used so the pdfplumber can utilize its cropping mechanism.
-    `writer_pct_height` | float | The writer's coordinates are found below the label `coordinates`. This can then be used to signify the anchoring [start of the document][start-of-content].
-    """  # noqa: E501
-
-    label: str
-    writer: str
-    coordinates: tuple[int, int, int, int]
-    opinion_pct_height: float
-    writer_pct_height: float
-
-    @classmethod
-    def extract(cls, im: numpy.ndarray) -> Self | None:
-        im_h, im_w, _ = im.shape
-        for cnt in get_contours(im, (50, 50)):
-            x, y, w, h = cv2.boundingRect(cnt)
-            x0_mid_left = (1 * im_w) / 4 < x
-            endpoint_on_right = x + w > im_w / 2
-            short_width = w > 200
-            if all([x0_mid_left, endpoint_on_right, short_width]):
-                sliced_im = im[y : y + h, x : x + w]
-                label = pytesseract.image_to_string(sliced_im).strip().upper()
-                y0, y1 = y + h, y + 270
-                writer_box = im[y0:y1]
-                writer = pytesseract.image_to_string(writer_box).strip()
-                if "OPINION" in label:
-                    return cls(
-                        label=label,
-                        coordinates=(x, y, w, h),
-                        writer=writer,
-                        opinion_pct_height=(y + h) / im_h,
-                        writer_pct_height=y1 / im_h,
-                    )
-
-        return None
+@dataclass
+class FrontpageMeta:
+    """Metadata of the frontpage`
+
+    Field | Description
+    --:|:--
+    `composition` | The composition of the Supreme Court that decided the case
+    `category` | When available, whether the case is a "Decision" or a "Resolution"
+    `header` | The top portion of the page, usually excluded from metadata
+    `writer` | When available, the writer of the case
+    `notice` | When True, means that there is no `category` available
+    """
 
-    @classmethod
-    def from_pdf(cls, pdf: PDF) -> Self:
-        page_one_im = get_img_from_page(pdf.pages[0])
-        opinion_label = cls.extract(page_one_im)
-        if not opinion_label:
-            raise Exception("Could not detect opinion in page 1.")
-        return opinion_label
+    composition: CourtCompositionChoices
+    category: DecisionCategoryChoices | None = None
+    header: CroppedPage | None = None
+    writer: str | None = None
+    notice: bool = False
```

### Comparing `corpus_unpdf-0.0.9/pyproject.toml` & `corpus_unpdf-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corpus-unpdf"
-version = "0.0.9"
+version = "0.1.0"
 description = "Parse Philippine Supreme Court decisions issued in PDF format as text."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/corpus-unpdf"
 documentation = "https://justmars.github.io/corpus-unpdf"
@@ -16,64 +16,34 @@
   "Development Status :: 4 - Beta",
   "Intended Audience :: Legal Industry",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-python-dotenv = "^0.21"
-pdfplumber = "^0.7.6"
-pillow = "^9.4.0"
-opencv-python = "^4.7.0.68"
-pytesseract = "^0.3.10"
-loguru = "^0.6.0"
+start-ocr = "^0.0.3"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
+pytest = "^7.3"
 pytest-env = "^0.8.1"
-pytest-datadir = "^1.4.1"
-pre-commit = "^2.21"
-jupyter = "^1.0.0"
-mkdocs = "^1.4.2"
-mkdocstrings = { extras = ["python"], version = "^0.20.0" }
-mkdocs-material = "^9.0.11"
-black = "^23.1.0"
-rich = "^13.3.1"
-
-[tool.pytest]
-minversion = "7.2"
-addopts = "-ra -q --cov=tests/"
-testpaths = ["tests"]
+pytest-datadir = "^1.4"
+pytest-cov = "^4.1"
+pre-commit = "^3.3"
+mkdocs = "^1.4"
+mkdocstrings = { extras = ["python"], version = "^0.22" }
+mkdocs-material = "^9.1"
+ipykernel = "^6.23"
 
 [tool.pytest.ini_options]
-env = ["MAGICK_HOME=/opt/homebrew/Cellar/imagemagick/7.1.0-61"]
+env = ["MAGICK_HOME=/opt/homebrew/Cellar/imagemagick/7.1.1-10"]
+minversion = "7.3"
+addopts = "-ra -x -q --doctest-modules --cov tests"
+testpaths = ["tests", "corpus_unpdf"]
 
 [tool.ruff]
 ignore = ["F401"]
-
-[tool.black]
-target-version = ['py311']
-line-length = 79
-include = '.pyi?$'
-exclude = '''
-/(
-    .git
-    | .hg
-    | .mypy_cache
-    | .tox
-    | .venv
-    | _build
-    | buck-out
-    | build
-    | dist
-)/
-'''
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-line_length = 79
-include_trailing_comma = 'True'
+fixable = ["F", "E", "W", "I001"]
+select = ["F", "E", "W", "I001"]
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `corpus_unpdf-0.0.9/PKG-INFO` & `corpus_unpdf-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 Metadata-Version: 2.1
 Name: corpus-unpdf
-Version: 0.0.9
+Version: 0.1.0
 Summary: Parse Philippine Supreme Court decisions issued in PDF format as text.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: opencv-python (>=4.7.0.68,<5.0.0.0)
-Requires-Dist: pdfplumber (>=0.7.6,<0.8.0)
-Requires-Dist: pillow (>=9.4.0,<10.0.0)
-Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
-Requires-Dist: python-dotenv (>=0.21,<0.22)
+Requires-Dist: start-ocr (>=0.0.3,<0.0.4)
 Project-URL: Documentation, https://justmars.github.io/corpus-unpdf
 Project-URL: Repository, https://github.com/justmars/corpus-unpdf
 Description-Content-Type: text/markdown
 
 # corpus-unpdf
 
 ![Github CI](https://github.com/justmars/corpus-unpdf/actions/workflows/main.yml/badge.svg)
```

