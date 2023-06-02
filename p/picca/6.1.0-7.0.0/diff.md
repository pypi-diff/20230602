# Comparing `tmp/picca-6.1.0.tar.gz` & `tmp/picca-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picca-6.1.0.tar", last modified: Sat Dec 24 19:33:09 2022, max compression
+gzip compressed data, was "picca-7.0.0.tar", last modified: Fri Jun  2 13:23:49 2023, max compression
```

## Comparing `picca-6.1.0.tar` & `picca-7.0.0.tar`

### file list

```diff
@@ -1,212 +1,214 @@
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.931293 picca-6.1.0/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    35141 2021-11-29 16:42:40.000000 picca-6.1.0/LICENSE
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6090 2022-12-24 19:33:09.931293 picca-6.1.0/PKG-INFO
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5763 2022-12-24 06:37:39.000000 picca-6.1.0/README.md
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.915293 picca-6.1.0/bin/
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    23434 2022-12-22 15:21:24.000000 picca-6.1.0/bin/picca_Pk1D.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     9354 2022-12-22 15:21:24.000000 picca-6.1.0/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15178 2022-12-24 19:29:18.000000 picca-6.1.0/bin/picca_cf.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    10900 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_cf1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    10572 2022-12-24 19:29:18.000000 picca-6.1.0/bin/picca_cf_angl.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12071 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_co.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14263 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_coadd_zint.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     9312 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5833 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     3480 2022-12-21 15:35:36.000000 picca-6.1.0/bin/picca_convert_transmission.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1908 2022-12-21 15:35:36.000000 picca-6.1.0/bin/picca_delta_extraction.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14989 2022-12-21 15:35:36.000000 picca-6.1.0/bin/picca_dmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12239 2022-12-21 15:35:36.000000 picca-6.1.0/bin/picca_export.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14187 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_export_co.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     4728 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    18993 2022-12-21 15:35:36.000000 picca-6.1.0/bin/picca_metal_dmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    17399 2022-12-21 15:35:36.000000 picca-6.1.0/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    27530 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_nersc_submit.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     2201 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_pk2fits.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5870 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1251 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_reduce_spall.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    18112 2022-12-21 15:35:36.000000 picca-6.1.0/bin/picca_wick.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16147 2022-12-24 19:29:18.000000 picca-6.1.0/bin/picca_xcf.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11397 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_xcf1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    13283 2022-02-03 13:41:19.000000 picca-6.1.0/bin/picca_xcf_angl.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14598 2022-12-21 15:35:36.000000 picca-6.1.0/bin/picca_xdmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    17088 2022-12-24 19:29:18.000000 picca-6.1.0/bin/picca_xwick.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.907293 picca-6.1.0/py/
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.915293 picca-6.1.0/py/picca/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       46 2021-11-29 16:42:41.000000 picca-6.1.0/py/picca/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       22 2022-12-24 19:30:16.000000 picca-6.1.0/py/picca/_version.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3364 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/bal_tools.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.919293 picca-6.1.0/py/picca/bin/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)        0 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/__init__.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.919293 picca-6.1.0/py/picca/bin/old/
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    43689 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/bin/old/picca_deltas.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      722 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/bin/old/picca_fitter2.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      575 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/bin/old/picca_fitter2_control.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      614 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/bin/old/picca_fitter2_control_mpi.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    23434 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/bin/picca_Pk1D.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     9354 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15178 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/bin/picca_cf.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    10900 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_cf1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    10572 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/bin/picca_cf_angl.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12071 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_co.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14263 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_coadd_zint.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     9312 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5833 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     3480 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/bin/picca_convert_transmission.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1908 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/bin/picca_delta_extraction.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14989 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/bin/picca_dmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12239 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/bin/picca_export.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14187 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_export_co.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     4728 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    18993 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/bin/picca_metal_dmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    17399 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    27530 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_nersc_submit.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     2201 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_pk2fits.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5870 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1251 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_reduce_spall.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    18112 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/bin/picca_wick.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16147 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/bin/picca_xcf.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11397 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_xcf1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    13283 2022-02-03 13:41:19.000000 picca-6.1.0/py/picca/bin/picca_xcf_angl.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14598 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/bin/picca_xdmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    17088 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/bin/picca_xwick.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    82994 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/cf.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10525 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/co.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10335 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/constants.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    12823 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/converters.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    50827 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/data.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.919293 picca-6.1.0/py/picca/delta_extraction/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5075 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/astronomical_object.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.919293 picca-6.1.0/py/picca/delta_extraction/astronomical_objects/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/astronomical_objects/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5710 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     9213 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25750 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/delta_extraction/astronomical_objects/forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11352 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5936 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1170 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    27062 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/config.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      941 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/correction.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.919293 picca-6.1.0/py/picca/delta_extraction/corrections/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/corrections/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3986 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/corrections/calibration_correction.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5974 2022-06-13 12:34:03.000000 picca-6.1.0/py/picca/delta_extraction/corrections/dust_correction.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3457 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/corrections/ivar_correction.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4115 2022-06-13 12:34:03.000000 picca-6.1.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    20398 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/delta_extraction/data.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.923293 picca-6.1.0/py/picca/delta_extraction/data_catalogues/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/data_catalogues/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    14759 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/data_catalogues/desi_data.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8585 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8906 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2145 2022-06-13 12:34:03.000000 picca-6.1.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10823 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1144 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/errors.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16147 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/expected_flux.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.923293 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    29862 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3784 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1688 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1718 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2563 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3865 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3960 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1729 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.923293 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    21268 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    15906 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19543 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    18098 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4628 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/expected_fluxes/utils.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.923293 picca-6.1.0/py/picca/delta_extraction/least_squares/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/least_squares/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6416 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7566 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1808 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/mask.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.923293 picca-6.1.0/py/picca/delta_extraction/masks/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/masks/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4058 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/masks/absorber_mask.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8257 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/masks/bal_mask.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11613 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/masks/dla_mask.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3130 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/masks/lines_mask.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2996 2022-06-13 12:34:03.000000 picca-6.1.0/py/picca/delta_extraction/quasar_catalogue.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.927293 picca-6.1.0/py/picca/delta_extraction/quasar_catalogues/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8026 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    12203 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1817 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/rejection_log.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.927293 picca-6.1.0/py/picca/delta_extraction/rejection_logs/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/rejection_logs/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2461 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3275 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8621 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/delta_extraction/survey.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10765 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/utils.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10817 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/delta_extraction/utils_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5953 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/dla.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.927293 picca-6.1.0/py/picca/fitter2/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)        0 2021-11-29 16:42:41.000000 picca-6.1.0/py/picca/fitter2/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19385 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/fitter2/chi2.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1031 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/control.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    13706 2021-11-29 16:42:41.000000 picca-6.1.0/py/picca/fitter2/control_mpi.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    20123 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/fitter2/data.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     6784 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/effective-bins.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.911293 picca-6.1.0/py/picca/fitter2/models/
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.927293 picca-6.1.0/py/picca/fitter2/models/DR16_blind_test_large/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.927293 picca-6.1.0/py/picca/fitter2/models/DR16_blind_test_small/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.927293 picca-6.1.0/py/picca/fitter2/models/DR9LyaMocks/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25920 2021-11-29 16:42:41.000000 picca-6.1.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.927293 picca-6.1.0/py/picca/fitter2/models/PlanckDR12/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25920 2021-11-29 16:42:41.000000 picca-6.1.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.927293 picca-6.1.0/py/picca/fitter2/models/PlanckDR16/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2021-11-29 16:42:41.000000 picca-6.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1556 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/myGamma.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8089 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/parser.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16465 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/pk.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      554 2021-11-29 16:42:41.000000 picca-6.1.0/py/picca/fitter2/priors.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5369 2021-11-29 16:42:41.000000 picca-6.1.0/py/picca/fitter2/sampler.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3921 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/fitter2/utils.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10748 2022-02-03 13:41:20.000000 picca-6.1.0/py/picca/fitter2/xi.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    63899 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/io.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.931293 picca-6.1.0/py/picca/pk1d/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19884 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/pk1d/compute_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    17419 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/pk1d/postproc_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8518 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/pk1d/prep_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      645 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/pk1d/utils.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    13939 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/prep_del.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19596 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/raw_io.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.931293 picca-6.1.0/py/picca/tests/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      250 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/tests/__init__.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.931293 picca-6.1.0/py/picca/tests/delta_extraction/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2022-03-31 16:50:19.000000 picca-6.1.0/py/picca/tests/delta_extraction/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10832 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/tests/delta_extraction/abstract_test.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    87682 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    23177 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/tests/delta_extraction/config_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10456 2022-06-13 12:34:03.000000 picca-6.1.0/py/picca/tests/delta_extraction/correction_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    62257 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/tests/delta_extraction/data_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    80849 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/tests/delta_extraction/expected_flux_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7912 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/tests/delta_extraction/mask_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    18721 2022-06-13 12:34:04.000000 picca-6.1.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6230 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/tests/delta_extraction/scripts_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7924 2022-09-15 13:32:16.000000 picca-6.1.0/py/picca/tests/delta_extraction/test_utils.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.931293 picca-6.1.0/py/picca/tests/old/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    17429 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/tests/old/test_1_deltas.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3651 2022-12-22 15:21:24.000000 picca-6.1.0/py/picca/tests/old/test_4_fitter2.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2022 2022-12-21 15:35:36.000000 picca-6.1.0/py/picca/tests/test_2_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    22733 2022-12-24 19:29:18.000000 picca-6.1.0/py/picca/tests/test_3_cor.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11334 2022-03-31 16:50:20.000000 picca-6.1.0/py/picca/tests/test_helpers.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16216 2022-03-31 16:50:20.000000 picca-6.1.0/py/picca/utils.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1504 2022-02-03 13:41:21.000000 picca-6.1.0/py/picca/wedgize.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    54086 2022-02-03 13:41:21.000000 picca-6.1.0/py/picca/xcf.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2022-12-24 19:33:09.915293 picca-6.1.0/py/picca.egg-info/
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     6090 2022-12-24 19:33:09.000000 picca-6.1.0/py/picca.egg-info/PKG-INFO
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     7113 2022-12-24 19:33:09.000000 picca-6.1.0/py/picca.egg-info/SOURCES.txt
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        1 2022-12-24 19:33:09.000000 picca-6.1.0/py/picca.egg-info/dependency_links.txt
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)       82 2022-12-24 19:33:09.000000 picca-6.1.0/py/picca.egg-info/requires.txt
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        6 2022-12-24 19:33:09.000000 picca-6.1.0/py/picca.egg-info/top_level.txt
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      133 2022-03-31 16:50:20.000000 picca-6.1.0/pyproject.toml
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       38 2022-12-24 19:33:09.931293 picca-6.1.0/setup.cfg
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1234 2022-12-21 15:35:36.000000 picca-6.1.0/setup.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.968002 picca-7.0.0/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    35141 2021-11-29 16:42:40.000000 picca-7.0.0/LICENSE
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6155 2023-06-02 13:23:49.964002 picca-7.0.0/PKG-INFO
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5828 2023-03-10 09:08:48.000000 picca-7.0.0/README.md
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.952002 picca-7.0.0/bin/
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    24135 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_Pk1D.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    10849 2023-06-02 13:08:37.000000 picca-7.0.0/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16058 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_cf.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11731 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_cf1d.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11265 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_cf_angl.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12071 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_co.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14263 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     9312 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5833 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     3480 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1908 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15850 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_dmat.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12239 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_export.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14187 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_export_co.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     4728 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    19846 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    18174 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    27530 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     2201 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_pk2fits.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5870 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1251 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    19061 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_wick.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16708 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_xcf.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12008 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_xcf1d.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    13810 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15413 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_xdmat.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    17951 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_xwick.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.948002 picca-7.0.0/py/
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.952002 picca-7.0.0/py/picca/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       46 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       22 2023-06-02 13:19:03.000000 picca-7.0.0/py/picca/_version.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3364 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bal_tools.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.956002 picca-7.0.0/py/picca/bin/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)        0 2022-02-03 13:41:19.000000 picca-7.0.0/py/picca/bin/__init__.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.956002 picca-7.0.0/py/picca/bin/old/
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    43689 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/old/picca_deltas.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      722 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/old/picca_fitter2.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      575 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/old/picca_fitter2_control.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      614 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/old/picca_fitter2_control_mpi.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    24135 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_Pk1D.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    10849 2023-06-02 13:08:37.000000 picca-7.0.0/py/picca/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16058 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_cf.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11731 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_cf1d.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11265 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_cf_angl.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12071 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_co.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14263 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     9312 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5833 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     3480 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1908 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15850 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_dmat.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12239 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_export.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14187 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_export_co.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     4728 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    19846 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    18174 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    27530 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     2201 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_pk2fits.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5870 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1251 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    19061 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_wick.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16708 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_xcf.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12008 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_xcf1d.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    13810 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15413 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_xdmat.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    17951 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_xwick.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    64077 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/cf.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7828 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/co.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10611 2023-05-31 16:28:55.000000 picca-7.0.0/py/picca/constants.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    12823 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/converters.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    51080 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/data.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.956002 picca-7.0.0/py/picca/delta_extraction/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5067 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_object.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5729 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     9213 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25713 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/forest.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11372 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5955 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1170 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    27062 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/config.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      941 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/correction.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/corrections/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/corrections/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4062 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/corrections/calibration_correction.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5974 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/corrections/dust_correction.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3454 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/corrections/ivar_correction.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4115 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    22238 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/data.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/data_catalogues/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    14819 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_data.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8585 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8906 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2145 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10874 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1131 2023-03-10 09:08:48.000000 picca-7.0.0/py/picca/delta_extraction/errors.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16433 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/expected_flux.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    30238 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3794 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1688 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1718 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2620 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3875 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3970 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1729 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    21268 2022-03-31 16:50:19.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    15906 2022-03-31 16:50:19.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19543 2022-03-31 16:50:19.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19675 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4628 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/utils.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/least_squares/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/least_squares/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6416 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7476 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2026 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/delta_extraction/mask.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/masks/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/masks/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4303 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/delta_extraction/masks/absorber_mask.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8367 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/masks/bal_mask.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     9918 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/masks/dla_mask.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3286 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/delta_extraction/masks/lines_mask.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2996 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/quasar_catalogue.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8146 2023-03-10 09:08:48.000000 picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    12201 2023-03-10 09:08:48.000000 picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1817 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/rejection_log.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/rejection_logs/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/rejection_logs/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2716 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3275 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8733 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/survey.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11272 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/utils.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10817 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/utils_pk1d.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5953 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/dla.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)        0 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/fitter2/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19385 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/chi2.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1031 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/control.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    13706 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/control_mpi.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    20123 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/data.py
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     6784 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/effective-bins.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.948002 picca-7.0.0/py/picca/fitter2/models/
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_large/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_small/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/DR9LyaMocks/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25920 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/Planck18/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2023-01-23 16:50:46.000000 picca-7.0.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/PlanckDR12/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25920 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/PlanckDR16/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-7.0.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1556 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/myGamma.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8089 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/parser.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16465 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/pk.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      554 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/priors.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5369 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/sampler.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3921 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/utils.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10748 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/xi.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    64892 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/io.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/pk1d/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19994 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/pk1d/compute_pk1d.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    38897 2023-06-02 13:08:37.000000 picca-7.0.0/py/picca/pk1d/postproc_pk1d.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     9245 2023-06-02 13:08:37.000000 picca-7.0.0/py/picca/pk1d/prep_pk1d.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1071 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/pk1d/utils.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    13939 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/prep_del.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19665 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/raw_io.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/tests/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      250 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/__init__.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/tests/delta_extraction/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/delta_extraction/__init__.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10670 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/tests/delta_extraction/abstract_test.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    88977 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    23177 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/delta_extraction/config_tests.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10454 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/tests/delta_extraction/correction_tests.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    63846 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/tests/delta_extraction/data_tests.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    81274 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/tests/delta_extraction/expected_flux_tests.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    31778 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/tests/delta_extraction/mask_tests.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    18721 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6230 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/delta_extraction/scripts_tests.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7957 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/tests/delta_extraction/test_utils.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/tests/old/
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    17429 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/old/test_1_deltas.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3651 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/old/test_4_fitter2.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3337 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/tests/test_2_pk1d.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    42559 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/tests/test_3_cor.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11334 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/test_helpers.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16216 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/utils.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1504 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/wedgize.py
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    40856 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/xcf.py
+drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.952002 picca-7.0.0/py/picca.egg-info/
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     6155 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/PKG-INFO
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     7168 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/SOURCES.txt
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        1 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/dependency_links.txt
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)       82 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/requires.txt
+-rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        6 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/top_level.txt
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      133 2022-03-31 16:50:20.000000 picca-7.0.0/pyproject.toml
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       38 2023-06-02 13:23:49.968002 picca-7.0.0/setup.cfg
+-rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1236 2023-03-10 09:08:44.000000 picca-7.0.0/setup.py
```

### Comparing `picca-6.1.0/LICENSE` & `picca-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/PKG-INFO` & `picca-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 6.1.0
+Version: 7.0.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
 Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -160,14 +160,16 @@
 
 ### For Developers
 Before submitting a PR please make sure to:
 1. Check the tutorials. Update them if necessary (typically the tutorial `picca_delta_extraction_configuration_tutorial` will need to be updated.
 2. Update the data model
 3. For every file you have modified run
    ```
-   yapf --style google file.py -i 
+   yapf --style google file.py -i
    ```
    to ensure the coding styles are maintained.
 4. Consider using pylint to help in the debug process. From the repo folder run
    ```
-   pylint py/picca/delta_extraction/**/*py
+   pylint py/picca/delta_extraction/
+   pylint py/picca/pk1d/
    ```
+   depending on the module you are working on.
```

### Comparing `picca-6.1.0/README.md` & `picca-7.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,16 @@
 
 ### For Developers
 Before submitting a PR please make sure to:
 1. Check the tutorials. Update them if necessary (typically the tutorial `picca_delta_extraction_configuration_tutorial` will need to be updated.
 2. Update the data model
 3. For every file you have modified run
    ```
-   yapf --style google file.py -i 
+   yapf --style google file.py -i
    ```
    to ensure the coding styles are maintained.
 4. Consider using pylint to help in the debug process. From the repo folder run
    ```
-   pylint py/picca/delta_extraction/**/*py
+   pylint py/picca/delta_extraction/
+   pylint py/picca/pk1d/
    ```
+   depending on the module you are working on.
```

### Comparing `picca-6.1.0/bin/picca_Pk1D.py` & `picca-7.0.0/bin/picca_Pk1D.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
                 delta.mean_reso=1e-3
                 delta.mean_reso_pix=1e-3
                 delta.exposures_diff = np.zeros(delta.delta.shape)
             running_on_raw_transmission = True
     elif args.in_format == 'ascii':
         ascii_file = open(file, 'r')
         deltas = [Delta.from_ascii(line) for line in ascii_file]
+        running_on_raw_transmission = False
 
     #add the check for linear binning on first spectrum only (assuming homogeneity within the file)
     delta = deltas[0]
     linear_binning, pixel_step = check_linear_binning(delta)
     if linear_binning:
         userprint("\n\nUsing linear binning, results will have units of AA")
         if (args.disable_reso_matrix or not hasattr(delta, 'resolution_matrix')
@@ -237,15 +238,16 @@
                 #in this case all is in AA space
                 if reso_correction == 'matrix':
                     correction_reso = compute_correction_reso_matrix(
                         reso_matrix=np.mean(reso_matrix_array[part_index],
                                             axis=1),
                         k=k,
                         delta_pixel=pixel_step,
-                        num_pixel=len(lambda_new))
+                        num_pixel=len(lambda_new),
+                        pixelization_correction = args.add_pixelization_correction)
                 elif reso_correction == 'Gaussian':
                     #this is roughly converting the mean resolution estimate back to pixels
                     #and then multiplying with pixel size
                     mean_reso_AA = pixel_step * delta.mean_reso_pix
                     correction_reso = compute_correction_reso(
                         delta_pixel=pixel_step, mean_reso=mean_reso_AA, k=k)
             elif not running_on_raw_transmission:
@@ -332,14 +334,18 @@
                     'name': 'LIN_BIN',
                     'value': linear_binning,
                     'comment': "analysis was performed on delta with linear binned lambda"
                 }, {
                     'name': 'LOS_ID',
                     'value': delta.los_id,
                     'comment': "line of sight identifier, e.g. THING_ID or TARGETID"
+                }, {
+                    'name': 'CHUNK_ID',
+                    'value': part_index,
+                    'comment': "Chunk (sub-forest) identifier"
                 },
                 ]
 
                 cols = [k, pk_raw, pk_noise, pk_diff, correction_reso, pk]
                 names = [
                     'K', 'PK_RAW', 'PK_NOISE', 'PK_DIFF', 'COR_RESO', 'PK'
                 ]
@@ -499,14 +505,23 @@
     parser.add_argument('--disable-reso-matrix',
                         default=False,
                         action='store_true',
                         required=False,
                         help=('do not use the resolution matrix even '
                               'if it exists and we are on linear binning'))
 
+    parser.add_argument('--add-pixelization-correction',
+                        default=False,
+                        action='store_true',
+                        required=False,
+                        help=('Add a pixelization correction, as if the resolution  '
+                              'matrix was doubly pixelized. Only use this option in '
+                              'quickquasars mocks'))
+
+
     parser.add_argument(
         '--force-output-in-velocity',
         default=False,
         action='store_true',
         required=False,
         help=
         ('store outputs in units of velocity even for linear binning computations'
```

### Comparing `picca-6.1.0/bin/picca_Pk1D_postprocess.py` & `picca-7.0.0/bin/picca_Pk1D_postprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,16 +113,24 @@
                         required=False,
                         help='Size of a spectrum pixel in Angstrom, used to'
                              'define the binning of the output wavenumber array')
 
     parser.add_argument('--weight-method',
                         type=str,
                         default='no_weights',
-                        help='Weighting scheme for the mean P1D computation,'
-                             'Possible options: no_weights, simple_snr, fit_snr')
+                        help='SNR weighting scheme for the mean P1D computation,'
+                             'Possible options: no_weights, fit_snr')
+
+    parser.add_argument('--apply_z_weights',
+                        action='store_true',
+                        default=False,
+                        required=False,
+                        help='If set, apply a z weighting scheme analog to that used for QMLE (eg. 2008.06421). '
+                             'Each chunk with mean redshift z contributes two nearest bins z_i (resp. z_j=z_i+dz), '
+                             'with weights |z-z_j|/dz (resp. |z-z_i|/dz).')
 
     parser.add_argument('--output-snrfit',
                         type=str,
                         default=None,
                         help='Name of the ASCII file where SNR fit results are stored,'
                         'if weight-method is fit_snr')
 
@@ -158,15 +166,34 @@
 
     parser.add_argument('--ncpu',
                         type=int,
                         default=8,
                         required=False,
                         help='Number of CPUs used to read input P1D files')
 
-    args = parser.parse_args(sys.argv[1:])
+    parser.add_argument('--covariance',
+                        action='store_true',
+                        default=False,
+                        required=False,
+                        help='Compute covariance matrix, cpu-intensive calculation')
+
+    parser.add_argument('--bootstrap',
+                        action='store_true',
+                        default=False,
+                        required=False,
+                        help='Compute covariance matrix with bootstrap method, very cpu-intensive calculation')
+
+    parser.add_argument('--nbootstrap',
+                        type=int,
+                        default=20,
+                        required=False,
+                        help='Number of bootstrap iteration used')
+
+
+    args = parser.parse_args(cmdargs)
 
     if (args.weight_method != 'no_weights') and (args.snr_cut_scheme is not None):
         raise ValueError("""You are using a weighting method with a
                             redshift-dependent SNR quality cut, this is not
                             tested and should bias the result""")
 
     if args.snr_cut_scheme == 'eboss':
@@ -202,19 +229,23 @@
     else:
         output_file = args.output_file
 
     postproc_pk1d.run_postproc_pk1d(args.in_dir, output_file,
                                     z_edges,
                                     k_edges,
                                     weight_method=args.weight_method,
+                                    apply_z_weights=args.apply_z_weights,
                                     output_snrfit=args.output_snrfit,
                                     snrcut=snrcut,
                                     zbins_snrcut=zbins_snrcut,
                                     nomedians=args.no_median,
                                     velunits=args.velunits,
                                     overwrite=args.overwrite,
-                                    ncpu = args.ncpu)
+                                    ncpu = args.ncpu,
+                                    compute_covariance=args.covariance,
+                                    compute_bootstrap=args.bootstrap,
+                                    number_bootstrap=args.nbootstrap)
 
 
 if __name__ == '__main__':
     cmdargs = sys.argv[1:]
     main(cmdargs)
```

### Comparing `picca-6.1.0/bin/picca_cf.py` & `picca-7.0.0/bin/picca_cf.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,28 @@
                         type=float,
                         default=10.,
                         required=False,
                         help=('Use only pairs of forest x object with the mean '
                               'of the last absorber redshift and the object '
                               'redshift smaller than z-cut-max'))
 
+    parser.add_argument('--z-min-sources',
+                        type=float,
+                        default=0.,
+                        required=False,
+                        help=('Limit the minimum redshift of the quasars '
+                              'used as sources for spectra'))
+
+    parser.add_argument('--z-max-sources',
+                        type=float,
+                        default=10.,
+                        required=False,
+                        help=('Limit the maximum redshift of the quasars '
+                              'used as sources for spectra'))
+
     parser.add_argument('--lambda-abs',
                         type=str,
                         default='LYA',
                         required=False,
                         help=('Name of the absorption in picca.constants '
                               'defining the redshift of the delta'))
 
@@ -245,24 +259,27 @@
                             Ok=args.fid_Ok,
                             wl=args.fid_wl,
                             blinding=blinding)
 
     t0 = time.time()
 
     ### Read data 1
+    print('z_min_sources', args.z_min_sources)
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cosmo,
                                                   max_num_spec=args.nspec,
                                                   no_project=args.no_project,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources,)
     del z_max
     cf.data = data
     cf.num_data = num_data
     cf.ang_max = utils.compute_ang_max(cosmo, cf.r_trans_max, z_min)
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
@@ -284,15 +301,17 @@
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cosmo,
             max_num_spec=args.nspec,
             no_project=args.no_project,
             nproc=args.nproc,
-            rebin_factor=args.rebin_factor)
+            rebin_factor=args.rebin_factor,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources,)
         del z_max2
         cf.data2 = data2
         cf.num_data2 = num_data2
         cf.ang_max = utils.compute_ang_max(cosmo, cf.r_trans_max, z_min, z_min2)
         userprint("")
         userprint("done, npix = {}".format(len(data2)))
```

### Comparing `picca-6.1.0/bin/picca_cf1d.py` & `picca-7.0.0/bin/picca_cf1d.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,28 @@
 
     parser.add_argument('--lambda-max',
                         type=float,
                         default=5500.,
                         required=False,
                         help='Upper limit on observed wavelength [Angstrom]')
 
+    parser.add_argument('--z-min-sources',
+                        type=float,
+                        default=0.,
+                        required=False,
+                        help=('Limit the minimum redshift of the quasars '
+                              'used as sources for spectra'))
+
+    parser.add_argument('--z-max-sources',
+                        type=float,
+                        default=10.,
+                        required=False,
+                        help=('Limit the maximum redshift of the quasars '
+                              'used as sources for spectra'))
+
     parser.add_argument('--dll',
                         type=float,
                         default=3.e-4,
                         required=False,
                         help='Loglam bin size')
 
     parser.add_argument(
@@ -160,15 +174,17 @@
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   args.z_evol,
                                                   args.z_ref,
                                                   cosmo=None,
                                                   max_num_spec=args.nspec,
-                                                  no_project=args.no_project)
+                                                  no_project=args.no_project,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     cf.data = data
     cf.num_data = num_data
     del z_min, z_max
     userprint("")
     userprint("done, npix = {}\n".format(len(data)))
 
     ### Read data 2
@@ -178,15 +194,17 @@
             args.in_dir2,
             cf.nside,
             cf.lambda_abs2,
             args.z_evol2,
             args.z_ref,
             cosmo=None,
             max_num_spec=args.nspec,
-            no_project=args.no_project)
+            no_project=args.no_project,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         cf.data2 = data2
         cf.num_data2 = num_data2
         del z_min2, z_max2
         userprint("")
         userprint("done, npix = {}\n".format(len(data2)))
     elif cf.lambda_abs != cf.lambda_abs2:
         cf.x_correlation = True
```

### Comparing `picca-6.1.0/bin/picca_cf_angl.py` & `picca-7.0.0/bin/picca_cf_angl.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -198,15 +214,17 @@
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cosmo=None,
                                                   max_num_spec=args.nspec,
-                                                  no_project=args.no_project)
+                                                  no_project=args.no_project,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     cf.data = data
     cf.num_data = num_data
     del z_min, z_max
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
     ### Read data 2
@@ -224,15 +242,17 @@
             args.in_dir2,
             cf.nside,
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cosmo=None,
             max_num_spec=args.nspec,
-            no_project=args.no_project)
+            no_project=args.no_project,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         cf.data2 = data2
         cf.num_data2 = num_data2
         del z_min2, z_max2
         userprint("")
         userprint("done, npix = {}".format(len(data2)))
 
     # compute correlation function, use pool to parallelize
```

### Comparing `picca-6.1.0/bin/picca_co.py` & `picca-7.0.0/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_coadd_zint.py` & `picca-7.0.0/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_compute_fvoigt.py` & `picca-7.0.0/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_compute_pk_pksb.py` & `picca-7.0.0/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_convert_transmission.py` & `picca-7.0.0/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_delta_extraction.py` & `picca-7.0.0/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_dmat.py` & `picca-7.0.0/bin/picca_dmat.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,14 +115,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -276,15 +292,17 @@
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cosmo,
                                                   max_num_spec=args.nspec,
                                                   no_project=args.no_project,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     del z_max
     cf.data = data
     cf.num_data = num_data
     cf.ang_max = utils.compute_ang_max(cosmo, cf.r_trans_max, z_min)
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
@@ -306,15 +324,17 @@
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cosmo,
             max_num_spec=args.nspec,
             no_project=args.no_project,
             nproc=args.nproc,
-            rebin_factor=args.rebin_factor)
+            rebin_factor=args.rebin_factor,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         del z_max2
         cf.data2 = data2
         cf.num_data2 = num_data2
         cf.ang_max = utils.compute_ang_max(cosmo, cf.r_trans_max, z_min, z_min2)
         userprint("")
         userprint("done, npix = {}".format(len(data2)))
 
@@ -334,30 +354,29 @@
     if args.nproc > 1:
         context = multiprocessing.get_context('fork')
         pool = context.Pool(processes=args.nproc)
         dmat_data = pool.map(calc_dmat, sorted(cpu_data.values()))
         pool.close()
     elif args.nproc == 1:
         dmat_data = map(calc_dmat, sorted(cpu_data.values()))
-        dmat_data = list(dmat_data)
 
     t2 = time.time()
     userprint(f'picca_dmat.py - Time computing distortion matrix: {(t2-t1)/60:.3f} minutes')
 
 
     # merge the results from different CPUs
-    dmat_data = np.array(dmat_data)
-    weights_dmat = dmat_data[:, 0].sum(axis=0)
-    dmat = dmat_data[:, 1].sum(axis=0)
-    r_par = dmat_data[:, 2].sum(axis=0)
-    r_trans = dmat_data[:, 3].sum(axis=0)
-    z = dmat_data[:, 4].sum(axis=0)
-    weights = dmat_data[:, 5].sum(axis=0)
-    num_pairs = dmat_data[:, 6].sum(axis=0)
-    num_pairs_used = dmat_data[:, 7].sum(axis=0)
+    dmat_data = list(dmat_data)
+    weights_dmat = np.array([item[0] for item in dmat_data]).sum(axis=0)
+    dmat = np.array([item[1] for item in dmat_data]).sum(axis=0)
+    r_par = np.array([item[2] for item in dmat_data]).sum(axis=0)
+    r_trans = np.array([item[3] for item in dmat_data]).sum(axis=0)
+    z = np.array([item[4] for item in dmat_data]).sum(axis=0)
+    weights = np.array([item[5] for item in dmat_data]).sum(axis=0)
+    num_pairs = np.array([item[6] for item in dmat_data]).sum(axis=0)
+    num_pairs_used = np.array([item[7] for item in dmat_data]).sum(axis=0)
 
     # normalize values
     w = weights > 0.
     r_par[w] /= weights[w]
     r_trans[w] /= weights[w]
     z[w] /= weights[w]
     w = weights_dmat > 0
```

### Comparing `picca-6.1.0/bin/picca_export.py` & `picca-7.0.0/bin/picca_export.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_export_co.py` & `picca-7.0.0/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_export_cross_covariance.py` & `picca-7.0.0/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_metal_dmat.py` & `picca-7.0.0/bin/picca_metal_dmat.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -309,15 +325,17 @@
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cf.cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     del z_max
     cf.data = data
     cf.num_data = num_data
     cf.ang_max = utils.compute_ang_max(cf.cosmo, cf.r_trans_max, z_min)
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
@@ -341,15 +359,17 @@
             cf.nside,
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cf.cosmo,
             max_num_spec=args.nspec,
             nproc=args.nproc,
-            rebin_factor=args.rebin_factor)
+            rebin_factor=args.rebin_factor,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         del z_max2
         cf.data2 = data2
         cf.num_data2 = num_data2
         cf.ang_max = utils.compute_ang_max(cf.cosmo, cf.r_trans_max, z_min,
                                            z_min2)
         userprint("")
         userprint("done, npix = {}".format(len(data2)))
@@ -407,26 +427,25 @@
                 pool = context.Pool(processes=args.nproc)
                 dmat_data = pool.map(calc_metal_dmat_wrapper,
                                      sorted(cpu_data.values()))
                 pool.close()
             elif args.nproc == 1:
                 dmat_data = map(calc_metal_dmat_wrapper,
                                 sorted(cpu_data.values()))
-                dmat_data = list(dmat_data)
 
             # merge the results from different CPUs
-            dmat_data = np.array(dmat_data)
-            weights_dmat = dmat_data[:, 0].sum(axis=0)
-            dmat = dmat_data[:, 1].sum(axis=0)
-            r_par = dmat_data[:, 2].sum(axis=0)
-            r_trans = dmat_data[:, 3].sum(axis=0)
-            z = dmat_data[:, 4].sum(axis=0)
-            weights = dmat_data[:, 5].sum(axis=0)
-            num_pairs = dmat_data[:, 6].sum(axis=0)
-            num_pairs_used = dmat_data[:, 7].sum(axis=0)
+            dmat_data = list(dmat_data)
+            weights_dmat = np.array([item[0] for item in dmat_data]).sum(axis=0)
+            dmat = np.array([item[1] for item in dmat_data]).sum(axis=0)
+            r_par = np.array([item[2] for item in dmat_data]).sum(axis=0)
+            r_trans = np.array([item[3] for item in dmat_data]).sum(axis=0)
+            z = np.array([item[4] for item in dmat_data]).sum(axis=0)
+            weights = np.array([item[5] for item in dmat_data]).sum(axis=0)
+            num_pairs = np.array([item[6] for item in dmat_data]).sum(axis=0)
+            num_pairs_used = np.array([item[7] for item in dmat_data]).sum(axis=0)
 
             # normalize_values
             w = weights > 0
             r_par[w] /= weights[w]
             r_trans[w] /= weights[w]
             z[w] /= weights[w]
             w = weights_dmat > 0
```

### Comparing `picca-6.1.0/bin/picca_metal_xdmat.py` & `picca-7.0.0/bin/picca_metal_xdmat.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -177,15 +193,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--metal-alpha',
         type=float,
         default=1.,
@@ -296,15 +312,17 @@
                                                   args.nside,
                                                   xcf.lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
 
     xcf.data = data
     xcf.num_data = num_data
 
     ### Find the redshift range
     if args.z_min_obj is None:
         r_comov_min = cosmo.get_r_comov(z_min)
