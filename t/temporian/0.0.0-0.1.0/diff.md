# Comparing `tmp/temporian-0.0.0-py3-none-any.whl.zip` & `tmp/temporian-0.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,265 @@
-Zip file size: 5627 bytes, number of entries: 5
--rw-r-----  2.0 unx    11358 b- defN 23-Feb-11 06:54 temporian-0.0.0.dist-info/LICENSE
--rw-r-----  2.0 unx     1385 b- defN 23-Feb-11 06:54 temporian-0.0.0.dist-info/METADATA
--rw-r-----  2.0 unx       92 b- defN 23-Feb-11 06:54 temporian-0.0.0.dist-info/WHEEL
--rw-r-----  2.0 unx        1 b- defN 23-Feb-11 06:54 temporian-0.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      396 b- defN 23-Feb-11 06:54 temporian-0.0.0.dist-info/RECORD
-5 files, 13232 bytes uncompressed, 4887 bytes compressed:  63.1%
+Zip file size: 403827 bytes, number of entries: 263
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian-0.1.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian.libs/
+-rw-r--r--  2.0 unx    23922 b- defN 23-Jun-02 13:07 temporian-0.1.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-02 13:07 temporian-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     5493 b- defN 23-Jun-02 13:07 temporian-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jun-02 13:07 temporian-0.1.0.dist-info/LICENSE
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/io/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/proto/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/test/
+-rw-r--r--  2.0 unx     2096 b- defN 23-Jun-02 13:07 temporian/__init__.py
+-rw-r--r--  2.0 unx      886 b- defN 23-Jun-02 13:07 temporian/BUILD
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy_cc/
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-02 13:07 temporian/implementation/__init__.py
+-rw-r--r--  2.0 unx      212 b- defN 23-Jun-02 13:07 temporian/implementation/BUILD
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/operators/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/data/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/test/
+-rw-r--r--  2.0 unx     1649 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/implementation_lib.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/__init__.py
+-rw-r--r--  2.0 unx      766 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/BUILD
+-rw-r--r--  2.0 unx     3248 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/evaluation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/utils.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/operators/scalar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/operators/binary/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/
+-rw-r--r--  2.0 unx     2781 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/since_last.py
+-rw-r--r--  2.0 unx     2730 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/unary.py
+-rw-r--r--  2.0 unx     3952 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/sample.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/glue.py
+-rw-r--r--  2.0 unx     2161 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/propagate.py
+-rw-r--r--  2.0 unx     1784 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/rename.py
+-rw-r--r--  2.0 unx     4325 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/drop_index.py
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/prefix.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/__init__.py
+-rw-r--r--  2.0 unx     6592 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/BUILD
+-rw-r--r--  2.0 unx     1457 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/filter.py
+-rw-r--r--  2.0 unx     1796 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/unique_timestamps.py
+-rw-r--r--  2.0 unx     6614 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/set_index.py
+-rw-r--r--  2.0 unx     1939 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/lag.py
+-rw-r--r--  2.0 unx     2432 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/all_operators.py
+-rw-r--r--  2.0 unx     4287 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/cast.py
+-rw-r--r--  2.0 unx     2180 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/select.py
+-rw-r--r--  2.0 unx     7138 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/base.py
+-rw-r--r--  2.0 unx     1203 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/moving_min.py
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/moving_count.py
+-rw-r--r--  2.0 unx     1304 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/moving_standard_deviation.py
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/simple_moving_average.py
+-rw-r--r--  2.0 unx     1203 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/moving_max.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/__init__.py
+-rw-r--r--  2.0 unx     2887 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/BUILD
+-rw-r--r--  2.0 unx     1203 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/moving_sum.py
+-rw-r--r--  2.0 unx     3084 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/window/base.py
+-rw-r--r--  2.0 unx     1318 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/hour.py
+-rw-r--r--  2.0 unx     1318 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/year.py
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/day_of_week.py
+-rw-r--r--  2.0 unx     1326 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/month.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/__init__.py
+-rw-r--r--  2.0 unx     2696 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/BUILD
+-rw-r--r--  2.0 unx     1334 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/minute.py
+-rw-r--r--  2.0 unx     1334 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/second.py
+-rw-r--r--  2.0 unx     1372 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/day_of_year.py
+-rw-r--r--  2.0 unx     1363 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/day_of_month.py
+-rw-r--r--  2.0 unx     1353 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/iso_week.py
+-rw-r--r--  2.0 unx     2651 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/calendar/base.py
+-rw-r--r--  2.0 unx     3125 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/scalar/relational_scalar.py
+-rw-r--r--  2.0 unx      692 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/scalar/__init__.py
+-rw-r--r--  2.0 unx     1195 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/scalar/BUILD
+-rw-r--r--  2.0 unx     4182 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py
+-rw-r--r--  2.0 unx     2204 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/scalar/base.py
+-rw-r--r--  2.0 unx      772 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/binary/__init__.py
+-rw-r--r--  2.0 unx     1467 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/binary/BUILD
+-rw-r--r--  2.0 unx     3735 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/binary/relational.py
+-rw-r--r--  2.0 unx     5112 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/binary/arithmetic.py
+-rw-r--r--  2.0 unx     3650 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/binary/base.py
+-rw-r--r--  2.0 unx     2457 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/binary/logical.py
+-rw-r--r--  2.0 unx     5142 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/select_test.py
+-rw-r--r--  2.0 unx     2513 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_second_test.py
+-rw-r--r--  2.0 unx    12033 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/arithmetic_multi_index_test.py
+-rw-r--r--  2.0 unx     3659 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/logical_test.py
+-rw-r--r--  2.0 unx     9306 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/lag_test.py
+-rw-r--r--  2.0 unx    11228 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/rename_test.py
+-rw-r--r--  2.0 unx     1928 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/prefix_test.py
+-rw-r--r--  2.0 unx     4756 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_day_of_month_test.py
+-rw-r--r--  2.0 unx     7929 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/unary_test.py
+-rw-r--r--  2.0 unx     3192 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_iso_week_test.py
+-rw-r--r--  2.0 unx     5101 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/glue_test.py
+-rw-r--r--  2.0 unx     2715 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_day_of_year_test.py
+-rw-r--r--  2.0 unx     3167 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/moving_max_test.py
+-rw-r--r--  2.0 unx     8254 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/moving_standard_deviation_test.py
+-rw-r--r--  2.0 unx     3159 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/moving_min_test.py
+-rw-r--r--  2.0 unx     2563 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_month_test.py
+-rw-r--r--  2.0 unx     2911 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/since_last_test.py
+-rw-r--r--  2.0 unx    11676 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/cast_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/__init__.py
+-rw-r--r--  2.0 unx    14161 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/BUILD
+-rw-r--r--  2.0 unx     2570 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/sample_test.py
+-rw-r--r--  2.0 unx     5951 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/filter_test.py
+-rw-r--r--  2.0 unx     7349 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/relational_scalar_test.py
+-rw-r--r--  2.0 unx     2359 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/propagate_test.py
+-rw-r--r--  2.0 unx     9439 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/simple_moving_average_test.py
+-rw-r--r--  2.0 unx     8133 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/moving_count_test.py
+-rw-r--r--  2.0 unx    16209 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/arithmetic_scalar_test.py
+-rw-r--r--  2.0 unx     2587 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_minute_test.py
+-rw-r--r--  2.0 unx     2684 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_year_test.py
+-rw-r--r--  2.0 unx     9443 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/arithmetic_test.py
+-rw-r--r--  2.0 unx     9704 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/moving_sum_test.py
+-rw-r--r--  2.0 unx     8293 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/drop_index_test.py
+-rw-r--r--  2.0 unx     1888 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/unique_timestamps_test.py
+-rw-r--r--  2.0 unx     7693 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/relational_test.py
+-rw-r--r--  2.0 unx     2586 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_day_of_week_test.py
+-rw-r--r--  2.0 unx     5934 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/set_index_test.py
+-rw-r--r--  2.0 unx     2494 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/operators/test/calendar_hour_test.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy/data/test/
+-rw-r--r--  2.0 unx     8661 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/plotter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/__init__.py
+-rw-r--r--  2.0 unx      705 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/BUILD
+-rw-r--r--  2.0 unx    20546 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/event_set.py
+-rw-r--r--  2.0 unx     6077 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/plotter_matplotlib.py
+-rw-r--r--  2.0 unx     8039 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/plotter_bokeh.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/test/__init__.py
+-rw-r--r--  2.0 unx      862 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/test/BUILD
+-rw-r--r--  2.0 unx     2358 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/test/plotter_test.py
+-rw-r--r--  2.0 unx     5942 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/test/event_to_df_test.py
+-rw-r--r--  2.0 unx    15740 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/test/df_to_event_test.py
+-rw-r--r--  2.0 unx     1735 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/data/test/event_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/test/__init__.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/test/BUILD
+-rw-r--r--  2.0 unx     3012 b- defN 23-Jun-02 13:07 temporian/implementation/numpy/test/registered_operators_test.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/__init__.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/BUILD
+-rw-r--r--  2.0 unx     1579 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/sample.cc
+-rw-r--r--  2.0 unx      421 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/pyinit.cc
+-rw-r--r--  2.0 unx    14765 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/window.cc
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/__init__.py
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/BUILD
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/sample.h
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/since_last.h
+-rwxr-xr-x  2.0 unx   438728 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/operators_cc.so
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/window.h
+-rw-r--r--  2.0 unx     1496 b- defN 23-Jun-02 13:07 temporian/implementation/numpy_cc/operators/since_last.cc
+-rw-r--r--  2.0 unx     1260 b- defN 23-Jun-02 13:07 temporian/io/save_event_set.py
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-02 13:07 temporian/io/__init__.py
+-rw-r--r--  2.0 unx      478 b- defN 23-Jun-02 13:07 temporian/io/BUILD
+-rw-r--r--  2.0 unx     1482 b- defN 23-Jun-02 13:07 temporian/io/read_event_set.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/utils/test/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/utils/__init__.py
+-rw-r--r--  2.0 unx      448 b- defN 23-Jun-02 13:07 temporian/utils/BUILD
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-02 13:07 temporian/utils/config.py
+-rw-r--r--  2.0 unx     1615 b- defN 23-Jun-02 13:07 temporian/utils/compile.bzl
+-rw-r--r--  2.0 unx      194 b- defN 23-Jun-02 13:07 temporian/utils/string.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Jun-02 13:07 temporian/utils/test/string_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/utils/test/__init__.py
+-rw-r--r--  2.0 unx      259 b- defN 23-Jun-02 13:07 temporian/utils/test/BUILD
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/operators/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/data/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/test/
+-rw-r--r--  2.0 unx    13532 b- defN 23-Jun-02 13:07 temporian/core/serialization.py
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-02 13:07 temporian/core/__init__.py
+-rw-r--r--  2.0 unx     1164 b- defN 23-Jun-02 13:07 temporian/core/BUILD
+-rw-r--r--  2.0 unx     1319 b- defN 23-Jun-02 13:07 temporian/core/operator_lib.py
+-rw-r--r--  2.0 unx    10870 b- defN 23-Jun-02 13:07 temporian/core/evaluation.py
+-rw-r--r--  2.0 unx    10365 b- defN 23-Jun-02 13:07 temporian/core/graph.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/operators/window/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/operators/calendar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/operators/scalar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/operators/binary/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/operators/test/
+-rw-r--r--  2.0 unx     3633 b- defN 23-Jun-02 13:07 temporian/core/operators/since_last.py
+-rw-r--r--  2.0 unx     7334 b- defN 23-Jun-02 13:07 temporian/core/operators/unary.py
+-rw-r--r--  2.0 unx     3283 b- defN 23-Jun-02 13:07 temporian/core/operators/sample.py
+-rw-r--r--  2.0 unx     4336 b- defN 23-Jun-02 13:07 temporian/core/operators/glue.py
+-rw-r--r--  2.0 unx     4526 b- defN 23-Jun-02 13:07 temporian/core/operators/propagate.py
+-rw-r--r--  2.0 unx     7313 b- defN 23-Jun-02 13:07 temporian/core/operators/rename.py
+-rw-r--r--  2.0 unx     7683 b- defN 23-Jun-02 13:07 temporian/core/operators/drop_index.py
+-rw-r--r--  2.0 unx     3020 b- defN 23-Jun-02 13:07 temporian/core/operators/prefix.py
+-rw-r--r--  2.0 unx      594 b- defN 23-Jun-02 13:07 temporian/core/operators/__init__.py
+-rw-r--r--  2.0 unx     6173 b- defN 23-Jun-02 13:07 temporian/core/operators/BUILD
+-rw-r--r--  2.0 unx     4126 b- defN 23-Jun-02 13:07 temporian/core/operators/filter.py
+-rw-r--r--  2.0 unx     2420 b- defN 23-Jun-02 13:07 temporian/core/operators/unique_timestamps.py
+-rw-r--r--  2.0 unx     5724 b- defN 23-Jun-02 13:07 temporian/core/operators/set_index.py
+-rw-r--r--  2.0 unx     5374 b- defN 23-Jun-02 13:07 temporian/core/operators/lag.py
+-rw-r--r--  2.0 unx     3900 b- defN 23-Jun-02 13:07 temporian/core/operators/all_operators.py
+-rw-r--r--  2.0 unx    10355 b- defN 23-Jun-02 13:07 temporian/core/operators/cast.py
+-rw-r--r--  2.0 unx     3873 b- defN 23-Jun-02 13:07 temporian/core/operators/select.py
+-rw-r--r--  2.0 unx    10081 b- defN 23-Jun-02 13:07 temporian/core/operators/base.py
+-rw-r--r--  2.0 unx     2411 b- defN 23-Jun-02 13:07 temporian/core/operators/window/moving_min.py
+-rw-r--r--  2.0 unx     2423 b- defN 23-Jun-02 13:07 temporian/core/operators/window/moving_count.py
+-rw-r--r--  2.0 unx     2640 b- defN 23-Jun-02 13:07 temporian/core/operators/window/moving_standard_deviation.py
+-rw-r--r--  2.0 unx     2622 b- defN 23-Jun-02 13:07 temporian/core/operators/window/simple_moving_average.py
+-rw-r--r--  2.0 unx     2393 b- defN 23-Jun-02 13:07 temporian/core/operators/window/moving_max.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/core/operators/window/__init__.py
+-rw-r--r--  2.0 unx     2941 b- defN 23-Jun-02 13:07 temporian/core/operators/window/BUILD
+-rw-r--r--  2.0 unx     3019 b- defN 23-Jun-02 13:07 temporian/core/operators/window/moving_sum.py
+-rw-r--r--  2.0 unx     3727 b- defN 23-Jun-02 13:07 temporian/core/operators/window/base.py
+-rw-r--r--  2.0 unx     1678 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/hour.py
+-rw-r--r--  2.0 unx     1623 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/year.py
+-rw-r--r--  2.0 unx     1751 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/day_of_week.py
+-rw-r--r--  2.0 unx     1784 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/month.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/__init__.py
+-rw-r--r--  2.0 unx     2461 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/BUILD
+-rw-r--r--  2.0 unx     1701 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/minute.py
+-rw-r--r--  2.0 unx     1698 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/second.py
+-rw-r--r--  2.0 unx     1735 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/day_of_year.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/day_of_month.py
+-rw-r--r--  2.0 unx     1711 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/iso_week.py
+-rw-r--r--  2.0 unx     2469 b- defN 23-Jun-02 13:07 temporian/core/operators/calendar/base.py
+-rw-r--r--  2.0 unx     5824 b- defN 23-Jun-02 13:07 temporian/core/operators/scalar/relational_scalar.py
+-rw-r--r--  2.0 unx      776 b- defN 23-Jun-02 13:07 temporian/core/operators/scalar/__init__.py
+-rw-r--r--  2.0 unx     1101 b- defN 23-Jun-02 13:07 temporian/core/operators/scalar/BUILD
+-rw-r--r--  2.0 unx     9487 b- defN 23-Jun-02 13:07 temporian/core/operators/scalar/arithmetic_scalar.py
+-rw-r--r--  2.0 unx     4891 b- defN 23-Jun-02 13:07 temporian/core/operators/scalar/base.py
+-rw-r--r--  2.0 unx      771 b- defN 23-Jun-02 13:07 temporian/core/operators/binary/__init__.py
+-rw-r--r--  2.0 unx     1205 b- defN 23-Jun-02 13:07 temporian/core/operators/binary/BUILD
+-rw-r--r--  2.0 unx     6276 b- defN 23-Jun-02 13:07 temporian/core/operators/binary/relational.py
+-rw-r--r--  2.0 unx     6545 b- defN 23-Jun-02 13:07 temporian/core/operators/binary/arithmetic.py
+-rw-r--r--  2.0 unx     3743 b- defN 23-Jun-02 13:07 temporian/core/operators/binary/base.py
+-rw-r--r--  2.0 unx     4147 b- defN 23-Jun-02 13:07 temporian/core/operators/binary/logical.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/core/operators/test/__init__.py
+-rw-r--r--  2.0 unx      409 b- defN 23-Jun-02 13:07 temporian/core/operators/test/BUILD
+-rw-r--r--  2.0 unx     3173 b- defN 23-Jun-02 13:07 temporian/core/operators/test/propagate_test.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/core/data/test/
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-02 13:07 temporian/core/data/__init__.py
+-rw-r--r--  2.0 unx      816 b- defN 23-Jun-02 13:07 temporian/core/data/BUILD
+-rw-r--r--  2.0 unx     3016 b- defN 23-Jun-02 13:07 temporian/core/data/dtype.py
+-rw-r--r--  2.0 unx     7070 b- defN 23-Jun-02 13:07 temporian/core/data/duration.py
+-rw-r--r--  2.0 unx    15003 b- defN 23-Jun-02 13:07 temporian/core/data/node.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Jun-02 13:07 temporian/core/data/feature.py
+-rw-r--r--  2.0 unx     4690 b- defN 23-Jun-02 13:07 temporian/core/data/sampling.py
+-rw-r--r--  2.0 unx      336 b- defN 23-Jun-02 13:07 temporian/core/data/test/BUILD
+-rw-r--r--  2.0 unx     1372 b- defN 23-Jun-02 13:07 temporian/core/data/test/node_test.py
+-rw-r--r--  2.0 unx     4461 b- defN 23-Jun-02 13:07 temporian/core/test/graph_test.py
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jun-02 13:07 temporian/core/test/serialization_test.py
+-rw-r--r--  2.0 unx     2604 b- defN 23-Jun-02 13:07 temporian/core/test/operator_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/core/test/__init__.py
+-rw-r--r--  2.0 unx     3041 b- defN 23-Jun-02 13:07 temporian/core/test/BUILD
+-rw-r--r--  2.0 unx     2970 b- defN 23-Jun-02 13:07 temporian/core/test/registered_operators_test.py
+-rw-r--r--  2.0 unx    17242 b- defN 23-Jun-02 13:07 temporian/core/test/magic_methods_test.py
+-rw-r--r--  2.0 unx     6967 b- defN 23-Jun-02 13:07 temporian/core/test/evaluation_test.py
+-rw-r--r--  2.0 unx     8451 b- defN 23-Jun-02 13:07 temporian/core/test/utils.py
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-02 13:07 temporian/proto/__init__.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Jun-02 13:07 temporian/proto/BUILD
+-rwxr-xr-x  2.0 unx     6248 b- defN 23-Jun-02 13:07 temporian/proto/core_pb2.py
+-rw-r--r--  2.0 unx     4627 b- defN 23-Jun-02 13:07 temporian/proto/core.proto
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/test/test_data/
+-rw-r--r--  2.0 unx     4851 b- defN 23-Jun-02 13:07 temporian/test/prototype_test_numpy.py
+-rw-r--r--  2.0 unx     5109 b- defN 23-Jun-02 13:07 temporian/test/api_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:07 temporian/test/__init__.py
+-rw-r--r--  2.0 unx      821 b- defN 23-Jun-02 13:07 temporian/test/BUILD
+-rw-r--r--  2.0 unx     2004 b- defN 23-Jun-02 13:07 temporian/test/io_test.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/test/test_data/io/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 13:07 temporian/test/test_data/prototype/
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-02 13:07 temporian/test/test_data/io/input.csv
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-02 13:07 temporian/test/test_data/prototype/left_event.csv
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-02 13:07 temporian/test/test_data/prototype/right_event.csv
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-02 13:07 temporian/test/test_data/prototype/output_event.csv
+263 files, 1263454 bytes uncompressed, 360255 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -1,16 +1,790 @@
-Filename: temporian-0.0.0.dist-info/LICENSE
+Filename: temporian-0.1.0.dist-info/
 Comment: 
 
