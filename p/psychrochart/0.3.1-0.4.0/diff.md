# Comparing `tmp/psychrochart-0.3.1.tar.gz` & `tmp/psychrochart-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.3.1.tar", last modified: Tue Nov 12 22:58:41 2019, max compression
+gzip compressed data, was "psychrochart-0.4.0.tar", max compression
```

## Comparing `psychrochart-0.3.1.tar` & `psychrochart-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0     3007 2019-11-12 22:57:38.364426 psychrochart-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2019-11-12 22:27:47.926360 psychrochart-0.3.1/LICENSE
--rw-r--r--   0        0        0     5702 2019-11-12 22:27:47.926472 psychrochart-0.3.1/README.md
--rw-r--r--   0        0        0      344 2019-11-12 22:27:47.919345 psychrochart-0.3.1/psychrochart/__init__.py
--rw-r--r--   0        0        0      353 2019-11-12 22:25:34.226855 psychrochart-0.3.1/psychrochart/__main__.py
--rw-r--r--   0        0        0      333 2019-11-12 22:25:34.227276 psychrochart-0.3.1/psychrochart/agg.py
--rw-r--r--   0        0        0    26513 2019-11-12 22:54:12.286948 psychrochart-0.3.1/psychrochart/chart.py
--rw-r--r--   0        0        0     1937 2017-07-16 07:58:55.000000 psychrochart-0.3.1/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2383 2019-11-12 22:27:47.657286 psychrochart-0.3.1/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     2745 2017-07-16 23:09:33.000000 psychrochart-0.3.1/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      509 2017-07-13 11:53:39.000000 psychrochart-0.3.1/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2144 2017-07-16 08:08:39.000000 psychrochart-0.3.1/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2178 2017-07-24 17:30:18.000000 psychrochart-0.3.1/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    13944 2019-11-12 22:54:59.568572 psychrochart-0.3.1/psychrochart/chartdata.py
--rw-r--r--   0        0        0     9094 2019-11-12 22:54:12.287172 psychrochart-0.3.1/psychrochart/psychrocurves.py
--rw-r--r--   0        0        0     2678 2019-11-12 22:54:12.287261 psychrochart-0.3.1/psychrochart/psychrolib_extra.py
--rw-r--r--   0        0        0     7328 2019-11-12 22:27:47.657433 psychrochart-0.3.1/psychrochart/util.py
--rw-r--r--   0        0        0     1436 2019-11-12 22:57:38.366367 psychrochart-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6626 1970-01-01 00:00:00.000000 psychrochart-0.3.1/setup.py
--rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 psychrochart-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3758 2023-06-02 06:57:29.062189 psychrochart-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-06-02 06:57:29.062189 psychrochart-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5844 2023-06-02 06:57:29.062189 psychrochart-0.4.0/README.md
+-rw-r--r--   0        0        0      344 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/__init__.py
+-rw-r--r--   0        0        0      353 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/__main__.py
+-rw-r--r--   0        0        0      278 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/agg.py
+-rw-r--r--   0        0        0    26781 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart.py
+-rw-r--r--   0        0        0     2157 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3044 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    14037 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chartdata.py
+-rw-r--r--   0        0        0     9199 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/psychrocurves.py
+-rw-r--r--   0        0        0     7460 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/util.py
+-rw-r--r--   0        0        0     2182 2023-06-02 06:57:29.146189 psychrochart-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7101 1970-01-01 00:00:00.000000 psychrochart-0.4.0/PKG-INFO
```

### Comparing `psychrochart-0.3.1/CHANGELOG.md` & `psychrochart-0.4.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0] - ♻️ Maintenance update to upgrade used libraries
+
+### Changes
+
+- 🐛 (from @simplynail in #25): fixing chart setup error with gca() call for recent Matplotlib versions
+- 🙈 Add missing .gitignore
+- 💥 **Update dependencies + minimal Python version to 3.10** to work with latest releases 🏄
+- 🎨 lint: Apply `isort` and `prettier`, and update typing
+- 🎨 lint: Evolve pre-commit config with ruff
+- 🍱 tests: Update SVG outputs from latest matplotlib
+- 🐛 Fix saving PNG with transparent background, by swapping `transparent=True` with `facecolor="none"`
+- 🗑️ Use `psychrolib.GetTDryBulbFromMoistAirVolumeAndHumRatio`, removing local method from here, now that it's included there
+- 👷 ci: **Swap travis CI config with GH actions to test + publish**
+
 ## [0.3.1] - 2019-11-12
 
 ### Changed
 
 - Fixed plotting of zones
 
 ## [0.3.0] - 2019-11-12
@@ -33,27 +47,27 @@
 
 ### Removed
 
 - Own collection of psychrometric equations
 
 ## [< 0.2.7] - Old versions changelog
 
-- v0.1.0:   Initial version.
-- v0.1.1:   Minor plotting fixes, set axis position, define P with `altitude_m` or `pressure_kpa`, reuse plot removing annotations (`chart.remove_annotations`). Axes as internal prop, lazy plotting, save to disk helper (`chart.save`).
-- v0.1.2:   Add `agg` module to set that `matplotlib` backend.
-- v0.1.3:   Add custom params for plotting styles, option to exclude first and last tick (`constant_{humid/temp}_label_include_limits`).
-- v0.1.4:   Customize labels and its locations for families of psychrometric curves.
-- v0.1.5:   Add Arrows, compatibility with the Home Assistant component `psychrometrics`.
-- v0.1.6:   Some cleaning, better typing, flake8, added `tox.ini`.
-- v0.1.7:   Methods to clean the plot (`.close_fig()`) and to remove the legend (`.remove_legend()`).
-- v0.1.8:   Memleak with `savefig`.
-- v0.1.10:  Fix plot limits, do not use pyplot, axes are not optional.
-- v0.1.11:  Add optional `Axes` as argument for `PsychroChart.plot`.
-- v0.1.12:  Add empiric equation for wet bulb temperature (@ZhukovGreen contribution).
-- v0.1.13:  Add convex hull option for overlay points.
-- v0.2.0:   Hide output in verbose mode, better convex hull zones syntax, stable.
-- v0.2.1:   Make `scipy` an optional requirement (it's only used for the ConvexHull zone).
-- v0.2.2:   Fix initial conditions for iteration solvers
-- v0.2.3:   Handle ConvexHull exception, overlay of series of points.
-- v0.2.4:   Set ASHRAE formulation for `saturation_pressure_water_vapor` as default. Minimal adjustments to iteration solvers for enthalpy and specific volume.
-- v0.2.5:   Fix coefficient in ASHRAE formulation for `dew_point_temperature`.
-- v0.2.6:   Add labels for connectors in chart legend (@@zhang-shen contribution).
+- v0.1.0: Initial version.
+- v0.1.1: Minor plotting fixes, set axis position, define P with `altitude_m` or `pressure_kpa`, reuse plot removing annotations (`chart.remove_annotations`). Axes as internal prop, lazy plotting, save to disk helper (`chart.save`).
+- v0.1.2: Add `agg` module to set that `matplotlib` backend.
+- v0.1.3: Add custom params for plotting styles, option to exclude first and last tick (`constant_{humid/temp}_label_include_limits`).
+- v0.1.4: Customize labels and its locations for families of psychrometric curves.
+- v0.1.5: Add Arrows, compatibility with the Home Assistant component `psychrometrics`.
+- v0.1.6: Some cleaning, better typing, flake8, added `tox.ini`.
+- v0.1.7: Methods to clean the plot (`.close_fig()`) and to remove the legend (`.remove_legend()`).
+- v0.1.8: Memleak with `savefig`.
+- v0.1.10: Fix plot limits, do not use pyplot, axes are not optional.
+- v0.1.11: Add optional `Axes` as argument for `PsychroChart.plot`.
+- v0.1.12: Add empiric equation for wet bulb temperature (@ZhukovGreen contribution).
+- v0.1.13: Add convex hull option for overlay points.
+- v0.2.0: Hide output in verbose mode, better convex hull zones syntax, stable.
+- v0.2.1: Make `scipy` an optional requirement (it's only used for the ConvexHull zone).
+- v0.2.2: Fix initial conditions for iteration solvers
+- v0.2.3: Handle ConvexHull exception, overlay of series of points.
+- v0.2.4: Set ASHRAE formulation for `saturation_pressure_water_vapor` as default. Minimal adjustments to iteration solvers for enthalpy and specific volume.
+- v0.2.5: Fix coefficient in ASHRAE formulation for `dew_point_temperature`.
+- v0.2.6: Add labels for connectors in chart legend (@@zhang-shen contribution).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psychrochart-0.3.1/LICENSE` & `psychrochart-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.3.1/README.md` & `psychrochart-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-# Psychrochart [![Travis Status](https://travis-ci.org/azogue/psychrochart.svg?branch=master)](https://travis-ci.org/azogue/psychrochart) [![Coverage Status](https://coveralls.io/repos/github/azogue/psychrochart/badge.svg?branch=master)](https://coveralls.io/github/azogue/psychrochart?branch=master) [![PyPi](https://pypip.in/v/psychrochart/badge.svg)](https://pypi.org/project/psychrochart/) [![Wheel](https://pypip.in/wheel/psychrochart/badge.svg)](https://pypi.org/project/psychrochart/)
+[![pre-commit.ci Status][pre-commit-ci-image]][pre-commit-ci-url]
+[![Build Status][build-image]][build-url]
+[![PyPI Version][pypi-image]][pypi-url]
+
+<!-- Badges -->
+
+[pre-commit-ci-image]: https://results.pre-commit.ci/badge/github/azogue/psychrochart/master.svg
+[pre-commit-ci-url]: https://results.pre-commit.ci/latest/github/azogue/psychrochart/master
+[build-image]: https://github.com/azogue/psychrochart/actions/workflows/main.yml/badge.svg
+[build-url]: https://github.com/azogue/psychrochart/actions/workflows/main.yml
+[pypi-image]: https://img.shields.io/pypi/v/psychrochart
+[pypi-url]: https://pypi.org/project/psychrochart/
 
+# Psychrochart
 
 A python 3 library to make **[psychrometric charts](https://en.wikipedia.org/wiki/Psychrometrics)** and overlay information on them.
 
 It implements a useful collection of psychrometric equations for moisture and humid air calculations, and the generation of beautiful and high customizable **psychrometric charts in SVG** with [`matplotlib`](https://matplotlib.org).
 
 **Psychrometric calculations to make the chart data are done with [`PsychroLib`](https://github.com/psychrometrics/psychrolib)** (summary paper in https://doi.org/10.21105/joss.01137).
 
@@ -18,21 +30,21 @@
 ```
 
 ## Features
 
 - **SI** units (with temperatures in celsius for better readability).
 - Easy style customization with a **JSON template** (colors, line styles and line widths).
 - Psychrometric charts within temperature and humidity ratio ranges, for any pressure\*, with:
-    * **Saturation line**
-    * **Constant RH lines**
-    * **Constant enthalpy lines**
-    * **Constant wet-bulb temperature lines**
-    * **Constant specific volume lines**
-    * **Constant dry-bulb temperature lines** (internal orthogonal grid, vertical)
-    * **Constant humidity ratio lines** (internal orthogonal grid, horizontal)
+  - **Saturation line**
+  - **Constant RH lines**
+  - **Constant enthalpy lines**
+  - **Constant wet-bulb temperature lines**
+  - **Constant specific volume lines**
+  - **Constant dry-bulb temperature lines** (internal orthogonal grid, vertical)
+  - **Constant humidity ratio lines** (internal orthogonal grid, horizontal)
 - Plot legend for each family of lines
 - Specify labels for each family of lines
 - **Overlay points, zones, arrows...**
 - **Export SVG, PNG files**
 
 \* The ranges of temperature, humidity and pressure where this library should provide good results are within the normal environments for people to live in. Don't expect right results if doing other type of thermodynamic calculations. Over saturated water vapor states are not implemented.
 
@@ -44,23 +56,23 @@
 # Load default style:
 chart_default = PsychroChart()
 axes = chart_default.plot()
 axes.get_figure()
 ```
 
 Called from a terminal (`python psychrochart`), it plots and shows the default chart using the default matplotlib backend, equivalent to this python script:
+
 ```python
 from psychrochart import PsychroChart
 import matplotlib.pyplot as plt
 
 PsychroChart().plot(ax=plt.gca())
 plt.show()
 ```
 
-
 ### Chart customization
 
 The default styling for charts is defined in JSON files that you can change, or you can pass a path of a file in JSON, or a dict, when you create the psychrometric chart object.
 Included styles are: `default`, `ashrae`, `interior` and `minimal`.
 
 ```python
 from psychrochart import load_config, PsychroChart
```

### Comparing `psychrochart-0.3.1/psychrochart/chart.py` & `psychrochart-0.4.0/psychrochart/chart.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 """A library to make psychrometric charts and overlay information in them."""
 import gc
 import logging
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Iterable
 
-import numpy as np
-import psychrolib as psy
 from matplotlib import figure
 from matplotlib.axes import Axes
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 from matplotlib.legend import Legend
+import numpy as np
+import psychrolib as psy
 from psychrolib import GetStandardAtmPressure, IP, SetUnitSystem, SI
-from scipy.spatial import ConvexHull
-from scipy.spatial.qhull import QhullError
+from scipy.spatial import ConvexHull, QhullError
 
 from .chartdata import (
     gen_points_in_constant_relative_humidity,
     make_constant_dry_bulb_v_line,
     make_constant_dry_bulb_v_lines,
     make_constant_enthalpy_lines,
     make_constant_humidity_ratio_h_lines,
@@ -43,51 +42,53 @@
 
 
 class PsychroChart:
     """Psychrometric chart object handler."""
 
     def __init__(
         self,
-        styles: Union[dict, str] = None,
-        zones_file: Union[dict, str] = None,
+        styles: dict[str, Any] | str | None = None,
+        zones_file: dict[str, Any] | str | None = None,
         use_unit_system_si: bool = True,
     ) -> None:
         """Create the PsychroChart object."""
-        self.d_config: dict = {}
-        self.figure_params: dict = {}
+        self.d_config: dict[str, Any] = {}
+        self.figure_params: dict[str, Any] = {}
         self.dbt_min = self.dbt_max = -100
         self.w_min = self.w_max = -1
         self.temp_step = 1.0
         self.altitude_m = -1
-        self.chart_params: dict = {}
+        self.chart_params: dict[str, Any] = {}
 
         # Set unit system for psychrolib and get standard pressure
         self.unit_system_si = use_unit_system_si
         if use_unit_system_si:
             SetUnitSystem(SI)
             logging.info("[SI units mode] ENABLED")
         else:
             SetUnitSystem(IP)
             logging.warning("[IP units mode] ENABLED")
         self.pressure = GetStandardAtmPressure(0.0)
 
-        self.constant_dry_temp_data: Optional[PsychroCurves] = None
-        self.constant_humidity_data: Optional[PsychroCurves] = None
-        self.constant_rh_data: Optional[PsychroCurves] = None
-        self.constant_h_data: Optional[PsychroCurves] = None
-        self.constant_v_data: Optional[PsychroCurves] = None
-        self.constant_wbt_data: Optional[PsychroCurves] = None
-        self.saturation: Optional[PsychroCurves] = None
-        self.zones: List = []
-
-        self._fig: Optional[figure.Figure] = None
-        self._canvas: Optional[FigureCanvas] = None
-        self._axes: Optional[Axes] = None
-        self._legend: Optional[Legend] = None
-        self._handlers_annotations: List = []
+        self.constant_dry_temp_data: PsychroCurves | None = None
+        self.constant_humidity_data: PsychroCurves | None = None
+        self.constant_rh_data: PsychroCurves | None = None
+        self.constant_h_data: PsychroCurves | None = None
+        self.constant_v_data: PsychroCurves | None = None
+        self.constant_wbt_data: PsychroCurves | None = None
+        self.saturation: PsychroCurves | None = None
+        # TODO evolve typing zones
+        self.zones: list = []
+
+        self._fig: figure.Figure | None = None
+        self._canvas: FigureCanvas | None = None
+        self._axes: Axes | None = None
+        self._legend: Legend | None = None
+        # TODO evolve typing handlers_annotations
+        self._handlers_annotations: list = []
 
         self._make_chart_data(styles, zones_file)
 
     def __repr__(self) -> str:
         """Return a string representation of the PsychroChart object."""
         return (
             f"<PsychroChart [{self.dbt_min:g}->{self.dbt_max:g} °C, "
@@ -108,16 +109,16 @@
         if self._fig is None:
             self.plot()
         assert isinstance(self._fig, figure.Figure)
         return self._fig
 
     def _make_chart_data(
         self,
-        styles: Union[dict, str] = None,
-        zones_file: Union[dict, str] = None,
+        styles: dict[str, Any] | str | None = None,
+        zones_file: dict[str, Any] | str | None = None,
     ) -> None:
         """Generate the data to plot the psychrometric chart."""
         # Get styling
         config = load_config(styles)
         self.d_config = config
         self.temp_step = config["limits"]["step_temp"]
 
@@ -233,15 +234,15 @@
                 family_label=self.chart_params["constant_wet_temp_label"],
             )
 
         # Zones
         if self.chart_params["with_zones"] or zones_file is not None:
             self.append_zones(zones_file)
 
-    def append_zones(self, zones: Union[dict, str] = None) -> None:
+    def append_zones(self, zones: dict[str, Any] | str | None = None) -> None:
         """Append zones as patches to the psychrometric chart."""
         if zones is None:
             # load default 'Comfort' zones (Spain RITE)
             d_zones = load_zones()
         else:
             d_zones = load_zones(zones)
 
@@ -251,19 +252,19 @@
             if zone_conf["zone_type"] in ("dbt-rh", "xy-points")
         ]
         if zones_ok:
             self.zones.append(PsychroCurves(zones_ok))
 
     def plot_points_dbt_rh(
         self,
-        points: Dict,
-        connectors: list = None,
-        convex_groups: list = None,
-        scatter_style: dict = None,
-    ) -> Dict:
+        points: dict[str, Any],
+        connectors: list | None = None,
+        convex_groups: list | None = None,
+        scatter_style: dict[str, Any] | None = None,
+    ) -> dict[str, Any]:
         """Append individual points, connectors and groups to the plot.
 
         * Pass a specific style dict to do a scatter plot:
             `scatter_style={'s': 5, 'alpha': .1, 'color': 'darkorange'}`
 
         * if you are plotting series of points, pass them as numpy arrays:
             `points={'points_series_name': (temp_array, humid_array)}`
@@ -322,15 +323,17 @@
              {"color": 'darkorange', "lw": 0, ...}),           # filling style
 
             # ...
         ]
         ```
         """
         use_scatter = False
-        points_plot: Dict[str, Tuple[List[float], List[float], dict]] = {}
+        points_plot: dict[
+            str, tuple[list[float], list[float], dict[str, Any]]
+        ] = {}
         default_style = {
             "marker": "o",
             "markersize": 10,
             "color": [1.0, 0.8, 0.1, 0.8],
             "linewidth": 0,
         }
         if scatter_style is not None:
@@ -432,15 +435,17 @@
                         int_points[hull.vertices, 1],
                         **style_fill,
                     )
                 )
 
         return points_plot
 
-    def plot_arrows_dbt_rh(self, points_pairs: Dict) -> Dict:
+    def plot_arrows_dbt_rh(
+        self, points_pairs: dict[str, Any]
+    ) -> dict[str, Any]:
         """Append individual points to the plot."""
         points_plot = {}
         default_style = {
             "linewidth": 0,
             "color": [1.0, 0.8, 0.1, 0.8],
             "arrowstyle": "wedge",
         }
@@ -475,16 +480,16 @@
             points_plot[key] = (temp1, w_g_ka1), (temp2, w_g_ka2), plot_params
 
         return points_plot
 
     def plot_vertical_dry_bulb_temp_line(
         self,
         temp: float,
-        style: dict = None,
-        label: str = None,
+        style: dict[str, Any] | None = None,
+        label: str | None = None,
         reverse: bool = False,
         **label_params,
     ) -> None:
         """Append a vertical line from w_min to w_sat."""
         style_curve = style or self.d_config["constant_dry_temp"]
         curve = make_constant_dry_bulb_v_line(
             self.w_min,
@@ -499,15 +504,15 @@
 
     def plot_legend(
         self,
         loc: str = "upper left",
         markerscale: float = 0.9,
         frameon: bool = True,
         fancybox: bool = True,
-        edgecolor: Union[str, Iterable] = "darkgrey",
+        edgecolor: str | Iterable = "darkgrey",
         fontsize: float = 15.0,
         labelspacing: float = 1.5,
         **params,
     ) -> None:
         """Append a legend to the psychrochart plot."""
         self._legend = self.axes.legend(
             loc=loc,
@@ -516,36 +521,39 @@
             edgecolor=edgecolor,
             fontsize=fontsize,
             fancybox=fancybox,
             labelspacing=labelspacing,
             **params,
         )
 
-    def _prepare_fig_and_axis(self, ax: Axes = None) -> Tuple[Axes, dict]:
+    def _prepare_fig_and_axis(self, ax: Axes = None) -> tuple[Axes, dict]:
         """Prepare matplotlib fig & Axes object for the chart."""
         fig_params = self.figure_params.copy()
         figsize = fig_params.pop("figsize", (16, 9))
         position = fig_params.pop("position", [0.025, 0.075, 0.925, 0.875])
 
         # Create figure and format axis
         self._fig = figure.Figure(figsize=figsize, dpi=150, frameon=False)
         self._canvas = FigureCanvas(self.figure)
         if ax is None:
-            ax = self.figure.gca(position=position)
+            ax = self.figure.add_subplot(position=position)
         ax.yaxis.tick_right()
         ax.yaxis.set_label_position("right")
         ax.set_xlim(self.dbt_min, self.dbt_max)
         ax.set_ylim(self.w_min, self.w_max)
         ax.grid(False)
         ax.grid(False, which="minor")
 
         return ax, fig_params
 
     def _set_tick_labels_in_main_axes(
-        self, ax: Axes, x_style_labels: dict, y_style_labels: dict
+        self,
+        ax: Axes,
+        x_style_labels: dict[str, Any],
+        y_style_labels: dict[str, Any],
     ):
         """Plot the psychrochart and return the matplotlib Axes instance."""
         if self.chart_params.get("with_constant_dry_temp", True):
             step_label = self.chart_params.get(
                 "constant_temp_label_step", None
             )
             if step_label:  # Explicit xticks
@@ -580,15 +588,15 @@
                         t for t in ticks if t not in [self.w_min, self.w_max]
                     ]
                 ax.set_yticks(ticks)
                 ax.set_yticklabels([f"{t:g}" for t in ticks], **y_style_labels)
         else:
             ax.set_yticks([])
 
-    def _apply_axis_styling(self, ax: Axes, fig_params: dict):
+    def _apply_axis_styling(self, ax: Axes, fig_params: dict[str, Any]):
         """Plot the psychrochart and return the matplotlib Axes instance."""
 
         def _apply_spines_style(axes, style, location="right"):
             for key in style:
                 if (key == "color") or (key == "c"):
                     axes.spines[location].set_color(style[key])
                 elif (key == "linewidth") or (key == "lw"):
```

### Comparing `psychrochart-0.3.1/psychrochart/chartdata.py` & `psychrochart-0.4.0/psychrochart/chartdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # -*- coding: utf-8 -*-
 """A library to make psychrometric charts and overlay information in them."""
-from typing import Callable, Dict, Iterable, List, Tuple, Union
+from typing import Any, Callable, Iterable
 
 import numpy as np
 from psychrolib import (
     GetHumRatioFromVapPres,
     GetMoistAirEnthalpy,
     GetMoistAirVolume,
     GetRelHumFromTWetBulb,
     GetSatVapPres,
     GetTDewPointFromVapPres,
     GetTDryBulbFromEnthalpyAndHumRatio,
+    GetTDryBulbFromMoistAirVolumeAndHumRatio,
     GetVapPresFromHumRatio,
     isIP,
 )
 from scipy.interpolate import interp1d
 
 from .psychrocurves import PsychroCurve, PsychroCurves
-from .psychrolib_extra import GetTDryBulbFromMoistAirVolume
 from .util import solve_curves_with_iteration
 
 f_vec_hum_ratio_from_vap_press = np.vectorize(GetHumRatioFromVapPres)
 f_vec_moist_air_enthalpy = np.vectorize(GetMoistAirEnthalpy)
 f_vec_moist_air_volume = np.vectorize(GetMoistAirVolume)
 f_vec_dew_point_from_vap_press = np.vectorize(GetTDewPointFromVapPres)
 f_vec_dry_temp_from_enthalpy = np.vectorize(GetTDryBulbFromEnthalpyAndHumRatio)
-f_vec_dry_temp_from_spec_vol = np.vectorize(GetTDryBulbFromMoistAirVolume)
+f_vec_dry_temp_from_spec_vol = np.vectorize(
+    GetTDryBulbFromMoistAirVolumeAndHumRatio
+)
 f_vec_sat_press = np.vectorize(GetSatVapPres)
 f_vec_vap_press_from_hum_ratio = np.vectorize(GetVapPresFromHumRatio)
 
 
 def _factor_out_w() -> float:
     """
     Conversion factor from internal units to plot units for humidity ratio.
@@ -66,47 +68,47 @@
 def _gen_list_curves_range_temps(
     func_curve: Callable,
     curves_values: Iterable[float],
     dbt_min: float,
     dbt_max: float,
     increment: float,
     pressure: float,
-) -> Tuple[np.array, List[np.array]]:
+) -> tuple[np.array, list[np.array]]:
     """Generate a curve from a range of temperatures."""
     temps = np.arange(dbt_min, dbt_max + increment, increment)
     curves = [func_curve(temps, value, pressure) for value in curves_values]
     return temps, curves
 
 
 def _get_humid_ratio_in_saturation(
-    dry_temps: np.ndarray, pressure: float,
+    dry_temps: np.ndarray, pressure: float
 ) -> np.array:
     sat_p = f_vec_sat_press(dry_temps)
     return _factor_out_w() * f_vec_hum_ratio_from_vap_press(sat_p, pressure)
 
 
 def gen_points_in_constant_relative_humidity(
     dry_temps: Iterable[float],
-    rh_percentage: Union[float, Iterable[float]],
+    rh_percentage: float | Iterable[float],
     pressure: float,
 ) -> np.array:
     """Generate a curve (numpy array) of constant humidity ratio."""
     return _factor_out_w() * f_vec_hum_ratio_from_vap_press(
-        f_vec_sat_press(dry_temps) * np.array(rh_percentage) / 100.0, pressure,
+        f_vec_sat_press(dry_temps) * np.array(rh_percentage) / 100.0, pressure
     )
 
 
 def make_constant_relative_humidity_lines(
     dbt_min: float,
     dbt_max: float,
     temp_step: float,
     pressure: float,
     rh_perc_values: Iterable[float],
     rh_label_values: Iterable[float],
-    style: dict,
+    style: dict[str, Any],
     label_loc: float,
     family_label: str,
 ) -> PsychroCurves:
     """Generate curves of constant relative humidity for the chart."""
     temps_ct_rh, curves_ct_rh = _gen_list_curves_range_temps(
         gen_points_in_constant_relative_humidity,
         rh_perc_values,
@@ -133,16 +135,16 @@
     )
 
 
 def make_constant_dry_bulb_v_line(
     w_humidity_ratio_min: float,
     temp: float,
     pressure: float,
-    style: dict,
-    type_curve: str = None,
+    style: dict[str, Any],
+    type_curve: str | None = None,
     reverse: bool = False,
 ) -> PsychroCurve:
     """Generate vertical line (constant dry bulb temp) up to saturation."""
     w_max = _factor_out_w() * GetHumRatioFromVapPres(
         GetSatVapPres(temp), pressure
     )
     if reverse:
@@ -154,15 +156,15 @@
     )
 
 
 def make_constant_dry_bulb_v_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     temps_vl: np.ndarray,
-    style: dict,
+    style: dict[str, Any],
     family_label: str,
 ) -> PsychroCurves:
     """Generate curves of constant dry bulb temperature (vertical)."""
     w_max_vec = _get_humid_ratio_in_saturation(temps_vl, pressure)
     return PsychroCurves(
         [
             PsychroCurve(
@@ -177,15 +179,15 @@
     )
 
 
 def make_constant_humidity_ratio_h_lines(
     dbt_max: float,
     pressure: float,
     ws_hl: Iterable[float],
-    style: dict,
+    style: dict[str, Any],
     family_label: str,
 ) -> PsychroCurves:
     """Generate curves of constant absolute humidity (horizontal)."""
     arr_hum_ratios = np.array(ws_hl) / _factor_out_w()
     dew_points = f_vec_dew_point_from_vap_press(
         dbt_max, f_vec_vap_press_from_hum_ratio(arr_hum_ratios, pressure)
     )
@@ -204,15 +206,15 @@
 
 
 def make_saturation_line(
     dbt_min: float,
     dbt_max: float,
     temp_step: float,
     pressure: float,
-    style: dict,
+    style: dict[str, Any],
 ) -> PsychroCurves:
     """Generate line of saturation for the psychrochart."""
     temps_sat_line = np.arange(dbt_min, dbt_max + temp_step, temp_step)
     w_sat = gen_points_in_constant_relative_humidity(
         temps_sat_line, 100.0, pressure
     )
     sat_c = PsychroCurve(temps_sat_line, w_sat, style, type_curve="saturation")
@@ -220,15 +222,15 @@
 
 
 def make_constant_enthalpy_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     enthalpy_values: Iterable[float],
     h_label_values: Iterable[float],
-    style: dict,
+    style: dict[str, Any],
     label_loc: float,
     family_label: str,
     saturation_curve: PsychroCurve,
 ) -> PsychroCurves:
     """Generate curves of constant enthalpy for the chart."""
     enthalpy_objective = np.array(enthalpy_values)
     temps_max_constant_h = f_vec_dry_temp_from_enthalpy(
@@ -248,15 +250,15 @@
         assume_sorted=True,
     )
     t_sat_points = solve_curves_with_iteration(
         "ENTHALPHY",
         enthalpy_objective,
         lambda *x: t_sat_interpolator(x[0]),
         lambda x: GetMoistAirEnthalpy(
-            x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure),
+            x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure)
         )
         / _factor_out_h(),
     )
     w_in_sat = _get_humid_ratio_in_saturation(t_sat_points, pressure)
 
     return PsychroCurves(
         [
@@ -281,15 +283,15 @@
 
 
 def make_constant_specific_volume_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     vol_values: np.ndarray,
     v_label_values: Iterable[float],
-    style: dict,
+    style: dict[str, Any],
     label_loc: float,
     family_label: str,
     saturation_curve: PsychroCurve,
 ) -> PsychroCurves:
     """Generate curves of constant specific volume for the chart."""
     temps_max_constant_v = f_vec_dry_temp_from_spec_vol(
         np.array(vol_values), w_humidity_ratio_min / _factor_out_w(), pressure
@@ -306,15 +308,15 @@
         assume_sorted=True,
     )
     t_sat_points = solve_curves_with_iteration(
         "CONSTANT VOLUME",
         vol_values,
         lambda *x: t_sat_interpolator(x[0]),
         lambda x: GetMoistAirVolume(
-            x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure), pressure,
+            x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure), pressure
         ),
     )
     w_in_sat = _get_humid_ratio_in_saturation(t_sat_points, pressure)
 
     return PsychroCurves(
         [
             PsychroCurve(
@@ -338,15 +340,15 @@
 
 
 def make_constant_wet_bulb_temperature_lines(
     dry_bulb_temp_max: float,
     pressure: float,
     wbt_values: np.ndarray,
     wbt_label_values: Iterable[float],
-    style: dict,
+    style: dict[str, Any],
     label_loc: float,
     family_label: str,
 ) -> PsychroCurves:
     """Generate curves of constant wet bulb temperature for the chart."""
     w_max_constant_wbt = f_vec_hum_ratio_from_vap_press(
         f_vec_sat_press(np.array(wbt_values)), pressure
     )
@@ -396,40 +398,40 @@
 def _make_zone_dbt_rh(
     t_min: float,
     t_max: float,
     increment: float,
     rh_min: float,
     rh_max: float,
     pressure: float,
-    style: dict = None,
-    label: str = None,
+    style: dict[str, Any] | None = None,
+    label: str | None = None,
 ) -> PsychroCurve:
     """Generate points for zone between constant dry bulb temps and RH."""
     temps = np.arange(t_min, t_max + increment, increment)
     curve_rh_up = gen_points_in_constant_relative_humidity(
         temps, rh_max, pressure
     )
     curve_rh_down = gen_points_in_constant_relative_humidity(
         temps, rh_min, pressure
     )
-    abs_humid: List[float] = (
+    abs_humid: list[float] = (
         list(curve_rh_up) + list(curve_rh_down)[::-1] + [curve_rh_up[0]]
     )
-    temps_zone: List[float] = list(temps) + list(temps)[::-1] + [temps[0]]
+    temps_zone: list[float] = list(temps) + list(temps)[::-1] + [temps[0]]
     return PsychroCurve(
         np.array(temps_zone),
         np.array(abs_humid),
         style,
         type_curve="constant_rh_data",
         label=label,
     )
 
 
 def make_zone_curve(
-    zone_conf: Dict, increment: float, pressure: float
+    zone_conf: dict[str, Any], increment: float, pressure: float
 ) -> PsychroCurve:
     """Generate points for zone between constant dry bulb temps and RH."""
     # TODO make conversion rh -> w and new zone_type: "dbt-rh-points"
     if zone_conf["zone_type"] == "dbt-rh":
         t_min, t_max = zone_conf["points_x"]
         rh_min, rh_max = zone_conf["points_y"]
         return _make_zone_dbt_rh(
```

### Comparing `psychrochart-0.3.1/psychrochart/psychrocurves.py` & `psychrochart-0.4.0/psychrochart/psychrocurves.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 """A library to make psychrometric charts and overlay information in them."""
 import json
 import logging
 from math import atan2, degrees
-from typing import AnyStr, Dict, List, Optional
+from typing import Any, AnyStr
 
-import numpy as np
 from matplotlib import patches
 from matplotlib.axes import Axes
 from matplotlib.path import Path
+import numpy as np
 
 from .util import mod_color
 
 
 def _between_limits(
     x_data: np.ndarray,
     y_data: np.ndarray,
@@ -36,31 +36,31 @@
 
 
 class PsychroCurve:
     """Object to store a psychrometric curve for plotting."""
 
     def __init__(
         self,
-        x_data: np.ndarray = None,
-        y_data: np.ndarray = None,
-        style: dict = None,
-        type_curve: str = None,
-        limits: dict = None,
-        label: str = None,
+        x_data: np.ndarray | None = None,
+        y_data: np.ndarray | None = None,
+        style: dict[str, Any] | None = None,
+        type_curve: str | None = None,
+        limits: dict[str, Any] | None = None,
+        label: str | None = None,
         label_loc: float = 0.75,
     ) -> None:
         """Create the Psychrocurve object."""
         self.x_data = np.array(x_data if x_data is not None else [])
         self.y_data = np.array(y_data if y_data is not None else [])
-        self.style: dict = style or {}
+        self.style: dict[str, Any] = style or {}
         self._type_curve = type_curve
         self._label = label
         self._label_loc = label_loc
         self._limits = limits
-        self._is_patch: bool = (style is not None and "facecolor" in style)
+        self._is_patch: bool = style is not None and "facecolor" in style
 
     def __bool__(self) -> bool:
         """Return the valid existence of the curve."""
         if (
             self.x_data is not None
             and len(self.x_data) > 1
             and self.y_data is not None
@@ -73,15 +73,15 @@
         """Object string representation."""
         name = "PsychroZone" if self._is_patch else "PsychroCurve"
         if self and self.x_data is not None:
             return f"<{name} {len(self.x_data)} values (label: {self._label})>"
         else:
             return f"<Empty {name} (label: {self._label})>"
 
-    def to_dict(self) -> Dict:
+    def to_dict(self) -> dict[str, Any]:
         """Return the curve as a dict."""
         if len(self.x_data) == 0 or len(self.y_data) == 0:
             return {}
         return {
             "x_data": self.x_data.tolist(),
             "y_data": self.y_data.tolist(),
             "style": self.style,
@@ -104,15 +104,15 @@
     @staticmethod
     def _annotate_label(
         ax: Axes,
         label: AnyStr,
         text_x: float,
         text_y: float,
         rotation: float,
-        text_style: Dict,
+        text_style: dict[str, Any],
     ):
         if abs(rotation) > 0:
             text_loc = np.array((text_x, text_y))
             text_style["rotation"] = ax.transData.transform_angles(
                 np.array((rotation,)), text_loc.reshape((1, 2))
             )[0]
             text_style["rotation_mode"] = "anchor"
@@ -166,18 +166,18 @@
                 self.add_label(ax)
 
         return ax
 
     def add_label(
         self,
         ax: Axes,
-        text_label: str = None,
-        va: str = None,
-        ha: str = None,
-        loc: float = None,
+        text_label: str | None = None,
+        va: str | None = None,
+        ha: str | None = None,
+        loc: float | None = None,
         **params,
     ) -> Axes:
         """Annotate the curve with its label."""
         num_samples = len(self.x_data)
         assert num_samples > 1
         text_style = {"va": "bottom", "ha": "left", "color": [0.0, 0.0, 0.0]}
         loc_f: float = self._label_loc if loc is None else loc
@@ -240,20 +240,20 @@
         return ax
 
 
 class PsychroCurves:
     """Object to store a list of psychrometric curves for plotting."""
 
     def __init__(
-        self, curves: List[PsychroCurve], family_label: str = None
+        self, curves: list[PsychroCurve], family_label: str | None = None
     ) -> None:
         """Create the Psychrocurves array object."""
-        self.curves: List[PsychroCurve] = curves
+        self.curves: list[PsychroCurve] = curves
         self.size: int = len(self.curves)
-        self.family_label: Optional[str] = family_label
+        self.family_label: str | None = family_label
 
     def __getitem__(self, item) -> PsychroCurve:
         """Get item from the PsychroCurve list."""
         return self.curves[item]
 
     def __repr__(self) -> str:
         """Object string representation."""
```

### Comparing `psychrochart-0.3.1/psychrochart/util.py` & `psychrochart-0.4.0/psychrochart/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 """A library to make psychrometric charts and overlay information in them."""
 import json
 import logging
 import os
 from pathlib import Path
 from time import time
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Sequence
 
 import numpy as np
 
 NUM_ITERS_MAX = 100
 
-path_styles = Path(__file__).parent / "chart_styles"
-DEFAULT_CHART_CONFIG_FILE = str(path_styles / "default_chart_config.json")
-ASHRAE_CHART_CONFIG_FILE = str(path_styles / "ashrae_chart_style.json")
-ASHRAE_IP_CHART_CONFIG_FILE = str(path_styles / "ashrae_ip_chart_style.json")
-INTERIOR_CHART_CONFIG_FILE = str(path_styles / "interior_chart_style.json")
-MINIMAL_CHART_CONFIG_FILE = str(path_styles / "minimal_chart_style.json")
-DEFAULT_ZONES_FILE = str(path_styles / "default_comfort_zones.json")
+PATH_STYLES = Path(__file__).parent / "chart_styles"
+DEFAULT_CHART_CONFIG_FILE = str(PATH_STYLES / "default_chart_config.json")
+ASHRAE_CHART_CONFIG_FILE = str(PATH_STYLES / "ashrae_chart_style.json")
+ASHRAE_IP_CHART_CONFIG_FILE = str(PATH_STYLES / "ashrae_ip_chart_style.json")
+INTERIOR_CHART_CONFIG_FILE = str(PATH_STYLES / "interior_chart_style.json")
+MINIMAL_CHART_CONFIG_FILE = str(PATH_STYLES / "minimal_chart_style.json")
+DEFAULT_ZONES_FILE = str(PATH_STYLES / "default_comfort_zones.json")
 
 STYLES = {
     "ashrae": ASHRAE_CHART_CONFIG_FILE,
     "ashrae_ip": ASHRAE_IP_CHART_CONFIG_FILE,
     "default": DEFAULT_CHART_CONFIG_FILE,
     "interior": INTERIOR_CHART_CONFIG_FILE,
     "minimal": MINIMAL_CHART_CONFIG_FILE,
@@ -42,16 +42,16 @@
 
         return _wrapper
 
     return _real_deco
 
 
 def _update_config(
-    old_conf: dict, new_conf: dict, recurs_idx: int = 0
-) -> Dict:
+    old_conf: dict[str, Any], new_conf: dict[str, Any], recurs_idx: int = 0
+) -> dict[str, Any]:
     """Update a dict recursively."""
     assert recurs_idx < 3
     if old_conf is None:
         return new_conf
     for key, value in old_conf.items():
         if key in new_conf:
             if isinstance(value, dict) and isinstance(new_conf[key], dict):
@@ -68,57 +68,62 @@
                 for key in filter(lambda x: x not in old_conf, new_conf)
             }
         )
     return old_conf
 
 
 def _load_config(
-    new_config: Union[Dict, str] = None, default_config_file: str = None,
-) -> Dict:
+    new_config: dict[str, Any] | str | None = None,
+    default_config_file: str | None = None,
+) -> dict[str, Any]:
     """Load plot parameters from a JSON file."""
     if default_config_file is not None:
         with open(default_config_file, encoding="utf-8") as f:
             config = json.load(f)
     else:
         config = None
     if new_config is not None:
         if isinstance(new_config, str):
-            new_config_d = {}  # type: dict
+            new_config_d = {}
             if new_config.endswith(".json"):
                 with open(new_config, encoding="utf-8") as f:
                     new_config_d.update(json.load(f))
             elif new_config in STYLES:
                 with open(STYLES[new_config], encoding="utf-8") as f:
                     new_config_d.update(json.load(f))
             config = _update_config(config, new_config_d)
         else:
             assert isinstance(new_config, dict)
             config = _update_config(config, new_config)
 
     return config
 
 
-def load_config(styles: Optional[Union[Dict, str]] = None) -> Dict:
+# TODO remove this config-loader method
+def load_config(styles: dict[str, Any] | str | None = None) -> dict[str, Any]:
     """Load the plot params for the psychrometric chart."""
     return _load_config(styles, default_config_file=DEFAULT_CHART_CONFIG_FILE)
 
 
-def load_zones(zones: Optional[Union[Dict, str]] = DEFAULT_ZONES_FILE) -> Dict:
+# TODO remove this config-loader method
+def load_zones(
+    zones: dict[str, Any] | str | None = DEFAULT_ZONES_FILE
+) -> dict[str, Any]:
     """Load a zones JSON file to overlay in the psychrometric chart."""
     return _load_config(zones)
 
 
 def _iter_solver(
     initial_value: np.ndarray,
     objective_value: np.ndarray,
     func_eval: Callable,
     initial_increment: float = 4.0,
     num_iters_max: int = NUM_ITERS_MAX,
     precision: float = 0.01,
-) -> Tuple[float, int]:
+) -> tuple[float, int]:
     """Solve by iteration."""
     decreasing = True
     increment = initial_increment
     num_iter = 0
     value_calc = initial_value.copy()
     error = objective_value - func_eval(initial_value)
     while abs(error) > precision and num_iter < num_iters_max:
@@ -165,15 +170,15 @@
     # "CONSTANT VOLUME": (0.0005, 1, 0.00000025, 0.0025, 0.75, 0.00000025),
     if family_name not in families.keys():  # pragma: no cover
         raise AssertionError(
             f"Need a valid family of curves: {list(families.keys())}"
         )
 
     precision_comp, initial_increment, precision = families[family_name]
-    calc_points: List[float] = []
+    calc_points: list[float] = []
     for objective in objective_values:
         try:
             calc_p, num_iter = _iter_solver(
                 np.array(func_init(objective)),
                 np.array(objective),
                 func_eval=func_eval,
                 initial_increment=initial_increment,
@@ -197,15 +202,15 @@
             )
             logging.error(msg)
             raise AssertionError(msg)
         calc_points.append(calc_p)
     return np.array(calc_points)
 
 
-def mod_color(color: Union[Tuple, List], modification: float) -> List[float]:
+def mod_color(color: Sequence[float], modification: float) -> list[float]:
     """Modify color with an alpha value or a darken/lighten percentage."""
     if abs(modification) < 0.999:  # is alpha level
         color = list(color[:3]) + [modification]
     else:
         color = [
             max(0.0, min(1.0, c * (1 + modification / 100))) for c in color
         ]
```

### Comparing `psychrochart-0.3.1/pyproject.toml` & `psychrochart-0.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,52 @@
+[tool.black]
+exclude = "^.*/charts/.*$"
+line_length = 79
+target_version = ["py311"]
+
+[tool.isort]
+profile = "black"
+force_sort_within_sections = true
+combine_as_imports = true
+line_length = 79
+py_version=311
+
+[tool.ruff]
+fix = true
+line-length = 79
+
+[tool.coverage.run]
+branch = true
+source = ["psychrochart"]
+relative_files = true
+
+[tool.coverage.paths]
+source = ["psychrochart/"]
+
+[tool.coverage.report]
+fail_under = 75
+skip_covered = true
+show_missing = true
+exclude_lines = [
+    "pragma: no cover",
+    "if __name__ == \"__main__\":",
+    "raise NotImplementedError",
+]
+
+[tool.pytest.ini_options]
+minversion = 6.0
+testpaths = "tests"
+addopts = "-vv -s --cov psychrochart --cov-report term --cov-report html"
+log_level = "INFO"
+log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
+log_date_format = "%Y-%m-%d %H:%M:%S"
+
 [tool.poetry]
 name = "psychrochart"
-version = "0.3.1"
+version = "0.4.0"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
@@ -16,33 +58,27 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 keywords=["psychrometrics", "moist", "humid air", "climate control", "matplotlib"]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-matplotlib = "^3.1"
-scipy = "^1.3"
-psychrolib = "^2.2"
-numpy = "^1.17"
+python = ">=3.10,<3.12"
+matplotlib = ">=3.7"
+scipy = ">=1.10"
+psychrolib = ">=2.5"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.0"
-pytest-sugar = "^0.9.2"
-pytest-cov = "^2.7"
-coveralls = "^1.8"
+pre-commit = ">=2.10.0"
+pytest = "*"
+pytest-cov = "*"
 
-[tool.black]
-exclude = "^.*/charts/.*$"
-line-length = 79
-target-version = ["py37"]
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