@@ -358,32 +376,31 @@
             context = multiprocessing.get_context('fork')
             pool = context.Pool(processes=args.nproc)
             dmat_data = pool.map(calc_metal_dmat_wrapper,
                                  sorted(cpu_data.values()))
             pool.close()
         elif args.nproc == 1:
             dmat_data = map(calc_metal_dmat_wrapper, sorted(cpu_data.values()))
-            dmat_data = list(dmat_data)
 
         # merge the results from different CPUs
-        dmat_data = np.array(dmat_data)
-        weights_dmat = dmat_data[:, 0].sum(axis=0)
-        dmat = dmat_data[:, 1].sum(axis=0)
-        r_par = dmat_data[:, 2].sum(axis=0)
-        r_trans = dmat_data[:, 3].sum(axis=0)
-        z = dmat_data[:, 4].sum(axis=0)
-        weights = dmat_data[:, 5].sum(axis=0)
+        dmat_data = list(dmat_data)
+        weights_dmat = np.array([item[0] for item in dmat_data]).sum(axis=0)
+        dmat = np.array([item[1] for item in dmat_data]).sum(axis=0)
+        r_par = np.array([item[2] for item in dmat_data]).sum(axis=0)
+        r_trans = np.array([item[3] for item in dmat_data]).sum(axis=0)
+        z = np.array([item[4] for item in dmat_data]).sum(axis=0)
+        weights = np.array([item[5] for item in dmat_data]).sum(axis=0)
 
         # normalize_values
         w = weights > 0
         r_par[w] /= weights[w]
         r_trans[w] /= weights[w]
         z[w] /= weights[w]
-        num_pairs = dmat_data[:, 6].sum(axis=0)
-        num_pairs_used = dmat_data[:, 7].sum(axis=0)
+        num_pairs = np.array([item[6] for item in dmat_data]).sum(axis=0)
+        num_pairs_used = np.array([item[7] for item in dmat_data]).sum(axis=0)
         w = weights_dmat > 0
         dmat[w, :] /= weights_dmat[w, None]
 
         # add these results to the list ofor the different metal absorption
         dmat_all.append(dmat)
         weights_dmat_all.append(weights_dmat)
         r_par_all.append(r_par)
```

### Comparing `picca-6.1.0/bin/picca_nersc_submit.py` & `picca-7.0.0/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_pk2fits.py` & `picca-7.0.0/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_plot_pk1d.py` & `picca-7.0.0/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_reduce_spall.py` & `picca-7.0.0/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/bin/picca_wick.py` & `picca-7.0.0/bin/picca_wick.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -303,15 +319,17 @@
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     for deltas in data.values():
         for delta in deltas:
             delta.fname = 'D1'
             for item in [
                     'cont', 'delta', 'order', 'ivar', 'exposures_diff',
                     'mean_snr', 'mean_reso', 'mean_z', 'delta_log_lambda'
             ]:
@@ -395,15 +413,17 @@
             cf.nside,
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cosmo,
             max_num_spec=args.nspec,
             nproc=args.nproc,
-            rebin_factor=args.rebin_factor)
+            rebin_factor=args.rebin_factor,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         for deltas in data.values():
             for delta in deltas:
                 delta.fname = 'D2'
                 for item in [
                         'cont', 'delta', 'order', 'ivar', 'exposures_diff',
                         'mean_snr', 'mean_reso', 'mean_z', 'delta_log_lambda'
                 ]:
@@ -433,25 +453,25 @@
         wick_data = pool.map(calc_wick_terms, sorted(cpu_data.values()))
     else:
         wick_data = [calc_wick_terms(arg) for arg in sorted(cpu_data.values())]
     userprint(" \nFinished\n")
     pool.close()
 
     # merge the results from the different CPUs
-    wick_data = np.array(wick_data)
-    weights_wick = wick_data[:, 0].sum(axis=0)
-    num_pairs_wick = wick_data[:, 1].sum(axis=0)
-    num_pairs = wick_data[:, 2].sum(axis=0)
-    num_pairs_used = wick_data[:, 3].sum(axis=0)
-    t1 = wick_data[:, 4].sum(axis=0)
-    t2 = wick_data[:, 5].sum(axis=0)
-    t3 = wick_data[:, 6].sum(axis=0)
-    t4 = wick_data[:, 7].sum(axis=0)
-    t5 = wick_data[:, 8].sum(axis=0)
-    t6 = wick_data[:, 9].sum(axis=0)
+    wick_data = list(wick_data)
+    weights_wick = np.array([item[0] for item in wick_data]).sum(axis=0)
+    num_pairs_wick = np.array([item[1] for item in wick_data]).sum(axis=0)
+    num_pairs = np.array([item[2] for item in wick_data]).sum(axis=0)
+    num_pairs_used = np.array([item[3] for item in wick_data]).sum(axis=0)
+    t1 = np.array([item[4] for item in wick_data]).sum(axis=0)
+    t2 = np.array([item[5] for item in wick_data]).sum(axis=0)
+    t3 = np.array([item[6] for item in wick_data]).sum(axis=0)
+    t4 = np.array([item[7] for item in wick_data]).sum(axis=0)
+    t5 = np.array([item[8] for item in wick_data]).sum(axis=0)
+    t6 = np.array([item[9] for item in wick_data]).sum(axis=0)
     weights = weights_wick * weights_wick[:, None]
     w = weights > 0.
     t1[w] /= weights[w]
     t2[w] /= weights[w]
     t3[w] /= weights[w]
     t4[w] /= weights[w]
     t5[w] /= weights[w]
```

### Comparing `picca-6.1.0/bin/picca_xcf.py` & `picca-7.0.0/bin/picca_xcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,29 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Min redshift of the background quasars'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -151,15 +166,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--fid-Om',
         type=float,
         default=0.315,
@@ -289,15 +304,17 @@
                                                   xcf.lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo=cosmo,
                                                   max_num_spec=args.nspec,
                                                   no_project=args.no_project,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     xcf.data = data
     xcf.num_data = num_data
     userprint("")
     userprint("done, npix = {}\n".format(len(data)))
     ### Remove <delta> vs. lambda_obs
     if not args.no_remove_mean_lambda_obs:
         Forest.delta_log_lambda = None
```

### Comparing `picca-6.1.0/bin/picca_xcf1d.py` & `picca-7.0.0/bin/picca_xcf1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -138,15 +154,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument('--no-project',
                         action='store_true',
                         required=False,
                         help='Do not project out continuum fitting modes')
@@ -195,15 +211,17 @@
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
                                                   args.nside,
                                                   lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo=None,
                                                   max_num_spec=args.nspec,
-                                                  no_project=args.no_project)
+                                                  no_project=args.no_project,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     xcf.data = data
     xcf.num_data = num_data
     sys.stderr.write("\n")
     userprint("done, npix = {}".format(len(data)))
 
     ### Remove <delta> vs. lambda_obs
     if not args.no_remove_mean_lambda_obs:
```

### Comparing `picca-6.1.0/bin/picca_xcf_angl.py` & `picca-7.0.0/bin/picca_xcf_angl.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -156,15 +172,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--fid-Om',
         type=float,
         default=0.315,
@@ -251,15 +267,17 @@
         args.in_dir,
         args.nside,
         constants.ABSORBER_IGM[args.lambda_abs],
         args.z_evol_del,
         args.z_ref,
         cosmo=cosmo,
         max_num_spec=args.nspec,
-        no_project=args.no_project)
+        no_project=args.no_project,
+        z_min_qso=args.z_min_sources,
+        z_max_qso=args.z_max_sources)
     xcf.data = data
     xcf.num_data = num_data
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
     ### Remove <delta> vs. lambda_obs
     if not args.no_remove_mean_lambda_obs:
```

### Comparing `picca-6.1.0/bin/picca_xdmat.py` & `picca-7.0.0/bin/picca_xdmat.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -159,15 +175,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--fid-Om',
         type=float,
         default=0.315,
@@ -265,15 +281,17 @@
                                                   args.nside,
                                                   xcf.lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo=cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     xcf.data = data
     xcf.num_data = num_data
     userprint("\n")
     userprint("done, npix = {}\n".format(len(data)))
 
     ### Find the redshift range
     if args.z_min_obj is None:
@@ -319,23 +337,23 @@
         dmat_data = map(calc_dmat, sorted(cpu_data.values()))
         dmat_data = list(dmat_data)
 
     t2 = time.time()
     userprint(f'picca_xdmat.py - Time computing distortion matrix: {(t2-t1)/60:.3f} minutes')
 
     # merge the results from different CPUs
-    dmat_data = np.array(dmat_data)
-    weights_dmat = dmat_data[:, 0].sum(axis=0)
-    dmat = dmat_data[:, 1].sum(axis=0)
-    r_par = dmat_data[:, 2].sum(axis=0)
-    r_trans = dmat_data[:, 3].sum(axis=0)
-    z = dmat_data[:, 4].sum(axis=0)
-    weights = dmat_data[:, 5].sum(axis=0)
-    num_pairs = dmat_data[:, 6].sum(axis=0)
-    num_pairs_used = dmat_data[:, 7].sum(axis=0)
+    dmat_data = list(dmat_data)
+    weights_dmat = np.array([item[0] for item in dmat_data]).sum(axis=0)
+    dmat = np.array([item[1] for item in dmat_data]).sum(axis=0)
+    r_par = np.array([item[2] for item in dmat_data]).sum(axis=0)
+    r_trans = np.array([item[3] for item in dmat_data]).sum(axis=0)
+    z = np.array([item[4] for item in dmat_data]).sum(axis=0)
+    weights = np.array([item[5] for item in dmat_data]).sum(axis=0)
+    num_pairs = np.array([item[6] for item in dmat_data]).sum(axis=0)
+    num_pairs_used = np.array([item[7] for item in dmat_data]).sum(axis=0)
 
     # normalize values
     w = weights > 0.
     r_par[w] /= weights[w]
     r_trans[w] /= weights[w]
     z[w] /= weights[w]
     w = weights_dmat > 0.
```

### Comparing `picca-6.1.0/bin/picca_xwick.py` & `picca-7.0.0/bin/picca_xwick.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,14 +126,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -149,15 +165,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--fid-Om',
         type=float,
         default=0.315,
@@ -232,15 +248,15 @@
                         help='Maximum number of spectra to read')
 
     parser.add_argument('--rebin-factor',
                         type=int,
                         default=None,
                         required=False,
                         help='Rebin factor for deltas. If not None, deltas will '
-                             'be rebinned by that factor')    
+                             'be rebinned by that factor')
 
     args = parser.parse_args(cmdargs)
     if args.nproc is None:
         args.nproc = cpu_count() // 2
 
     # setup variables in module xcf
     xcf.r_par_min = args.rp_min
@@ -277,15 +293,17 @@
                                                   args.nside,
                                                   xcf.lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo=cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     for deltas in data.values():
         for delta in deltas:
             delta.fname = 'D1'
             for item in [
                     'cont', 'delta', 'order', 'ivar', 'exposures_diff',
                     'mean_snr', 'mean_reso', 'mean_z', 'delta_log_lambda'
             ]:
@@ -386,25 +404,25 @@
     context = multiprocessing.get_context('fork')
     pool = context.Pool(processes=min(args.nproc, len(cpu_data.values())))
     userprint(" \nStarting\n")
     wick_data = pool.map(calc_wick_terms, sorted(cpu_data.values()))
     userprint(" \nFinished\n")
     pool.close()
 
-    wick_data = np.array(wick_data)
-    weights_wick = wick_data[:, 0].sum(axis=0)
-    num_pairs_wick = wick_data[:, 1].sum(axis=0)
-    npairs = wick_data[:, 2].sum(axis=0)
-    npairs_used = wick_data[:, 3].sum(axis=0)
-    t1 = wick_data[:, 4].sum(axis=0)
-    t2 = wick_data[:, 5].sum(axis=0)
-    t3 = wick_data[:, 6].sum(axis=0)
-    t4 = wick_data[:, 7].sum(axis=0)
-    t5 = wick_data[:, 8].sum(axis=0)
-    t6 = wick_data[:, 9].sum(axis=0)
+    wick_data = list(wick_data)
+    weights_wick = np.array([item[0] for item in wick_data]).sum(axis=0)
+    num_pairs_wick = np.array([item[1] for item in wick_data]).sum(axis=0)
+    npairs = np.array([item[2] for item in wick_data]).sum(axis=0)
+    npairs_used = np.array([item[3] for item in wick_data]).sum(axis=0)
+    t1 = np.array([item[4] for item in wick_data]).sum(axis=0)
+    t2 = np.array([item[5] for item in wick_data]).sum(axis=0)
+    t3 = np.array([item[6] for item in wick_data]).sum(axis=0)
+    t4 = np.array([item[7] for item in wick_data]).sum(axis=0)
+    t5 = np.array([item[8] for item in wick_data]).sum(axis=0)
+    t6 = np.array([item[9] for item in wick_data]).sum(axis=0)
     weights = weights_wick * weights_wick[:, None]
     w = weights > 0.
     t1[w] /= weights[w]
     t2[w] /= weights[w]
     t3[w] /= weights[w]
     t4[w] /= weights[w]
     t5[w] /= weights[w]
```

### Comparing `picca-6.1.0/py/picca/bal_tools.py` & `picca-7.0.0/py/picca/bal_tools.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/old/picca_deltas.py` & `picca-7.0.0/py/picca/bin/old/picca_deltas.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/old/picca_fitter2.py` & `picca-7.0.0/py/picca/bin/old/picca_fitter2.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/old/picca_fitter2_control.py` & `picca-7.0.0/py/picca/bin/old/picca_fitter2_control.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/old/picca_fitter2_control_mpi.py` & `picca-7.0.0/py/picca/bin/old/picca_fitter2_control_mpi.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_Pk1D.py` & `picca-7.0.0/py/picca/bin/picca_Pk1D.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
                 delta.mean_reso=1e-3
                 delta.mean_reso_pix=1e-3
                 delta.exposures_diff = np.zeros(delta.delta.shape)
             running_on_raw_transmission = True
     elif args.in_format == 'ascii':
         ascii_file = open(file, 'r')
         deltas = [Delta.from_ascii(line) for line in ascii_file]
+        running_on_raw_transmission = False
 
     #add the check for linear binning on first spectrum only (assuming homogeneity within the file)
     delta = deltas[0]
     linear_binning, pixel_step = check_linear_binning(delta)
     if linear_binning:
         userprint("\n\nUsing linear binning, results will have units of AA")
         if (args.disable_reso_matrix or not hasattr(delta, 'resolution_matrix')
@@ -237,15 +238,16 @@
                 #in this case all is in AA space
                 if reso_correction == 'matrix':
                     correction_reso = compute_correction_reso_matrix(
                         reso_matrix=np.mean(reso_matrix_array[part_index],
                                             axis=1),
                         k=k,
                         delta_pixel=pixel_step,
-                        num_pixel=len(lambda_new))
+                        num_pixel=len(lambda_new),
+                        pixelization_correction = args.add_pixelization_correction)
                 elif reso_correction == 'Gaussian':
                     #this is roughly converting the mean resolution estimate back to pixels
                     #and then multiplying with pixel size
                     mean_reso_AA = pixel_step * delta.mean_reso_pix
                     correction_reso = compute_correction_reso(
                         delta_pixel=pixel_step, mean_reso=mean_reso_AA, k=k)
             elif not running_on_raw_transmission:
@@ -332,14 +334,18 @@
                     'name': 'LIN_BIN',
                     'value': linear_binning,
                     'comment': "analysis was performed on delta with linear binned lambda"
                 }, {
                     'name': 'LOS_ID',
                     'value': delta.los_id,
                     'comment': "line of sight identifier, e.g. THING_ID or TARGETID"
+                }, {
+                    'name': 'CHUNK_ID',
+                    'value': part_index,
+                    'comment': "Chunk (sub-forest) identifier"
                 },
                 ]
 
                 cols = [k, pk_raw, pk_noise, pk_diff, correction_reso, pk]
                 names = [
                     'K', 'PK_RAW', 'PK_NOISE', 'PK_DIFF', 'COR_RESO', 'PK'
                 ]
@@ -499,14 +505,23 @@
     parser.add_argument('--disable-reso-matrix',
                         default=False,
                         action='store_true',
                         required=False,
                         help=('do not use the resolution matrix even '
                               'if it exists and we are on linear binning'))
 
+    parser.add_argument('--add-pixelization-correction',
+                        default=False,
+                        action='store_true',
+                        required=False,
+                        help=('Add a pixelization correction, as if the resolution  '
+                              'matrix was doubly pixelized. Only use this option in '
+                              'quickquasars mocks'))
+
+
     parser.add_argument(
         '--force-output-in-velocity',
         default=False,
         action='store_true',
         required=False,
         help=
         ('store outputs in units of velocity even for linear binning computations'
```

### Comparing `picca-6.1.0/py/picca/bin/picca_Pk1D_postprocess.py` & `picca-7.0.0/py/picca/bin/picca_Pk1D_postprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,16 +113,24 @@
                         required=False,
                         help='Size of a spectrum pixel in Angstrom, used to'
                              'define the binning of the output wavenumber array')
 
     parser.add_argument('--weight-method',
                         type=str,
                         default='no_weights',
-                        help='Weighting scheme for the mean P1D computation,'
-                             'Possible options: no_weights, simple_snr, fit_snr')
+                        help='SNR weighting scheme for the mean P1D computation,'
+                             'Possible options: no_weights, fit_snr')
+
+    parser.add_argument('--apply_z_weights',
+                        action='store_true',
+                        default=False,
+                        required=False,
+                        help='If set, apply a z weighting scheme analog to that used for QMLE (eg. 2008.06421). '
+                             'Each chunk with mean redshift z contributes two nearest bins z_i (resp. z_j=z_i+dz), '
+                             'with weights |z-z_j|/dz (resp. |z-z_i|/dz).')
 
     parser.add_argument('--output-snrfit',
                         type=str,
                         default=None,
                         help='Name of the ASCII file where SNR fit results are stored,'
                         'if weight-method is fit_snr')
 
@@ -158,15 +166,34 @@
 
     parser.add_argument('--ncpu',
                         type=int,
                         default=8,
                         required=False,
                         help='Number of CPUs used to read input P1D files')
 
-    args = parser.parse_args(sys.argv[1:])
+    parser.add_argument('--covariance',
+                        action='store_true',
+                        default=False,
+                        required=False,
+                        help='Compute covariance matrix, cpu-intensive calculation')
+
+    parser.add_argument('--bootstrap',
+                        action='store_true',
+                        default=False,
+                        required=False,
+                        help='Compute covariance matrix with bootstrap method, very cpu-intensive calculation')
+
+    parser.add_argument('--nbootstrap',
+                        type=int,
+                        default=20,
+                        required=False,
+                        help='Number of bootstrap iteration used')
+
+
+    args = parser.parse_args(cmdargs)
 
     if (args.weight_method != 'no_weights') and (args.snr_cut_scheme is not None):
         raise ValueError("""You are using a weighting method with a
                             redshift-dependent SNR quality cut, this is not
                             tested and should bias the result""")
 
     if args.snr_cut_scheme == 'eboss':
@@ -202,19 +229,23 @@
     else:
         output_file = args.output_file
 
     postproc_pk1d.run_postproc_pk1d(args.in_dir, output_file,
                                     z_edges,
                                     k_edges,
                                     weight_method=args.weight_method,
+                                    apply_z_weights=args.apply_z_weights,
                                     output_snrfit=args.output_snrfit,
                                     snrcut=snrcut,
                                     zbins_snrcut=zbins_snrcut,
                                     nomedians=args.no_median,
                                     velunits=args.velunits,
                                     overwrite=args.overwrite,
-                                    ncpu = args.ncpu)
+                                    ncpu = args.ncpu,
+                                    compute_covariance=args.covariance,
+                                    compute_bootstrap=args.bootstrap,
+                                    number_bootstrap=args.nbootstrap)
 
 
 if __name__ == '__main__':
     cmdargs = sys.argv[1:]
     main(cmdargs)
```

### Comparing `picca-6.1.0/py/picca/bin/picca_cf.py` & `picca-7.0.0/py/picca/bin/picca_cf.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,28 @@
                         type=float,
                         default=10.,
                         required=False,
                         help=('Use only pairs of forest x object with the mean '
                               'of the last absorber redshift and the object '
                               'redshift smaller than z-cut-max'))
 
+    parser.add_argument('--z-min-sources',
+                        type=float,
+                        default=0.,
+                        required=False,
+                        help=('Limit the minimum redshift of the quasars '
+                              'used as sources for spectra'))
+
+    parser.add_argument('--z-max-sources',
+                        type=float,
+                        default=10.,
+                        required=False,
+                        help=('Limit the maximum redshift of the quasars '
+                              'used as sources for spectra'))
+
     parser.add_argument('--lambda-abs',
                         type=str,
                         default='LYA',
                         required=False,
                         help=('Name of the absorption in picca.constants '
                               'defining the redshift of the delta'))
 
@@ -245,24 +259,27 @@
                             Ok=args.fid_Ok,
                             wl=args.fid_wl,
                             blinding=blinding)
 
     t0 = time.time()
 
     ### Read data 1
+    print('z_min_sources', args.z_min_sources)
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cosmo,
                                                   max_num_spec=args.nspec,
                                                   no_project=args.no_project,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources,)
     del z_max
     cf.data = data
     cf.num_data = num_data
     cf.ang_max = utils.compute_ang_max(cosmo, cf.r_trans_max, z_min)
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
@@ -284,15 +301,17 @@
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cosmo,
             max_num_spec=args.nspec,
             no_project=args.no_project,
             nproc=args.nproc,
-            rebin_factor=args.rebin_factor)
+            rebin_factor=args.rebin_factor,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources,)
         del z_max2
         cf.data2 = data2
         cf.num_data2 = num_data2
         cf.ang_max = utils.compute_ang_max(cosmo, cf.r_trans_max, z_min, z_min2)
         userprint("")
         userprint("done, npix = {}".format(len(data2)))
```

### Comparing `picca-6.1.0/py/picca/bin/picca_cf1d.py` & `picca-7.0.0/py/picca/bin/picca_cf1d.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,28 @@
 
     parser.add_argument('--lambda-max',
                         type=float,
                         default=5500.,
                         required=False,
                         help='Upper limit on observed wavelength [Angstrom]')
 
+    parser.add_argument('--z-min-sources',
+                        type=float,
+                        default=0.,
+                        required=False,
+                        help=('Limit the minimum redshift of the quasars '
+                              'used as sources for spectra'))
+
+    parser.add_argument('--z-max-sources',
+                        type=float,
+                        default=10.,
+                        required=False,
+                        help=('Limit the maximum redshift of the quasars '
+                              'used as sources for spectra'))
+
     parser.add_argument('--dll',
                         type=float,
                         default=3.e-4,
                         required=False,
                         help='Loglam bin size')
 
     parser.add_argument(
@@ -160,15 +174,17 @@
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   args.z_evol,
                                                   args.z_ref,
                                                   cosmo=None,
                                                   max_num_spec=args.nspec,
-                                                  no_project=args.no_project)
+                                                  no_project=args.no_project,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     cf.data = data
     cf.num_data = num_data
     del z_min, z_max
     userprint("")
     userprint("done, npix = {}\n".format(len(data)))
 
     ### Read data 2
@@ -178,15 +194,17 @@
             args.in_dir2,
             cf.nside,
             cf.lambda_abs2,
             args.z_evol2,
             args.z_ref,
             cosmo=None,
             max_num_spec=args.nspec,
-            no_project=args.no_project)
+            no_project=args.no_project,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         cf.data2 = data2
         cf.num_data2 = num_data2
         del z_min2, z_max2
         userprint("")
         userprint("done, npix = {}\n".format(len(data2)))
     elif cf.lambda_abs != cf.lambda_abs2:
         cf.x_correlation = True
```

### Comparing `picca-6.1.0/py/picca/bin/picca_cf_angl.py` & `picca-7.0.0/py/picca/bin/picca_cf_angl.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -198,15 +214,17 @@
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cosmo=None,
                                                   max_num_spec=args.nspec,
-                                                  no_project=args.no_project)
+                                                  no_project=args.no_project,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     cf.data = data
     cf.num_data = num_data
     del z_min, z_max
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
     ### Read data 2
@@ -224,15 +242,17 @@
             args.in_dir2,
             cf.nside,
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cosmo=None,
             max_num_spec=args.nspec,
-            no_project=args.no_project)
+            no_project=args.no_project,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         cf.data2 = data2
         cf.num_data2 = num_data2
         del z_min2, z_max2
         userprint("")
         userprint("done, npix = {}".format(len(data2)))
 
     # compute correlation function, use pool to parallelize
```

### Comparing `picca-6.1.0/py/picca/bin/picca_co.py` & `picca-7.0.0/py/picca/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_coadd_zint.py` & `picca-7.0.0/py/picca/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_compute_fvoigt.py` & `picca-7.0.0/py/picca/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_compute_pk_pksb.py` & `picca-7.0.0/py/picca/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_convert_transmission.py` & `picca-7.0.0/py/picca/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_delta_extraction.py` & `picca-7.0.0/py/picca/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_dmat.py` & `picca-7.0.0/py/picca/bin/picca_dmat.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,14 +115,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -276,15 +292,17 @@
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cosmo,
                                                   max_num_spec=args.nspec,
                                                   no_project=args.no_project,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     del z_max
     cf.data = data
     cf.num_data = num_data
     cf.ang_max = utils.compute_ang_max(cosmo, cf.r_trans_max, z_min)
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
@@ -306,15 +324,17 @@
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cosmo,
             max_num_spec=args.nspec,
             no_project=args.no_project,
             nproc=args.nproc,
-            rebin_factor=args.rebin_factor)
+            rebin_factor=args.rebin_factor,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         del z_max2
         cf.data2 = data2
         cf.num_data2 = num_data2
         cf.ang_max = utils.compute_ang_max(cosmo, cf.r_trans_max, z_min, z_min2)
         userprint("")
         userprint("done, npix = {}".format(len(data2)))
 
@@ -334,30 +354,29 @@
     if args.nproc > 1:
         context = multiprocessing.get_context('fork')
         pool = context.Pool(processes=args.nproc)
         dmat_data = pool.map(calc_dmat, sorted(cpu_data.values()))
         pool.close()
     elif args.nproc == 1:
         dmat_data = map(calc_dmat, sorted(cpu_data.values()))
-        dmat_data = list(dmat_data)
 
     t2 = time.time()
     userprint(f'picca_dmat.py - Time computing distortion matrix: {(t2-t1)/60:.3f} minutes')
 
 
     # merge the results from different CPUs
-    dmat_data = np.array(dmat_data)
-    weights_dmat = dmat_data[:, 0].sum(axis=0)
-    dmat = dmat_data[:, 1].sum(axis=0)
-    r_par = dmat_data[:, 2].sum(axis=0)
-    r_trans = dmat_data[:, 3].sum(axis=0)
-    z = dmat_data[:, 4].sum(axis=0)
-    weights = dmat_data[:, 5].sum(axis=0)
-    num_pairs = dmat_data[:, 6].sum(axis=0)
-    num_pairs_used = dmat_data[:, 7].sum(axis=0)
+    dmat_data = list(dmat_data)
+    weights_dmat = np.array([item[0] for item in dmat_data]).sum(axis=0)
+    dmat = np.array([item[1] for item in dmat_data]).sum(axis=0)
+    r_par = np.array([item[2] for item in dmat_data]).sum(axis=0)
+    r_trans = np.array([item[3] for item in dmat_data]).sum(axis=0)
+    z = np.array([item[4] for item in dmat_data]).sum(axis=0)
+    weights = np.array([item[5] for item in dmat_data]).sum(axis=0)
+    num_pairs = np.array([item[6] for item in dmat_data]).sum(axis=0)
+    num_pairs_used = np.array([item[7] for item in dmat_data]).sum(axis=0)
 
     # normalize values
     w = weights > 0.
     r_par[w] /= weights[w]
     r_trans[w] /= weights[w]
     z[w] /= weights[w]
     w = weights_dmat > 0
```

### Comparing `picca-6.1.0/py/picca/bin/picca_export.py` & `picca-7.0.0/py/picca/bin/picca_export.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_export_co.py` & `picca-7.0.0/py/picca/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_export_cross_covariance.py` & `picca-7.0.0/py/picca/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_metal_dmat.py` & `picca-7.0.0/py/picca/bin/picca_metal_dmat.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -309,15 +325,17 @@
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cf.cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     del z_max
     cf.data = data
     cf.num_data = num_data
     cf.ang_max = utils.compute_ang_max(cf.cosmo, cf.r_trans_max, z_min)
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
@@ -341,15 +359,17 @@
             cf.nside,
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cf.cosmo,
             max_num_spec=args.nspec,
             nproc=args.nproc,
-            rebin_factor=args.rebin_factor)
+            rebin_factor=args.rebin_factor,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         del z_max2
         cf.data2 = data2
         cf.num_data2 = num_data2
         cf.ang_max = utils.compute_ang_max(cf.cosmo, cf.r_trans_max, z_min,
                                            z_min2)
         userprint("")
         userprint("done, npix = {}".format(len(data2)))
@@ -407,26 +427,25 @@
                 pool = context.Pool(processes=args.nproc)
                 dmat_data = pool.map(calc_metal_dmat_wrapper,
                                      sorted(cpu_data.values()))
                 pool.close()
             elif args.nproc == 1:
                 dmat_data = map(calc_metal_dmat_wrapper,
                                 sorted(cpu_data.values()))
-                dmat_data = list(dmat_data)
 
             # merge the results from different CPUs
-            dmat_data = np.array(dmat_data)
-            weights_dmat = dmat_data[:, 0].sum(axis=0)
-            dmat = dmat_data[:, 1].sum(axis=0)
-            r_par = dmat_data[:, 2].sum(axis=0)
-            r_trans = dmat_data[:, 3].sum(axis=0)
-            z = dmat_data[:, 4].sum(axis=0)
-            weights = dmat_data[:, 5].sum(axis=0)
-            num_pairs = dmat_data[:, 6].sum(axis=0)
-            num_pairs_used = dmat_data[:, 7].sum(axis=0)
+            dmat_data = list(dmat_data)
+            weights_dmat = np.array([item[0] for item in dmat_data]).sum(axis=0)
+            dmat = np.array([item[1] for item in dmat_data]).sum(axis=0)
+            r_par = np.array([item[2] for item in dmat_data]).sum(axis=0)
+            r_trans = np.array([item[3] for item in dmat_data]).sum(axis=0)
+            z = np.array([item[4] for item in dmat_data]).sum(axis=0)
+            weights = np.array([item[5] for item in dmat_data]).sum(axis=0)
+            num_pairs = np.array([item[6] for item in dmat_data]).sum(axis=0)
+            num_pairs_used = np.array([item[7] for item in dmat_data]).sum(axis=0)
 
             # normalize_values
             w = weights > 0
             r_par[w] /= weights[w]
             r_trans[w] /= weights[w]
             z[w] /= weights[w]
             w = weights_dmat > 0
```

### Comparing `picca-6.1.0/py/picca/bin/picca_metal_xdmat.py` & `picca-7.0.0/py/picca/bin/picca_metal_xdmat.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -177,15 +193,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--metal-alpha',
         type=float,
         default=1.,
@@ -296,15 +312,17 @@
                                                   args.nside,
                                                   xcf.lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
 
     xcf.data = data
     xcf.num_data = num_data
 
     ### Find the redshift range
     if args.z_min_obj is None:
         r_comov_min = cosmo.get_r_comov(z_min)
@@ -358,32 +376,31 @@
             context = multiprocessing.get_context('fork')
             pool = context.Pool(processes=args.nproc)
             dmat_data = pool.map(calc_metal_dmat_wrapper,
                                  sorted(cpu_data.values()))
             pool.close()
         elif args.nproc == 1:
             dmat_data = map(calc_metal_dmat_wrapper, sorted(cpu_data.values()))
-            dmat_data = list(dmat_data)
 
         # merge the results from different CPUs
-        dmat_data = np.array(dmat_data)
-        weights_dmat = dmat_data[:, 0].sum(axis=0)
-        dmat = dmat_data[:, 1].sum(axis=0)
-        r_par = dmat_data[:, 2].sum(axis=0)
-        r_trans = dmat_data[:, 3].sum(axis=0)
-        z = dmat_data[:, 4].sum(axis=0)
-        weights = dmat_data[:, 5].sum(axis=0)
+        dmat_data = list(dmat_data)
+        weights_dmat = np.array([item[0] for item in dmat_data]).sum(axis=0)
+        dmat = np.array([item[1] for item in dmat_data]).sum(axis=0)
+        r_par = np.array([item[2] for item in dmat_data]).sum(axis=0)
+        r_trans = np.array([item[3] for item in dmat_data]).sum(axis=0)
+        z = np.array([item[4] for item in dmat_data]).sum(axis=0)
+        weights = np.array([item[5] for item in dmat_data]).sum(axis=0)
 
         # normalize_values
         w = weights > 0
         r_par[w] /= weights[w]
         r_trans[w] /= weights[w]
         z[w] /= weights[w]
-        num_pairs = dmat_data[:, 6].sum(axis=0)
-        num_pairs_used = dmat_data[:, 7].sum(axis=0)
+        num_pairs = np.array([item[6] for item in dmat_data]).sum(axis=0)
+        num_pairs_used = np.array([item[7] for item in dmat_data]).sum(axis=0)
         w = weights_dmat > 0
         dmat[w, :] /= weights_dmat[w, None]
 
         # add these results to the list ofor the different metal absorption
         dmat_all.append(dmat)
         weights_dmat_all.append(weights_dmat)
         r_par_all.append(r_par)
```

### Comparing `picca-6.1.0/py/picca/bin/picca_nersc_submit.py` & `picca-7.0.0/py/picca/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_pk2fits.py` & `picca-7.0.0/py/picca/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_plot_pk1d.py` & `picca-7.0.0/py/picca/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_reduce_spall.py` & `picca-7.0.0/py/picca/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/bin/picca_wick.py` & `picca-7.0.0/py/picca/bin/picca_wick.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -303,15 +319,17 @@
                                                   cf.nside,
                                                   cf.lambda_abs,
                                                   cf.alpha,
                                                   cf.z_ref,
                                                   cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     for deltas in data.values():
         for delta in deltas:
             delta.fname = 'D1'
             for item in [
                     'cont', 'delta', 'order', 'ivar', 'exposures_diff',
                     'mean_snr', 'mean_reso', 'mean_z', 'delta_log_lambda'
             ]:
@@ -395,15 +413,17 @@
             cf.nside,
             cf.lambda_abs2,
             cf.alpha2,
             cf.z_ref,
             cosmo,
             max_num_spec=args.nspec,
             nproc=args.nproc,
-            rebin_factor=args.rebin_factor)
+            rebin_factor=args.rebin_factor,
+            z_min_qso=args.z_min_sources,
+            z_max_qso=args.z_max_sources)
         for deltas in data.values():
             for delta in deltas:
                 delta.fname = 'D2'
                 for item in [
                         'cont', 'delta', 'order', 'ivar', 'exposures_diff',
                         'mean_snr', 'mean_reso', 'mean_z', 'delta_log_lambda'
                 ]:
@@ -433,25 +453,25 @@
         wick_data = pool.map(calc_wick_terms, sorted(cpu_data.values()))
     else:
         wick_data = [calc_wick_terms(arg) for arg in sorted(cpu_data.values())]
     userprint(" \nFinished\n")
     pool.close()
 
     # merge the results from the different CPUs