-Filename: temporian-0.0.0.dist-info/METADATA
+Filename: temporian/
 Comment: 
 
-Filename: temporian-0.0.0.dist-info/WHEEL
+Filename: temporian.libs/
 Comment: 
 
-Filename: temporian-0.0.0.dist-info/top_level.txt
+Filename: temporian-0.1.0.dist-info/RECORD
 Comment: 
 
-Filename: temporian-0.0.0.dist-info/RECORD
+Filename: temporian-0.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: temporian-0.1.0.dist-info/METADATA
+Comment: 
+
+Filename: temporian-0.1.0.dist-info/LICENSE
+Comment: 
+
+Filename: temporian/implementation/
+Comment: 
+
+Filename: temporian/io/
+Comment: 
+
+Filename: temporian/utils/
+Comment: 
+
+Filename: temporian/core/
+Comment: 
+
+Filename: temporian/proto/
+Comment: 
+
+Filename: temporian/test/
+Comment: 
+
+Filename: temporian/__init__.py
+Comment: 
+
+Filename: temporian/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/
+Comment: 
+
+Filename: temporian/implementation/__init__.py
+Comment: 
+
+Filename: temporian/implementation/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/
+Comment: 
+
+Filename: temporian/implementation/numpy/data/
+Comment: 
+
+Filename: temporian/implementation/numpy/test/
+Comment: 
+
+Filename: temporian/implementation/numpy/implementation_lib.py
+Comment: 
+
+Filename: temporian/implementation/numpy/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/evaluation.py
+Comment: 
+
+Filename: temporian/implementation/numpy/utils.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/scalar/
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/binary/
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/since_last.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/unary.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/sample.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/glue.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/propagate.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/rename.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/drop_index.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/prefix.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/filter.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/unique_timestamps.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/set_index.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/lag.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/all_operators.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/cast.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/select.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/base.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/moving_min.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/moving_count.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/moving_standard_deviation.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/simple_moving_average.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/moving_max.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/moving_sum.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/window/base.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/hour.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/year.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/day_of_week.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/month.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/minute.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/second.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/day_of_year.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/day_of_month.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/iso_week.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/calendar/base.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/scalar/relational_scalar.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/scalar/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/scalar/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/scalar/base.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/binary/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/binary/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/binary/relational.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/binary/arithmetic.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/binary/base.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/binary/logical.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/select_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_second_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/arithmetic_multi_index_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/logical_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/lag_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/rename_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/prefix_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_day_of_month_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/unary_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_iso_week_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/glue_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_day_of_year_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/moving_max_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/moving_standard_deviation_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/moving_min_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_month_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/since_last_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/cast_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/sample_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/filter_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/relational_scalar_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/propagate_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/simple_moving_average_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/moving_count_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/arithmetic_scalar_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_minute_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_year_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/arithmetic_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/moving_sum_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/drop_index_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/unique_timestamps_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/relational_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_day_of_week_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/set_index_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/operators/test/calendar_hour_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/test/
+Comment: 
+
+Filename: temporian/implementation/numpy/data/plotter.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/data/event_set.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/plotter_matplotlib.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/plotter_bokeh.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/test/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/test/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/data/test/plotter_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/test/event_to_df_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/test/df_to_event_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/data/test/event_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy/test/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy/test/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy/test/registered_operators_test.py
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/sample.cc
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/pyinit.cc
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/window.cc
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/__init__.py
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/BUILD
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/sample.h
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/since_last.h
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/operators_cc.so
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/window.h
+Comment: 
+
+Filename: temporian/implementation/numpy_cc/operators/since_last.cc
+Comment: 
+
+Filename: temporian/io/save_event_set.py
+Comment: 
+
+Filename: temporian/io/__init__.py
+Comment: 
+
+Filename: temporian/io/BUILD
+Comment: 
+
+Filename: temporian/io/read_event_set.py
+Comment: 
+
+Filename: temporian/utils/test/
+Comment: 
+
+Filename: temporian/utils/__init__.py
+Comment: 
+
+Filename: temporian/utils/BUILD
+Comment: 
+
+Filename: temporian/utils/config.py
+Comment: 
+
+Filename: temporian/utils/compile.bzl
+Comment: 
+
+Filename: temporian/utils/string.py
+Comment: 
+
+Filename: temporian/utils/test/string_test.py
+Comment: 
+
+Filename: temporian/utils/test/__init__.py
+Comment: 
+
+Filename: temporian/utils/test/BUILD
+Comment: 
+
+Filename: temporian/core/operators/
+Comment: 
+
+Filename: temporian/core/data/
+Comment: 
+
+Filename: temporian/core/test/
+Comment: 
+
+Filename: temporian/core/serialization.py
+Comment: 
+
+Filename: temporian/core/__init__.py
+Comment: 
+
+Filename: temporian/core/BUILD
+Comment: 
+
+Filename: temporian/core/operator_lib.py
+Comment: 
+
+Filename: temporian/core/evaluation.py
+Comment: 
+
+Filename: temporian/core/graph.py
+Comment: 
+
+Filename: temporian/core/operators/window/
+Comment: 
+
+Filename: temporian/core/operators/calendar/
+Comment: 
+
+Filename: temporian/core/operators/scalar/
+Comment: 
+
+Filename: temporian/core/operators/binary/
+Comment: 
+
+Filename: temporian/core/operators/test/
+Comment: 
+
+Filename: temporian/core/operators/since_last.py
+Comment: 
+
+Filename: temporian/core/operators/unary.py
+Comment: 
+
+Filename: temporian/core/operators/sample.py
+Comment: 
+
+Filename: temporian/core/operators/glue.py
+Comment: 
+
+Filename: temporian/core/operators/propagate.py
+Comment: 
+
+Filename: temporian/core/operators/rename.py
+Comment: 
+
+Filename: temporian/core/operators/drop_index.py
+Comment: 
+
+Filename: temporian/core/operators/prefix.py
+Comment: 
+
+Filename: temporian/core/operators/__init__.py
+Comment: 
+
+Filename: temporian/core/operators/BUILD
+Comment: 
+
+Filename: temporian/core/operators/filter.py
+Comment: 
+
+Filename: temporian/core/operators/unique_timestamps.py
+Comment: 
+
+Filename: temporian/core/operators/set_index.py
+Comment: 
+
+Filename: temporian/core/operators/lag.py
+Comment: 
+
+Filename: temporian/core/operators/all_operators.py
+Comment: 
+
+Filename: temporian/core/operators/cast.py
+Comment: 
+
+Filename: temporian/core/operators/select.py
+Comment: 
+
+Filename: temporian/core/operators/base.py
+Comment: 
+
+Filename: temporian/core/operators/window/moving_min.py
+Comment: 
+
+Filename: temporian/core/operators/window/moving_count.py
+Comment: 
+
+Filename: temporian/core/operators/window/moving_standard_deviation.py
+Comment: 
+
+Filename: temporian/core/operators/window/simple_moving_average.py
+Comment: 
+
+Filename: temporian/core/operators/window/moving_max.py
+Comment: 
+
+Filename: temporian/core/operators/window/__init__.py
+Comment: 
+
+Filename: temporian/core/operators/window/BUILD
+Comment: 
+
+Filename: temporian/core/operators/window/moving_sum.py
+Comment: 
+
+Filename: temporian/core/operators/window/base.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/hour.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/year.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/day_of_week.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/month.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/__init__.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/BUILD
+Comment: 
+
+Filename: temporian/core/operators/calendar/minute.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/second.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/day_of_year.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/day_of_month.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/iso_week.py
+Comment: 
+
+Filename: temporian/core/operators/calendar/base.py
+Comment: 
+
+Filename: temporian/core/operators/scalar/relational_scalar.py
+Comment: 
+
+Filename: temporian/core/operators/scalar/__init__.py
+Comment: 
+
+Filename: temporian/core/operators/scalar/BUILD
+Comment: 
+
+Filename: temporian/core/operators/scalar/arithmetic_scalar.py
+Comment: 
+
+Filename: temporian/core/operators/scalar/base.py
+Comment: 
+
+Filename: temporian/core/operators/binary/__init__.py
+Comment: 
+
+Filename: temporian/core/operators/binary/BUILD
+Comment: 
+
+Filename: temporian/core/operators/binary/relational.py
+Comment: 
+
+Filename: temporian/core/operators/binary/arithmetic.py
+Comment: 
+
+Filename: temporian/core/operators/binary/base.py
+Comment: 
+
+Filename: temporian/core/operators/binary/logical.py
+Comment: 
+
+Filename: temporian/core/operators/test/__init__.py
+Comment: 
+
+Filename: temporian/core/operators/test/BUILD
+Comment: 
+
+Filename: temporian/core/operators/test/propagate_test.py
+Comment: 
+
+Filename: temporian/core/data/test/
+Comment: 
+
+Filename: temporian/core/data/__init__.py
+Comment: 
+
+Filename: temporian/core/data/BUILD
+Comment: 
+
+Filename: temporian/core/data/dtype.py
+Comment: 
+
+Filename: temporian/core/data/duration.py
+Comment: 
+
+Filename: temporian/core/data/node.py
+Comment: 
+
+Filename: temporian/core/data/feature.py
+Comment: 
+
+Filename: temporian/core/data/sampling.py
+Comment: 
+
+Filename: temporian/core/data/test/BUILD
+Comment: 
+
+Filename: temporian/core/data/test/node_test.py
+Comment: 
+
+Filename: temporian/core/test/graph_test.py
+Comment: 
+
+Filename: temporian/core/test/serialization_test.py
+Comment: 
+
+Filename: temporian/core/test/operator_test.py
+Comment: 
+
+Filename: temporian/core/test/__init__.py
+Comment: 
+
+Filename: temporian/core/test/BUILD
+Comment: 
+
+Filename: temporian/core/test/registered_operators_test.py
+Comment: 
+
+Filename: temporian/core/test/magic_methods_test.py
+Comment: 
+
+Filename: temporian/core/test/evaluation_test.py
+Comment: 
+
+Filename: temporian/core/test/utils.py
+Comment: 
+
+Filename: temporian/proto/__init__.py
+Comment: 
+
+Filename: temporian/proto/BUILD
+Comment: 
+
+Filename: temporian/proto/core_pb2.py
+Comment: 
+
+Filename: temporian/proto/core.proto
+Comment: 
+
+Filename: temporian/test/test_data/
+Comment: 
+
+Filename: temporian/test/prototype_test_numpy.py
+Comment: 
+
+Filename: temporian/test/api_test.py
+Comment: 
+
+Filename: temporian/test/__init__.py
+Comment: 
+
+Filename: temporian/test/BUILD
+Comment: 
+
+Filename: temporian/test/io_test.py
+Comment: 
+
+Filename: temporian/test/test_data/io/
+Comment: 
+
+Filename: temporian/test/test_data/prototype/
+Comment: 
+
+Filename: temporian/test/test_data/io/input.csv
+Comment: 
+
+Filename: temporian/test/test_data/prototype/left_event.csv
+Comment: 
+
+Filename: temporian/test/test_data/prototype/right_event.csv
+Comment: 
+
+Filename: temporian/test/test_data/prototype/output_event.csv
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `temporian-0.0.0.dist-info/LICENSE` & `temporian-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