-    wick_data = np.array(wick_data)
-    weights_wick = wick_data[:, 0].sum(axis=0)
-    num_pairs_wick = wick_data[:, 1].sum(axis=0)
-    num_pairs = wick_data[:, 2].sum(axis=0)
-    num_pairs_used = wick_data[:, 3].sum(axis=0)
-    t1 = wick_data[:, 4].sum(axis=0)
-    t2 = wick_data[:, 5].sum(axis=0)
-    t3 = wick_data[:, 6].sum(axis=0)
-    t4 = wick_data[:, 7].sum(axis=0)
-    t5 = wick_data[:, 8].sum(axis=0)
-    t6 = wick_data[:, 9].sum(axis=0)
+    wick_data = list(wick_data)
+    weights_wick = np.array([item[0] for item in wick_data]).sum(axis=0)
+    num_pairs_wick = np.array([item[1] for item in wick_data]).sum(axis=0)
+    num_pairs = np.array([item[2] for item in wick_data]).sum(axis=0)
+    num_pairs_used = np.array([item[3] for item in wick_data]).sum(axis=0)
+    t1 = np.array([item[4] for item in wick_data]).sum(axis=0)
+    t2 = np.array([item[5] for item in wick_data]).sum(axis=0)
+    t3 = np.array([item[6] for item in wick_data]).sum(axis=0)
+    t4 = np.array([item[7] for item in wick_data]).sum(axis=0)
+    t5 = np.array([item[8] for item in wick_data]).sum(axis=0)
+    t6 = np.array([item[9] for item in wick_data]).sum(axis=0)
     weights = weights_wick * weights_wick[:, None]
     w = weights > 0.
     t1[w] /= weights[w]
     t2[w] /= weights[w]
     t3[w] /= weights[w]
     t4[w] /= weights[w]
     t5[w] /= weights[w]
```

### Comparing `picca-6.1.0/py/picca/bin/picca_xcf.py` & `picca-7.0.0/py/picca/bin/picca_xcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,29 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Min redshift of the background quasars'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -151,15 +166,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--fid-Om',
         type=float,
         default=0.315,
@@ -289,15 +304,17 @@
                                                   xcf.lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo=cosmo,
                                                   max_num_spec=args.nspec,
                                                   no_project=args.no_project,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     xcf.data = data
     xcf.num_data = num_data
     userprint("")
     userprint("done, npix = {}\n".format(len(data)))
     ### Remove <delta> vs. lambda_obs
     if not args.no_remove_mean_lambda_obs:
         Forest.delta_log_lambda = None
```

### Comparing `picca-6.1.0/py/picca/bin/picca_xcf1d.py` & `picca-7.0.0/py/picca/bin/picca_xcf1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -138,15 +154,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument('--no-project',
                         action='store_true',
                         required=False,
                         help='Do not project out continuum fitting modes')
@@ -195,15 +211,17 @@
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
                                                   args.nside,
                                                   lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo=None,
                                                   max_num_spec=args.nspec,
-                                                  no_project=args.no_project)
+                                                  no_project=args.no_project,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     xcf.data = data
     xcf.num_data = num_data
     sys.stderr.write("\n")
     userprint("done, npix = {}".format(len(data)))
 
     ### Remove <delta> vs. lambda_obs
     if not args.no_remove_mean_lambda_obs:
```

### Comparing `picca-6.1.0/py/picca/bin/picca_xcf_angl.py` & `picca-7.0.0/py/picca/bin/picca_xcf_angl.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -156,15 +172,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--fid-Om',
         type=float,
         default=0.315,
@@ -251,15 +267,17 @@
         args.in_dir,
         args.nside,
         constants.ABSORBER_IGM[args.lambda_abs],
         args.z_evol_del,
         args.z_ref,
         cosmo=cosmo,
         max_num_spec=args.nspec,
-        no_project=args.no_project)
+        no_project=args.no_project,
+        z_min_qso=args.z_min_sources,
+        z_max_qso=args.z_max_sources)
     xcf.data = data
     xcf.num_data = num_data
     userprint("")
     userprint("done, npix = {}".format(len(data)))
 
     ### Remove <delta> vs. lambda_obs
     if not args.no_remove_mean_lambda_obs:
```

### Comparing `picca-6.1.0/py/picca/bin/picca_xdmat.py` & `picca-7.0.0/py/picca/bin/picca_xdmat.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -159,15 +175,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--fid-Om',
         type=float,
         default=0.315,
@@ -265,15 +281,17 @@
                                                   args.nside,
                                                   xcf.lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo=cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     xcf.data = data
     xcf.num_data = num_data
     userprint("\n")
     userprint("done, npix = {}\n".format(len(data)))
 
     ### Find the redshift range
     if args.z_min_obj is None:
@@ -319,23 +337,23 @@
         dmat_data = map(calc_dmat, sorted(cpu_data.values()))
         dmat_data = list(dmat_data)
 
     t2 = time.time()
     userprint(f'picca_xdmat.py - Time computing distortion matrix: {(t2-t1)/60:.3f} minutes')
 
     # merge the results from different CPUs
-    dmat_data = np.array(dmat_data)
-    weights_dmat = dmat_data[:, 0].sum(axis=0)
-    dmat = dmat_data[:, 1].sum(axis=0)
-    r_par = dmat_data[:, 2].sum(axis=0)
-    r_trans = dmat_data[:, 3].sum(axis=0)
-    z = dmat_data[:, 4].sum(axis=0)
-    weights = dmat_data[:, 5].sum(axis=0)
-    num_pairs = dmat_data[:, 6].sum(axis=0)
-    num_pairs_used = dmat_data[:, 7].sum(axis=0)
+    dmat_data = list(dmat_data)
+    weights_dmat = np.array([item[0] for item in dmat_data]).sum(axis=0)
+    dmat = np.array([item[1] for item in dmat_data]).sum(axis=0)
+    r_par = np.array([item[2] for item in dmat_data]).sum(axis=0)
+    r_trans = np.array([item[3] for item in dmat_data]).sum(axis=0)
+    z = np.array([item[4] for item in dmat_data]).sum(axis=0)
+    weights = np.array([item[5] for item in dmat_data]).sum(axis=0)
+    num_pairs = np.array([item[6] for item in dmat_data]).sum(axis=0)
+    num_pairs_used = np.array([item[7] for item in dmat_data]).sum(axis=0)
 
     # normalize values
     w = weights > 0.
     r_par[w] /= weights[w]
     r_trans[w] /= weights[w]
     z[w] /= weights[w]
     w = weights_dmat > 0.
```

### Comparing `picca-6.1.0/py/picca/bin/picca_xwick.py` & `picca-7.0.0/py/picca/bin/picca_xwick.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,14 +126,30 @@
         default=10.,
         required=False,
         help=('Use only pairs of forest x object with the mean of the last '
               'absorber redshift and the object redshift smaller than '
               'z-cut-max'))
 
     parser.add_argument(
+        '--z-min-sources',
+        type=float,
+        default=0.,
+        required=False,
+        help=('Limit the minimum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
+        '--z-max-sources',
+        type=float,
+        default=10.,
+        required=False,
+        help=('Limit the maximum redshift of the quasars '
+                'used as sources for spectra'))
+
+    parser.add_argument(
         '--lambda-abs',
         type=str,
         default='LYA',
         required=False,
         help=('Name of the absorption in picca.constants defining the redshift '
               'of the delta'))
 
@@ -149,15 +165,15 @@
         default=2.9,
         required=False,
         help='Exponent of the redshift evolution of the delta field')
 
     parser.add_argument(
         '--z-evol-obj',
         type=float,
-        default=1.,
+        default=1.44,
         required=False,
         help='Exponent of the redshift evolution of the object field')
 
     parser.add_argument(
         '--fid-Om',
         type=float,
         default=0.315,
@@ -232,15 +248,15 @@
                         help='Maximum number of spectra to read')
 
     parser.add_argument('--rebin-factor',
                         type=int,
                         default=None,
                         required=False,
                         help='Rebin factor for deltas. If not None, deltas will '
-                             'be rebinned by that factor')    
+                             'be rebinned by that factor')
 
     args = parser.parse_args(cmdargs)
     if args.nproc is None:
         args.nproc = cpu_count() // 2
 
     # setup variables in module xcf
     xcf.r_par_min = args.rp_min
@@ -277,15 +293,17 @@
                                                   args.nside,
                                                   xcf.lambda_abs,
                                                   args.z_evol_del,
                                                   args.z_ref,
                                                   cosmo=cosmo,
                                                   max_num_spec=args.nspec,
                                                   nproc=args.nproc,
-                                                  rebin_factor=args.rebin_factor)
+                                                  rebin_factor=args.rebin_factor,
+                                                  z_min_qso=args.z_min_sources,
+                                                  z_max_qso=args.z_max_sources)
     for deltas in data.values():
         for delta in deltas:
             delta.fname = 'D1'
             for item in [
                     'cont', 'delta', 'order', 'ivar', 'exposures_diff',
                     'mean_snr', 'mean_reso', 'mean_z', 'delta_log_lambda'
             ]:
@@ -386,25 +404,25 @@
     context = multiprocessing.get_context('fork')
     pool = context.Pool(processes=min(args.nproc, len(cpu_data.values())))
     userprint(" \nStarting\n")
     wick_data = pool.map(calc_wick_terms, sorted(cpu_data.values()))
     userprint(" \nFinished\n")
     pool.close()
 
-    wick_data = np.array(wick_data)
-    weights_wick = wick_data[:, 0].sum(axis=0)
-    num_pairs_wick = wick_data[:, 1].sum(axis=0)
-    npairs = wick_data[:, 2].sum(axis=0)
-    npairs_used = wick_data[:, 3].sum(axis=0)
-    t1 = wick_data[:, 4].sum(axis=0)
-    t2 = wick_data[:, 5].sum(axis=0)
-    t3 = wick_data[:, 6].sum(axis=0)
-    t4 = wick_data[:, 7].sum(axis=0)
-    t5 = wick_data[:, 8].sum(axis=0)
-    t6 = wick_data[:, 9].sum(axis=0)
+    wick_data = list(wick_data)
+    weights_wick = np.array([item[0] for item in wick_data]).sum(axis=0)
+    num_pairs_wick = np.array([item[1] for item in wick_data]).sum(axis=0)
+    npairs = np.array([item[2] for item in wick_data]).sum(axis=0)
+    npairs_used = np.array([item[3] for item in wick_data]).sum(axis=0)
+    t1 = np.array([item[4] for item in wick_data]).sum(axis=0)
+    t2 = np.array([item[5] for item in wick_data]).sum(axis=0)
+    t3 = np.array([item[6] for item in wick_data]).sum(axis=0)
+    t4 = np.array([item[7] for item in wick_data]).sum(axis=0)
+    t5 = np.array([item[8] for item in wick_data]).sum(axis=0)
+    t6 = np.array([item[9] for item in wick_data]).sum(axis=0)
     weights = weights_wick * weights_wick[:, None]
     w = weights > 0.
     t1[w] /= weights[w]
     t2[w] /= weights[w]
     t3[w] /= weights[w]
     t4[w] /= weights[w]
     t5[w] /= weights[w]
```

### Comparing `picca-6.1.0/py/picca/cf.py` & `picca-7.0.0/py/picca/cf.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,18 +13,19 @@
     - compute_wick_terms
     - compute_wickT123_pairs
     - compute_wickT45_pairs
 See the respective docstrings for more details
 """
 import numpy as np
 from healpy import query_disc
-from numba import jit, int32
+from numba import njit, int32
 
 from . import constants
 from .utils import userprint
+import warnings
 
 num_bins_r_par = None
 num_bins_r_trans = None
 num_model_bins_r_trans = None
 num_model_bins_r_par = None
 r_par_max = None
 r_par_min = None
@@ -193,108 +194,15 @@
     xi[w] /= weights[w]
     r_par[w] /= weights[w]
     r_trans[w] /= weights[w]
     z[w] /= weights[w]
     return weights, xi, r_par, r_trans, z, num_pairs
 
 
-#-- This has been superseeded by compute_xi_forest_pairs_fast
-#-- and will be deprecated
-@jit
-def compute_xi_forest_pairs(z1, r_comov1, dist_m1, weights1, delta1, z2,
-                            r_comov2, dist_m2, weights2, delta2, ang,
-                            same_half_plate):
-    """Computes the contribution of a given pair of forests to the correlation
-    function.
-
-    Args:
-        z1: array of float
-            Redshift of pixel 1
-        r_comov1: array of float
-            Comoving distance for forest 1 (in Mpc/h)
-        dist_m1: array of float
-            Comoving angular distance for forest 1 (in Mpc/h)
-        weights1: array of float
-            Pixel weights for forest 1
-        delta1: array of float
-            Delta field for forest 1
-        z2: array of float
-            Redshift of pixel 2
-        r_comov2: array of float
-            Comoving distance for forest 2 (in Mpc/h)
-        dist_m2: array of float
-            Comoving angular distance for forest 2 (in Mpc/h)
-        weights2: array of float
-            Pixel weights for forest 2
-        delta2: array of float
-            Delta field for forest 2
-        ang: array of float
-            Angular separation between pixels in forests 1 and 2
-        same_half_plate: bool
-            Flag to determine if the two forests are on the same half plate
-
-    Returns:
-        The following variables:
-            rebin_weight: The weight of the correlation function pixels
-                properly rebinned
-            rebin_xi: The correlation function properly rebinned
-            rebin_r_par: The parallel distance of the correlation function
-                pixels properly rebinned
-            rebin_r_trans: The transverse distance of the correlation function
-                pixels properly rebinned
-            rebin_z: The redshift of the correlation function pixels properly
-                rebinned
-            rebin_num_pairs: The number of pairs of the correlation function
-                pixels properly rebinned
-    """
-    delta_times_weight1 = delta1 * weights1
-    delta_times_weight2 = delta2 * weights2
-    if ang_correlation:
-        r_par = r_comov1 / r_comov2[:, None]
-        if not x_correlation:
-            r_par[r_par < 1.] = 1. / r_par[r_par < 1.]
-        r_trans = ang * np.ones_like(r_par)
-    else:
-        r_par = (r_comov1 - r_comov2[:, None]) * np.cos(ang / 2)
-        if not x_correlation:
-            r_par = abs(r_par)
-        r_trans = (dist_m1 + dist_m2[:, None]) * np.sin(ang / 2)
-    delta_times_weight12 = delta_times_weight1 * delta_times_weight2[:, None]
-    weights12 = weights1 * weights2[:, None]
-    z = (z1 + z2[:, None]) / 2
-
-    w = (r_par < r_par_max) & (r_trans < r_trans_max) & (r_par >= r_par_min)
-
-    r_par = r_par[w]
-    r_trans = r_trans[w]
-    z = z[w]
-    delta_times_weight12 = delta_times_weight12[w]
-    weights12 = weights12[w]
-    bins_r_par = np.floor((r_par - r_par_min) / (r_par_max - r_par_min) *
-                          num_bins_r_par).astype(int)
-    bins_r_trans = (r_trans / r_trans_max * num_bins_r_trans).astype(int)
-    bins = bins_r_trans + num_bins_r_trans * bins_r_par
-
-    if remove_same_half_plate_close_pairs and same_half_plate:
-        w = abs(r_par) < (r_par_max - r_par_min) / num_bins_r_par
-        delta_times_weight12[w] = 0.
-        weights12[w] = 0.
-
-    rebin_xi = np.bincount(bins, weights=delta_times_weight12)
-    rebin_weight = np.bincount(bins, weights=weights12)
-    rebin_r_par = np.bincount(bins, weights=r_par * weights12)
-    rebin_r_trans = np.bincount(bins, weights=r_trans * weights12)
-    rebin_z = np.bincount(bins, weights=z * weights12)
-    rebin_num_pairs = np.bincount(bins, weights=(weights12 > 0.))
-
-    return (rebin_weight, rebin_xi, rebin_r_par, rebin_r_trans, rebin_z,
-            rebin_num_pairs)
-
-
-@jit(nopython=True)
+@njit
 def compute_xi_forest_pairs_fast(z1, r_comov1, dist_m1, weights1, delta1, z2,
                                  r_comov2, dist_m2, weights2, delta2, ang,
                                  same_half_plate, rebin_weight, rebin_xi,
                                  rebin_r_par, rebin_r_trans, rebin_z,
                                  rebin_num_pairs):
     """Computes the contribution of a given pair of forests to the correlation
     function. Fills rebin_* on place.
@@ -364,15 +272,15 @@
             delta_times_weight12 = delta_times_weight1 * delta_times_weight2
             weights12 = weights1[i] * weights2[j]
             z = (z1[i] + z2[j]) / 2
 
             bins_r_par = np.floor(
                 (r_par - r_par_min) / (r_par_max - r_par_min) * num_bins_r_par)
             bins_r_trans = np.floor(r_trans / r_trans_max * num_bins_r_trans)
-            bins = np.int(bins_r_trans + num_bins_r_trans * bins_r_par)
+            bins = int(bins_r_trans + num_bins_r_trans * bins_r_par)
 
             if remove_same_half_plate_close_pairs and same_half_plate:
                 if np.abs(r_par) < (r_par_max - r_par_min) / num_bins_r_par:
                     continue
 
             rebin_xi[bins] += delta_times_weight12
             rebin_weight[bins] += weights12
@@ -457,262 +365,15 @@
     dmat = dmat.reshape(num_bins_r_par * num_bins_r_trans,
                         num_model_bins_r_par * num_model_bins_r_trans)
 
     return (weights_dmat, dmat, r_par_eff, r_trans_eff, z_eff, weight_eff,
             num_pairs, num_pairs_used)
 
 
-#-- This has been superseeded by compute_dmat_forest_pairs_fast
-#-- and will be deprecated
-@jit
-def compute_dmat_forest_pairs(log_lambda1, log_lambda2, r_comov1, r_comov2,
-                              dist_m1, dist_m2, z1, z2, weights1, weights2, ang,
-                              weights_dmat, dmat, r_par_eff, r_trans_eff, z_eff,
-                              weight_eff, same_half_plate, order1, order2):
-    """Computes the contribution of a given pair of forests to the distortion
-    matrix.
-
-    Args:
-        log_lambda1: array of float
-            Logarithm of the wavelength (in Angs) for forest 1
-        log_lambda2: array of float
-            Logarithm of the wavelength (in Angs) for forest 2
-        r_comov1: array of floats
-            Comoving distance (in Mpc/h) for forest 1
-        r_comov2: array of floats
-            Comoving distance (in Mpc/h) for forest 2
-        dist_m1: array of floats
-            Angular distance for forest 1
-        dist_m2: array of floats
-            Angular distance for forest 2
-        z1: array of floats
-            Redshifts for forest 1
-        z2: array of floats
-            Redshifts for forest 2
-        weights1: array of floats
-            Weights for forest 1
-        weights2: array of floats
-            Weights for forest 2
-        ang: array of floats
-            Angular separation between pixels in forests 1 and 2
-        weights_dmat: array of floats
-            Total weight in the distortion matrix pixels
-        dmat: array of floats
-            The distortion matrix
-        r_par_eff: array of floats
-            Effective parallel distance for the distortion matrix bins
-        r_trans_eff: array of floats
-            Effective transverse distance for the distortion matrix bins
-        z_eff: array of floats
-            Effective redshift for the distortion matrix bins
-        weight_eff: array of floats
-            Effective weight of the distortion matrix pixels
-        same_half_plate: bool
-            Flag to determine if the two forests are on the same half plate
-        order1: 0 or 1
-            Order of the log10(lambda) polynomial for the continuum fit in
-            forest 1
-        order 2: 0 or 1
-            Order of the log10(lambda) polynomial for the continuum fit in
-            forest 2
-    """
-    # find distances between pixels
-    r_par = (r_comov1[:, None] - r_comov2) * np.cos(ang / 2)
-    if not x_correlation:
-        r_par = abs(r_par)
-    r_trans = (dist_m1[:, None] + dist_m2) * np.sin(ang / 2)
-    z = (z1[:, None] + z2) / 2.
-
-    w = (r_par < r_par_max) & (r_trans < r_trans_max) & (r_par >= r_par_min)
-
-    # locate bins pixels are contributing to (correlation bins)
-    bins_r_par = np.floor((r_par - r_par_min) / (r_par_max - r_par_min) *
-                          num_bins_r_par).astype(int)
-    bins_r_trans = (r_trans / r_trans_max * num_bins_r_trans).astype(int)
-    bins = bins_r_trans + num_bins_r_trans * bins_r_par
-    bins = bins[w]
-
-    # locate bins pixels are contributing to (model bins)
-    model_bins_r_par = np.floor((r_par - r_par_min) / (r_par_max - r_par_min) *
-                                num_model_bins_r_par).astype(int)
-    model_bins_r_trans = (r_trans / r_trans_max *
-                          num_model_bins_r_trans).astype(int)
-    model_bins = model_bins_r_trans + num_model_bins_r_trans * model_bins_r_par
-    model_bins = model_bins[w]
-
-    # compute useful auxiliar variables to speed up computation of eta
-    # (equation 6 of du Mas des Bourboux et al. 2020)
-
-    # denominator second term in equation 6 of du Mas des Bourboux et al. 2020
-    sum_weights1 = weights1.sum()
-    sum_weights2 = weights2.sum()
-
-    # mean of log_lambda
-    mean_log_lambda1 = np.average(log_lambda1, weights=weights1)
-    mean_log_lambda2 = np.average(log_lambda2, weights=weights2)
-
-    # log_lambda minus its mean
-    log_lambda_minus_mean1 = log_lambda1 - mean_log_lambda1
-    log_lambda_minus_mean2 = log_lambda2 - mean_log_lambda2
-
-    # denominator third term in equation 6 of du Mas des Bourboux et al. 2020
-    sum_weights_square_log_lambda_minus_mean1 = (
-        weights1 * log_lambda_minus_mean1**2).sum()
-    sum_weights_square_log_lambda_minus_mean2 = (
-        weights2 * log_lambda_minus_mean2**2).sum()
-
-    # auxiliar variables to loop over distortion matrix bins
-    num_pixels1 = len(log_lambda1)
-    num_pixels2 = len(log_lambda2)
-    ij = np.arange(num_pixels1)[:, None] + num_pixels1 * np.arange(num_pixels2)
-    ij = ij[w]
-
-    weights12 = weights1[:, None] * weights2
-    weights12 = weights12[w]
-
-    if remove_same_half_plate_close_pairs and same_half_plate:
-        weights12[abs(r_par[w]) < (r_par_max - r_par_min) / num_bins_r_par] = 0.
-
-    rebin = np.bincount(model_bins, weights=weights12 * r_par[w])
-    r_par_eff[:rebin.size] += rebin
-    rebin = np.bincount(model_bins, weights=weights12 * r_trans[w])
-    r_trans_eff[:rebin.size] += rebin
-    rebin = np.bincount(model_bins, weights=weights12 * z[w])
-    z_eff[:rebin.size] += rebin
-    rebin = np.bincount(model_bins, weights=weights12)
-    weight_eff[:rebin.size] += rebin
-
-    rebin = np.bincount(bins, weights=weights12)
-    weights_dmat[:len(rebin)] += rebin
-
-    # Combining equation 21 and equation 6 of du Mas des Bourboux et al. 2020
-    # we find an equation with 9 terms comming from the product of two eta
-    # The variables below stand for 8 of these 9 terms (the first one is
-    # pretty trivial)
-
-    # first eta, first term: kronecker delta
-    # second eta, second term: weight/sum(weights)
-    eta1 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans * num_pixels1)
-
-    # first eta, second term: weight/sum(weights)
-    # second eta, first term: kronecker delta
-    eta2 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans * num_pixels2)
-
-    # first eta, first term: kronecker delta
-    # second eta, third term: (non-zero only for order=1)
-    #   weight*(Lambda-bar(Lambda))*(Lambda-bar(Lambda))/
-    #   sum(weight*(Lambda-bar(Lambda)**2))
-    eta3 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans * num_pixels1)
-
-    # first eta, third term: (non-zero only for order=1)
-    #   weight*(Lambda-bar(Lambda))*(Lambda-bar(Lambda))/
-    #   sum(weight*(Lambda-bar(Lambda)**2))
-    # second eta, first term: kronecker delta
-    eta4 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans * num_pixels2)
-
-    # first eta, second term: weight/sum(weights)
-    # second eta, second term: weight/sum(weights)
-    eta5 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans)
-
-    # first eta, second term: weight/sum(weights)
-    # second eta, third term: (non-zero only for order=1)
-    #   weight*(Lambda-bar(Lambda))*(Lambda-bar(Lambda))/
-    #   sum(weight*(Lambda-bar(Lambda)**2))
-    eta6 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans)
-
-    # first eta, third term: (non-zero only for order=1)
-    #   weight*(Lambda-bar(Lambda))*(Lambda-bar(Lambda))/
-    #   sum(weight*(Lambda-bar(Lambda)**2))
-    # second eta, second term: weight/sum(weights)
-    eta7 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans)
-
-    # first eta, third term: (non-zero only for order=1)
-    #   weight*(Lambda-bar(Lambda))*(Lambda-bar(Lambda))/
-    #   sum(weight*(Lambda-bar(Lambda)**2))
-    # second eta, third term: (non-zero only for order=1)
-    #   weight*(Lambda-bar(Lambda))*(Lambda-bar(Lambda))/
-    #   sum(weight*(Lambda-bar(Lambda)**2))
-    eta8 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans)
-
-    # compute the contributions to the distortion matrix
-    rebin = np.bincount(ij % num_pixels1 + num_pixels1 * model_bins,
-                        weights=((np.ones(num_pixels1)[:, None] * weights2)[w] /
-                                 sum_weights2))
-    eta1[:len(rebin)] += rebin
-    rebin = np.bincount(
-        ((ij - ij % num_pixels1) // num_pixels1 + num_pixels2 * model_bins),
-        weights=((weights1[:, None] * np.ones(num_pixels2))[w] / sum_weights1))
-    eta2[:len(rebin)] += rebin
-    rebin = np.bincount(model_bins,
-                        weights=((weights1[:, None] * weights2)[w] /
-                                 sum_weights1 / sum_weights2))
-    eta5[:len(rebin)] += rebin
-
-    if order2 == 1:
-        rebin = np.bincount(ij % num_pixels1 + num_pixels1 * model_bins,
-                            weights=((np.ones(num_pixels1)[:, None] * weights2 *
-                                      log_lambda_minus_mean2)[w] /
-                                     sum_weights_square_log_lambda_minus_mean2))
-        eta3[:len(rebin)] += rebin
-        rebin = np.bincount(
-            model_bins,
-            weights=(((weights1[:, None] *
-                       (weights2 * log_lambda_minus_mean2))[w] / sum_weights1 /
-                      sum_weights_square_log_lambda_minus_mean2)))
-        eta6[:len(rebin)] += rebin
-    if order1 == 1:
-        rebin = np.bincount(
-            ((ij - ij % num_pixels1) // num_pixels1 + num_pixels2 * model_bins),
-            weights=(((weights1 * log_lambda_minus_mean1)[:, None] *
-                      np.ones(num_pixels2))[w] /
-                     sum_weights_square_log_lambda_minus_mean1))
-        eta4[:len(rebin)] += rebin
-        rebin = np.bincount(
-            model_bins,
-            weights=((
-                (weights1 * log_lambda_minus_mean1)[:, None] * weights2)[w] /
-                     sum_weights_square_log_lambda_minus_mean1 / sum_weights2))
-        eta7[:len(rebin)] += rebin
-        if order2 == 1:
-            rebin = np.bincount(
-                model_bins,
-                weights=(((weights1 * log_lambda_minus_mean1)[:, None] *
-                          (weights2 * log_lambda_minus_mean2))[w] /
-                         sum_weights_square_log_lambda_minus_mean1 /
-                         sum_weights_square_log_lambda_minus_mean2))
-            eta8[:len(rebin)] += rebin
-
-    # Now add all the contributions together
-    unique_model_bins = np.unique(model_bins)
-    for index, (bin, model_bin) in enumerate(zip(bins, model_bins)):
-        # first eta, first term: kronecker delta
-        # second eta, first term: kronecker delta
-        dmat[model_bin + num_model_bins_r_par * num_model_bins_r_trans *
-             bin] += weights12[index]
-        i = ij[index] % num_pixels1
-        j = (ij[index] - i) // num_pixels1
-        # rest of the terms
-        for unique_model_bin in unique_model_bins:
-            dmat[unique_model_bin +
-                 num_model_bins_r_par * num_model_bins_r_trans * bin] += (
-                     weights12[index] *
-                     (eta5[unique_model_bin] + eta6[unique_model_bin] *
-                      log_lambda_minus_mean2[j] + eta7[unique_model_bin] *
-                      log_lambda_minus_mean1[i] + eta8[unique_model_bin] *
-                      log_lambda_minus_mean1[i] * log_lambda_minus_mean2[j]) -
-                     (weights12[index] *
-                      (eta1[i + num_pixels1 * unique_model_bin] +
-                       eta2[j + num_pixels2 * unique_model_bin] +
-                       eta3[i + num_pixels1 * unique_model_bin] *
-                       log_lambda_minus_mean2[j] +
-                       eta4[j + num_pixels2 * unique_model_bin] *
-                       log_lambda_minus_mean1[i])))
-
-
-@jit(nopython=True)
+@njit
 def compute_dmat_forest_pairs_fast(log_lambda1, log_lambda2, r_comov1, r_comov2,
                                    dist_m1, dist_m2, z1, z2, weights1, weights2,
                                    ang, weights_dmat, dmat, r_par_eff,
                                    r_trans_eff, z_eff, weight_eff,
                                    same_half_plate, order1, order2):
 
     #-- First, determine how many relevant pixel pairs for speed up
@@ -1390,117 +1051,15 @@
                 ### TODO: when there is two different catalogs
                 ### delta3 and delta1 have the same 'fname'
 
     return (weights_wick, num_pairs_wick, num_pairs, num_pairs_used, t1, t2, t3,
             t4, t5, t6)
 
 
-#@jit    #this is the old routine and might be removed anytime
-def compute_wickT123_pairs_slow(r_comov1, r_comov2, ang, weights1, weights2, z1,
-                                z2, weighted_xi_1d_1, weighted_xi_1d_2,
-                                weights_wick, num_pairs_wick, t1, t2, t3):
-    """
-    Computes the Wick expansion terms 1, 2, and 3 of a given pair of forests
-
-    Each of the terms represents the contribution of different type of pairs as
-    illustrated in figure A.1 from Delubac et al. 2015
-
-    Args:
-        r_comov1: array of floats
-            Comoving distance (in Mpc/h) for forest 1
-        r_comov2: array of floats
-            Comoving distance (in Mpc/h) for forest 2
-        ang: array of floats
-            Angular separation between pixels in forests 1 and 2
-        weights1: array of floats
-            Weights for forest 1
-        weights2: array of floats
-            Weights for forest 2
-        z1: array of floats
-            Redshifts for forest 1
-        z2: array of floats
-            Redshifts for forest 2
-        weighted_xi_1d_1: array of floats
-            Weighted 1D correlation function for forest 1
-        weighted_xi_1d_2: array of floats
-            Weighted 1D correlation function for forest 2
-        weights_wick: array of floats
-            Total weight in the covariance matrix pixels
-        num_pairs_wick: array of floats
-            Total number of pairs in the covariance matrix pixels
-        t1: array of floats
-            Wick expansion, term 1
-        t2: array of floats
-            Wick expansion, term 2
-        t3: array of floats
-            Wick expansion, term 3
-    """
-    num_pixels1 = len(r_comov1)
-    num_pixels2 = len(r_comov2)
-    i1 = np.arange(num_pixels1)
-    i2 = np.arange(num_pixels2)
-    z_weight_evol1 = ((1 + z1) / (1 + z_ref))**(alpha - 1)
-    z_weight_evol2 = ((1 + z2) / (1 + z_ref))**(alpha2 - 1)
-
-    bins = i1[:, None] + num_pixels1 * i2
-    r_par = (r_comov1[:, None] - r_comov2) * np.cos(ang / 2)
-    if not x_correlation:
-        r_par = abs(r_par)
-    r_trans = (r_comov1[:, None] + r_comov2) * np.sin(ang / 2)
-    bins_r_par = np.floor((r_par - r_par_min) / (r_par_max - r_par_min) *
-                          num_bins_r_par).astype(int)
-    bins_r_trans = (r_trans / r_trans_max * num_bins_r_trans).astype(int)
-    bins_forest = bins_r_trans + num_bins_r_trans * bins_r_par
-    weights12 = weights1[:, None] * weights2
-    weight1 = weights1[:, None] * np.ones(weights2.size)
-    weight2 = np.ones(weights1.size)[:, None] * weights2
-    z_weight_evol = z_weight_evol1[:, None] * z_weight_evol2
-
-    w = (r_par < r_par_max) & (r_trans < r_trans_max) & (r_par >= r_par_min)
-    if w.sum() == 0:
-        return
-
-    bins = bins[w]
-    bins_forest = bins_forest[w]
-    weights12 = weights12[w]
-    weight1 = weight1[w]
-    weight2 = weight2[w]
-    z_weight_evol = z_weight_evol[w]
-
-    for index1 in range(bins_forest.size):
-        p1 = bins_forest[index1]
-        i1 = bins[index1] % num_pixels1
-        j1 = (bins[index1] - i1) // num_pixels1
-        weights_wick[p1] += weights12[index1]
-        num_pairs_wick[p1] += 1
-        t1[p1, p1] += weights12[index1] * z_weight_evol[index1]
-
-        for index2 in range(index1 + 1, bins_forest.size):
-            p2 = bins_forest[index2]
-            i2 = bins[index2] % num_pixels1
-            j2 = (bins[index2] - i2) // num_pixels1
-            if i1 == i2:
-                prod = weighted_xi_1d_2[
-                    j1, j2] * weight1[index1] * z_weight_evol1[i1]
-                t2[p1, p2] += prod
-                t2[p2, p1] += prod
-            elif j1 == j2:
-                prod = weighted_xi_1d_1[
-                    i1, i2] * weight2[index2] * z_weight_evol2[j1]
-                t2[p1, p2] += prod
-                t2[p2, p1] += prod
-            else:
-                prod = weighted_xi_1d_1[i1, i2] * weighted_xi_1d_2[j1, j2]
-                t3[p1, p2] += prod
-                t3[p2, p1] += prod
-
-    return
-
-
-@jit(nopython=True)
+@njit
 def compute_wickT123_pairs(r_comov1, r_comov2, ang, weights1, weights2, z1, z2,
                            weighted_xi_1d_1, weighted_xi_1d_2, weights_wick,
                            num_pairs_wick, t1, t2, t3):
     """
     Computes the Wick expansion terms 1, 2, and 3 of a given pair of forests
 
     Each of the terms represents the contribution of different type of pairs as
@@ -1612,15 +1171,15 @@
                 prod = weighted_xi_1d_1[i1, i2] * weighted_xi_1d_2[j1, j2]
                 t3[p1, p2] += prod
                 t3[p2, p1] += prod
 
     return
 
 
-@jit
+@njit
 def compute_wickT45_pairs(r_comov1, r_comov2, r_comov3, ang12, ang13, ang23,
                           weights1, weights2, weights3, z1, z2, z3,
                           weighted_xi_1d_1, weighted_xi_1d_2, weighted_xi_1d_3,
                           fname1, fname2, fname3, t4, t5):
     """
     Computes the Wick expansion terms 4 and 5 of a given set of 3 forests
 
@@ -1659,14 +1218,16 @@
         fname3: string
             Flag name identifying the group of deltas for forest 3
         t4: array of floats
             Wick expansion, term 4
         t5: array of floats
             Wick expansion, term 5
     """
+    warnings.warn("Currently using a slow non-jit compiled function compute_wickT45_pairs, this will be deprecated as a faster one exists!")
+
     ### forest-1 x forest-2
     r_par = (r_comov1[:, None] - r_comov2) * np.cos(ang12 / 2.)
     if not x_correlation:
         r_par = np.absolute(r_par)
     r_trans = (r_comov1[:, None] + r_comov2) * np.sin(ang12 / 2.)
     bins1_12 = (np.arange(r_comov1.size)[:, None] *
                 np.ones(r_comov2.size)).astype(int)
@@ -1757,15 +1318,15 @@
                 t5[p1, p2] += prod
                 t5[p2, p1] += prod
 
     return
 
 
 #TODO: this should be completed at some point, the function above did not work either, and numba-ing the output dict is not simple
-@jit(nopython=True)
+@njit
 def compute_wickT45_pairs_fast(r_comov1, r_comov2, r_comov3, ang12, ang13,
                                ang23, weights1, weights2, weights3, z1, z2, z3,
                                weighted_xi_1d_1, weighted_xi_1d_2,
                                weighted_xi_1d_3, fname1, fname2, fname3, t4,
                                t5):
     """
     Computes the Wick expansion terms 4 and 5 of a given set of 3 forests
```

### Comparing `picca-6.1.0/py/picca/co.py` & `picca-7.0.0/py/picca/co.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     - fill_neighs
     - compute_xi
     - compute_xi_forest_pairs
 See the respective docstrings for more details
 """
 import numpy as np
 from healpy import query_disc
-from numba import jit
+from numba import njit
 
 from .utils import userprint
+import warnings
 
 num_bins_r_par = None
 num_bins_r_trans = None
 r_par_min = None
 r_par_max = None
 r_trans_max = None
 ang_max = None
@@ -127,82 +128,15 @@
     w = weights > 0.
     r_par[w] /= weights[w]
     r_trans[w] /= weights[w]
     z[w] /= weights[w]
     return weights, r_par, r_trans, z, num_pairs
 
 
-@jit  #will be deprecated
-def compute_xi_forest_pairs_slow(z1, r_comov1, dist_m1, weights1, z2, r_comov2,
-                                 dist_m2, weights2, ang):
-    """Computes the contribution of a given pair of forests to the correlation
-    function.
-
-    Args:
-        z1: array of float
-            Redshift of pixel 1
-        r_comov1: array of float
-            Comoving distance for forest 1 (in Mpc/h)
-        dist_m1: array of float
-            Comoving angular distance for forest 1 (in Mpc/h)
-        weights1: array of float
-            Pixel weights for forest 1
-        z2: array of float
-            Redshift of pixel 2
-        r_comov2: array of float
-            Comoving distance for forest 2 (in Mpc/h)
-        dist_m2: array of float
-            Comoving angular distance for forest 2 (in Mpc/h)
-        weights2: array of float
-            Pixel weights for forest 2
-        ang: array of float
-            Angular separation between pixels in forests 1 and 2
-
-    Returns:
-        The following variables:
-            rebin_weight: The weight of the correlation function pixels
-                properly rebinned
-            rebin_r_par: The parallel distance of the correlation function
-                pixels properly rebinned
-            rebin_r_trans: The transverse distance of the correlation function
-                pixels properly rebinned
-            rebin_z: The redshift of the correlation function pixels properly
-                rebinned
-            rebin_num_pairs: The number of pairs of the correlation function
-                pixels properly rebinned
-    """
-    r_par = (r_comov1 - r_comov2) * np.cos(ang / 2.)
-    if not x_correlation or type_corr in ['DR', 'RD']:
-        r_par = np.absolute(r_par)
-    r_trans = (dist_m1 + dist_m2) * np.sin(ang / 2.)
-    z = (z1 + z2) / 2.
-    weights12 = weights1 * weights2
-
-    w = (r_par >= r_par_min) & (r_par < r_par_max) & (r_trans < r_trans_max)
-    w &= (weights12 > 0.)
-    r_par = r_par[w]
-    r_trans = r_trans[w]
-    z = z[w]
-    weights12 = weights12[w]
-
-    bins_r_par = np.floor((r_par - r_par_min) / (r_par_max - r_par_min) *
-                          num_bins_r_par).astype(int)
-    bins_r_trans = (r_trans / r_trans_max * num_bins_r_trans).astype(int)
-    bins = bins_r_trans + num_bins_r_trans * bins_r_par
-
-    rebin_weight = np.bincount(bins, weights=weights12)
-    rebin_r_par = np.bincount(bins, weights=r_par * weights12)
-    rebin_r_trans = np.bincount(bins, weights=r_trans * weights12)
-    rebin_z = np.bincount(bins, weights=z * weights12)
-    rebin_num_pairs = np.bincount(bins)
-
-    return rebin_weight, rebin_r_par, rebin_r_trans, rebin_z, rebin_num_pairs
-
-
-@jit(nopython=True)
+@njit
 def compute_xi_forest_pairs(z1, r_comov1, dist_m1, weights1, z2, r_comov2,
                             dist_m2, weights2, ang):
     """Computes the contribution of a given pair of forests to the correlation
     function.
 
     Args:
         z1: array of float
@@ -264,27 +198,27 @@
     rebin_r_trans = numba_bincount(bins, weights=r_trans * weights12)
     rebin_z = numba_bincount(bins, weights=z * weights12)
     rebin_num_pairs = numba_bincount_noweights(bins)
 
     return rebin_weight, rebin_r_par, rebin_r_trans, rebin_z, rebin_num_pairs
 
 
-@jit(nopython=True)
+@njit
 def numba_bincount_noweights(bins):
     if len(bins) == 0:
         return np.zeros(0, dtype=np.int64)
     maxbins = bins.max() + 1
     num_bins = len(bins)
     out = np.zeros(maxbins, dtype=np.int64)
     for ind in range(num_bins):
         out[bins[ind]] += 1
     return out
 
 
-@jit(nopython=True)
+@njit
 def numba_bincount(bins, weights):
     if len(bins) == 0:
         return np.zeros(0, dtype=weights.dtype)
     maxbins = bins.max() + 1
     num_bins = len(bins)
     out = np.zeros(maxbins, dtype=weights.dtype)
     for ind in range(num_bins):
```

### Comparing `picca-6.1.0/py/picca/constants.py` & `picca-7.0.0/py/picca/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             distances
 
         Raises:
             NotImplementedError: Function was not specified
         """
         raise NotImplementedError("Function should be specified at run-time")
 
-    def __init__(self,Om,Ok=0.,Or=0.,wl=-1.,H0=100.,blinding=False):
+    def __init__(self,Om,Ok=0.,Or=0.,wl=-1.,blinding=False):
         """Initializes the methods for this instance
 
         Args:
             Om: float - default: 0.3
                 Matter density
             Ok: float - default: 0.0
                 Curvature density
@@ -172,25 +172,31 @@
                 Radiation density
             wl: float - default: -1.0
                 Dark energy equation of state
             H0: float - default: 100.0
                 Hubble constant at redshift 0 (in km/s/Mpc)
         """
 
+        # WARNING: This is introduced due to historical issues in how this class
+        # is coded. Using H0=100 implies that we are returning the distances
+        # in Mpc/h instead of Mpc. This class should be fixed at some point to
+        # make what we are doing more clear.
+        H0 = 100.0
+
         # Blind data
         if blinding == "none":
             userprint("ATTENTION: Analysis is not blinded!")
         else:
             userprint(f"ATTENTION: Analysis is blinded with strategy {blinding}")
 
         if blinding not in  ["strategyB", "strategyBC"]:
-            userprint(f"Om={Om}, Or={Or}, wl={wl}, H0={H0}")
+            userprint(f"Om={Om}, Or={Or}, wl={wl}")
         else:
             userprint("The specified cosmology is "
-                      f"not used: Om={Om}, Or={Or}, wl={wl}, H0={H0}")
+                      f"not used: Om={Om}, Or={Or}, wl={wl}")
             # blind test small
             filename = "DR16_blind_test_small/DR16_blind_test_small.fits"
             # blind test large
             #filename = "DR16_blind_test_small/DR16_blind_test_large.fits"
             # load Om
             filename = resource_filename('picca', 'fitter2')+'/models/{}'.format(filename)
             hdu = fitsio.FITS(filename)
```

### Comparing `picca-6.1.0/py/picca/converters.py` & `picca-7.0.0/py/picca/converters.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/data.py` & `picca-7.0.0/py/picca/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1186,23 +1186,27 @@
         cont = None
 
         return cls(thingid, ra, dec, z_qso, plate, mjd, fiberid, log_lambda,
                    weights, cont, delta, order, ivar, exposures_diff, mean_snr,
                    mean_reso, mean_z, delta_log_lambda)
 
     @classmethod
-    def from_image(cls, hdul, pk1d_type=False):
+    def from_image(cls, hdul, pk1d_type=False, z_min_qso=0, z_max_qso=10):
         """Initialize instance from an ascii file.
 
         Args:
             hdu: fitsio.hdu.table.TableHDU
                 A Header Data Unit opened with fitsio
             pk1d_type: bool - default: False
                 Specifies if the fits file is formatted for the 1D Power
                 Spectrum analysis
+            z_min_qso: float - default: 0
+                Specifies the minimum redshift for QSOs
+            z_max_qso: float - default: 10
+                Specifies the maximum redshift for QSOs
         Returns:
             a Delta instance
         """
         if pk1d_type:
             raise ValueError("ImageHDU format not implemented for Pk1D forests.")
 
         header = hdul["METADATA"].read_header()
@@ -1267,27 +1271,28 @@
             weights_i, cont_i, delta_i, order_i, ivar_i, exposures_diff_i, mean_snr_i,
             mean_reso_i, mean_z_i, resolution_matrix_i,
             mean_resolution_matrix_i, mean_reso_pix_i, w_i
         ) in zip(los_id, ra, dec, z_qso, plate, mjd, fiberid, repeat(log_lambda),
                    weights, cont, delta, order, ivar, exposures_diff, mean_snr,
                    mean_reso, mean_z, resolution_matrix,
                    mean_resolution_matrix, mean_reso_pix, w):
-            deltas.append(cls(
-                los_id_i, ra_i, dec_i, z_qso_i, plate_i, mjd_i, fiberid_i, log_lambda[w_i],
-                weights_i[w_i] if weights_i is not None else None, 
-                cont_i[w_i], 
-                delta_i[w_i],
-                order_i, 
-                ivar_i[w_i] if ivar_i is not None else None,
-                exposures_diff_i[w_i] if exposures_diff_i is not None else None, 
-                mean_snr_i, mean_reso_i, mean_z_i,
-                resolution_matrix_i if resolution_matrix_i is not None else None,
-                mean_resolution_matrix_i if mean_resolution_matrix_i is not None else None,
-                mean_reso_pix_i,
-            ))
+            if z_qso_i >= z_min_qso and z_qso_i <= z_max_qso:        
+                deltas.append(cls(
+                    los_id_i, ra_i, dec_i, z_qso_i, plate_i, mjd_i, fiberid_i, log_lambda[w_i],
+                    weights_i[w_i] if weights_i is not None else None, 
+                    cont_i[w_i], 
+                    delta_i[w_i],
+                    order_i, 
+                    ivar_i[w_i] if ivar_i is not None else None,
+                    exposures_diff_i[w_i] if exposures_diff_i is not None else None, 
+                    mean_snr_i, mean_reso_i, mean_z_i,
+                    resolution_matrix_i if resolution_matrix_i is not None else None,
+                    mean_resolution_matrix_i if mean_resolution_matrix_i is not None else None,
+                    mean_reso_pix_i,
+                ))
 
         return deltas
 
     def project(self):
         """Project the delta field.
 
         The projection gets rid of the distortion caused by the continuum
@@ -1311,25 +1316,24 @@
                 np.sum(self.weights * meanless_log_lambda**2))
             res = mean_delta_log_lambda * meanless_log_lambda
         elif self.order == 1:
             res = self.delta
 
         self.delta -= mean_delta + res
 
-    def rebin(self, factor):
+    def rebin(self, factor, dwave=0.8):
         """Rebin deltas by an integer factor
 
         Args:
             factor: int
                 Factor to rebin deltas (new_bin_size = factor * old_bin_size)
+            dwave: float
+                Delta lambda of original deltas
         """
         wave = 10**np.array(self.log_lambda)
-        dwave = wave[1] - wave[0]
-        if not np.isclose(dwave, wave[-1] - wave[-2]):
-            raise ValueError('Delta rebinning only implemented for linear lambda bins')
 
         start = wave.min() - dwave / 2
         num_bins = np.ceil(((wave[-1] - wave[0]) / dwave + 1) / factor)
 
         edges = np.arange(num_bins) * dwave * factor + start
 
         new_indx = np.searchsorted(edges, wave)
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/astronomical_object.py` & `picca-7.0.0/py/picca/delta_extraction/astronomical_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,8 +184,8 @@
         method self.get_metadata
 
         Return
         ------
         metadata_units: list
         A list with the units of the line-of-sight data
         """
-        return ["", "DEGREES", "DEGREES", ""]
+        return ["", "rad", "rad", ""]
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py` & `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 class DesiForest(Forest):
     """Forest Object
 
     Class Methods
     -------------
     (see Forest in py/picca/delta_extraction/astronomical_objects/forest.py)
+    get_cont_units
     get_metadata_dtype
     get_metadata_units
 
     Methods
     -------
     (see Forest in py/picca/delta_extraction/astronomical_objects/forest.py)
     __init__
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py` & `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/astronomical_objects/forest.py` & `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/forest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import numpy as np
 from numba import njit
 from numba.types import bool_
 
 from picca.delta_extraction.astronomical_object import AstronomicalObject
 from picca.delta_extraction.errors import AstronomicalObjectError
-from picca.delta_extraction.utils import find_bins
+from picca.delta_extraction.utils import find_bins_lin, find_bins_log
 
 defaults = {
     "mask fields": [
         "flux",
         "ivar",
         "transmission_correction",
         "log_lambda",
@@ -54,15 +54,15 @@
     wslice_inner = np.zeros(bincounts.size, dtype=bool_)
     wslice_inner[first_nonzero_idx:last_nonzero_idx] = 1
 
     return wslice_inner
 
 @njit()
 def rebin(log_lambda, flux, ivar, transmission_correction, z, wave_solution,
-          log_lambda_grid, log_lambda_rest_frame_grid):
+          log_lambda_grid, log_lambda_rest_frame_grid, find_bins):
     """Rebin the arrays and update control variables
     Rebinned arrays are flux, ivar, lambda_ or log_lambda, and
     transmission_correction. Control variables are mean_snr
 
     Arguments
     ---------
     log_lambda: array of float
@@ -136,37 +136,32 @@
 
     # compute bins
     # Remove only out-of-bounds pixels
     if wave_solution == "log":
         pixel_step = log_lambda_grid[1] - log_lambda_grid[0]
         half_pixel_step = pixel_step / 2.
 
-        half_pixel_step_rest_frame = (log_lambda_rest_frame_grid[1] -
-                                      log_lambda_rest_frame_grid[0]) / 2.
-
         w1 &= log_lambda >= log_lambda_grid[0] - half_pixel_step
         w1 &= log_lambda < log_lambda_grid[-1] + half_pixel_step
         w1 &= (log_lambda - np.log10(1. + z) >=
-               log_lambda_rest_frame_grid[0] - half_pixel_step_rest_frame)
+               log_lambda_rest_frame_grid[0])
         w1 &= (log_lambda - np.log10(1. + z) <
-               log_lambda_rest_frame_grid[-1] + half_pixel_step_rest_frame)
+               log_lambda_rest_frame_grid[-1])
 
     elif wave_solution == "lin":
         pixel_step = 10**log_lambda_grid[1] - 10**log_lambda_grid[0]
         half_pixel_step = pixel_step / 2.
 
-        half_pixel_step_rest_frame = (10**log_lambda_rest_frame_grid[1] -
-                                      10**log_lambda_rest_frame_grid[0]) / 2.
         lambda_ = 10**log_lambda
         w1 &= (lambda_ >= 10**log_lambda_grid[0] - half_pixel_step)
         w1 &= (lambda_ < 10**log_lambda_grid[-1] + half_pixel_step)
         w1 &= (lambda_ / (1. + z) >=
-               10**log_lambda_rest_frame_grid[0] - half_pixel_step_rest_frame)
+               10**log_lambda_rest_frame_grid[0])
         w1 &= (lambda_ / (1. + z) <
-               10**log_lambda_rest_frame_grid[-1] + half_pixel_step_rest_frame)
+               10**log_lambda_rest_frame_grid[-1])
     else:
         raise AstronomicalObjectError("Error in Forest.rebin(). "
                                       "Class variable 'wave_solution' "
                                       "must be either 'lin' or 'log'.")
 
     if (w1 & (ivar > 0.)).sum() == 0:
         log_lambda = np.zeros(0)
@@ -183,15 +178,16 @@
 
     log_lambda = log_lambda[w1]
     flux = flux[w1]
     ivar = ivar[w1]
     transmission_correction = transmission_correction[w1]
     # Out-of-bounds pixels are removed. IVAR=0 pixels are kept
 
-    bins = find_bins(log_lambda, log_lambda_grid, wave_solution)
+
+    bins = find_bins(log_lambda, log_lambda_grid)
     binned_arr_size = bins.max() + 1
 
     # Find non-empty bins. There will be empty bins
     # at the lower end by construction.
     bincounts = np.bincount(bins, minlength=binned_arr_size)
     wslice_inner = get_inner_region_slice(bincounts)
     final_arr_size = np.sum(wslice_inner)
@@ -220,15 +216,15 @@
     # then rebin wavelength
     if wave_solution == "log":
         log_lambda = (log_lambda_grid[0] + pixel_step *
                     np.arange(binned_arr_size)[wslice_inner])
     else:  # we have already checked that it will always be "lin" at this point
         log_lambda = np.log10(10**log_lambda_grid[0] + pixel_step *
                     np.arange(binned_arr_size)[wslice_inner])
-    rebin_bins = find_bins(log_lambda, log_lambda_grid, wave_solution)
+    rebin_bins = find_bins(log_lambda, log_lambda_grid)
 
     # finally update control variables
     snr = flux * np.sqrt(ivar)
     mean_snr = np.mean(snr[w2])
 
     # return weights and binning solution to be used by child classes if
     # required
@@ -238,14 +234,15 @@
 class Forest(AstronomicalObject):
     """Forest Object
 
     Class Methods
     -------------
     (see AstronomicalObject in py/picca/delta_extraction/astronomical_objects/forest.py)
     class_variable_check
+    get_cont_units
     get_metadata_dtype
     get_metadata_units
     set_class_variables
 
     Methods
     -------
     (see AstronomicalObject in py/picca/delta_extraction/astronomical_object.py)
@@ -316,14 +313,16 @@
     transmission_correction: array of float
     Transmission correction.
 
     weights: array of float or None
     Weights associated to the delta field. None for no information
     """
     blinding = "none"
+    find_bins = None # this will store the correct find_bins function
+    flux_units = None
     log_lambda_grid = np.array([])  #None
     log_lambda_rest_frame_grid = np.array([])  #None
     log_lambda_index = np.array([]) #None
     mask_fields = []  #None
     wave_solution = None
 
     def __init__(self, **kwargs):
@@ -492,15 +491,15 @@
         names = []
         comments = []
         units = []
         if Forest.wave_solution == "log":
             cols += [self.log_lambda]
             names += ["LOGLAM"]
             comments += ["Log lambda"]
-            units += ["log Angstrom"]
+            units += ["log(Angstrom)"]
             array_size = self.log_lambda.size
         elif Forest.wave_solution == "lin":
             cols += [10**self.log_lambda]
             names += ["LAMBDA"]
             comments += ["Lambda"]
             units += ["Angstrom"]
             array_size = self.log_lambda.size
@@ -532,15 +531,15 @@
         if self.continuum is None:
             cols += [np.zeros(array_size, dtype=float)]
         else:
             cols += [self.continuum]
         names += ["CONT"]
         comments += ["Quasar continuum. Check input "
                      "spectra for units"]
-        units += ["Flux units"]
+        units += [Forest.flux_units]
 
         return cols, names, units, comments
 
     def get_header(self):
         """Return line-of-sight data to be saved as a fits file header
 
         Adds to specific Forest keys to general header (defined in class
@@ -671,24 +670,25 @@
         AstronomicalObjectError if Forest.wave_solution is not 'lin' or 'log'
         AstronomicalObjectError if ivar only has zeros
         """
         (self.log_lambda, self.flux, self.ivar, self.transmission_correction,
          self.mean_snr, bins, self.log_lambda_index, rebin_ivar, orig_ivar, w1,
          w2, wslice_inner) = rebin(self.log_lambda, self.flux, self.ivar,
                      self.transmission_correction, self.z, Forest.wave_solution,
-                     Forest.log_lambda_grid, Forest.log_lambda_rest_frame_grid)
+                     Forest.log_lambda_grid, Forest.log_lambda_rest_frame_grid,
+                     Forest.find_bins)
 
         # return weights and binning solution to be used by child classes if
         # required
         return rebin_ivar, orig_ivar, w1, w2, wslice_inner, bins
 
     @classmethod
     def set_class_variables(cls, lambda_min, lambda_max, lambda_min_rest_frame,
                             lambda_max_rest_frame, pixel_step,
-                            pixel_step_rest_frame, wave_solution):
+                            pixel_step_rest_frame, wave_solution, flux_units):
         """Set class variables
 
         Arguments
         ---------
         lambda_min: float
         Logarithm of the minimum wavelength (in Angs) to be considered in a forest.
 
@@ -705,30 +705,39 @@
         Wavelength cahnge between two pixels. If pixel_step is "log" this is in
         units of the logarithm of the wavelength (in Angs). If pixel_step is "lin"
         this is in units of the wavelength (in Angs).
 
         wave_solution: "log" or "lin"
         Specifies whether we want to construct a wavelength grid that is evenly
         spaced on wavelength (lin) or on the logarithm of the wavelength (log)
+
+        flux_units: str
+        Flux units
         """
         if wave_solution == "log":
             cls.log_lambda_grid = np.arange(
                 np.log10(lambda_min),
                 np.log10(lambda_max) + pixel_step / 2, pixel_step)
             cls.log_lambda_rest_frame_grid = np.arange(
-                np.log10(lambda_min_rest_frame) + pixel_step_rest_frame / 2,
-                np.log10(lambda_max_rest_frame), pixel_step_rest_frame)
+                np.log10(lambda_min_rest_frame),
+                np.log10(lambda_max_rest_frame) + pixel_step_rest_frame / 2,
+                pixel_step_rest_frame)
+            cls.find_bins = find_bins_log
         elif wave_solution == "lin":
             cls.log_lambda_grid = np.log10(
                 np.arange(lambda_min, lambda_max + pixel_step / 2, pixel_step))
             cls.log_lambda_rest_frame_grid = np.log10(
-                np.arange(lambda_min_rest_frame + pixel_step_rest_frame / 2,
-                          lambda_max_rest_frame, pixel_step_rest_frame))
+                np.arange(lambda_min_rest_frame,
+                          lambda_max_rest_frame + pixel_step_rest_frame / 2,
+                          pixel_step_rest_frame))
+            cls.find_bins = find_bins_lin
         else:
             raise AstronomicalObjectError("Error in setting Forest class "
                                           "variables. 'wave_solution' "
                                           "must be either 'lin' or 'log'. "
                                           f"Found: {wave_solution}")
 
         cls.wave_solution = wave_solution
 
         cls.mask_fields = defaults.get("mask fields").copy()
+
+        cls.flux_units = flux_units
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py` & `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         names += ["IVAR", "DIFF", "RESO", "RESO_PIX"]
         comments += [
             "Inverse variance. Check input spectra for units",
             "Difference. Check input spectra for units",
             "Resolution estimate (FWHM) for each pixel in units of km/s"
             "Resolution estimate (sigma) for each pixel in units of pixel size"
         ]
-        units += ["Flux units", "Flux units", "", ""]
+        units += [f"({Forest.flux_units})^-1", Forest.flux_units, "", ""]
 
         return cols, names, units, comments
 
     def get_header(self):
         """Return line-of-sight data to be saved as a fits file header
 
         Adds to specific Pk1dForest keys to general header (defined in class
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py` & `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 class SdssForest(Forest):
     """Forest Object
 
     Class Methods
     -------------
     (see Forest in py/picca/delta_extraction/astronomical_objects/forest.py)
+    get_cont_units
     get_metadata_dtype
     get_metadata_units
 
     Methods
     -------
     (see Forest in py/picca/delta_extraction/astronomical_objects/forest.py)
     __init__
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py` & `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/config.py` & `picca-7.0.0/py/picca/delta_extraction/config.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/correction.py` & `picca-7.0.0/py/picca/delta_extraction/correction.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/corrections/calibration_correction.py` & `picca-7.0.0/py/picca/delta_extraction/corrections/calibration_correction.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,40 +43,40 @@
         """
         filename = config.get("filename")
         if filename is None:
             raise CorrectionError(
                 "Missing argument 'filename' required by SdssCalibrationCorrection"
             )
         try:
-            hdu = fitsio.read(filename, ext="STACK_DELTAS")
-            if "loglam" in hdu.dtype.names:
-                stack_log_lambda = hdu['loglam']
+            hdu = fitsio.FITS(filename)["STACK_DELTAS"]
+            if "LOGLAM" in [name.upper() for name in hdu.get_colnames()]:
+                stack_log_lambda = hdu['LOGLAM'].read()
                 self.wave_solution = "log"
-            elif "lambda" in hdu.dtype.names:
-                stack_lambda = hdu['lambda']
+            elif "LAMBDA" in [name.upper() for name in hdu.get_colnames()]:
+                stack_lambda = hdu['LAMBDA'].read()
                 self.wave_solution = "lin"
             else:
                 raise CorrectionError("Error loading CalibrationCorrection. In "
                                       "extension 'STACK_DELTAS' in file "
-                                      f"{filename} one of the fields 'loglam' "
-                                      "or 'lambda' should be present. I did not"
+                                      f"{filename} one of the fields 'LOGLAM' "
+                                      "or 'LAMBDA' should be present. I did not "
                                       "find them.")
-            stack_delta = hdu['stack']
+            stack_delta = hdu['STACK'].read()
         except OSError as error:
             raise CorrectionError(
                 "Error loading CalibrationCorrection. "
                 f"Failed to find or open file {filename}"
             ) from error
         except ValueError as error:
             raise CorrectionError(
                 "Error loading CalibrationCorrection. "
                 f"File {filename} does not have fields "
                 "'loglam' and/or 'stack' in HDU 'STACK_DELTAS'"
             ) from error
-        w = (stack_delta != 0.)
+        w = stack_delta != 0.
         if self.wave_solution == "log":
             self.correct_flux = interp1d(stack_log_lambda[w],
                                          stack_delta[w],
                                          fill_value="extrapolate",
                                          kind="nearest")
         elif self.wave_solution == "lin":
             self.correct_flux = interp1d(stack_lambda[w],
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/corrections/dust_correction.py` & `picca-7.0.0/py/picca/delta_extraction/corrections/dust_correction.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/corrections/ivar_correction.py` & `picca-7.0.0/py/picca/delta_extraction/corrections/ivar_correction.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,29 +45,29 @@
         self.logger = logging.getLogger(__name__)
 
         filename = config.get("filename")
         if filename is None:
             raise CorrectionError("Missing argument 'filename' required by SdssIvarCorrection")
         try:
             hdu = fitsio.read(filename, ext="VAR_FUNC")
-            if "loglam" in hdu.dtype.names:
-                log_lambda = hdu['loglam']
-            elif "lambda" in hdu.dtype.names:
-                self.logger.warning("DeprecationWarning: Reading correction using 'lambda'. "
-                                    "Newer versions of picca always save 'log_lambda' and "
+            if "LOGLAM" in hdu.dtype.names:
+                log_lambda = hdu['LOGLAM']
+            elif "LAMBDA" in hdu.dtype.names:
+                self.logger.warning("DeprecationWarning: Reading correction using 'LAMBDA'. "
+                                    "Newer versions of picca always save 'LOGLAM' and "
                                     "so this option will be removed in the future.")
-                log_lambda = np.log10(hdu['lambda'])
+                log_lambda = np.log10(hdu['LAMBDA'])
             else:
                 raise CorrectionError("Error loading IvarCorrection. In "
                                       "extension 'VAR_FUNC' in file "
-                                      f"{filename} one of the fields 'loglam' "
-                                      "or 'lambda' should be present. I did not"
+                                      f"{filename} one of the fields 'LOGLAM' "
+                                      "or 'LAMBDA' should be present. I did not "
                                       "find them.")
 
-            eta = hdu['eta']
+            eta = hdu['ETA']
         except OSError as error:
             raise CorrectionError(
                 "Error loading CalibrationCorrection. "
                 f"Failed to find or open file {filename}"
             ) from error
         except ValueError as error:
             raise CorrectionError(
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/corrections/optical_depth_correction.py` & `picca-7.0.0/py/picca/delta_extraction/corrections/optical_depth_correction.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/data.py` & `picca-7.0.0/py/picca/delta_extraction/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,73 +75,126 @@
     forests: List of forests
     List of forests to later add to rejection log as accepted.
     """
     results = fitsio.FITS(f"{out_dir}/Delta/delta-{healpix}.fits.gz",
                           'rw',
                           clobber=True)
 
-    # Saving metadata card
-    metadata_header = {
-        "WAVE_SOLUTION": Forest.wave_solution,
-        "BLINDING": Forest.blinding,
-    }
+    results.write(None) # This works as Primary
 
+    hdr = fitsio.FITSHDR()
+    hdr.add_record({
+        "name": "BUNIT",
+        "value": "Angstrom",
+        "comment": "wavelength units",
+    })
+    hdr.add_record({
+        "name": "WAVE_SOLUTION",
+        "value": Forest.wave_solution,
+        "comment": "chosen wavelength solution",
+    })
     if Forest.wave_solution == "log":
-        metadata_header["DELTA_LOG_LAMBDA"] = Forest.log_lambda_grid[
-            1] - Forest.log_lambda_grid[0]
+        hdr.add_record({
+            "name": "DELTA_LOG_LAMBDA",
+            "value": round(Forest.log_lambda_grid[1] -
+                           Forest.log_lambda_grid[0],2),
+            "comment": "pixel step",
+        })
     elif Forest.wave_solution == "lin":
-        metadata_header["DELTA_LAMBDA"] = 10**Forest.log_lambda_grid[
-            1] - 10**Forest.log_lambda_grid[0]
+        hdr.add_record({
+            "name": "DELTA_LAMBDA",
+            "value": round(10**Forest.log_lambda_grid[1] -
+                        10**Forest.log_lambda_grid[0], 2),
+            "comment": "pixel step",
+        })
     else:
         raise DataError("Error in _save_deltas_one_healpix_image"
                         "Class variable 'wave_solution' "
                         "must be either 'lin' or 'log'. "
                         f"Found: '{Forest.wave_solution}'")
-
     results.write(
         10**Forest.log_lambda_grid,
         extname="LAMBDA",
+        header=hdr
     )
+    results["LAMBDA"].write_comment("Wavelength grid")
+    results["LAMBDA"].write_checksum()
 
+    hdr = fitsio.FITSHDR()
+    hdr.add_record({
+        "name": "BLINDING",
+        "value": Forest.blinding,
+        "comment": "blinding scheme used",
+    })
     results.write(
         np.array(
             [tuple(forest.get_metadata()) for forest in forests
             ],  # Structured arrays need to take tuples as input.
             dtype=forests[0].get_metadata_dtype(),
         ),
-        header=metadata_header,
+        header=hdr,
         #TODO: Figure out how to add comments.
         units=forests[0].get_metadata_units(),
         extname="METADATA")
+    results["METADATA"].write_comment("Per-forest metadata")
+    results["METADATA"].write_checksum()
 
     # Filling image information
     delta = np.full((len(forests), len(Forest.log_lambda_grid)), np.nan)
     for i, forest in enumerate(forests):
         delta[i][forest.log_lambda_index] = forest.deltas
 
+    hdr = fitsio.FITSHDR()
+    hdr.add_record({
+        "name": "BUNIT",
+        "value": "",
+        "comment": "delta units (unitless)",
+    })
+    delta_label = "DELTA" if Forest.blinding == "none" else "DELTA_BLIND"
     results.write(
-        delta, extname="DELTA" if Forest.blinding == "none" else "DELTA_BLIND")
+        delta,
+        header=hdr,
+        extname=delta_label)
+    results[delta_label].write_comment("Flux transmission field in " +
+                                       "wavelength bins")
+    results[delta_label].write_checksum()
 
     weight = np.full((len(forests), len(Forest.log_lambda_grid)), np.nan)
     for i, forest in enumerate(forests):
         weight[i][forest.log_lambda_index] = forest.weights
 
+    hdr = fitsio.FITSHDR()
+    hdr.add_record({
+        "name": "BUNIT",
+        "value": "",
+        "comment": "weight units (unitless)",
+    })
     results.write(
         weight,
         extname="WEIGHT",
     )
+    results["WEIGHT"].write_comment("Weights in wavelength bins")
+    results["WEIGHT"].write_checksum()
 
     continuum = np.full((len(forests), len(Forest.log_lambda_grid)), np.nan)
     for i, forest in enumerate(forests):
         continuum[i][forest.log_lambda_index] = forest.continuum
 
+    hdr = fitsio.FITSHDR()
+    hdr.add_record({
+        "name": "BUNIT",
+        "value": Forest.flux_units,
+        "comment": "flux units",
+    })
     results.write(
         continuum,
         extname="CONT",
     )
+    results["CONT"].write_comment("Quasar continuum in wavelength bins")
+    results["CONT"].write_checksum()
 
     return forests
 
 
 def _save_deltas_one_healpix_table(out_dir, healpix, forests):
     """Saves the deltas that belong to one healpix.
 
@@ -319,14 +372,18 @@
         # this should not be reached as wave_solution is either "lin" or "log"
         # added here only in case we add another wave_solution in the future
         else:  # pragma: no cover
             raise DataError(
                 "Unrecognised value for 'wave solution'. Expected either "
                 f"'lin' or 'log'. Found '{wave_solution}'.")
 
+        flux_units = config.get("flux units")
+        if flux_units is None:
+            raise DataError("Missing argument 'flux units' required by Data")
+
         lambda_max = config.getfloat("lambda max")
         if lambda_max is None:
             raise DataError("Missing argument 'lambda max' required by Data")
         lambda_max_rest_frame = config.getfloat("lambda max rest frame")
         if lambda_max_rest_frame is None:
             raise DataError(
                 "Missing argument 'lambda max rest frame' required by Data")
@@ -337,15 +394,15 @@
         if lambda_min_rest_frame is None:
             raise DataError(
                 "Missing argument 'lambda min rest frame' required by Data")
 
         Forest.set_class_variables(lambda_min, lambda_max,
                                    lambda_min_rest_frame, lambda_max_rest_frame,
                                    pixel_step, pixel_step_rest_frame,
-                                   wave_solution)
+                                   wave_solution, flux_units)
 
         # instance variables
         self.analysis_type = config.get("analysis type")
         if self.analysis_type is None:
             raise DataError("Missing argument 'analysis type' required by Data")
         if self.analysis_type not in accepted_analysis_type:
             raise DataError("Invalid argument 'analysis type' required by "
@@ -377,15 +434,15 @@
                 "required by Data")
 
         self.num_processors = config.getint("num processors")
         if self.num_processors is None:
             raise DataError(
                 "Missing argument 'num processors' required by Data")
         if self.num_processors == 0:
-            self.num_processors = (multiprocessing.cpu_count() // 2)
+            self.num_processors = multiprocessing.cpu_count() // 2
 
         self.out_dir = config.get("out dir")
         if self.out_dir is None:
             raise DataError("Missing argument 'out dir' required by Data")
 
         rejection_log_file = config.get("rejection log file")
         if rejection_log_file is None:
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/data_catalogues/desi_data.py` & `picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         Arguments
         ---------
         config: configparser.SectionProxy
         Parsed options to initialize class
         """
         self.logger = logging.getLogger(__name__)
 
+        config["flux units"] = "10**-17 erg/(s cm2 Angstrom)"
         super().__init__(config)
 
         # load variables from config
         self.unblind = None
         self.use_non_coadded_spectra = None
         self.__parse_config(config)
 
@@ -333,15 +334,15 @@
             # Fluxes from the different spectrographs will be coadded
             for spec in spectrographs_data.values():
                 if self.use_non_coadded_spectra:
                     ivar = np.atleast_2d(spec['IVAR'][w_t])
                     ivar_coadded_flux = np.atleast_2d(
                         ivar * spec['FLUX'][w_t]).sum(axis=0)
                     ivar = ivar.sum(axis=0)
-                    flux = (ivar_coadded_flux / ivar)
+                    flux = ivar_coadded_flux / ivar
                 else:
                     flux = spec['FLUX'][w_t].copy()
                     ivar = spec['IVAR'][w_t].copy()
 
                 args = {
                     "flux": flux,
                     "ivar": ivar,
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py` & `picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/data_catalogues/desi_tile.py` & `picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_tile.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py` & `picca-7.0.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/data_catalogues/sdss_data.py` & `picca-7.0.0/py/picca/delta_extraction/data_catalogues/sdss_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         """
         self.logger = logging.getLogger(__name__)
 
         # load variables from config
         self.mode = None
         self.__parse_config(config)
 
+        config["flux units"] = "10**-19 W/(m2 nm)"
         super().__init__(config)
 
         # load DRQ Catalogue
         catalogue = DrqCatalogue(config).catalogue
 
         # read data
         if self.mode == "spplate":
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/errors.py` & `picca-7.0.0/py/picca/delta_extraction/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,8 +60,8 @@
 class RejectionLogError(Exception):
     """
         Exceptions ocurred in class RejectionLog
     """
 
 
 if __name__ == '__main__':
-    raise Exception()
+    pass
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_flux.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,49 @@
 import fitsio
 import numpy as np
 from scipy.interpolate import interp1d
 
 from picca.delta_extraction.astronomical_objects.forest import Forest
 from picca.delta_extraction.astronomical_objects.pk1d_forest import Pk1dForest
 from picca.delta_extraction.errors import ExpectedFluxError, AstronomicalObjectError
-from picca.delta_extraction.utils import find_bins
 
 accepted_options = [
-    "iter out prefix", "num bins variance", "num processors", "out dir"
+    "iter out prefix", "num bins variance", "num processors", "out dir",
+    "var lss mod"
 ]
 
 defaults = {
     "iter out prefix": "delta_attributes",
     "num bins variance": 20,
     "num processors": 0,
+    "var lss mod": 1.0,
 }
 
 
 class ExpectedFlux:
     """Abstract class from which all classes computing the expected flux
     must inherit. Classes that inherit from this should be initialized using
     a configparser.SectionProxy instance.
 
     Methods
     -------
     __init__
+    _initialize_mean_continuum_arrays
+    _initialize_variance_wavelength_array
+    __parse_config
+    compute_delta_stack
     compute_expected_flux
+    compute_forest_weights
+    _compute_mean_cont
+    compute_forest_weights
     extract_deltas
+    hdu_cont
+    hdu_fit_metadata
+    hdu_var_func
+    save_iteration_step
 
     Attributes
     ----------
     los_ids: dict
     A dictionary to store the mean expected flux and the weights for each line
     of sight. Keys are the identifier for the line of sight and values are
     dictionaries with the keys "mean expected flux" (continuum times stack of
@@ -59,14 +71,15 @@
         """Initialize class instance"""
         self.los_ids = {}
 
         self.iter_out_prefix = None
         self.out_dir = None
         self.num_bins_variance = None
         self.num_processors = None
+        self.var_lss_mod = None
         self.__parse_config(config)
 
         # check that Forest class variables are set
         # these are required in order to initialize the arrays
         try:
             Forest.class_variable_check()
         except AstronomicalObjectError as error:
@@ -108,41 +121,29 @@
 
     def _initialize_variance_wavelength_array(self):
         """Initialize the wavelength array where variance functions will be
         computed
         The initialized arrays are:
         - self.log_lambda_var_func_grid
         """
-        # initialize the variance-related variables (see equation 4 of
-        # du Mas des Bourboux et al. 2020 for details on these variables)
         if Forest.wave_solution == "log":
-            self.log_lambda_var_func_grid = (
-                Forest.log_lambda_grid[0] +
-                (np.arange(self.num_bins_variance) + .5) *
-                (Forest.log_lambda_grid[-1] - Forest.log_lambda_grid[0]) /
+            self.log_lambda_var_func_grid = np.linspace(
+                Forest.log_lambda_grid[0],
+                Forest.log_lambda_grid[-1],
                 self.num_bins_variance)
-        # TODO: this is related with the todo in check the effect of finding
-        # the nearest bin in log_lambda space versus lambda space infunction
-        # find_bins in utils.py. Once we understand that we can remove
-        # the dependence from Forest from here too.
         elif Forest.wave_solution == "lin":
-            self.log_lambda_var_func_grid = np.log10(
-                10**Forest.log_lambda_grid[0] +
-                (np.arange(self.num_bins_variance) + .5) *
-                (10**Forest.log_lambda_grid[-1] -
-                 10**Forest.log_lambda_grid[0]) / self.num_bins_variance)
-
-        # TODO: Replace the if/else block above by something like the commented
-        # block below. We need to check the impact of doing this on the final
-        # deltas first (eta, var_lss and fudge will be differently sampled).
-        #start of commented block
-        #resize = len(Forest.log_lambda_grid)/self.num_bins_variance
-        #print(resize)
-        #self.log_lambda_var_func_grid = Forest.log_lambda_grid[::int(resize)]
-        #end of commented block
+            self.log_lambda_var_func_grid = np.log10(np.linspace(
+                10**Forest.log_lambda_grid[0],
+                10**Forest.log_lambda_grid[-1],
+                self.num_bins_variance))
+        else:
+            raise ExpectedFluxError("Error in setting Forest class "
+                                          "variables. 'wave_solution' "
+                                          "must be either 'lin' or 'log'. "
+                                          f"Found: {Forest.wave_solution}")
 
     def __parse_config(self, config):
         """Parse the configuration options
 
         Arguments
         ---------
         config: configparser.SectionProxy
@@ -169,22 +170,27 @@
                 "Missing argument 'num bins variance' required by ExpectedFlux")
 
         self.num_processors = config.getint("num processors")
         if self.num_processors is None:
             raise ExpectedFluxError(
                 "Missing argument 'num processors' required by ExpectedFlux")
         if self.num_processors == 0:
-            self.num_processors = (multiprocessing.cpu_count() // 2)
+            self.num_processors = multiprocessing.cpu_count() // 2
 
         self.out_dir = config.get("out dir")
         if self.out_dir is None:
             raise ExpectedFluxError(
                 "Missing argument 'out dir' required by ExpectedFlux")
         self.out_dir += "Log/"
 
+        self.var_lss_mod = config.getfloat("var lss mod")
+        if self.var_lss_mod is None:
+            raise ExpectedFluxError(
+                "Missing argument 'var lss mod' required by ExpectedFlux")
+
     def compute_delta_stack(self, forests, stack_from_deltas=False):
         """Compute a stack of the delta field as a function of wavelength
 
         Arguments
         ---------
         forests: List of Forest
         A list of Forest from which to compute the deltas.
@@ -203,18 +209,18 @@
                 # ignore forest if continuum could not be computed
                 if forest.continuum is None:
                     continue
 
                 delta = np.zeros_like(forest.log_lambda)
                 w = forest.ivar > 0
                 delta[w] = forest.flux[w] / forest.continuum[w]
-                weights = 1. / self.compute_forest_variance(forest, forest.continuum)
+                weights = self.compute_forest_weights(forest, forest.continuum)
 
-            bins = find_bins(forest.log_lambda, Forest.log_lambda_grid,
-                             Forest.wave_solution)
+            bins = Forest.find_bins( # pylint: disable=not-callable
+                forest.log_lambda, Forest.log_lambda_grid)
             stack_delta += np.bincount(bins, weights=delta * weights, minlength=stack_delta.size)
             stack_weight += np.bincount(bins, weights=weights, minlength=stack_delta.size)
 
         w = stack_weight > 0
         stack_delta[w] /= stack_weight[w]
 
         self.get_stack_delta = interp1d(
@@ -266,23 +272,28 @@
         # first compute <F/C> in bins. C=Cont_old*spectrum_dependent_fitting_fct
         # (and Cont_old is constant for all spectra in a bin), thus we actually
         # compute
         #    1/Cont_old * <F/spectrum_dependent_fitting_function>
         for forest in forests:
             if forest.bad_continuum_reason is not None:
                 continue
-            bins = find_bins(forest.log_lambda - np.log10(1 + forest.z),
-                             Forest.log_lambda_rest_frame_grid,
-                             Forest.wave_solution)
+            bins = Forest.find_bins( # pylint: disable=not-callable
+                forest.log_lambda - np.log10(1 + forest.z),
+                Forest.log_lambda_rest_frame_grid)
 
-            weights = 1. / self.compute_forest_variance(forest, forest.continuum)
+            weights = self.compute_forest_weights(forest, forest.continuum)
             forest_continuum = which_cont(forest)
-            mean_cont += np.bincount(bins, weights=forest_continuum * weights,
+            mean_cont += np.bincount(
+                bins,
+                weights=forest_continuum * weights,
+                minlength=mean_cont.size)
+            mean_cont_weight += np.bincount(
+                bins,
+                weights=weights,
                 minlength=mean_cont.size)
-            mean_cont_weight += np.bincount(bins, weights=weights, minlength=mean_cont.size)
 
         w = mean_cont_weight > 0
         mean_cont[w] /= mean_cont_weight[w]
         mean_cont /= mean_cont[w].mean()
         log_lambda_cont = Forest.log_lambda_rest_frame_grid[w]
 
         # the new mean continuum is multiplied by the previous one to recover
@@ -292,30 +303,30 @@
                                       new_cont,
                                       fill_value="extrapolate")
         self.get_mean_cont_weight = interp1d(log_lambda_cont,
                                              mean_cont_weight[w],
                                              fill_value=0.0,
                                              bounds_error=False)
 
-    def compute_forest_variance(self, forest, continuum):
-        """Compute the forest variance
+    def compute_forest_weights(self, forest, continuum):
+        """Compute the forest weights
 
         Arguments
         ---------
         forest: Forest
         A forest instance where the variance will be computed
 
         continuum: array of float
         Quasar continuum associated with the forest
 
         Raise
         -----
         MeanExpectedFluxError if function was not overloaded by child class
         """
-        raise ExpectedFluxError("Function 'compute_forest_variance' was not "
+        raise ExpectedFluxError("Function 'compute_forest_weights' was not "
                                 "overloaded by child class")
 
     def extract_deltas(self, forest):
         """Apply the continuum to compute the delta field
 
         Arguments
         ---------
@@ -346,16 +357,19 @@
         The open fits file
         """
         results.write([
             Forest.log_lambda_rest_frame_grid,
             self.get_mean_cont(Forest.log_lambda_rest_frame_grid),
             self.get_mean_cont_weight(Forest.log_lambda_rest_frame_grid),
         ],
-                      names=['loglam_rest', 'mean_cont', 'weight'],
+                      names=['LOGLAM_REST', 'MEAN_CONT', 'WEIGHT'],
+                      units=['log(Angstrom)', Forest.flux_units, ''],
                       extname='CONT')
+        results["CONT"].write_comment("Mean quasar continuum")
+        results["CONT"].write_checksum()
 
     def hdu_fit_metadata(self, results):
         """Add to the results file an HDU with the fits results
 
         This function is a placeholder here and should be overloaded by child
         classes if they require it
 
@@ -369,26 +383,33 @@
         """Add to the results file an HDU with the delta stack
 
         Arguments
         ---------
         results: fitsio.FITS
         The open fits file
         """
-        header = {}
+        header = fitsio.FITSHDR()
         if hasattr(self, 'order'):
-            header["FITORDER"] = self.order
+            header.add_record({
+                "name": "FITORDER",
+                "value": self.order,
+                "comment": "",
+            })
 
         results.write([
             Forest.log_lambda_grid,
             self.get_stack_delta(Forest.log_lambda_grid),
             self.get_stack_delta_weights(Forest.log_lambda_grid)
         ],
-                      names=['loglam', 'stack', 'weight'],
+                      names=['LOGLAM', 'STACK', 'WEIGHT'],
+                      units=['log(Angstrom)', '', ''],
                       header=header,
                       extname='STACK_DELTAS')
+        results['STACK_DELTAS'].write_comment("Delta mean properties")
+        results['STACK_DELTAS'].write_checksum()
 
     def hdu_var_func(self, results):
         """Add to the results file an HDU with the variance functions
 
         This function is a placeholder here and should be overloaded by child
         classes if they require it
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     _initialize_get_fudge
     _initialize_get_var_lss
     _initialize_mean_continuum_arrays
     _initialize_variance_wavelength_array
     _initialize_variance_functions
     __parse_config
     compute_delta_stack
-    compute_forest_variance
+    compute_forest_weights
     compute_mean_cont
     compute_expected_flux
     compute_var_stats
     get_continuum_weights
     hdu_cont
     hdu_stack_deltas
     hdu_var_func
@@ -458,36 +458,37 @@
             self.logger.progress(
                 f"Continuum fitting: ending iteration {iteration} of "
                 f"{self.num_iterations}")
 
         # now loop over forests to populate los_ids
         self.populate_los_ids(forests)
 
-    def compute_forest_variance(self, forest, continuum):
+    def compute_forest_weights(self, forest, continuum):
         """Compute the forest variance following du Mas des Bourboux 2020
 
         Arguments
         ---------
         forest: Forest
         A forest instance where the variance will be computed
 
         continuum: array of float
         Quasar continuum associated with the forest
         """
         w = forest.ivar > 0
-        variance = np.empty_like(forest.log_lambda)
-        variance[~w] = np.inf
+        weights = np.empty_like(forest.log_lambda)
+        weights[~w] = 0.0
 
         var_pipe = 1. / forest.ivar[w] / continuum[w]**2
         var_lss = self.get_var_lss(forest.log_lambda[w])
         eta = self.get_eta(forest.log_lambda[w])
         fudge = self.get_fudge(forest.log_lambda[w])
-        variance[w] = eta * var_pipe + var_lss + fudge / var_pipe
+        weights[w] = 1.0/(
+            eta * var_pipe + self.var_lss_mod*var_lss + fudge / var_pipe)
 
-        return variance
+        return weights
 
     # TODO: We should check if we can directly compute the mean continuum
     # in particular this means:
     # 1. check that we can use forest.continuum instead of
     #    forest.flux/forest.continuum right before `mean_cont[:len(cont)] += cont`
     # 2. check that in that case we don't need to use the new_cont
     # 3. check that this is not propagated elsewhere through self.get_mean_cont
@@ -644,62 +645,67 @@
                 cont_fit = self.continuum_fit_parameters.get(los_id)
                 los_id_list.append(los_id)
                 zero_point_list.append(cont_fit[0])
                 slope_list.append(cont_fit[1])
                 chi2_list.append(cont_fit[2])
                 ndata_list.append(cont_fit[3])
                 if any(np.isnan(cont_fit)):
-                    accepted_fit.append("no")
+                    accepted_fit.append(False)
                 else:
-                    accepted_fit.append("yes")
+                    accepted_fit.append(True)
             values = [
                 np.array(los_id_list),
                 np.array(zero_point_list),
                 np.array(slope_list),
                 np.array(chi2_list),
                 np.array(ndata_list, dtype=int),
                 np.array(accepted_fit),
             ]
             names = [
-                "los_id",
-                "zero_point",
-                "slope",
-                "chi2",
-                "num_datapoints",
-                "accepted_fit",
+                "LOS_ID",
+                "ZERO_POINT",
+                "SLOPE",
+                "CHI2",
+                "NUM_DATAPOINTS",
+                "ACCEPTED_FIT",
             ]
 
             results.write(values, names=names, extname='FIT_METADATA')
+            results["FIT_METADATA"].write_comment("Quasar continuum in wavelength bins")
+            results["FIT_METADATA"].write_checksum()
 
     def hdu_var_func(self, results):
         """Add to the results file an HDU with the variance functions
 
         Arguments
         ---------
         results: fitsio.FITS
         The open fits file
         """
         values = [
             self.log_lambda_var_func_grid,
             self.get_eta(self.log_lambda_var_func_grid),
             self.get_var_lss(self.log_lambda_var_func_grid),
             self.get_fudge(self.log_lambda_var_func_grid),
-            self.get_num_pixels(self.log_lambda_var_func_grid),
-            self.get_valid_fit(self.log_lambda_var_func_grid)
+            self.get_num_pixels(self.log_lambda_var_func_grid).astype(np.int32),
+            self.get_valid_fit(self.log_lambda_var_func_grid).astype(bool)
         ]
         names = [
-            "loglam",
-            "eta",
-            "var_lss",
-            "fudge",
-            "num_pixels",
-            "valid_fit",
+            "LOGLAM",
+            "ETA",
+            "VAR_LSS",
+            "FUDGE",
+            "NUM_PIXELS",
+            "VALID_FIT",
         ]
+        units = ["log(Angstrom)", "", "", "", "", ""]
 
-        results.write(values, names=names, extname='VAR_FUNC')
+        results.write(values, names=names, units=units, extname='VAR_FUNC')
+        results["VAR_FUNC"].write_comment("Variance fitted functions")
+        results["VAR_FUNC"].write_checksum()
 
     def populate_los_ids(self, forests):
         """Populate the dictionary los_ids with the mean expected flux, weights,
         and inverse variance arrays for each line-of-sight.
 
         Arguments
         ---------
@@ -714,15 +720,15 @@
             # mean_expected_flux points to forest.continuum and
             # forest.continuum gets modified within if statement
             mean_expected_flux = np.copy(forest.continuum)
             if self.force_stack_delta_to_zero:
                 stack_delta = self.get_stack_delta(forest.log_lambda)
                 mean_expected_flux *= stack_delta
 
-            weights = 1. / self.compute_forest_variance(forest, mean_expected_flux)
+            weights = self.compute_forest_weights(forest, mean_expected_flux)
 
             forest_info = {
                 "mean expected flux": mean_expected_flux,
                 "weights": weights,
                 "continuum": forest.continuum,
             }
             if isinstance(forest, Pk1dForest):
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,17 @@
         super().__init__(config)
 
     def _initialize_get_eta(self):
         """Initialiaze function get_eta"""
         # initialize eta factor
         if self.eta_value.endswith(".fits") or self.eta_value.endswith(
                 ".fits.gz"):
-            hdu = fitsio.read(self.eta_value, ext="VAR_FUNC")
-            self.get_eta = interp1d(hdu["loglam"],
-                                    hdu["eta"],
+            hdu = fitsio.FITS(self.eta_value)["VAR_FUNC"]
+            self.get_eta = interp1d(hdu["LOGLAM"].read(),
+                                    hdu["ETA"].read(),
                                     fill_value='extrapolate',
                                     kind='nearest')
         else:
             eta = np.ones(self.num_bins_variance) * float(self.eta_value)
             self.get_eta = interp1d(self.log_lambda_var_func_grid,
                                     eta,
                                     fill_value='extrapolate',
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 ],
                                            remove=True)
 
 defaults = update_default_options(defaults, defaults2)
 defaults = update_default_options(defaults, defaults3)
 defaults = update_default_options(defaults, {
     "num iterations": 1,
-})
+},
+                                  force_overwrite=True)
+
 
 
 class Dr16FixedEtaVarlssFudgeExpectedFlux(Dr16FixedEtaExpectedFlux,
                                           Dr16FixedVarlssExpectedFlux,
                                           Dr16FixedFudgeExpectedFlux):
     """Class to the expected flux similar to Dr16ExpectedFlux but fixing
     eta, var_lss and fudge
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,17 @@
         super().__init__(config)
 
     def _initialize_get_fudge(self):
         """Initialiaze function get_fudge"""
         # initialize fudge factor
         if self.fudge_value.endswith(".fits") or self.fudge_value.endswith(
                 ".fits.gz"):
-            hdu = fitsio.read(self.fudge_value, ext="VAR_FUNC")
-            self.get_fudge = interp1d(hdu["loglam"],
-                                      hdu["fudge"],
+            hdu = fitsio.FITS(self.fudge_value)["VAR_FUNC"]
+            self.get_fudge = interp1d(hdu["LOGLAM"].read(),
+                                      hdu["FUDGE"].read(),
                                       fill_value='extrapolate',
                                       kind='nearest')
         else:
             fudge = np.ones(self.num_bins_variance) * float(self.fudge_value)
             self.get_fudge = interp1d(self.log_lambda_var_func_grid,
                                       fudge,
                                       fill_value='extrapolate',
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,17 @@
         super().__init__(config)
 
     def _initialize_get_var_lss(self):
         """Initialiaze function get_var_lss"""
         # initialize fudge factor
         if self.var_lss_value.endswith(".fits") or self.var_lss_value.endswith(
                 ".fits.gz"):
-            hdu = fitsio.read(self.var_lss_value, ext="VAR_FUNC")
-            self.get_var_lss = interp1d(hdu["loglam"],
-                                        hdu["var_lss"],
+            hdu = fitsio.FITS(self.var_lss_value)["VAR_FUNC"]
+            self.get_var_lss = interp1d(hdu["LOGLAM"].read(),
+                                        hdu["VAR_LSS"].read(),
                                         fill_value='extrapolate',
                                         kind='nearest')
         else:
             var_lss = np.ones(self.num_bins_variance) * float(
                 self.var_lss_value)
             self.get_var_lss = interp1d(self.log_lambda_var_func_grid,
                                         var_lss,
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,29 @@
 import healpy
 from pkg_resources import resource_filename
 
 from picca.delta_extraction.astronomical_objects.forest import Forest
 from picca.delta_extraction.astronomical_objects.pk1d_forest import Pk1dForest
 from picca.delta_extraction.errors import ExpectedFluxError
 from picca.delta_extraction.expected_flux import ExpectedFlux, defaults, accepted_options
-from picca.delta_extraction.utils import (find_bins, update_accepted_options,
+from picca.delta_extraction.utils import (update_accepted_options,
                                           update_default_options)
 
 accepted_options = update_accepted_options(accepted_options, [
-    "input directory", "raw statistics file", "use constant weight",
-    "num bins variance", "force stack delta to zero"
+    "input directory", "raw statistics file", "recompute var lss",
+    "use splines", "use constant weight","num bins variance",
+    "force stack delta to zero"
 ])
 
 defaults = update_default_options(defaults, {
     "raw statistics file": "",
     "use constant weight": False,
-    "force stack delta to zero": False
+    "force stack delta to zero": False,
+    "use splines": False,
+    "recompute var lss": True
 })
 
 IN_NSIDE = 16
 
 
 class TrueContinuum(ExpectedFlux):
     """Class to compute the expected flux using the true unabsorbed contiuum
@@ -116,17 +119,42 @@
         self.input_directory = config.get("input directory")
         if self.input_directory is None:
             raise ExpectedFluxError(
                 "Missing argument 'input directory' required "
                 "by TrueContinuum")
 
         self.use_constant_weight = config.getboolean("use constant weight")
+        if self.use_constant_weight is None:
+            raise ExpectedFluxError(
+                "Missing argument 'use constant weight' required "
+                "by TrueContinuum")
+
         self.raw_statistics_filename = config.get("raw statistics file")
+        if self.raw_statistics_filename is None:
+            raise ExpectedFluxError(
+                "Missing argument 'raw statistics filename' required "
+                "by TrueContinuum")
 
         self.force_stack_delta_to_zero = config.getboolean("force stack delta to zero")
+        if self.force_stack_delta_to_zero is None:
+            raise ExpectedFluxError(
+                "Missing argument 'force stack delta to zero' required "
+                "by TrueContinuum")
+
+        self.use_splines = config.getboolean("use splines")
+        if self.use_splines is None:
+            raise ExpectedFluxError(
+                "Missing argument 'use splines' required "
+                "by TrueContinuum")
+
+        self.recompute_varlss = config.getboolean("recompute var lss")
+        if self.recompute_varlss is None:
+            raise ExpectedFluxError(
+                "Missing argument 'recompute var lss' required "
+                "by TrueContinuum")
 
     def compute_expected_flux(self, forests):
         """
 
         Arguments
         ---------
         forests: List of Forest
@@ -137,18 +165,19 @@
         ExpectedFluxError if Forest.wave_solution is not 'lin' or 'log'
         """
         forests = self.read_all_true_continua(forests)
 
         # the might be some small changes in the var_lss compared to the read
         # values due to some smoothing of the forests
         # thus, we recompute it from the actual deltas
-        self.compute_var_lss(forests)
-        # note that this does not change the output deltas but might slightly
-        # affect the mean continuum so we have to compute it after updating
-        # var_lss
+        if self.recompute_varlss:
+            self.compute_var_lss(forests)
+            # note that this does not change the output deltas but might slightly
+            # affect the mean continuum so we have to compute it after updating
+            # var_lss
         self.compute_mean_cont(forests)
 
         self.compute_delta_stack(forests)
 
         self.save_iteration_step(iteration=-1)
 
         # now loop over forests to populate los_ids
@@ -162,56 +191,59 @@
         ---------
         forests: List of Forest
         A list of Forest from which to compute the deltas.
         """
 
         return super()._compute_mean_cont(forests)
 
-    def compute_forest_variance(self, forest, continuum):
+    def compute_forest_weights(self, forest, continuum):
         """Compute the forest variance
 
         Arguments
         ---------
         forest: Forest
         A forest instance where the variance will be computed
 
         continuum: array of float
         Quasar continuum associated with the forest
         """
         w = forest.ivar > 0
-        variance = np.empty_like(forest.log_lambda)
-        variance[~w] = np.inf
+        weights = np.empty_like(forest.log_lambda)
+        weights[~w] = 0.0
 
         if self.use_constant_weight:
-            variance[w] = 1
+            weights[w] = 1
         else:
             var_lss = self.get_var_lss(forest.log_lambda[w])
             ivar_pipe = forest.ivar * forest.continuum**2
-            variance[w] = var_lss + 1/ivar_pipe[w]
+            weights[w] = 1.0/(self.var_lss_mod * var_lss + 1/ivar_pipe[w])
 
-        return variance
+        return weights
 
     def hdu_var_func(self, results):
         """Add to the results file an HDU with the variance functions
 
         Arguments
         ---------
         results: fitsio.FITS
         The open fits file
         """
         values = [
             self.log_lambda_var_func_grid,
             self.get_var_lss(self.log_lambda_var_func_grid),
         ]
         names = [
-            "loglam",
-            "var_lss",
+            "LOGLAM",
+            "VAR_LSS",
         ]
+        units = ["log(Angstrom)", ""]
 
-        results.write(values, names=names, extname='VAR_FUNC')
+        results.write(values, names=names, units=units, extname='VAR_FUNC')
+        results["VAR_FUNC"].write_comment("Variance fitted functions")
+        results["VAR_FUNC"].write_checksum()
 
     def populate_los_ids(self, forests):
         """Populate the dictionary los_ids with the mean expected flux, weights,
         and inverse variance arrays for each line-of-sight.
 
         Arguments
         ---------
@@ -225,15 +257,15 @@
             # get the variance functions
             if self.use_constant_weight:
                 w = forest.ivar>0
                 weights = np.empty_like(forest.log_lambda)
                 weights[w] = 1
                 weights[~w] = 0
             else:
-                weights = 1. / self.compute_forest_variance(
+                weights = self.compute_forest_weights(
                     forest, forest.continuum)
 
             mean_expected_flux = np.copy(forest.continuum)
             if self.force_stack_delta_to_zero:
                 stack_delta = self.get_stack_delta(forest.log_lambda)
                 mean_expected_flux *= stack_delta
 
@@ -389,14 +421,17 @@
         header = hdul[1].read_header()
         fits_data = hdul[1].read()
         hdul.close()
         is_rawfile_consistent = True
         err_msg = ("raw statistics file pixelization scheme does not match "
                    "input pixelization scheme.\n")
 
+        pixel_step = None
+        pixel_step_key = None
+        log_lambda = None
         if Forest.wave_solution == "log":
             pixel_step = Forest.log_lambda_grid[1] - Forest.log_lambda_grid[0]
             pixel_step_key = 'DEL_LL'
             log_lambda = fits_data['LAMBDA']
 
             if header['LINEAR']:
                 is_rawfile_consistent = False
@@ -443,16 +478,20 @@
               - 10**Forest.log_lambda_rest_frame_grid[-2])/2
         is_rawfile_consistent, err_msg = _check_header_consistency(
             'LR_MAX', lambda_rest_max, atol, is_rawfile_consistent, err_msg)
 
         if not is_rawfile_consistent:
             raise ExpectedFluxError(err_msg)
 
-        flux_variance = fits_data['VAR']
-        mean_flux = fits_data['MEANFLUX']
+        if self.use_splines:
+            flux_variance = fits_data['VAR_SPLINE']
+            mean_flux = fits_data['MEANFLUX_SPLINE']
+        else:
+            flux_variance = fits_data['VAR']
+            mean_flux = fits_data['MEANFLUX']
 
         var_lss = flux_variance / mean_flux**2
 
         self.get_var_lss = interp1d(log_lambda,
                                     var_lss,
                                     fill_value='extrapolate',
                                     kind='nearest')
@@ -471,17 +510,17 @@
         forests: List of Forest
         A list of Forest from which to compute the deltas."""
         var_lss = np.zeros_like(Forest.log_lambda_grid)
         counts = np.zeros_like(Forest.log_lambda_grid)
 
         for forest in forests:
             w = forest.ivar > 0
-            log_lambda_bins = find_bins(forest.log_lambda,
-                                        Forest.log_lambda_grid,
-                                        Forest.wave_solution)[w]
+            log_lambda_bins = Forest.find_bins( # pylint: disable=not-callable
+                forest.log_lambda,
+                Forest.log_lambda_grid)[w]
             var_pipe = 1. / forest.ivar[w] / forest.continuum[w]**2
             deltas = forest.flux[w] / forest.continuum[w] - 1
             var_lss[log_lambda_bins] += deltas**2 - var_pipe
             counts[log_lambda_bins] += 1
 
         w = counts > 0
         var_lss[w] /= counts[w]
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/expected_fluxes/utils.py` & `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/utils.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py` & `picca-7.0.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py` & `picca-7.0.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """This module defines the class LeastsSquaresVarStats"""
 import numpy as np
 
 from picca.delta_extraction.astronomical_objects.forest import Forest
-from picca.delta_extraction.utils import find_bins
 
 VAR_PIPE_MIN = np.log10(1e-5)
 VAR_PIPE_MAX = np.log10(2.)
 NUM_VAR_BINS = 100
 
 FUDGE_REF = 1e-7
 
@@ -157,22 +156,22 @@
             var_pipe[w]  = 1 / forest.ivar[w] / forest.continuum[w]**2
             var_pipe[~w] = np.inf
 
             w &= ((np.log10(var_pipe) > VAR_PIPE_MIN) &
                  (np.log10(var_pipe) < VAR_PIPE_MAX))
 
             # select the pipeline variance bins
-            var_pipe_bins = np.floor(
+            var_pipe_bins = (
                 (np.log10(var_pipe[w]) - VAR_PIPE_MIN) /
                 (VAR_PIPE_MAX - VAR_PIPE_MIN) * NUM_VAR_BINS).astype(int)
 
             # select the wavelength bins
-            log_lambda_bins = find_bins(forest.log_lambda[w],
-                                        self.log_lambda_var_func_grid,
-                                        Forest.wave_solution)
+            log_lambda_bins = Forest.find_bins( # pylint: disable=not-callable
+                forest.log_lambda[w],
+                self.log_lambda_var_func_grid)
 
             # compute overall bin
             bins = var_pipe_bins + NUM_VAR_BINS * log_lambda_bins
 
             # compute deltas
             delta = forest.flux[w] / forest.continuum[w] - 1
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/mask.py` & `picca-7.0.0/py/picca/delta_extraction/mask.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,22 @@
     else:
         setattr(forest, param, getattr(forest, param)[w])
 
 def _set_ivar_to_zero(forest, param, w):
     if param == 'ivar':
         forest.ivar[~w] = 0
 
+accepted_options = ["keep pixels"]
+
+defaults = {
+    "keep pixels": False,
+}
+
+
+
 class Mask:
     """Abstract class from which all Masks must inherit.
     Classes that inherit from this should be initialized using
     a configparser.SectionProxy instance.
 
     Arguments
     ---------
@@ -37,15 +45,19 @@
     If keep_masked_pixels=True, then points to _set_ivar_to_zero.
     Otherwise, points to _remove_pixels.
     """
     def __init__(self, config):
         """Initialize class instance"""
         self.los_id = {}
 
-        keep_masked_pixels = config.getboolean("keep pixels", fallback=False)
+        keep_masked_pixels = config.getboolean("keep pixels")
+        if keep_masked_pixels is None:
+            raise MaskError(
+                "Missing argument 'keep pixels' required "
+                "by Mask")
 
         if keep_masked_pixels:
             self._masker = _set_ivar_to_zero
         else:
             self._masker = _remove_pixels
 
     def apply_mask(self, forest):
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/masks/absorber_mask.py` & `picca-7.0.0/py/picca/delta_extraction/masks/absorber_mask.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,27 @@
 import logging
 
 import fitsio
 import numpy as np
 
 from picca.delta_extraction.astronomical_objects.forest import Forest
 from picca.delta_extraction.errors import MaskError
-from picca.delta_extraction.mask import Mask
-
-defaults = {
-    "absorber mask width": 2.5,
-    "los_id name": "THING_ID",
-}
-
-accepted_options = ["absorber mask width", "filename", "keep pixels", "los_id name"]
+from picca.delta_extraction.mask import Mask, accepted_options, defaults
+from picca.delta_extraction.utils import (update_accepted_options,
+                                          update_default_options)
+
+accepted_options = update_accepted_options(accepted_options, [
+    "absorber mask width", "filename", "los_id name",
+])
+
+defaults = update_default_options(
+    defaults, {
+        "absorber mask width": 2.5,
+        "los_id name": "THING_ID",
+    })
 
 class AbsorberMask(Mask):
     """Class to mask Absorbers
 
     Methods
     -------
     __init__
@@ -75,15 +80,15 @@
                 f"Error loading AbsorberMask. File {filename} does not have "
                 f"fields '{aux}' in HDU 'ABSORBERCAT'"
             ) from error
 
         # group absorbers on the same line of sight together
         self.los_ids = {}
         for los_id in np.unique(cat[los_id_name]):
-            w = (los_id == cat[los_id_name])
+            w = los_id == cat[los_id_name]
             self.los_ids[los_id] = list(cat[los_id_name][w])
         num_absorbers = np.sum(
             [len(los_id) for los_id in self.los_ids.values()])
 
         self.logger.progress(f" In catalog: {num_absorbers} absorbers")
         self.logger.progress(f" In catalog: {len(self.los_ids)} forests have "
                              "absorbers\n")
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/masks/bal_mask.py` & `picca-7.0.0/py/picca/delta_extraction/masks/bal_mask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """This module defines the classes BalMask and Dla used in the
 masking of DLAs"""
 import logging
 
 import fitsio
 import numpy as np
+from numba import njit
 
 from picca.delta_extraction.astronomical_objects.forest import Forest
 from picca.delta_extraction.errors import MaskError
-from picca.delta_extraction.mask import Mask
-from picca.delta_extraction.utils import SPEED_LIGHT
-
-defaults = {
-    "bal index type": "ai",
-    "los_id name": "THING_ID",
-}
-
-accepted_options = ["bal index type", "filename", "los_id name", "keep pixels"]
+from picca.delta_extraction.mask import Mask, accepted_options, defaults
+from picca.delta_extraction.utils import (
+    SPEED_LIGHT, update_accepted_options, update_default_options)
+
+accepted_options = update_accepted_options(accepted_options, [
+    "bal index type", "filename", "los_id name", "keep pixels"
+])
+
+defaults = update_default_options(
+    defaults, {
+        "bal index type": "ai",
+        "los_id name": "THING_ID",
+    })
 
 # Wavelengths in Angstroms
-lines = np.array([
+LINES = np.array([
     ("lCIV", 1549),
     ("lSiIV1", 1394),
     ("lSiIV2", 1403),
     ("lNV", 1240.81),
     ("lLya", 1216.1),
     ("lCIII", 1175),
     ("lPV1", 1117),
@@ -31,14 +36,63 @@
     ("lSIV2", 1074),
     ("lLyb", 1020),
     ("lOIV", 1031),
     ("lOVI", 1037),
     ("lOI", 1039),
     ], dtype=[("name", "U10"), ("value", float)])
 
+@njit()
+def add_bal_rest_frame(los_id, los_id_array, min_velocities_array, max_velocities_array):
+    """Creates a list of wavelengths to be masked out by forest.mask
+
+    Arguments
+    ---------
+    los_id: str
+    Line-of-sight id
+
+    los_id_name: str
+    Name of the line-of-sight id
+
+    Return
+    ------
+    log_lambda_min: array of float
+    Array with the minimum log(wavelength) values in the masks intervals
+
+    log_lambda_max: array of float
+    Array with the maximum log(wavelength) values in the masks intervals
+    """
+    # Match thing_id of object to BAL catalog index
+    # Will there be duplicates or only one index?
+    match_index = np.where(los_id_array == los_id)[0]
+
+    # Store the min/max velocity pairs from the BAL catalog
+    min_velocities = min_velocities_array[match_index].ravel()
+    max_velocities = max_velocities_array[match_index].ravel()
+
+    # Remove non-positive velocity rows
+    w = (min_velocities > 0) & (max_velocities > 0)
+    min_velocities = min_velocities[w]
+    max_velocities = max_velocities[w]
+
+    num_velocities = min_velocities.size
+    if num_velocities == 0:
+        return np.zeros(0), np.zeros(0)
+
+    # Calculate mask width for each velocity pair, for each emission line
+    # This might be  bit confusing, since BAL absorption is
+    # blueshifted from the emission lines. The “minimum velocity”
+    # corresponds to the red side of the BAL absorption (the larger
+    # wavelength value), and the “maximum velocity” corresponds to
+    # the blue side (the smaller wavelength value).
+    lambda_max = np.outer(LINES['value'], 1 - min_velocities / SPEED_LIGHT).ravel()
+    lambda_min = np.outer(LINES['value'], 1 - max_velocities / SPEED_LIGHT).ravel()
+    log_lambda_min = np.log10(lambda_min)
+    log_lambda_max = np.log10(lambda_max)
+
+    return log_lambda_min, log_lambda_max
 
 class BalMask(Mask):
     """Class to mask BALs
 
     Methods
     -------
     __init__
@@ -105,17 +159,18 @@
             raise MaskError(
                 "Unrecognized los_id name. Expected one of 'THING_ID' "
                 f" or 'TARGETID'. Found {los_id_name}")
 
         # setup bal index limit
         self.bal_index_type = config.get("bal index type")
         if self.bal_index_type is None:
-            self.bal_index_type = MaskError(
+            raise MaskError(
                 "Missing argument 'bal index type' "
                 "required by BalMask")
+        columns_list = None
         if self.bal_index_type == "ai":
             columns_list = [los_id_name, 'VMIN_CIV_450', 'VMAX_CIV_450']
         elif self.bal_index_type == "bi":
             columns_list = [los_id_name, 'VMIN_CIV_2000', 'VMAX_CIV_2000']
         else:
             self.bal_index_type = MaskError(
                 "In BalMask, unrecognized value "
@@ -125,15 +180,19 @@
 
         self.velocity_list = columns_list[1:]
 
         self.logger.progress(f"Reading BAL catalog from: {filename}")
 
         try:
             hdul = fitsio.FITS(filename)
-            self.cat = {col: hdul[ext_name][col][:] for col in columns_list}
+            self.cat = {
+                col: (hdul[ext_name][col][:].astype(np.int64)
+                    if col == los_id_name else
+                    hdul[ext_name][col][:].astype(np.float64))
+                for col in columns_list}
         except OSError as error:
             raise MaskError(
                 f"Error loading BalMask. File {filename} does "
                 f"not have extension '{ext_name}'"
             ) from error
         except ValueError as error:
             aux = "', '".join(columns_list)
@@ -141,96 +200,54 @@
                 f"Error loading BalMask. File {filename} does "
                 f"not have fields '{aux}' in HDU '{ext_name}'"
             ) from error
         finally:
             hdul.close()
 
         # compute info for each line of sight
-        self.los_ids = {}
-        for los_id in np.unique(self.cat[los_id_name]):
-            self.los_ids[los_id] = self.add_bal_rest_frame(los_id, los_id_name)
+        self.los_ids = {
+            los_id: (
+                los_id,
+                self.cat[los_id_name],
+                self.cat[self.velocity_list[0]],
+                self.cat[self.velocity_list[1]])
+            for los_id in np.unique(self.cat[los_id_name])
+        }
 
-        num_bals = np.sum([len(los_id) for los_id in self.los_ids.values()
-                          if los_id is not None])
+        num_bals = len(self.los_ids)
         self.logger.progress(f'In catalog: {num_bals} BAL quasars')
 
-    def add_bal_rest_frame(self, los_id, los_id_name):
-        """Creates a list of wavelengths to be masked out by forest.mask
-
-        Arguments
-        ---------
-        los_id: str
-        Line-of-sight id
-
-        los_id_name: str
-        Name of the line-of-sight id
-        """
-        # Match thing_id of object to BAL catalog index
-        # Will there be duplicates or only one index?
-        match_index = np.where(self.cat[los_id_name] == los_id)[0]
-
-        # Store the min/max velocity pairs from the BAL catalog
-        colmin = self.cat[self.velocity_list[0]]
-        colmax = self.cat[self.velocity_list[1]]
-        # np.array of minimum velocities
-        min_velocities = np.array(colmin[match_index], dtype=float)
-        # np.array of maximum velocities
-        max_velocities = np.array(colmax[match_index], dtype=float)
-        # Remove non-positive velocity rows
-        w = (min_velocities>0) & (max_velocities>0)
-        min_velocities = min_velocities[w]
-        max_velocities = max_velocities[w]
-
-        num_velocities = min_velocities.size
-        if num_velocities == 0:
-            return None
-
-        num_lines = lines.size
-        mask_rest_frame_bal = np.empty(num_velocities * num_lines,
-            dtype=[('log_lambda_min', 'f8'), ('log_lambda_max', 'f8'),
-            ('lambda_min', 'f8'), ('lambda_max', 'f8')])
-
-        # Calculate mask width for each velocity pair, for each emission line
-        # This might be  bit confusing, since BAL absorption is
-        # blueshifted from the emission lines. The “minimum velocity”
-        # corresponds to the red side of the BAL absorption (the larger
-        # wavelength value), and the “maximum velocity” corresponds to
-        # the blue side (the smaller wavelength value).
-        lambda_max = np.outer(lines['value'], 1 - min_velocities / SPEED_LIGHT).ravel()
-        lambda_min = np.outer(lines['value'], 1 - max_velocities / SPEED_LIGHT).ravel()
-        mask_rest_frame_bal['lambda_min'] = lambda_min
-        mask_rest_frame_bal['lambda_max'] = lambda_max
-        mask_rest_frame_bal['log_lambda_min'] = np.log10(lambda_min)
-        mask_rest_frame_bal['log_lambda_max'] = np.log10(lambda_max)
-
-        return mask_rest_frame_bal
-
     def apply_mask(self, forest):
         """Apply the mask. The mask is done by removing the affected
         pixels from the arrays in Forest.mask_fields
 
         Arguments
         ---------
         forest: Forest
         A Forest instance to which the correction is applied
 
         Raise
         -----
         MaskError if Forest.wave_solution is not 'log'
         """
-        mask_table = self.los_ids.get(forest.los_id)
+        if self.los_ids.get(forest.los_id) is None:
+            return
+
+        log_lambda_min, log_lambda_max = add_bal_rest_frame(
+            *self.los_ids.get(forest.los_id))
 
-        if (mask_table is None) or len(mask_table) == 0:
+        if len(log_lambda_min) == 0:
             return
 
         # find out which pixels to mask
         w = np.ones(forest.log_lambda.size, dtype=bool)
         rest_frame_log_lambda = forest.log_lambda - np.log10(1. + forest.z)
-        mask_idx_ranges = np.searchsorted(rest_frame_log_lambda,
-                [mask_table['log_lambda_min'], mask_table['log_lambda_max']]).T
+        mask_idx_ranges = np.searchsorted(
+            rest_frame_log_lambda,
+            [log_lambda_min, log_lambda_max]).T
         # Make sure first index comes before the second
         mask_idx_ranges.sort(axis=1)
 
         for idx1, idx2 in mask_idx_ranges:
             w[idx1:idx2] = 0
 
         # do the actual masking
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/masks/dla_mask.py` & `picca-7.0.0/py/picca/delta_extraction/masks/dla_mask.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,167 @@
 """This module defines the classes DlaMask and Dla used in the
 masking of DLAs"""
 import logging
 
 from astropy.table import Table
 import fitsio
 import numpy as np
+from numba import njit
 
 from picca.delta_extraction.astronomical_objects.forest import Forest
 from picca.delta_extraction.errors import MaskError
-from picca.delta_extraction.mask import Mask
-from picca.delta_extraction.utils import ABSORBER_IGM
-
-defaults = {
-    "dla mask limit": 0.8,
-    "los_id name": "THING_ID",
-}
-
-accepted_options = ["dla mask limit", "los_id name", "mask file", "filename", "keep pixels"]
+from picca.delta_extraction.mask import Mask, accepted_options, defaults
+from picca.delta_extraction.utils import (
+    ABSORBER_IGM, update_accepted_options, update_default_options)
+
+accepted_options = update_accepted_options(accepted_options, [
+    "dla mask limit", "los_id name", "mask file", "filename"
+])
+
+defaults = update_default_options(
+    defaults, {
+        "dla mask limit": 0.8,
+        "los_id name": "THING_ID",
+    })
 
 np.random.seed(0)
 NUM_POINTS = 10000
 GAUSSIAN_DIST = np.random.normal(size=NUM_POINTS) * np.sqrt(2)
 
 
+@njit
+def dla_profile(lambda_, z_abs, nhi):
+    """Compute DLA profile
+
+    Arguments
+    ---------
+    lambda_: array of floats
+    Wavelength (in Angs)
+
+    z_abs: float
+    Redshift of the absorption
+
+    nhi: float
+    DLA column density in log10(cm^-2)
+    """
+    transmission = np.exp(
+        -tau_lya(lambda_, z_abs, nhi)
+        -tau_lyb(lambda_, z_abs, nhi))
+    return transmission
+
+### Implementation of Pasquier code,
+###     also in Rutten 2003 at 3.3.3
+LAMBDA_LYA = float(ABSORBER_IGM["LYA"]) ## Lya wavelength [A]
+@njit
+def tau_lya(lambda_, z_abs, nhi):
+    """Compute the optical depth for Lyman-alpha absorption.
+
+    Arguments
+    ---------
+    lambda_: array of floats
+    Wavelength (in Angs)
+
+    z_abs: float
+    Redshift of the absorption
+
+    nhi: float
+    DLA column density in log10(cm^-2)
+
+    Return
+    ------
+    tau: array of float
+    The optical depth.
+    """
+    gamma = 6.625e8  ## damping constant of the transition [s^-1]
+    osc_strength = 0.4164  ## oscillator strength of the atomic transition
+    speed_light = 3e8  ## speed of light [m/s]
+    thermal_velocity = 30000.  ## sqrt(2*k*T/m_proton) with
+    ## T = 5*10^4 ## [m.s^-1]
+    nhi_cm2 = 10**nhi  ## column density [cm^-2]
+    lambda_rest_frame = lambda_ / (1 + z_abs)
+    ## wavelength at DLA restframe [A]
+
+    u_voight = ((speed_light / thermal_velocity) *
+                (LAMBDA_LYA / lambda_rest_frame - 1))
+    ## dimensionless frequency offset in Doppler widths.
+    a_voight = LAMBDA_LYA * 1e-10 * gamma / (4 * np.pi * thermal_velocity)
+    ## Voigt damping parameter
+    voigt_profile = voigt(a_voight, u_voight)
+    thermal_velocity /= 1000.
+    ## 1.497e-16 = e**2/(4*sqrt(pi)*epsilon0*m_electron*c)*1e-10
+    ## [m^2.s^-1.m/]
+    ## we have b/1000 & 1.497e-15 to convert
+    ## 1.497e-15*osc_strength*lambda_rest_frame*h/n to cm^2
+    tau = (1.497e-15 * nhi_cm2 * osc_strength * lambda_rest_frame * voigt_profile /
+           thermal_velocity)
+    return tau
+
+LAMBDA_LYB = float(ABSORBER_IGM["LYB"])
+@njit
+def tau_lyb(lambda_, z_abs, nhi):
+    """Compute the optical depth for Lyman-beta absorption.
+
+    Arguments
+    ---------
+    lambda_: array of floats
+    Wavelength (in Angs)
+
+    z_abs: float
+    Redshift of the absorption
+
+    nhi: float
+    DLA column density in log10(cm^-2)
+
+    Return
+    ------
+    tau: array of float
+    The optical depth.
+    """
+    gamma = 0.079120
+    osc_strength = 1.897e8
+    speed_light = 3e8  ## speed of light m/s
+    thermal_velocity = 30000.
+    nhi_cm2 = 10**nhi
+    lambda_rest_frame = lambda_ / (1 + z_abs)
+
+    u_voight = ((speed_light / thermal_velocity) *
+                (LAMBDA_LYB / lambda_rest_frame - 1))
+    a_voight = LAMBDA_LYB * 1e-10 * gamma / (4 * np.pi * thermal_velocity)
+    voigt_profile = voigt(a_voight, u_voight)
+    thermal_velocity /= 1000.
+    tau = (1.497e-15 * nhi_cm2 * osc_strength * lambda_rest_frame * voigt_profile /
+           thermal_velocity)
+    return tau
+
+# maybe we should replace this by scipy.special.voigt_profile?
+# if it is in numba
+@njit
+def voigt(a_voight, u_voight):
+    """Compute the classical Voigt function
+
+    Arguments
+    ---------
+    a_voight: float
+    Voigt damping parameter.
+
+    u_voight: array of floats
+    Dimensionless frequency offset in Doppler widths.
+
+    Return
+    ------
+    voigt: array of float
+    The Voigt function for each element in a, u
+    """
+    unnormalized_voigt = np.zeros_like(u_voight)
+    for index in range(unnormalized_voigt.shape[0]):
+        unnormalized_voigt[index] = np.mean(
+            1.0 / (a_voight**2 + (GAUSSIAN_DIST - u_voight[index])**2)
+        )
+    return unnormalized_voigt * a_voight / np.sqrt(np.pi)
+
 class DlaMask(Mask):
     """Class to mask DLAs
 
     Methods
     -------
     __init__
     apply_mask
@@ -99,15 +234,15 @@
                 f"Error loading DlaMask. File {filename} does "
                 f"not have fields '{aux}' in HDU 'DLACAT'"
             ) from error
 
         # group DLAs on the same line of sight together
         self.los_ids = {}
         for los_id in np.unique(cat[los_id_name]):
-            w = (los_id == cat[los_id_name])
+            w = los_id == cat[los_id_name]
             self.los_ids[los_id] = list(zip(cat[z_colname][w], cat['NHI'][w]))
         num_dlas = np.sum([len(los_id) for los_id in self.los_ids.values()])
 
         self.logger.progress(f'In catalog: {num_dlas} DLAs')
         self.logger.progress(f'In catalog: {len(self.los_ids)} forests have a DLA\n')
 
         # setup transmission limit
@@ -148,218 +283,23 @@
         """
         lambda_ = 10**forest.log_lambda
 
         # load DLAs
         if self.los_ids.get(forest.los_id) is not None:
             dla_transmission = np.ones(len(lambda_))
             for (z_abs, nhi) in self.los_ids.get(forest.los_id):
-                dla_transmission *= DlaProfile(lambda_, z_abs,
-                                               nhi).transmission
+                dla_transmission *= dla_profile(lambda_, z_abs,
+                                                nhi)
 
             # find out which pixels to mask
             w = dla_transmission > self.dla_mask_limit
             if len(self.mask) > 0:
                 for mask_range in self.mask:
                     for (z_abs, nhi) in self.los_ids.get(forest.los_id):
                         w &= ((lambda_ / (1. + z_abs) < mask_range['wave_min'])
                               | (lambda_ /
                                  (1. + z_abs) > mask_range['wave_max']))
 
             # do the actual masking
             forest.transmission_correction *= dla_transmission
             for param in Forest.mask_fields:
                 self._masker(forest, param, w)
-
-class DlaProfile:
-    """Class to represent Damped Lyman-alpha Absorbers.
-
-    Methods
-    -------
-    __init__
-    profile_lya_absorption
-    profile_lyb_absorption
-    tau_lya
-    tau_lyb
-    voigt
-
-    Attributes
-    ----------
-    log_lambda: array of float
-    Logarithm of the wavelength (in Angs)
-
-    nhi: float
-    DLA column density in log10(cm^-2)
-
-    transmission: array of floats
-    Decrease of the transmitted flux due to the presence of a DLA
-
-    z_abs: float
-    Redshift of the absorption
-    """
-    def __init__(self, lambda_, z_abs, nhi):
-        """Initialize class instance.
-
-        Arguments
-        ---------
-        lambda_: array of floats
-        Wavelength (in Angs)
-
-        z_abs: float
-        Redshift of the absorption
-
-        nhi: float
-        DLA column density in log10(cm^-2)
-        """
-        self.z_abs = z_abs
-        self.nhi = nhi
-
-        self.transmission = self.profile_lya_absorption(lambda_, z_abs, nhi)
-        self.transmission *= self.profile_lyb_absorption(lambda_, z_abs, nhi)
-
-    @staticmethod
-    def profile_lya_absorption(lambda_, z_abs, nhi):
-        """Compute the absorption profile for Lyman-alpha absorption.
-
-        Arguments
-        ---------
-        lambda_: array of floats
-        Wavelength (in Angs)
-
-        z_abs: float
-        Redshift of the absorption
-
-        nhi: float
-        DLA column density in log10(cm^-2)
-
-        Return
-        ------
-        profile: array of floats
-        The absorption profile.
-        """
-        return np.exp(-DlaProfile.tau_lya(lambda_, z_abs, nhi))
-
-    @staticmethod
-    def profile_lyb_absorption(lambda_, z_abs, nhi):
-        """Computes the absorption profile for Lyman-beta absorption.
-
-        Arguments
-        ---------
-        lambda_: array of floats
-        Wavelength (in Angs)
-
-        z_abs: float
-        Redshift of the absorption
-
-        nhi: float
-        DLA column density in log10(cm^-2)
-
-        Return
-        ------
-        profile: array of floats
-        The absorption profile.
-        """
-        return np.exp(-DlaProfile.tau_lyb(lambda_, z_abs, nhi))
-
-    ### Implementation of Pasquier code,
-    ###     also in Rutten 2003 at 3.3.3
-    @staticmethod
-    def tau_lya(lambda_, z_abs, nhi):
-        """Compute the optical depth for Lyman-alpha absorption.
-
-        Arguments
-        ---------
-        lambda_: array of floats
-        Wavelength (in Angs)
-
-        z_abs: float
-        Redshift of the absorption
-
-        nhi: float
-        DLA column density in log10(cm^-2)
-
-        Return
-        ------
-        tau: array of float
-        The optical depth.
-        """
-        lambda_lya = ABSORBER_IGM["LYA"]  ## Lya wavelength [A]
-        gamma = 6.625e8  ## damping constant of the transition [s^-1]
-        osc_strength = 0.4164  ## oscillator strength of the atomic transition
-        speed_light = 3e8  ## speed of light [m/s]
-        thermal_velocity = 30000.  ## sqrt(2*k*T/m_proton) with
-        ## T = 5*10^4 ## [m.s^-1]
-        nhi_cm2 = 10**nhi  ## column density [cm^-2]
-        lambda_rest_frame = lambda_ / (1 + z_abs)
-        ## wavelength at DLA restframe [A]
-
-        u_voight = ((speed_light / thermal_velocity) *
-                    (lambda_lya / lambda_rest_frame - 1))
-        ## dimensionless frequency offset in Doppler widths.
-        a_voight = lambda_lya * 1e-10 * gamma / (4 * np.pi * thermal_velocity)
-        ## Voigt damping parameter
-        voigt = DlaProfile.voigt(a_voight, u_voight)
-        thermal_velocity /= 1000.
-        ## 1.497e-16 = e**2/(4*sqrt(pi)*epsilon0*m_electron*c)*1e-10
-        ## [m^2.s^-1.m/]
-        ## we have b/1000 & 1.497e-15 to convert
-        ## 1.497e-15*osc_strength*lambda_rest_frame*h/n to cm^2
-        tau = (1.497e-15 * nhi_cm2 * osc_strength * lambda_rest_frame * voigt /
-               thermal_velocity)
-        return tau
-
-    @staticmethod
-    def tau_lyb(lambda_, z_abs, nhi):
-        """Compute the optical depth for Lyman-beta absorption.
-
-        Arguments
-        ---------
-        lambda_: array of floats
-        Wavelength (in Angs)
-
-        z_abs: float
-        Redshift of the absorption
-
-        nhi: float
-        DLA column density in log10(cm^-2)
-
-        Return
-        ------
-        tau: array of float
-        The optical depth.
-        """
-        lam_lyb = ABSORBER_IGM["LYB"]
-        gamma = 0.079120
-        osc_strength = 1.897e8
-        speed_light = 3e8  ## speed of light m/s
-        thermal_velocity = 30000.
-        nhi_cm2 = 10**nhi
-        lambda_rest_frame = lambda_ / (1 + z_abs)
-
-        u_voight = ((speed_light / thermal_velocity) *
-                    (lam_lyb / lambda_rest_frame - 1))
-        a_voight = lam_lyb * 1e-10 * gamma / (4 * np.pi * thermal_velocity)
-        voigt = DlaProfile.voigt(a_voight, u_voight)
-        thermal_velocity /= 1000.
-        tau = (1.497e-15 * nhi_cm2 * osc_strength * lambda_rest_frame * voigt /
-               thermal_velocity)
-        return tau
-
-    @staticmethod
-    def voigt(a_voight, u_voight):
-        """Compute the classical Voigt function
-
-        Arguments
-        ---------
-        a_voight: array of floats
-        Voigt damping parameter.
-
-        u_voight: array of floats
-        Dimensionless frequency offset in Doppler widths.
-
-        Return
-        ------
-        voigt: array of float
-        The Voigt function for each element in a, u
-        """
-        unnormalized_voigt = np.mean(
-            1 / (a_voight**2 + (GAUSSIAN_DIST[:, None] - u_voight)**2), axis=0)
-        return unnormalized_voigt * a_voight / np.sqrt(np.pi)
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/masks/lines_mask.py` & `picca-7.0.0/py/picca/delta_extraction/masks/lines_mask.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """This module defines the class LinesMask in the masking of (sky) lines"""
 from astropy.table import Table
 import numpy as np
 
 from picca.delta_extraction.astronomical_objects.forest import Forest
 from picca.delta_extraction.errors import MaskError
 from picca.delta_extraction.mask import Mask
-
-defaults = {
-    "absorber mask width": 2.5,
-}
-
-accepted_options = ["filename", "keep pixels"]
-
+from picca.delta_extraction.mask import ( # pylint: disable=unused-import
+    accepted_options, defaults)
+from picca.delta_extraction.utils import update_accepted_options
+
+accepted_options = update_accepted_options(accepted_options, [
+    "filename"
+])
 
 class LinesMask(Mask):
     """Class to mask (sky) lines
 
     Methods
     -------
     __init__
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/quasar_catalogue.py` & `picca-7.0.0/py/picca/delta_extraction/quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py` & `picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,16 @@
                     "When TILEID is in the catalogue, PETAL_LOC is also "
                     "expected to be present but it is not.")
         if 'NIGHT' in catalogue.colnames:
             keep_columns += ['NIGHT']
         # TODO: remove this once we settle on a name for LAST_NIGHT/LASTNIGHT
         if "LAST_NIGHT" in catalogue.colnames:
             catalogue.rename_column("LAST_NIGHT", "LASTNIGHT")
+        if "COADD_LASTNIGHT" in catalogue.colnames:
+            catalogue.rename_column("COADD_LASTNIGHT", "LASTNIGHT")
         if 'LASTNIGHT' in catalogue.colnames:
             keep_columns += ['LASTNIGHT']
         if 'SURVEY' in catalogue.colnames:
             keep_columns += ['SURVEY']
         if 'DESI_TARGET' in catalogue.colnames:
             keep_columns += ['DESI_TARGET']
         if 'SV1_DESI_TARGET' in catalogue.colnames:
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py` & `picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
             0: 'SKY',
             1: 'LITTLE_COVERAGE',
             7: 'UNPLUGGED',
             8: 'BAD_TARGET',
             9: 'NODATA'
         }
         for z_warn_bit, z_warn_bit_name in bad_z_warn_bit.items():
-            wbit = (catalogue["ZWARNING"] & 2**z_warn_bit == 0)
+            wbit = catalogue["ZWARNING"] & 2**z_warn_bit == 0
             w &= wbit
             self.logger.progress(f"Found {np.sum(w)} spectra without {z_warn_bit} "
                                  f"bit set: {z_warn_bit_name}")
         self.logger.progress(f"# unique objs: {len(drq_catalogue)}")
         self.logger.progress(f"# spectra: {w.sum()}")
         catalogue = catalogue[w]
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/rejection_log.py` & `picca-7.0.0/py/picca/delta_extraction/rejection_log.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py` & `picca-7.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,28 @@
         file: str
         Filename of the rejection log
         """
         super().__init__(file)
 
         self.dtypes = None
         self.data = []
+        self.units = None
 
     def initialize_rejection_log(self, forest):
         """Initialize rejection log
 
         Arguments
         ---------
         forest: Forest
         Forest to obtain metadata dtypes
         """
         self.dtypes = forest.get_metadata_dtype() + [('FOREST_SIZE', int),
                                                      ('REJECTION_STATUS', 'S12')
                                                     ]
+        self.units = forest.get_metadata_units() + ['', '']
         self.initialized = True
 
     def add_to_rejection_log(self, forest, rejection_status):
         """Adds to the rejection log arrays.
         In the log forest metadata will be saved along with the forest size and
         rejection status.
 
@@ -84,9 +86,12 @@
         rejection_log = fitsio.FITS(self.file, 'rw', clobber=True)
 
         rejection_log.write(
             np.array(
                 self.data,
                 dtype=self.dtypes,
             ),
-            extname="rejection_log",
+            units=self.units,
+            extname="REJECTION_LOG",
         )
+        rejection_log["REJECTION_LOG"].write_comment("Rejected forest statistics")
+        rejection_log["REJECTION_LOG"].write_checksum()
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py` & `picca-7.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/delta_extraction/survey.py` & `picca-7.0.0/py/picca/delta_extraction/survey.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,26 +109,32 @@
         self.masks = None
         self.data = None
         self.expected_flux = None
         self.num_processors = None
 
     def apply_corrections(self):
         """Apply the corrections. To be run after self.read_corrections()"""
+        if len(self.corrections) == 0:
+            return
+
         t0 = time.time()
         self.logger.info("Applying corrections")
 
         for forest_index, _ in enumerate(self.data.forests):
             for correction_index, _ in enumerate(self.corrections):
                 self.corrections[correction_index].apply_correction(self.data.forests[forest_index])
 
         t1 = time.time()
         self.logger.info(f"Time spent applying corrections: {t1-t0}")
 
     def apply_masks(self):
         """Apply the corrections. To be run after self.read_corrections()"""
+        if len(self.masks) == 0:
+            return
+
         t0 = time.time()
         self.logger.info("Applying masks")
 
         if self.num_processors > 1:
             context = multiprocessing.get_context('fork')
             # Pick a large chunk size such that masks are
             # copied as few times as possible
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/utils.py` & `picca-7.0.0/py/picca/delta_extraction/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,58 +130,62 @@
     # get the list with the valid options
     try:
         accepted_options = getattr(module_object, "accepted_options")
     except AttributeError:
         accepted_options = []
     return class_object, default_args, accepted_options
 
-
 @njit()
-def find_bins(original_array, grid_array, wave_solution):
+def find_bins_lin(original_array, grid_array):
     """For each element in original_array, find the corresponding bin in grid_array
 
+    This function assumes that wavelength grid that is evenly spaced on wavelength
+
     Arguments
     ---------
     original_array: array of float
     Read array, e.g. forest.log_lambda
 
     grid_array: array of float
     Common array, e.g. Forest.log_lambda_grid
 
-    wave_solution: "log" or "lin"
-    Specifies whether we want to construct a wavelength grid that is evenly
-    spaced on wavelength (lin) or on the logarithm of the wavelength (log)
+    Return
+    ------
+    found_bin: array of int
+    An array of size original_array.size filled with values smaller than
+    grid_array.size with the bins correspondance
+    """
+    aux = 10**grid_array[0]
+    step = 10**grid_array[1] - aux
+    found_bin = ((10**original_array - aux) / step + 0.5).astype(np.int64)
+    return found_bin
+
+@njit()
+def find_bins_log(original_array, grid_array):
+    """For each element in original_array, find the corresponding bin in grid_array
+
+    This function assumes that wavelength grid that is evenly spaced on the
+    logarithm of the wavelength
+
+    Arguments
+    ---------
+    original_array: array of float
+    Read array, e.g. forest.log_lambda
+
+    grid_array: array of float
+    Common array, e.g. Forest.log_lambda_grid
 
     Return
     ------
     found_bin: array of int
     An array of size original_array.size filled with values smaller than
     grid_array.size with the bins correspondance
     """
-    if wave_solution == "log":
-        pass
-    elif wave_solution == "lin":
-        original_array = 10**original_array
-        grid_array = 10**grid_array
-    else:  # pragma: no cover
-        raise DeltaExtractionError(
-            "Error in function find_bins from py/picca/delta_extraction/utils.py"
-            "expected wavelength solution to be either 'log' or 'lin'. ")
-    original_array_size = original_array.size
-    grid_array_size = grid_array.size
-    found_bin = np.zeros(original_array_size, dtype=np.int64)
-    for index1 in range(original_array_size):
-        min_dist = np.finfo(np.float64).max
-        for index2 in range(grid_array_size):
-            dist = np.abs(grid_array[index2] - original_array[index1])
-            if dist < min_dist:
-                min_dist = dist
-                found_bin[index1] = index2
-            else:
-                break
+    step = grid_array[1] - grid_array[0]
+    found_bin = ((original_array - grid_array[0]) / step + 0.5).astype(np.int64)
     return found_bin
 
 PROGRESS_LEVEL_NUM = 15
 logging.addLevelName(PROGRESS_LEVEL_NUM, "PROGRESS")
 
 
 def progress(self, message, *args, **kws):
@@ -295,25 +299,31 @@
             if item in accepted_options:
                 accepted_options.remove(item)
     else:
         accepted_options = sorted(list(set(accepted_options + new_options)))
 
     return accepted_options
 
-def update_default_options(default_options, new_options):
+def update_default_options(default_options, new_options, force_overwrite=False):
     """Update the content of the list of accepted options
 
     Arguments
     ---------
     default_options: dict
     The current default options
 
     new_options: dict
     The new options
 
+    force_overwrite: bool - default: False
+    If different values for a specific key are given the code raises an error
+    complaining about conflicting default values. If `force_overwrite` is True,
+    keep the value from new_options instead. This should be used with caution
+    and only to overwrite default values from parent classes.
+
     Return
     ------
     default_options: dict
     The updated default options
     """
     default_options = default_options.copy()
     for key, value in new_options.items():
@@ -321,16 +331,19 @@
             default_value = default_options.get(key)
             if type(default_value) is not type(value):
                 raise DeltaExtractionError(
                     f"Incompatible defaults are being added. Key {key} "
                     "found to have values with different type: "
                     f"{type(default_value)} and {type(value)}. "
                     "Revise your recent changes or contact picca developpers.")
-            if default_value != value:
+            if default_value != value and not force_overwrite:
                 raise DeltaExtractionError(
                     f"Incompatible defaults are being added. Key {key} "
                     f"found to have two default values: '{value}' and '{default_value}' "
-                    "Revise your recent changes or contact picca developpers.")
+                    "Please revise your recent changes. If you really want to "
+                    "overwrite the default values of a parent class, then pass "
+                    "`force_overload=True`. If you are unsure what this message "
+                    "means contact picca developpers.")
         else:
             default_options[key] = value
 
     return default_options
```

### Comparing `picca-6.1.0/py/picca/delta_extraction/utils_pk1d.py` & `picca-7.0.0/py/picca/delta_extraction/utils_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/dla.py` & `picca-7.0.0/py/picca/dla.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/chi2.py` & `picca-7.0.0/py/picca/fitter2/chi2.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/control.py` & `picca-7.0.0/py/picca/fitter2/control.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/control_mpi.py` & `picca-7.0.0/py/picca/fitter2/control_mpi.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/data.py` & `picca-7.0.0/py/picca/fitter2/data.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/effective-bins.py` & `picca-7.0.0/py/picca/fitter2/effective-bins.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits` & `picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits` & `picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits` & `picca-7.0.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits` & `picca-7.0.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits` & `picca-7.0.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits` & `picca-7.0.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/myGamma.py` & `picca-7.0.0/py/picca/fitter2/myGamma.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/parser.py` & `picca-7.0.0/py/picca/fitter2/parser.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/pk.py` & `picca-7.0.0/py/picca/fitter2/pk.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/priors.py` & `picca-7.0.0/py/picca/fitter2/priors.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/sampler.py` & `picca-7.0.0/py/picca/fitter2/sampler.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/utils.py` & `picca-7.0.0/py/picca/fitter2/utils.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/fitter2/xi.py` & `picca-7.0.0/py/picca/fitter2/xi.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/io.py` & `picca-7.0.0/py/picca/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1400,65 +1400,83 @@
     elif len(in_dir) > 5 and in_dir[-5:] == '.fits':
         files += glob.glob(in_dir)
     else:
         files += glob.glob(in_dir + '/*.fits') + glob.glob(in_dir
                                                            + '/*.fits.gz')
     filename = files[0]
     hdul = fitsio.FITS(filename)
-    header = hdul[1].read_header()
-    # new runs of picca_deltas should have a blinding keyword
-    if "BLINDING" in header:
+    if "LAMBDA" in hdul: # This is for ImageHDU format
+        header = hdul["METADATA"].read_header()
         blinding = header["BLINDING"]
-    # older runs are not from DESI main survey and should not be blinded
-    else:
-        blinding = "none"
+    else: # This is for BinTable format
+        header = hdul[1].read_header()
+        if "BLINDING" in header:
+            blinding = header["BLINDING"]
+        else:
+            blinding = "none"
 
     return blinding
 
-
-def read_delta_file(filename, rebin_factor=None):
+def read_delta_file(filename, z_min_qso=0, z_max_qso=10, rebin_factor=None):
     """Extracts deltas from a single file.
     Args:
         filename: str
-            Path to the file to read        
+            Path to the file to read
+        z_min_qso: float - default: 0
+            Specifies the minimum redshift for QSOs
+        z_max_qso: float - default: 10
+            Specifies the maximum redshift for QSOs
         rebin_factor: int - default: None
             Factor to rebin the lambda grid by. If None, no rebinning is done.
     Returns:
         deltas:
             A dictionary with the data. Keys are the healpix numbers of each
                 spectrum. Values are lists of delta instances.
     """
 
     hdul = fitsio.FITS(filename)
     # If there is an extension called lambda format is image
     if 'LAMBDA' in hdul:
-        deltas = Delta.from_image(hdul)
+        deltas = Delta.from_image(hdul, z_min_qso=z_min_qso, z_max_qso=z_max_qso)
     else:
-        deltas = [Delta.from_fitsio(hdu) for hdu in hdul[1:]]
-    
-    hdul.close()
+        deltas = [Delta.from_fitsio(hdu) for hdu in hdul[1:] if z_min_qso<hdu.read_header()['Z']<z_max_qso]
 
-    # Rebin
+# Rebin
     if rebin_factor is not None:
+        if 'LAMBDA' in hdul:
+            card = 'LAMBDA'
+        else:
+            card = 1
+
+        if hdul[card].read_header()['WAVE_SOLUTION'] != 'lin':
+            raise ValueError('Delta rebinning only implemented for linear \
+                    lambda bins')
+        
+        dwave = hdul[card].read_header()['DELTA_LAMBDA']
+            
         for i in range(len(deltas)):
-            deltas[i].rebin(rebin_factor)
+            deltas[i].rebin(rebin_factor, dwave=dwave)
+            
+    hdul.close()
 
     return deltas
 
 
 def read_deltas(in_dir,
                 nside,
                 lambda_abs,
                 alpha,
                 z_ref,
                 cosmo,
                 max_num_spec=None,
                 no_project=False,
                 nproc=None,
-                rebin_factor=None):
+                rebin_factor=None,
+                z_min_qso=0,
+                z_max_qso=10):
     """Reads deltas and computes their redshifts.
 
     Fills the fields delta.z and multiplies the weights by
         `(1+z)^(alpha-1)/(1+z_ref)^(alpha-1)`
     (equation 7 of du Mas des Bourboux et al. 2020)
 
     Args:
@@ -1481,14 +1499,18 @@
         no_project: bool - default: False
             If True, project the deltas (see equation 5 of du Mas des Bourboux
             et al. 2020)
         nproc: int - default: None
             Number of cpus for parallelization. If None, uses all available.
         rebin_factor: int - default: None
             Factor to rebin the lambda grid by. If None, no rebinning is done.
+        z_min_qso: float - default: 0
+            Specifies the minimum redshift for QSOs
+        z_max_qso: float - default: 10
+            Specifies the maximum redshift for QSOs
 
     Returns:
         The following variables:
             data: A dictionary with the data. Keys are the healpix numbers of
                 each spectrum. Values are lists of delta instances.
             num_data: Number of spectra in data.
             z_min: Minimum redshift of the loaded deltas.
@@ -1508,15 +1530,15 @@
         files += sorted(glob.glob(in_dir + '/*.fits') + glob.glob(in_dir +
                                                             '/*.fits.gz'))
     files = sorted(files)
 
     if rebin_factor is not None:
         userprint(f"Rebinning deltas by a factor of {rebin_factor}\n")
 
-    arguments = [(f, rebin_factor) for f in files]
+    arguments = [(f, z_min_qso, z_max_qso, rebin_factor) for f in files]
     pool = Pool(processes=nproc)
     results = pool.starmap(read_delta_file, arguments)
     pool.close()
 
     deltas = []
     num_data = 0
     for delta in results:
@@ -1634,15 +1656,15 @@
             nightcol='TARGETID'
         else:
             raise Exception("The catalog does not have a NIGHT or LAST_NIGHT entry")
 
     for index, healpix in enumerate(unique_healpix):
         userprint("{} of {}".format(index, len(unique_healpix)))
         w = healpixs == healpix
-        if 'desi' in mode:
+        if 'TARGETID' in catalog.colnames:
             if 'FIBER' in catalog.colnames:
                 fibercol = "FIBER"
             else:
                 fibercol = "TARGETID"
             objs[healpix] = [
                 QSO(entry['TARGETID'], entry['RA'], entry['DEC'], entry['Z'],
                 entry['TARGETID'], entry[nightcol], entry[fibercol])
```

### Comparing `picca-6.1.0/py/picca/pk1d/compute_pk1d.py` & `picca-7.0.0/py/picca/pk1d/compute_pk1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
     # rebin not mixing pixels separated by masks
     bins = np.floor((lambda_or_log_lambda - lambda_or_log_lambda.min()) /
                     rebin_delta_lambda_or_log_lambda + 0.5).astype(int)
 
     rebin_exposure_diff = np.bincount(bins.astype(int), weights=exposures_diff)
     rebin_counts = np.bincount(bins.astype(int))
-    w = (rebin_counts > 0)
+    w = rebin_counts > 0
     if len(rebin_counts) == 0:
         userprint("Error: exposures_diff size = 0 ", exposures_diff)
     rebin_exposure_diff = rebin_exposure_diff[w] / np.sqrt(rebin_counts[w])
 
     # now merge the rebinned array into a noise array
     noise = np.zeros(exposures_diff.size)
     for index in range(len(exposures_diff) // len(rebin_exposure_diff) + 1):
@@ -299,15 +299,15 @@
     k: array of float
     The Fourier modes the Power Spectrum is measured on
 
     pk: array of float
     The Power Spectrum
     """
     if linear_binning:  # spectral length in AA
-        length_lambda = (delta_lambda_or_log_lambda * len(delta))
+        length_lambda = delta_lambda_or_log_lambda * len(delta)
     else:  # spectral length in km/s
         length_lambda = (delta_lambda_or_log_lambda * constants.SPEED_LIGHT *
                          np.log(10.) * len(delta))
 
     # make 1D FFT
     num_pixels = len(delta)
     fft_delta = rfft(delta)
@@ -410,15 +410,16 @@
     pixelization_factor = np.sinc(k * delta_pixel / (2 * np.pi))**2
 
     correction *= np.exp(-(k * mean_reso)**2)
     correction *= pixelization_factor
     return correction
 
 
-def compute_correction_reso_matrix(reso_matrix, k, delta_pixel, num_pixel):
+def compute_correction_reso_matrix(reso_matrix, k, delta_pixel, num_pixel,
+                                   pixelization_correction = False):
     """Computes the resolution correction based on the resolution matrix using linear binning
 
     Arguments
     ---------
     delta_pixel: float
     Variation of the logarithm of the wavelength between two pixels
     (in km/s or Ang depending on the units of k submitted)
@@ -444,27 +445,28 @@
     #first compute the power in the resmat for each pixel, then average
     for resmat in reso_matrix:
         r = np.append(resmat, np.zeros(num_pixel - resmat.size))
         k_resmat, w2 = compute_pk_raw(delta_pixel, r, linear_binning=True)
         try:
             assert np.all(k_resmat == k)
         except AssertionError as error:
-            raise Exception(
+            raise AssertionError(
                 "for some reason the resolution matrix correction has "
                 "different k scaling than the pk") from error
         w2 /= w2[0]
         w2_arr.append(w2)
 
     w_res2 = np.mean(w2_arr, axis=0)
-    pixelization_factor = np.sinc(k * delta_pixel / (2 * np.pi))**2
 
     # the following assumes that the resolution matrix is storing the actual
     # resolution convolved with the pixelization kernel along each matrix axis
     correction = w_res2
-    correction /= pixelization_factor
+    if pixelization_correction :
+        pixelization_factor = np.sinc(k * delta_pixel / (2 * np.pi))**2
+        correction /= pixelization_factor
 
     return correction
 
 
 class Pk1D:
     """Class to represent the 1D Power Spectrum for a given forest
```

### Comparing `picca-6.1.0/py/picca/pk1d/prep_pk1d.py` & `picca-7.0.0/py/picca/pk1d/prep_pk1d.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,139 +30,171 @@
     Array containing the logarithm of the wavelengths (in Angs)
 
     Return
     ------
     exposure_diff: array of float
     The difference between exposures
     """
-    num_exp_per_col = hdul[0].read_header()['NEXP'] // 2
+    num_exp_per_col = hdul[0].read_header()["NEXP"] // 2
     flux_total_odd = np.zeros(log_lambda.size)
     ivar_total_odd = np.zeros(log_lambda.size)
     flux_total_even = np.zeros(log_lambda.size)
     ivar_total_even = np.zeros(log_lambda.size)
 
     if num_exp_per_col < 2:
         userprint("DBG : not enough exposures for diff")
 
     for index_exp in range(num_exp_per_col):
         for index_col in range(2):
-            log_lambda_exp = hdul[(4 + index_exp +
-                                   index_col * num_exp_per_col)]["loglam"][:]
-            flux_exp = hdul[(4 + index_exp +
-                             index_col * num_exp_per_col)]["flux"][:]
-            ivar_exp = hdul[(4 + index_exp +
-                             index_col * num_exp_per_col)]["ivar"][:]
+            log_lambda_exp = hdul[(4 + index_exp + index_col * num_exp_per_col)][
+                "loglam"
+            ][:]
+            flux_exp = hdul[(4 + index_exp + index_col * num_exp_per_col)]["flux"][:]
+            ivar_exp = hdul[(4 + index_exp + index_col * num_exp_per_col)]["ivar"][:]
             mask = hdul[4 + index_exp + index_col * num_exp_per_col]["mask"][:]
             log_lambda_bins = np.searchsorted(log_lambda, log_lambda_exp)
 
             # exclude masks 25 (COMBINEREJ), 23 (BRIGHTSKY)?
-            rebin_ivar_exp = np.bincount(log_lambda_bins,
-                                         weights=ivar_exp * (mask & 2**25 == 0))
-            rebin_flux_exp = np.bincount(log_lambda_bins,
-                                         weights=(ivar_exp * flux_exp *
-                                                  (mask & 2**25 == 0)))
+            rebin_ivar_exp = np.bincount(
+                log_lambda_bins, weights=ivar_exp * (mask & 2**25 == 0)
+            )
+            rebin_flux_exp = np.bincount(
+                log_lambda_bins, weights=(ivar_exp * flux_exp * (mask & 2**25 == 0))
+            )
 
             if index_exp % 2 == 1:
-                flux_total_odd[:len(rebin_ivar_exp) - 1] += rebin_flux_exp[:-1]
-                ivar_total_odd[:len(rebin_ivar_exp) - 1] += rebin_ivar_exp[:-1]
+                flux_total_odd[: len(rebin_ivar_exp) - 1] += rebin_flux_exp[:-1]
+                ivar_total_odd[: len(rebin_ivar_exp) - 1] += rebin_ivar_exp[:-1]
             else:
-                flux_total_even[:len(rebin_ivar_exp) - 1] += rebin_flux_exp[:-1]
-                ivar_total_even[:len(rebin_ivar_exp) - 1] += rebin_ivar_exp[:-1]
+                flux_total_even[: len(rebin_ivar_exp) - 1] += rebin_flux_exp[:-1]
+                ivar_total_even[: len(rebin_ivar_exp) - 1] += rebin_ivar_exp[:-1]
 
     w = ivar_total_odd > 0
     flux_total_odd[w] /= ivar_total_odd[w]
     w = ivar_total_even > 0
     flux_total_even[w] /= ivar_total_even[w]
 
     alpha = 1
     if num_exp_per_col % 2 == 1:
-        num_even_exp = (num_exp_per_col - 1) // 2
-        alpha = np.sqrt(4. * num_even_exp *
-                        (num_even_exp + 1)) / num_exp_per_col
+        num_exp_even = (num_exp_per_col - 1) // 2
+        alpha = np.sqrt(4.0 * num_exp_even * (num_exp_even + 1)) / num_exp_per_col
     # TODO: CHECK THE * alpha (Nathalie)
     exposures_diff = 0.5 * (flux_total_even - flux_total_odd) * alpha
 
     return exposures_diff
 
 
-def exp_diff_desi(hdul, mask_targetid):
+def exp_diff_desi(
+    file,
+    mask_targetid,
+    method_alpha="desi_array",
+    use_only_even=False,
+):
     """Compute the difference between exposures.
 
     More precisely compute de semidifference between two customized coadded
     spectra obtained from weighted averages of the even-number exposures, for
     the first spectrum, and of the odd-number exposures, for the second one
     (see section 3.2 of Chabanier et al. 2019).
 
     Arguments
     ---------
-    hdul: fitsio.fitslib.FITS
-    Header Data Unit List opened by fitsio
+    file: fitsio.fitslib.FITS
+    Header Data Unit List opened by fitsio.
 
-    mask targetid: array of int
-    Targetids to select for calculating the exp differences
+    mask_targetid: array of int
+    Targetids to select for calculating the exposure differences.
+
+    method_alpha: str
+    Method to compute alpha. Defaults to "desi_array".
+
+    use_only_even: bool
+    Flag to indicate whether to use only even-number exposures. Defaults to False.
 
     Return
     ------
     diff: array of float
     The difference between exposures
     """
-    argsort = np.flip(np.argsort(hdul["TEFF_LYA"][mask_targetid][:]))
-    flux = hdul["FL"][mask_targetid][argsort, :]
-    ivar = hdul["IV"][mask_targetid][argsort, :]
-    teff_lya = hdul["TEFF_LYA"][mask_targetid][argsort]
+    argsort = np.flip(np.argsort(np.mean(file["IV"][mask_targetid], axis=1)))
+
+    teff_lya = file["TEFF_LYA"][mask_targetid][argsort]
+    flux = file["FL"][mask_targetid][argsort, :]
+    ivar = file["IV"][mask_targetid][argsort, :]
 
     num_exp = len(flux)
     if num_exp < 2:
-        userprint("DBG : not enough exposures for diff, spectra rejected")
+        print("Not enough exposures for diff, spectra rejected")
         return None
-    flux_total_odd = np.zeros(flux.shape[1])
-    ivar_total_odd = np.zeros(flux.shape[1])
-    flux_total_even = np.zeros(flux.shape[1])
-    ivar_total_even = np.zeros(flux.shape[1])
-    teff_even = 0
-    teff_odd = 0
-    teff_total = np.sum(teff_lya)
-    teff_last = teff_lya[-1]
-    for index_exp in range(2 * (num_exp // 2)):
-        flexp = flux[index_exp]
-        ivexp = ivar[index_exp]
-        teff_lya_exp = teff_lya[index_exp]
-        if index_exp % 2 == 1:
-            flux_total_odd += flexp * ivexp
-            ivar_total_odd += ivexp
-            teff_odd += teff_lya_exp
-        else:
-            flux_total_even += flexp * ivexp
-            ivar_total_even += ivexp
-            teff_even += teff_lya_exp
-
-    w = ivar_total_odd > 0
-    flux_total_odd[w] /= ivar_total_odd[w]
-    w = ivar_total_even > 0
-    flux_total_even[w] /= ivar_total_even[w]
-
-    alpha = 1
-    if num_exp % 2 == 1:
-        # Ignasi: these variables were unsused so I commented them out
-        # n_even = (num_exp - 1) // 2
-        # alpha_n_old = np.sqrt(4. * n_even * (num_exp - n_even)) / num_exp
-        # alpha_N = np.sqrt(4.*t_even*(t_exp-t_even))/t_exp
-        # alpha_c_new = np.sqrt((teff_total - teff_last) / teff_total)
-        alpha_n_new = np.sqrt(
-            (teff_total - teff_last) * (teff_total + teff_last)) / teff_total
-        alpha = alpha_n_new
-    diff = 0.5 * (flux_total_even - flux_total_odd) * alpha
+    if use_only_even:
+        if num_exp % 2 == 1:
+            print("Odd number of exposures discarded")
+            return None
+
+    time_even = 0
+    time_odd = 0
+    time_exp = np.sum(teff_lya)
+
+    even_inds = slice(0, 2 * (num_exp // 2), 2)
+    odd_inds = slice(1, 2 * (num_exp // 2), 2)
+    flux_tot_odd = (flux[odd_inds] * ivar[odd_inds]).sum(axis=0)
+    ivar_tot_odd = (ivar[odd_inds]).sum(axis=0)
+    flux_tot_even = (flux[even_inds] * ivar[even_inds]).sum(axis=0)
+    ivar_tot_even = (ivar[even_inds]).sum(axis=0)
+    ivar_tot = ivar[:num_exp].sum(axis=0)
+
+    mask_odd = ivar_tot_odd > 0
+    flux_tot_odd[mask_odd] /= ivar_tot_odd[mask_odd]
+    mask_even = ivar_tot_even > 0
+    flux_tot_even[mask_even] /= ivar_tot_even[mask_even]
+
+    if method_alpha == "eboss":
+        alpha = 1
+        if num_exp % 2 == 1:
+            n_even = num_exp // 2
+            alpha = np.sqrt(4.0 * n_even * (n_even + 1)) / num_exp
+
+    elif method_alpha == "eboss_corr":
+        alpha = 1
+        if num_exp % 2 == 1:
+            n_even = num_exp // 2
+            alpha = np.sqrt((2 * n_even) / (num_exp))
+
+    elif method_alpha == "desi_array":
+        mask = mask_odd & mask_even & (ivar_tot > 0)
+        alpha_array = np.ones(flux.shape[1])
+        alpha_array[mask] = (1 / np.sqrt(ivar_tot[mask])) / (
+            0.5 * np.sqrt((1 / ivar_tot_even[mask]) + (1 / ivar_tot_odd[mask]))
+        )
+        alpha = alpha_array
+
+    elif method_alpha == "desi_mean_array":
+        alpha_array = np.ones(flux.shape[1])
+        alpha_array[mask] = (1 / np.sqrt(ivar_tot[mask])) / (
+            0.5 * np.sqrt((1 / ivar_tot_even[mask]) + (1 / ivar_tot_odd[mask]))
+        )
+        alpha = np.nanmean((1 / np.sqrt(ivar_tot[mask]))) / np.nanmean(
+            (0.5 * np.sqrt((1 / ivar_tot_even[mask]) + (1 / ivar_tot_odd[mask])))
+        )
+
+    elif method_alpha == "desi_time":
+        alpha = 2 * np.sqrt(
+            (time_odd * time_even) / (time_exp * (time_odd + time_even))
+        )
 
+    diff = 0.5 * (flux_tot_even - flux_tot_odd) * alpha
     return diff
 
 
-def spectral_resolution(wdisp,
-                        with_correction=False,
-                        fiberid=None,
-                        log_lambda=None):
+def spectral_resolution(
+    wdisp,
+    with_correction=False,
+    fiberid=None,
+    log_lambda=None,
+):
     # TODO: fix docstring
     """Compute the spectral resolution
 
     Arguments
     ---------
     wdisp: array of float
     ?
@@ -178,31 +210,37 @@
     Logarithm of the wavelength (in Angstroms)
 
     Return
     ------
     reso: array of float
     The spectral resolution
     """
-    reso = wdisp * SPEED_LIGHT * 1.0e-4 * np.log(10.)
+    reso = wdisp * SPEED_LIGHT * 1.0e-4 * np.log(10.0)
 
     if with_correction:
-        lambda_ = np.power(10., log_lambda)
+        lambda_ = np.power(10.0, log_lambda)
         # compute the wavelength correction
         correction = 1.267 - 0.000142716 * lambda_ + 1.9068e-08 * lambda_ * lambda_
         correction[lambda_ > 6000.0] = 1.097
 
         # add the fiberid correction
         # fiberids greater than 500 corresponds to the second spectrograph
         fiberid = fiberid % 500
         if fiberid < 100:
-            correction = (1. + (correction - 1) * .25 + (correction - 1) * .75 *
-                          (fiberid) / 100.)
+            correction = (
+                1.0
+                + (correction - 1) * 0.25
+                + (correction - 1) * 0.75 * (fiberid) / 100.0
+            )
         elif fiberid > 400:
-            correction = (1. + (correction - 1) * .25 + (correction - 1) * .75 *
-                          (500 - fiberid) / 100.)
+            correction = (
+                1.0
+                + (correction - 1) * 0.25
+                + (correction - 1) * 0.75 * (500 - fiberid) / 100.0
+            )
 
         # apply the correction
         reso *= correction
 
     return reso
 
 
@@ -222,26 +260,29 @@
     ------
     rms_in_pixel: float
     The spectral resolution
 
     avg_reso_in_km_per_s: float
     The average resolution in km/s
     """
-    delta_log_lambda = ((log_lambda[-1] - log_lambda[0]) /
-                        float(len(log_lambda) - 1))
+    delta_log_lambda = (log_lambda[-1] - log_lambda[0]) / float(len(log_lambda) - 1)
     reso = np.clip(reso_matrix, 1.0e-6, 1.0e6)
 
     #
     rms_in_pixel = (
-        np.sqrt(1.0 / 2.0 /
-                np.log(reso[len(reso) // 2][:] / reso[len(reso) // 2 - 1][:])) +
-        np.sqrt(4.0 / 2.0 /
-                np.log(reso[len(reso) // 2][:] / reso[len(reso) // 2 - 2][:])) +
-        np.sqrt(1.0 / 2.0 /
-                np.log(reso[len(reso) // 2][:] / reso[len(reso) // 2 + 1][:])) +
-        np.sqrt(4.0 / 2.0 / np.log(
-            reso[len(reso) // 2][:] / reso[len(reso) // 2 + 2][:]))) / 4.0
+        np.sqrt(
+            1.0 / 2.0 / np.log(reso[len(reso) // 2][:] / reso[len(reso) // 2 - 1][:])
+        )
+        + np.sqrt(
+            4.0 / 2.0 / np.log(reso[len(reso) // 2][:] / reso[len(reso) // 2 - 2][:])
+        )
+        + np.sqrt(
+            1.0 / 2.0 / np.log(reso[len(reso) // 2][:] / reso[len(reso) // 2 + 1][:])
+        )
+        + np.sqrt(
+            4.0 / 2.0 / np.log(reso[len(reso) // 2][:] / reso[len(reso) // 2 + 2][:])
+        )
+    ) / 4.0
 
-    avg_reso_in_km_per_s = (rms_in_pixel * SPEED_LIGHT * delta_log_lambda *
-                            np.log(10.0))
+    avg_reso_in_km_per_s = rms_in_pixel * SPEED_LIGHT * delta_log_lambda * np.log(10.0)
 
     return rms_in_pixel, avg_reso_in_km_per_s
```

### Comparing `picca-6.1.0/py/picca/prep_del.py` & `picca-7.0.0/py/picca/prep_del.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/raw_io.py` & `picca-7.0.0/py/picca/raw_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
         header['Z'] = delta.z_qso
         header['PMF'] = '{}-{}-{}'.format(delta.plate, delta.mjd, delta.fiberid)
         header['THING_ID'] = delta.thingid
         header['PLATE'] = delta.plate
         header['MJD'] = delta.mjd
         header['FIBERID'] = delta.fiberid
         header['ORDER'] = delta.order
+        header['WAVE_SOLUTION'] = 'lin' if lin_spaced else 'log'
 
         cols = [
             delta.log_lambda, delta.delta, delta.weights,
             np.ones(delta.log_lambda.size)
         ]
         names = ['LOGLAM', 'DELTA', 'WEIGHT', 'CONT']
         results.write(cols,
@@ -306,16 +307,16 @@
     accepted_z_keys = ['Z', 'Z_QSO_RSD']
     z_key = key_val.intersection(accepted_z_keys).pop()
     if not z_key:
         err_msg = f"Z key has to be one of {', '.join(accepted_z_keys)}"
         userprint(f"ERROR: {err_msg}")
         raise KeyError(err_msg)
 
-    w = hdu['Z'][:] > max(0., lambda_min / lambda_max_rest_frame - 1.)
-    w &= hdu['Z'][:] < max(0., lambda_max / lambda_min_rest_frame - 1.)
+    w = hdu[z_key][:] > max(0., lambda_min / lambda_max_rest_frame - 1.)
+    w &= hdu[z_key][:] < max(0., lambda_max / lambda_min_rest_frame - 1.)
     objs_ra = hdu['RA'][:][w].astype('float64') * np.pi / 180.
     objs_dec = hdu['DEC'][:][w].astype('float64') * np.pi / 180.
     objs_thingid = objs_thingid[w]
     hdul.close()
     userprint('INFO: Found {} quasars'.format(objs_ra.size))
 
     # Load list of transmission files
```

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/abstract_test.py` & `picca-7.0.0/py/picca/tests/delta_extraction/abstract_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,22 +170,20 @@
                             print(f"\n For header {orig_header['EXTNAME']}")
                             print(
                                 f"Different values found for key {key}: "
                                 f"orig: {orig_header[key]}, new: {new_header[key]}"
                             )
                         self.assertTrue(
                             (orig_header[key] == new_header[key]) or
-                            (np.isclose(orig_header[key], new_header[key])))
+                            (not isinstance(orig_header[key], str) and np.isclose(orig_header[key], new_header[key])))
                 for key in new_header:
                     if key not in orig_header:
                         print(f"\nOriginal file: {orig_file}")
                         print(f"New file: {new_file}")
                         print(f"key {key} missing in orig header")
-                        if key in ["MEANSNR", "BLINDING"]:
-                            continue
                     self.assertTrue(key in orig_header)
                 # check data
                 orig_data = orig_hdul[hdu_name].data
                 new_data = new_hdul[hdu_name].data
                 if orig_data is None:
                     self.assertTrue(new_data is None)
                 elif orig_data.dtype.names is None:
@@ -236,16 +234,14 @@
                                 (np.allclose(orig_data[col],
                                              new_data[col],
                                              equal_nan=True,
                                              rtol=rtol)))
                     for col in new_data.dtype.names:
                         if col not in orig_data.dtype.names:
                             print(f"Column {col} missing in orig header")
-                            if col in ["num_pixels", "valid_fit"]:
-                                continue
                         self.assertTrue(col in orig_data.dtype.names)
         finally:
             orig_hdul.close()
             new_hdul.close()
 
 
 if __name__ == '__main__':
```

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/astronomical_object_tests.py` & `picca-7.0.0/py/picca/tests/delta_extraction/astronomical_object_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,15 +594,15 @@
         """
         self.assertTrue(isinstance(test_obj, Forest))
         cols, names, units, comments = test_obj.get_data()
 
         if Forest.wave_solution == "log":
             self.assertTrue(names[0] == "LOGLAM")
             self.assertTrue(np.allclose(cols[0], test_obj.log_lambda))
-            self.assertTrue(units[0] == "log Angstrom")
+            self.assertTrue(units[0] == "log(Angstrom)")
             self.assertTrue(comments[0] == "Log lambda")
         elif Forest.wave_solution == "lin":
             self.assertTrue(names[0] == "LAMBDA")
             self.assertTrue(np.allclose(cols[0], 10**test_obj.log_lambda))
             self.assertTrue(units[0] == "Angstrom")
             self.assertTrue(comments[0] == "Lambda")
 
@@ -637,15 +637,15 @@
         self.assertTrue(
             comments[3] == ("Quasar continuum. "
                             "Check input spectra for units"))
 
         if isinstance(test_obj, Pk1dForest):
             self.assertTrue(names[4] == "IVAR")
             self.assertTrue(np.allclose(cols[4], test_obj.ivar))
-            self.assertTrue(units[4] == "Flux units")
+            self.assertTrue(units[4] == "(Flux units)^-1")
             self.assertTrue(
                 comments[4] == "Inverse variance. Check input spectra for units")
 
             self.assertTrue(names[5] == "DIFF")
             self.assertTrue(np.allclose(cols[5], test_obj.exposures_diff))
             self.assertTrue(units[5] == "Flux units")
             self.assertTrue(
@@ -951,14 +951,17 @@
 
     def test_desi_forest_get_data(self):
         """Test method get_data for DesiForest."""
         # set class variables
         setup_forest(wave_solution="lin")
         kwargs_desi_forest  = get_desi_kwargs_input("lin", "1")
 
+        Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 0.8, 0.8,
+                                   "lin", "Flux units")
+
         # create a DesiForest
         test_obj = DesiForest(**kwargs_desi_forest)
         test_obj.rebin()
 
         self.assert_get_data(test_obj)
 
     def test_desi_forest_get_header(self):
@@ -1208,14 +1211,17 @@
     def test_desi_pk1d_forest_get_data(self):
         """Test method get_data for DesiPk1dForest."""
         # set class variables
         setup_forest(wave_solution="lin")
         setup_pk1d_forest("LYA")
         kwargs_desi_pk1d_forest = get_desi_kwargs_input("lin", "1", is_p1d=True)
 
+        Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 0.8, 0.8,
+                                   "lin", "Flux units")
+
         # create a DesiPk1dForest
         test_obj = DesiPk1dForest(**kwargs_desi_pk1d_forest)
         test_obj.rebin()
         self.assert_get_data(test_obj)
 
     def test_desi_pk1d_forest_get_header(self):
         """Test method get_header for DesiPk1dForest."""
@@ -1574,24 +1580,29 @@
 
     def test_forest_get_data(self):
         """Test method get_data for Forest."""
         # set class variables; case: logarithmic wavelength solution
         setup_forest(wave_solution="log", rebin=3)
         kwargs_forest_log  = get_kwargs_input("log", "1")
 
+        Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 50e-4, 50e-4,
+                                   "log", "Flux units")
         # create a Forest
         test_obj = Forest(**kwargs_forest_log)
         test_obj.rebin()
         self.assert_get_data(test_obj)
 
         # set class variables; case: linear wavelength solution
         reset_forest()
         setup_forest(wave_solution="lin")
         kwargs_forest_lin  = get_kwargs_input("lin", "1")
 
+        Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 0.8, 0.8,
+                                   "lin", "Flux units")
+
         # create a Forest
         test_obj = Forest(**kwargs_forest_lin)
         test_obj.rebin()
         self.assert_get_data(test_obj)
 
         # check data format when blinding is engaged
         Forest.blinding = "corr_yshift"
@@ -1644,67 +1655,70 @@
             test_obj.get_header()
         self.compare_error_message(context_manager, expected_message)
 
     def test_forest_set_class_variables(self):
         """Test class method set_class_variables from Forest"""
         # logarithmic binning
         Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 50e-4, 50e-4,
-                                   "log")
+                                   "log", "test")
 
         log_lambda_grid = np.array([
             3.5563025, 3.5613025, 3.5663025, 3.5713025, 3.5763025, 3.5813025,
             3.5863025, 3.5913025, 3.5963025, 3.6013025, 3.6063025, 3.6113025,
             3.6163025, 3.6213025, 3.6263025, 3.6313025, 3.6363025, 3.6413025,
             3.6463025, 3.6513025, 3.6563025, 3.6613025, 3.6663025, 3.6713025,
             3.6763025, 3.6813025, 3.6863025, 3.6913025, 3.6963025, 3.7013025,
             3.7063025, 3.7113025, 3.7163025, 3.7213025, 3.7263025, 3.7313025,
-            3.7363025, 3.7413025
+            3.7363025, 3.7413025,
         ])
         self.assertTrue(np.allclose(Forest.log_lambda_grid, log_lambda_grid))
 
         log_lambda_rest_frame_grid = np.array([
-            3.01953334, 3.02453334, 3.02953334, 3.03453334, 3.03953334,
-            3.04453334, 3.04953334, 3.05453334, 3.05953334, 3.06453334,
-            3.06953334, 3.07453334
+            3.01703334, 3.02203334, 3.02703334, 3.03203334, 3.03703334,
+            3.04203334, 3.04703334, 3.05203334, 3.05703334, 3.06203334,
+            3.06703334, 3.07203334, 3.07703334,
         ])
         self.assertTrue(np.allclose(Forest.log_lambda_rest_frame_grid,
                                     log_lambda_rest_frame_grid))
 
         self.assertTrue(Forest.mask_fields, defaults_forest.get("mask fields"))
         self.assertTrue(Forest.wave_solution == "log")
+        self.assertTrue(Forest.flux_units == "test")
 
         # linear binning
         Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 100, 100,
-                                   "lin")
+                                   "lin", "test")
 
         log_lambda_grid = np.array([
             3.5563025 , 3.56820172, 3.5797836 , 3.59106461, 3.60205999,
             3.61278386, 3.62324929, 3.63346846, 3.64345268, 3.65321251,
             3.66275783, 3.67209786, 3.68124124, 3.69019608, 3.69897   ,
-            3.70757018, 3.71600334, 3.72427587, 3.73239376, 3.74036269
+            3.70757018, 3.71600334, 3.72427587, 3.73239376, 3.74036269,
         ])
         self.assertTrue(np.allclose(Forest.log_lambda_grid, log_lambda_grid))
 
         log_lambda_rest_frame_grid = np.array([
-            3.0374265 , 3.07554696
+            3.01703334, 3.05690485, 3.09342169,
         ])
+        print(Forest.log_lambda_rest_frame_grid)
         self.assertTrue(np.allclose(Forest.log_lambda_rest_frame_grid,
                                     log_lambda_rest_frame_grid))
 
         self.assertTrue(Forest.mask_fields, defaults_forest.get("mask fields"))
         self.assertTrue(Forest.wave_solution == "lin")
+        self.assertTrue(Forest.flux_units == "test")
 
         # specifying wrong bining should raise and error
         expected_message = (
             "Error in setting Forest class variables. 'wave_solution' "
             "must be either 'lin' or 'log'. Found: wrong"
         )
         with self.assertRaises(AstronomicalObjectError) as context_manager:
             Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 100, 100,
-                                       "wrong")
+                                       "wrong", "")
         self.compare_error_message(context_manager, expected_message)
 
     def test_pk1d_forest(self):
         """Test constructor for Pk1dForest object."""
         kwargs_pk1d_forest_log = get_kwargs_input("log", "1", is_p1d=True)
 
         # create a Pk1dForest with missing Pk1dForest class variables
@@ -1908,24 +1922,29 @@
         """Test method get_data for Pk1dForest."""
         # set class variables; case: logarithmic wavelength solution
         setup_forest(wave_solution="log", rebin=3)
         setup_pk1d_forest("LYA")
         kwargs_pk1d_forest_log = get_kwargs_input("log", "1", is_p1d=True)
         kwargs_pk1d_forest_lin = get_kwargs_input("lin", "1", is_p1d=True)
 
+        Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 50e-4, 50e-4,
+                                   "log", "Flux units")
+
         # create a Pk1dForest
         test_obj = Pk1dForest(**kwargs_pk1d_forest_log)
         test_obj.rebin()
         self.assert_get_data(test_obj)
 
         # set class variables; case: linear wavelength solution
         reset_forest()
         setup_forest(wave_solution="lin")
         setup_pk1d_forest("LYA")
 
+        Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 0.8, 0.8,
+                                   "lin", "Flux units")
         # create a Forest
         test_obj = Pk1dForest(**kwargs_pk1d_forest_lin)
         test_obj.rebin()
         self.assert_get_data(test_obj)
 
     def test_pk1d_forest_get_header(self):
         """Test method get_header for Pk1dForest."""
@@ -2129,14 +2148,17 @@
 
     def test_sdss_forest_get_data(self):
         """Test method get_data for SdssForest."""
         # set class variables
         setup_forest(wave_solution="log", rebin=3)
         kwargs_sdss_forest = get_sdss_kwargs_input("log", "1")
 
+        Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 50e-4, 50e-4,
+                                   "log", "Flux units")
+
         # create an SdssForest
         test_obj = SdssForest(**kwargs_sdss_forest)
         test_obj.rebin()
         self.assert_get_data(test_obj)
 
     def test_sdss_forest_get_header(self):
         """Test method get_header for SdssForest."""
@@ -2313,14 +2335,17 @@
     def test_sdss_pk1d_forest_get_data(self):
         """Test method get_data for SdssPk1dForest."""
         # set class variables
         setup_forest(wave_solution="log", rebin=3)
         setup_pk1d_forest("LYA")
         kwargs_sdss_pk1d_forest = get_sdss_kwargs_input("log", "1", is_p1d=True)
 
+        Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, 50e-4, 50e-4,
+                                   "log", "Flux units")
+
         # create an SdssPk1dForest
         test_obj = SdssPk1dForest(**kwargs_sdss_pk1d_forest)
         self.assert_get_data(test_obj)
 
     def test_sdss_pk1d_forest_get_header(self):
         """Test method get_header for SdssPk1dForest."""
         # set class variables
```

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/config_tests.py` & `picca-7.0.0/py/picca/tests/delta_extraction/config_tests.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/correction_tests.py` & `picca-7.0.0/py/picca/tests/delta_extraction/correction_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,19 +46,17 @@
         not initialized.
         """
         # create Correction instance
         correction = Correction()
 
         # run apply_correction, this should raise CorrectionError
         forest = copy.deepcopy(forest1)
-
         expected_message = ("Function 'apply_correction' was not overloaded by "
                             "child class")
         with self.assertRaises(CorrectionError) as context_manager:
-
             correction.apply_correction(forest)
         self.compare_error_message(context_manager, expected_message)
 
     def test_calibration_correction(self):
         """Test correct initialisation and inheritance for class
         CalibrationCorrection
```

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/data_tests.py` & `picca-7.0.0/py/picca/tests/delta_extraction/data_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         config.read_dict({"data": {
                             "out dir": f"{THIS_DIR}/results/",
                             "rejection log file": "rejection_log.fits.gz",
                             "wave solution": "log",
                             "delta log lambda": 3e-4,
                             "input directory": f"{THIS_DIR}/data/",
                             "num processors": 1,
+                            "flux units": "Flux units",
                          }})
         for key, value in defaults_data.items():
             if key not in config["data"]:
                 config["data"][key] = str(value)
 
         data = Data(config["data"])
 
@@ -114,14 +115,15 @@
         config.read_dict({"data": {"minimum number pixels in forest": 40,
                                    "out dir": f"{THIS_DIR}/results/",
                                    "rejection log file": "rejection_log.fits.gz",
                                    "wave solution": "log",
                                    "delta log lambda": 3e-4,
                                    "input directory": f"{THIS_DIR}/data/",
                                    "num processors": 1,
+                                   "flux units": "Flux units",
                          }})
         for key, value in defaults_data.items():
             if key not in config["data"]:
                 config["data"][key] = str(value)
         data = Data(config["data"])
 
         self.assertTrue(len(data.forests) == 0)
@@ -176,46 +178,62 @@
             "Missing argument 'delta lambda' required by Data when "
             "'wave solution' is set to 'lin'"
         )
         with self.assertRaises(DataError) as context_manager:
             Data(config["data"])
         self.compare_error_message(context_manager, expected_message)
 
+        # create a Data instance with missing flux units
+        config = ConfigParser()
+        config.read_dict({"data": {
+            "wave solution": "lin",
+            "delta lambda": 0.8,
+        }})
+        expected_message = (
+            "Missing argument 'flux units' required by Data"
+        )
+        with self.assertRaises(DataError) as context_manager:
+            Data(config["data"])
+        self.compare_error_message(context_manager, expected_message)
+
         # create a Data instance with missing lambda_max
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
         }})
         expected_message = (
             "Missing argument 'lambda max' required by Data"
         )
         with self.assertRaises(DataError) as context_manager:
             Data(config["data"])
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing lambda_max_rest_frame
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
         }})
         expected_message = (
             "Missing argument 'lambda max rest frame' required by Data"
         )
         with self.assertRaises(DataError) as context_manager:
             Data(config["data"])
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing lambda_min
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
         }})
         expected_message = (
             "Missing argument 'lambda min' required by Data"
         )
         with self.assertRaises(DataError) as context_manager:
@@ -223,14 +241,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing lambda_min_rest_frame
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
         }})
         expected_message = (
             "Missing argument 'lambda min rest frame' required by Data"
         )
@@ -239,14 +258,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing analysis_type
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
         }})
         expected_message = (
             "Missing argument 'analysis type' required by Data"
@@ -256,14 +276,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with wrong analysis_type
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "INVALID"
         }})
         expected_message = (
@@ -276,14 +297,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing lambda_abs_igm
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "PK 1D",
         }})
         expected_message = (
@@ -295,14 +317,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with invallid lambda_abs_igm
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "PK 1D",
             "lambda abs IGM": "wrong",
         }})
@@ -316,14 +339,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing input_directory
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
         }})
         expected_message = (
@@ -334,14 +358,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing min_num_pix
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
         }})
@@ -353,14 +378,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing num_processors
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
             "minimum number pixels in forest": 50,
@@ -373,14 +399,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing out_dir
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
             "minimum number pixels in forest": 50,
@@ -394,14 +421,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing rejection_log_file
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
             "minimum number pixels in forest": 50,
@@ -416,14 +444,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with invalid rejection_log_file (including folders)
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
             "minimum number pixels in forest": 50,
@@ -440,14 +469,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with invalid rejection_log_file (wrong extension)
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
             "minimum number pixels in forest": 50,
@@ -466,14 +496,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing save format
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
             "minimum number pixels in forest": 50,
@@ -489,14 +520,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with invalid save format
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
             "minimum number pixels in forest": 50,
@@ -513,14 +545,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing minimal snr bao3d
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "BAO 3D",
             "input directory": f"{THIS_DIR}/data",
             "minimum number pixels in forest": 50,
@@ -539,14 +572,15 @@
         self.compare_error_message(context_manager, expected_message)
 
         # create a Data instance with missing minimal snr bao3d
         config = ConfigParser()
         config.read_dict({"data": {
             "wave solution": "lin",
             "delta lambda": 0.8,
+            "flux units": "Flux units",
             "lambda max": 5500.0,
             "lambda max rest frame": 1200.0,
             "lambda min": 3600.0,
             "lambda min rest frame": 1040.0,
             "analysis type": "PK 1D",
             "lambda abs IGM": "LYA",
             "input directory": f"{THIS_DIR}/data",
@@ -570,18 +604,20 @@
         # create Data instance
         config = ConfigParser()
         config.read_dict({"data": {
                             "out dir": f"{THIS_DIR}/results/",
                             "rejection log file": "rejection_log.fits.gz",
                             "save format": "BinTableHDU",
                             "wave solution": "log",
+                            "flux units": "Flux units",
                             "delta log lambda": 3e-4,
                             "delta log lambda rest frame": 3e-4,
                             "input directory": f"{THIS_DIR}/data/",
                             "num processors": 1,
+                            "flux units": "Flux units",
                         }})
         for key, value in defaults_data.items():
             if key not in config["data"]:
                 config["data"][key] = str(value)
         data = Data(config["data"])
 
         # add dummy forests
@@ -615,14 +651,15 @@
                                    "rejection log file": "rejection_log.fits.gz",
                                     "save format": "BinTableHDU",
                                    "wave solution": "log",
                                    "delta log lambda": 3e-4,
                                    "delta log lambda rest frame": 3e-4,
                                    "input directory": f"{THIS_DIR}/data/",
                                    "num processors": 1,
+                                   "flux units": "Flux units",
                          }})
         for key, value in defaults_data.items():
             if key not in config["data"]:
                 config["data"][key] = str(value)
         data = Data(config["data"])
 
         # add dummy forest
@@ -643,14 +680,15 @@
                                     "save format": "BinTableHDU",
                                    "wave solution": "log",
                                    "delta log lambda": 3e-4,
                                    "delta log lambda rest frame": 3e-4,
                                    "input directory": f"{THIS_DIR}/data/",
                                    "minimal snr bao3d": 100000000,
                                    "num processors": 1,
+                                   "flux units": "Flux units",
                          }})
         for key, value in defaults_data.items():
             if key not in config["data"]:
                 config["data"][key] = str(value)
         data = Data(config["data"])
 
         # add dummy forest
```

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/expected_flux_tests.py` & `picca-7.0.0/py/picca/tests/delta_extraction/expected_flux_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,15 @@
         config = ConfigParser()
         config.read_dict({
             "data": desi_healpix_kwargs,
             "expected flux": {
                 "iter out prefix": "iter_out_prefix",
                 "out dir": f"{THIS_DIR}/results/",
                 "num processors": 1,
+                "var lss mod": 1.0,
             },
         })
         for key, value in defaults_dr16_expected_flux.items():
             if key not in config["expected flux"]:
                 config["expected flux"][key] = str(value)
         for key, value in defaults_desi_healpix.items():
             if key not in config["data"]:
@@ -753,15 +754,16 @@
 
         # create a Dr16ExpectedFlux with missing 'force stack delta to zero'
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
-            "num processors": 1
+            "num processors": 1,
+            "var lss mod": 1.0,
         }})
         expected_message = (
             "Missing argument 'force stack delta to zero' required by Dr16ExpectedFlux"
         )
         with self.assertRaises(ExpectedFluxError) as context_manager:
             Dr16ExpectedFlux(config["expected_flux"])
         self.compare_error_message(context_manager, expected_message)
@@ -769,14 +771,15 @@
         # create a Dr16ExpectedFlux with missing 'limit eta'
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
         }})
         expected_message = (
             "Missing argument 'limit eta' required by Dr16ExpectedFlux"
         )
         with self.assertRaises(ExpectedFluxError) as context_manager:
             Dr16ExpectedFlux(config["expected_flux"])
@@ -785,14 +788,15 @@
         # create a Dr16ExpectedFlux with missing 'limit var lss'
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "0.0, 1.90",
         }})
         expected_message = (
             "Missing argument 'limit var lss' required by Dr16ExpectedFlux"
         )
         with self.assertRaises(ExpectedFluxError) as context_manager:
@@ -802,14 +806,15 @@
         # create a Dr16ExpectedFlux with missing num_iterations
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "0.0, 1.90",
             "limit var lss": "0.0, 1.90",
         }})
         expected_message = (
             "Missing argument 'min qso in fit' required by Dr16ExpectedFlux"
         )
@@ -820,14 +825,15 @@
         # create a Dr16ExpectedFlux with missing num_iterations
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "0.0, 1.90",
             "limit var lss": "0.0, 1.90",
             "min num qso in fit": 100,
         }})
         expected_message = (
             "Missing argument 'num iterations' required by Dr16ExpectedFlux"
@@ -839,14 +845,15 @@
         # create a Dr16ExpectedFlux with missing order
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "0.0, 1.90",
             "limit var lss": "0.0, 1.90",
             "min num qso in fit": 100,
             "num iterations": 5,
         }})
         expected_message = (
@@ -859,14 +866,15 @@
         # create a Dr16ExpectedFlux with missing use_constant_weight
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "0.0, 1.90",
             "limit var lss": "0.0, 1.90",
             "min num qso in fit": 100,
             "num iterations": 5,
             "order": 1,
         }})
@@ -880,14 +888,15 @@
         # create a Dr16ExpectedFlux with missing use_ivar_as_weight
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "0.0, 1.90",
             "limit var lss": "0.0, 1.90",
             "min num qso in fit": 100,
             "num iterations": 5,
             "order": 1,
             "use constant weight": False,
@@ -902,14 +911,15 @@
         # create a Dr16ExpectedFlux instance; case: limit eta and limit var_lss with ()
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "(0.0, 1.90)",
             "limit var lss": "(0.5, 1.40)",
             "min num qso in fit": 100,
             "num iterations": 5,
             "order": 1,
             "use constant weight": False,
@@ -922,14 +932,15 @@
         # create a Dr16ExpectedFlux instance; case: limit eta and limit var_lss with []
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "[0.0, 1.90]",
             "limit var lss": "[0.5, 1.40]",
             "min num qso in fit": 100,
             "num iterations": 5,
             "order": 1,
             "use constant weight": False,
@@ -943,14 +954,15 @@
         # without parenthesis
         config = ConfigParser()
         config.read_dict({"expected_flux": {
             "iter out prefix": f"iter_out_prefix",
             "out dir": f"{THIS_DIR}/results/",
             "num bins variance": 20,
             "num processors": 1,
+            "var lss mod": 1.0,
             "force stack delta to zero": True,
             "limit eta": "0.0, 1.90",
             "limit var lss": "0.5, 1.40",
             "min num qso in fit": 100,
             "num iterations": 5,
             "order": 1,
             "use constant weight": False,
@@ -1121,14 +1133,15 @@
         config = ConfigParser()
         config.read_dict({
             "expected flux": {
                 "iter out prefix": "delta_attributes",
                 "out dir": f"{THIS_DIR}/results/",
                 "num bins variance": 20,
                 "num processors": 1,
+                "var lss mod": 1.0,
             },
         })
         # this should raise an error as Forest variables are not defined
         expected_message = (
             "Forest class variables need to be set before initializing "
             "variables here.")
         with self.assertRaises(ExpectedFluxError) as context_manager:
```

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py` & `picca-7.0.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/scripts_tests.py` & `picca-7.0.0/py/picca/tests/delta_extraction/scripts_tests.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/tests/delta_extraction/test_utils.py` & `picca-7.0.0/py/picca/tests/delta_extraction/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # reset Forest and Pk1dForest class variables
 def reset_forest():
     """Reset the class variables of Forest and Pk1dForest"""
     Forest.wave_solution = None
     Forest.log_lambda_grid = np.array([])
     Forest.log_lambda_rest_frame_grid = np.array([])
     Forest.mask_fields = []
+    Forest.flux_units = None
     Pk1dForest.lambda_abs_igm = None
 
 # setup Forest class variables
 def setup_forest(wave_solution, rebin=1, pixel_step=None):
     """Set Forest class variables
 
     Arguments
@@ -43,15 +44,15 @@
         elif wave_solution == "lin":
             pixel_step = 1
 
     pixel_step *= rebin
     pixel_step_rf = pixel_step
 
     Forest.set_class_variables(3600.0, 5500.0, 1040.0, 1200.0, pixel_step, pixel_step_rf,
-                               wave_solution)
+                               wave_solution, "")
 
 setup_forest("log", rebin=3)
 
 # setup Pk1dForest class variables
 def setup_pk1d_forest(absorber):
     """Set Pk1dForest class variables
```

### Comparing `picca-6.1.0/py/picca/tests/old/test_1_deltas.py` & `picca-7.0.0/py/picca/tests/old/test_1_deltas.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/tests/old/test_4_fitter2.py` & `picca-7.0.0/py/picca/tests/old/test_4_fitter2.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/tests/test_2_pk1d.py` & `picca-7.0.0/py/picca/tests/test_2_pk1d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 import os
 import glob
+import shutil
 import numpy as np
 import fitsio
 import healpy
 
 from picca.utils import userprint
 
 from picca.tests.test_helpers import AbstractTest
@@ -17,15 +18,15 @@
 
     def produce_folder(self):
         """
             Create the necessary folders
         """
 
         userprint("\n")
-        lst_fold = ["/Products/", "/Products/Pk1D/"]
+        lst_fold = ["/Products/", "/Products/Pk1D/", "/Products/meanPk1D/"]
 
         for fold in lst_fold:
             if not os.path.isdir(self._branchFiles + fold):
                 os.mkdir(self._branchFiles + fold)
 
         return
 
@@ -69,10 +70,38 @@
         if self._test:
             path1 = self._masterFiles + "/test_Pk1D/Pk1D_raw.fits.gz"
             path2 = self._branchFiles + "/Products/Pk1D_raw/Pk1D-0.fits.gz"
             self.compare_fits(path1, path2, "picca_Pk1D.py")
 
         return
 
+    def test_meanPk1D(self):
+        """
+            Runs a simple test of Pk1d postprocessing
+        """
+        import picca.bin.picca_Pk1D_postprocess as picca_Pk1D_postprocess
+
+        self._test = True
+        userprint("\n")
+        ### Send
+        #- picca_Pk1D_postprocess.py takes all Pk1D*.fits.gz files in in-dir
+        #  => copy a single file
+        shutil.copy(self._masterFiles + "/test_Pk1D/Pk1D.fits.gz",
+                    self._branchFiles + "/Products/meanPk1D")
+        print(os.listdir(self._branchFiles + "/Products/meanPk1D"))
+        cmd = "picca_Pk1D_postprocess.py "
+        cmd += " --in-dir " + self._branchFiles + "/Products/meanPk1D"
+        cmd += " --output-file " + self._branchFiles + "/Products/meanPk1D/meanPk1D.fits.gz"
+        #- small sample => k,z-bins changed wrt default ones
+        cmd += " --zedge-min 2.1 --zedge-max 3.1 --zedge-bin 0.2"
+        cmd += " --kedge-min 0.015 --kedge-max 0.035 --kedge-bin 0.005"
+        picca_Pk1D_postprocess.main(cmd.split()[1:])
+
+        ### Test
+        if self._test:
+            path1 = self._masterFiles + "/test_Pk1D/meanPk1D.fits.gz"
+            path2 = self._branchFiles + "/Products/meanPk1D/meanPk1D.fits.gz"
+            self.compare_fits(path1, path2, "picca_Pk1D_postprocess.py")
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `picca-6.1.0/py/picca/tests/test_helpers.py` & `picca-7.0.0/py/picca/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/utils.py` & `picca-7.0.0/py/picca/utils.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/wedgize.py` & `picca-7.0.0/py/picca/wedgize.py`

 * *Files identical despite different names*

### Comparing `picca-6.1.0/py/picca/xcf.py` & `picca-7.0.0/py/picca/xcf.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     - compute_wickT1234_pairs
     - compute_wickT1234_pairs
     - compute_xi_1d
 See the respective docstrings for more details
 """
 import numpy as np
 from healpy import query_disc
-from numba import jit, int32
+from numba import njit, int32
 
 from . import constants
 from .utils import userprint
+import warnings
 
 num_bins_r_par = None
 num_bins_r_trans = None
 num_model_bins_r_par = None
 num_model_bins_r_trans = None
 r_par_max = None
 r_par_min = None
@@ -167,93 +168,15 @@
     xi[w] /= weights[w]
     r_par[w] /= weights[w]
     r_trans[w] /= weights[w]
     z[w] /= weights[w]
     return weights, xi, r_par, r_trans, z, num_pairs
 
 
-#-- This has been superseeded by compute_xi_forest_pairs_fast
-#-- and will be deprecated
-@jit
-def compute_xi_forest_pairs(z1, r_comov1, dist_m1, weights1, delta1, z2,
-                            r_comov2, dist_m2, weights2, ang):
-    """Computes the contribution of a given pair of forests to the correlation
-    function.
-
-    Args:
-        z1: array of float
-            Redshift of pixel 1
-        r_comov1: array of float
-            Comoving distance for forest 1 (in Mpc/h)
-        dist_m1: array of float
-            Comoving angular distance for forest 1 (in Mpc/h)
-        weights1: array of float
-            Pixel weights for forest 1
-        delta1: array of float
-            Delta field for forest 1
-        z2: array of float
-            Redshift of pixel 2
-        r_comov2: array of float
-            Comoving distance for forest 2 (in Mpc/h)
-        dist_m2: array of float
-            Comoving angular distance for forest 2 (in Mpc/h)
-        weights2: array of float
-            Pixel weights for forest 2
-        ang: array of float
-            Angular separation between pixels in forests 1 and 2
-
-    Returns:
-        The following variables:
-            rebin_weight: The weight of the correlation function pixels
-                properly rebinned
-            rebin_xi: The correlation function properly rebinned
-            rebin_r_par: The parallel distance of the correlation function
-                pixels properly rebinned
-            rebin_r_trans: The transverse distance of the correlation function
-                pixels properly rebinned
-            rebin_z: The redshift of the correlation function pixels properly
-                rebinned
-            rebin_num_pairs: The number of pairs of the correlation function
-                pixels properly rebinned
-    """
-    if ang_correlation:
-        r_par = r_comov1[:, None] / r_comov2
-        r_trans = ang * np.ones_like(r_par)
-    else:
-        r_par = (r_comov1[:, None] - r_comov2) * np.cos(ang / 2)
-        r_trans = (dist_m1[:, None] + dist_m2) * np.sin(ang / 2)
-    z = (z1[:, None] + z2) / 2
-
-    weights12 = weights1[:, None] * weights2
-    delta_times_weight = (weights1 * delta1)[:, None] * weights2
-
-    w = (r_par > r_par_min) & (r_par < r_par_max) & (r_trans < r_trans_max)
-    r_par = r_par[w]
-    r_trans = r_trans[w]
-    z = z[w]
-    weights12 = weights12[w]
-    delta_times_weight = delta_times_weight[w]
-
-    bins_r_par = ((r_par - r_par_min) / (r_par_max - r_par_min) *
-                  num_bins_r_par).astype(int)
-    bins_r_trans = (r_trans / r_trans_max * num_bins_r_trans).astype(int)
-    bins = bins_r_trans + num_bins_r_trans * bins_r_par
-
-    rebin_xi = np.bincount(bins, weights=delta_times_weight)
-    rebin_weight = np.bincount(bins, weights=weights12)
-    rebin_r_par = np.bincount(bins, weights=r_par * weights12)
-    rebin_r_trans = np.bincount(bins, weights=r_trans * weights12)
-    rebin_z = np.bincount(bins, weights=z * weights12)
-    rebin_num_pairs = np.bincount(bins, weights=(weights12 > 0.))
-
-    return (rebin_weight, rebin_xi, rebin_r_par, rebin_r_trans, rebin_z,
-            rebin_num_pairs)
-
-
-@jit(nopython=True)
+@njit
 def compute_xi_forest_pairs_fast(z1, r_comov1, dist_m1, weights1, delta1, z2,
                                  r_comov2, dist_m2, weights2, ang, rebin_weight,
                                  rebin_xi, rebin_r_par, rebin_r_trans, rebin_z,
                                  rebin_num_pairs):
     """Computes the contribution of a given pair of forests to the correlation
     function.
 
@@ -312,15 +235,15 @@
             delta_times_weight = delta1[i] * weights1[i] * weights2[j]
             weights12 = weights1[i] * weights2[j]
             z = (z1[i] + z2[j]) / 2
 
             bins_r_par = np.floor(
                 (r_par - r_par_min) / (r_par_max - r_par_min) * num_bins_r_par)
             bins_r_trans = np.floor(r_trans / r_trans_max * num_bins_r_trans)
-            bins = np.int(bins_r_trans + num_bins_r_trans * bins_r_par)
+            bins = int(bins_r_trans + num_bins_r_trans * bins_r_par)
 
             rebin_xi[bins] += delta_times_weight
             rebin_weight[bins] += weights12
             rebin_r_par[bins] += r_par * weights12
             rebin_r_trans[bins] += r_trans * weights12
             rebin_z[bins] += z * weights12
             rebin_num_pairs[bins] += 1
@@ -391,157 +314,15 @@
     dmat = dmat.reshape(num_bins_r_par * num_bins_r_trans,
                         num_model_bins_r_par * num_model_bins_r_trans)
 
     return (weights_dmat, dmat, r_par_eff, r_trans_eff, z_eff, weight_eff,
             num_pairs, num_pairs_used)
 
 
-#-- This has been superseeded by compute_dmat_forest_pairs_fast
-#-- and will be deprecated
-@jit
-def compute_dmat_forest_pairs(log_lambda1, r_comov1, dist_m1, z1, weights1,
-                              r_comov2, dist_m2, z2, weights2, ang,
-                              weights_dmat, dmat, r_par_eff, r_trans_eff, z_eff,
-                              weight_eff):
-    """Computes the contribution of a given pair of forests-quasar to the
-    distortion matrix.
-
-    Args:
-        log_lambda1: array of float
-            Logarithm of the wavelength (in Angs) for forest 1
-        r_comov1: array of floats
-            Comoving distance (in Mpc/h) for forest 1
-        dist_m1: array of floats
-            Angular distance for forest 1
-        z1: array of floats
-            Redshifts for forest 1
-        weights1: array of floats
-            Weights for forest 1
-        r_comov2: array of floats
-            Comoving distance (in Mpc/h) for forest 2
-        dist_m2: array of floats
-            Angular distance for forest 2
-        z2: array of floats
-            Redshifts for forest 2
-        weights2: array of floats
-            Weights for forest 2
-        ang: array of floats
-            Angular separation between pixels in forests 1 and 2
-        weights_dmat: array of floats
-            Total weight in the distortion matrix pixels
-        dmat: array of floats
-            The distortion matrix
-        r_par_eff: array of floats
-            Effective parallel distance for the distortion matrix bins
-        r_trans_eff: array of floats
-            Effective transverse distance for the distortion matrix bins
-        z_eff: array of floats
-            Effective redshift for the distortion matrix bins
-        weight_eff: array of floats
-            Effective weight of the distortion matrix pixels
-    """
-    # find distances between pixels
-    r_par = (r_comov1[:, None] - r_comov2) * np.cos(ang / 2)
-    r_trans = (dist_m1[:, None] + dist_m2) * np.sin(ang / 2)
-    z = (z1[:, None] + z2) / 2.
-    w = (r_par > r_par_min) & (r_par < r_par_max) & (r_trans < r_trans_max)
-
-    # locate bins pixels are contributing to (correlation bins)
-    bins_r_par = ((r_par - r_par_min) / (r_par_max - r_par_min) *
-                  num_bins_r_par).astype(int)
-    bins_r_trans = (r_trans / r_trans_max * num_bins_r_trans).astype(int)
-    bins = bins_r_trans + num_bins_r_trans * bins_r_par
-    bins = bins[w]
-
-    # locate bins pixels are contributing to (model bins)
-    model_bins_r_par = ((r_par - r_par_min) / (r_par_max - r_par_min) *
-                        num_model_bins_r_par).astype(int)
-    model_bins_r_trans = (r_trans / r_trans_max *
-                          num_model_bins_r_trans).astype(int)
-    model_bins = model_bins_r_trans + num_model_bins_r_trans * model_bins_r_par
-    model_bins = model_bins[w]
-
-    # compute useful auxiliar variables to speed up computation of eta
-    # (equation 6 of du Mas des Bourboux et al. 2020)
-
-    # denominator second term in equation 6 of du Mas des Bourboux et al. 2020
-    sum_weights1 = weights1.sum()
-
-    # mean of log_lambda
-    mean_log_lambda1 = np.average(log_lambda1, weights=weights1)
-
-    # log_lambda minus its mean
-    log_lambda_minus_mean1 = log_lambda1 - mean_log_lambda1
-
-    # denominator third term in equation 6 of du Mas des Bourboux et al. 2020
-    sum_weights_square_log_lambda_minus_mean1 = (
-        weights1 * log_lambda_minus_mean1**2).sum()
-
-    # auxiliar variables to loop over distortion matrix bins
-    num_pixels1 = len(log_lambda1)
-    num_pixels2 = len(r_comov2)
-    ij = np.arange(num_pixels1)[:, None] + num_pixels1 * np.arange(num_pixels2)
-    ij = ij[w]
-
-    weights12 = weights1[:, None] * weights2
-    weights12 = weights12[w]
-
-    rebin = np.bincount(model_bins, weights=weights12 * r_par[w])
-    r_par_eff[:rebin.size] += rebin
-    rebin = np.bincount(model_bins, weights=weights12 * r_trans[w])
-    r_trans_eff[:rebin.size] += rebin
-    rebin = np.bincount(model_bins, weights=weights12 * z[w])
-    z_eff[:rebin.size] += rebin
-    rebin = np.bincount(model_bins, weights=weights12)
-    weight_eff[:rebin.size] += rebin
-
-    rebin = np.bincount(bins, weights=weights12)
-    weights_dmat[:len(rebin)] += rebin
-
-    # Combining equation 22 and equation 6 of du Mas des Bourboux et al. 2020
-    # we find an equation with 3 terms comming from the product of two eta
-    # The variables below stand for 2 of these 3 terms (the first one is
-    # pretty trivial) and are named to match those of module cf
-
-    # first eta, second term: weight/sum(weights)
-    eta2 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans * num_pixels2)
-    # first eta, third term: (non-zero only for order=1)
-    #   weight*(Lambda-bar(Lambda))*(Lambda-bar(Lambda))/
-    eta4 = np.zeros(num_model_bins_r_par * num_model_bins_r_trans * num_pixels2)
-
-    # compute the contributions to the distortion matrix
-    rebin = np.bincount(
-        ((ij - ij % num_pixels1) // num_pixels1 + num_pixels2 * model_bins),
-        weights=((weights1[:, None] * np.ones(num_pixels2))[w] / sum_weights1))
-    eta2[:len(rebin)] += rebin
-    rebin = np.bincount(
-        ((ij - ij % num_pixels1) // num_pixels1 + num_pixels2 * model_bins),
-        weights=(((weights1 * log_lambda_minus_mean1)[:, None] *
-                  np.ones(num_pixels2))[w] /
-                 sum_weights_square_log_lambda_minus_mean1))
-    eta4[:len(rebin)] += rebin
-
-    # Now add all the contributions together
-    unique_model_bins = np.unique(model_bins)
-    for index, (bin, model_bin) in enumerate(zip(bins, model_bins)):
-        # first eta, first term: kronecker delta
-        dmat[model_bin + num_model_bins_r_par * num_model_bins_r_trans *
-             bin] += weights12[index]
-        i = ij[index] % num_pixels1
-        j = (ij[index] - i) // num_pixels1
-        # rest of the terms
-        for unique_model_bin in unique_model_bins:
-            dmat[unique_model_bin + num_model_bins_r_par *
-                 num_model_bins_r_trans * bin] -= weights12[index] * (
-                     eta2[j + num_pixels2 * unique_model_bin] +
-                     eta4[j + num_pixels2 * unique_model_bin] *
-                     log_lambda_minus_mean1[i])
-
-
-@jit(nopython=True)
+@njit
 def compute_dmat_forest_pairs_fast(log_lambda1, r_comov1, dist_m1, z1, weights1,
                                    r_comov2, dist_m2, z2, weights2, ang,
                                    weights_dmat, dmat, r_par_eff, r_trans_eff,
                                    z_eff, weight_eff, order1):
 
     #-- First, determine how many relevant pixel pairs for speed up
     num_pairs = 0
@@ -927,112 +708,15 @@
                                       aux_r_comov2, r_comov3, r_comov4,
                                       weights1, aux_weights2, weights3,
                                       weights4, aux_thingid2, thingid4, t5, t6)
 
     return weights_wick, num_pairs_wick, num_pairs, num_pairs_used, t1, t2, t3, t4, t5, t6
 
 
-#@jit   #this will be removed in the future, it's an older implementation that does not work properly with current numba
-def compute_wickT1234_pairs_slow(ang, r_comov1, r_comov2, z1, z2, weights1,
-                                 weights2, weighted_xi_1d_1, weights_wick,
-                                 num_pairs_wick, t1, t2, t3, t4):
-    """
-    Computes the Wick expansion terms 1, 2, and 3 of a given pair of forests
-
-    Each of the terms represents the contribution of different type of pairs as
-    illustrated in figure A.1 from Delubac et al. 2015
-
-    Args:
-        ang: array of floats
-            Angular separation between pixels in forests 1 and 2
-        r_comov1: array of floats
-            Comoving distance (in Mpc/h) for forest 1
-        r_comov2: array of floats
-            Comoving distance (in Mpc/h) for forest 2
-        z1: array of floats
-            Redshifts for forest 1
-        z2: array of floats
-            Redshifts for forest 2
-        weights1: array of floats
-            Weights for forest 1
-        weights2: array of floats
-            Weights for forest 2
-        weighted_xi_1d_1: array of floats
-            Weighted 1D correlation function for forest 1
-        weights_wick: array of floats
-            Total weight in the covariance matrix pixels
-        num_pairs_wick: array of floats
-            Total number of pairs in the covariance matrix pixels
-        t1: array of floats
-            Wick expansion, term 1
-        t2: array of floats
-            Wick expansion, term 2
-        t3: array of floats
-            Wick expansion, term 3
-        t4: array of floats
-            Wick expansion, term 4
-    """
-    r_par = (r_comov1[:, None] - r_comov2) * np.cos(ang / 2.)
-    r_trans = (r_comov1[:, None] + r_comov2) * np.sin(ang / 2.)
-    z_weight_evol1 = ((1. + z1) / (1. + z_ref))**(alpha - 1.)
-    z_weight_evol2 = ((1. + z2) / (1. + z_ref))**(alpha_obj - 1.)
-    weights12 = weights1[:, None] * weights2
-    weight1 = weights1[:, None] * np.ones(len(r_comov2))
-    index_delta = np.arange(r_comov1.size)[:, None] * np.ones(len(r_comov2),
-                                                              dtype='int')
-    index_obj = (np.ones(r_comov1.size, dtype='int')[:, None] *
-                 np.arange(len(r_comov2)))
-
-    bins_r_par = ((r_par - r_par_min) / (r_par_max - r_par_min) *
-                  num_bins_r_par).astype(int)
-    bins_r_trans = (r_trans / r_trans_max * num_bins_r_trans).astype(int)
-    bins_forest = bins_r_trans + num_bins_r_trans * bins_r_par
-
-    w = (r_par > r_par_min) & (r_par < r_par_max) & (r_trans < r_trans_max)
-    if w.sum() == 0:
-        return
-
-    bins_forest = bins_forest[w]
-    weights12 = weights12[w]
-    weight1 = weight1[w]
-    index_delta = index_delta[w]
-    index_obj = index_obj[w]
-
-    for index1 in range(bins_forest.size):
-        p1 = bins_forest[index1]
-        i1 = index_delta[index1]
-        j1 = index_obj[index1]
-        weights_wick[p1] += weights12[index1]
-        num_pairs_wick[p1] += 1
-        t1[p1,
-           p1] += weights12[index1]**2 / weight1[index1] * z_weight_evol1[i1]
-
-        for index2 in range(index1 + 1, bins_forest.size):
-            p2 = bins_forest[index2]
-            i2 = index_delta[index2]
-            j2 = index_obj[index2]
-            if j1 == j2:
-                prod = weighted_xi_1d_1[i1, i2] * (z_weight_evol2[j1]**2)
-                t2[p1, p2] += prod
-                t2[p2, p1] += prod
-            elif i1 == i2:
-                prod = (weights12[index1] * weights12[index2] /
-                        weight1[index1] * z_weight_evol1[i1])
-                t3[p1, p2] += prod
-                t3[p2, p1] += prod
-            else:
-                prod = (weighted_xi_1d_1[i1, i2] * z_weight_evol2[j1] *
-                        z_weight_evol2[j2])
-                t4[p1, p2] += prod
-                t4[p2, p1] += prod
-
-    return
-
-
-@jit
+@njit
 def compute_wickT56_pairs(ang12, ang34, ang13, r_comov1, r_comov2, r_comov3,
                           r_comov4, weights1, weights2, weights3, weights4,
                           thingid2, thingid4, t5, t6):
     """
     Compute the Wick covariance matrix for the object-pixel cross-correlation
     for the T5 and T6 diagrams: i.e. the contribution of the 3D auto-correlation
     to the covariance matrix
@@ -1210,15 +894,15 @@
     xi_1d[w] /= weights1d[w]
     r_par1d[w] /= weights1d[w]
     z[w] /= weights1d[w]
 
     return weights1d, xi_1d, r_par1d, z, num_pairs1d
 
 
-@jit(nopython=True)
+@njit
 def compute_wickT1234_pairs(ang, r_comov1, r_comov2, z1, z2, weights1, weights2,
                             weighted_xi_1d_1, weights_wick, num_pairs_wick, t1,
                             t2, t3, t4):
     """
     Computes the Wick expansion terms 1, 2, and 3 of a given pair of forests
 
     Each of the terms represents the contribution of different type of pairs as
```

### Comparing `picca-6.1.0/py/picca.egg-info/PKG-INFO` & `picca-7.0.0/py/picca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 6.1.0
+Version: 7.0.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
 Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -160,14 +160,16 @@
 
 ### For Developers
 Before submitting a PR please make sure to:
 1. Check the tutorials. Update them if necessary (typically the tutorial `picca_delta_extraction_configuration_tutorial` will need to be updated.
 2. Update the data model
 3. For every file you have modified run
    ```
-   yapf --style google file.py -i 
+   yapf --style google file.py -i
    ```
    to ensure the coding styles are maintained.
 4. Consider using pylint to help in the debug process. From the repo folder run
    ```
-   pylint py/picca/delta_extraction/**/*py
+   pylint py/picca/delta_extraction/
+   pylint py/picca/pk1d/
    ```
+   depending on the module you are working on.
```

### Comparing `picca-6.1.0/py/picca.egg-info/SOURCES.txt` & `picca-7.0.0/py/picca.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
 py/picca/fitter2/priors.py
 py/picca/fitter2/sampler.py
 py/picca/fitter2/utils.py
 py/picca/fitter2/xi.py
 py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
 py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
 py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
+py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits
 py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
 py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
 py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
 py/picca/pk1d/compute_pk1d.py
 py/picca/pk1d/postproc_pk1d.py
 py/picca/pk1d/prep_pk1d.py
 py/picca/pk1d/utils.py
```

### Comparing `picca-6.1.0/setup.py` & `picca-7.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_namespace_packages, setup
 from pathlib import Path
 
 scripts = sorted(glob.glob('bin/picca*'))
 
 description = (f"Package for Igm Cosmological-Correlations Analyses\n"
-              "commit hash: {git.Repo('.').head.object.hexsha}")
+               f"commit hash: {git.Repo('.').head.object.hexsha}")
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 exec(open('py/picca/_version.py').read())
 version = __version__
 
 setup(name="picca",
```

