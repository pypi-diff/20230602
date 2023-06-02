# Comparing `tmp/django_marina-23.4.tar.gz` & `tmp/django_marina-23.5.tar.gz`

## Comparing `django_marina-23.4.tar` & `django_marina-23.5.tar`

### file list

```diff
@@ -1,298 +1,319 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 django_marina-23.4/.DS_Store
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 django_marina-23.4/.readthedocs.yml
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 django_marina-23.4/CHANGELOG.md
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 django_marina-23.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 django_marina-23.4/Makefile
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/manage.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 django_marina-23.4/requirements-dev.txt
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 django_marina-23.4/tox.ini
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 django_marina-23.4/.github/dependabot.yml
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 django_marina-23.4/.github/workflows/dependabot-auto-approve-and-merge.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_marina-23.4/.github/workflows/test.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1024c46eeebfddd9
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/11c104e958fca970
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/11f1cbea2e7c1ef3
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/11f70c0dd6e655e2
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/13083e3d792d3151
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/133247f993b34e0d
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/142785e97b4cf74f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/143e80cb705de0b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/154ac96b7a9c4c26
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/15d1a8f69df6395
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/18d06dc21b74bfd2
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/190b08956f165527
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/19a968c1275adfdf
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1abea56c7d1ab303
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1b1308a706406783
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1b53ba39e1f57e58
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1bb1eb28ecbe1fd
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1c70287f931fd26f
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1d5212aad6aa1740
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1e7643c29d4d410
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1fc507464a0e6288
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/221f399498345b28
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/22d256aa42f4eeda
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2543204f398cb739
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2623a935f18c2389
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/26cb16652fde39d7
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/27bf07d792f63194
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2a86af9fbe9f5871
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2ac6b5f709e2223a
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2ad7e8df3f10e03
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2b90dd378c3d45bb
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2cd00f2b457dca82
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2d486d58c50ef5d7
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2d9464ac3cccc68b
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2d9b1f2723f75b46
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2e2d73549bcbd61e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/30cac57ee17b54d1
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/33869e8b2a934d4
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/33fbb16a8b89fbcc
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3486a583c5aae9c7
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/36e6efd54df5afda
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/36f56c23a36b0c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3867c51af477cf8d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/398b3cd46b054c5f
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3d59ae216a1c8181
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3ed6018cf5986c69
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3f0a57d8e69fb2da
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/41e0cb6bd3f98ee7
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/426cc96891369f10
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/42c20bab2f436d88
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/4313e83d0210a742
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/44097d4abe3025ec
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/44942ac379b31cf6
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/45ce23f60dd162f5
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/46a11b89a78d7ffd
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/472c3f1f2242535d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/47443eca57e44398
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/47594234b4ccf212
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/480bf6ada218a25
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/480cc16ccd1404aa
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/487962ffa1611e85
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/497399ebe720f9f7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/49a09ccc457b7f8b
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/4b66ca14605f82bd
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/4cf1f7dc83495933
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/4e3954633a0bf2c7
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5146d8a06953ab21
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/515c8d28fb372ac5
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/51dc5c6c713b9817
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/52250ca9a5c62bef
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5486c94fca9b1c86
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/55430fc79027d1a4
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5594aca919406ac5
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/55dd803e72f04fe6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/56c1a9758a8f943b
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/56f9652bf17b47c8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/578c047a3a0f989d
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/583248f9f63239ea
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5878ea8c01a175da
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/58c51b85d06e4d50
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5abb45f46cb2832b
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5bf79e77047465ba
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5cd5ffb8cf153388
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/602da119750b3c0f
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/608f1cb6c8d08d58
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/612cc2c4101efdd3
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/619e52f91b053290
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/630db95a305be885
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/630fe3444c7a9094
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6482a66319d710a8
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/64c23f13928d78e5
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/65afbecf5a75a81f
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/67b3a5b865e402f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/68b9472faaa1823f
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/69641bc8de3b442
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6a3063597a8f25f5
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6cb371e95d06ba12
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6df151341fbfb8fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6e212e1d6037d4e9
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6e87d3cd8e10064c
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6f068a2700da29d6
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6faf75218bac593c
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6fe58ded543446d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7099ef80a1047a93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/72063909866fadb2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/73da658a4784702c
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/73e7a5b4e3ea202b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/74fd2e3339bcf92c
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/75b4b597d009513b
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/76f0cbdaaae53850
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/77489570a19c7986
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/797af1fa82c5ae92
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7a556dfd6c4b2fb
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7ac66889f8779e3d
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7bd79d720f2a2380
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7d149554663b0573
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7f6beb0d17265650
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/81920bc911181e1d
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/829977667da261ed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/82a0d542c75229cc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/830bb9643cae8f59
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/857794017ccd3c9a
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/85d8fe88d14c01ed
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8aff278ff88851fc
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8c720e348bd5351
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8cecabf7e2e19ce0
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8de8c7f68e3bd5e8
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8ebd74a1c0aa90ef
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8f67a558c3de3d82
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8f701c80389b53e5
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/915d0a3fd2d99117
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/91883a456f61783b
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/91faf7bebf5a0364
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9208aef60c2e233d
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/92293a3e521c27c2
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/93357306a59c700
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/933b6c3b6533ae7d
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/94e658d64ad183ca
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/95862bd589a59374
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/97353516d8c365c2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/97a2fe8e0165782a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/984410d645d90d0f
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9c0c889ee7eadadf
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9c25e661e2484ef9
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9d74f5d5028ef03e
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9ef744015358e12d
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a040d7c9218123ca
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a04c25f87109c873
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a156d024a5d30cab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a313e9f602097400
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a42fb8397a68c523
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a4cdec6301ee4304
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a5790219187b8cd3
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a57a669de607793f
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a62363bb26f41068
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a85868f8fbb6c1ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a951830ea8bdeb48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/abe363314a4cd4c3
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ace934c109ecdcbc
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ad78c14c4521b7e3
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ae55027ec67feed3
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ae7d2ea132c983db
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/aec4a4843275828b
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/aed55d37c0eca6f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b07b696460410c7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b0eb3a72a03e2dce
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b13e7fe605f50044
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b176e5c537beec8f
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b28fa1841f276735
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b2c1c0a97e5c5a2d
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b2e33bf0db76941f
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b3836daea2af04d4
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b3ee4610a623f211
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b7d63c347a5fe5f4
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b9c6cb6048b64e78
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ba0e2ad2cf9080ec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/bb6c759e4234e819
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/bba357a2a553736b
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/bcd30fab31815a22
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/be51610ec1a12bc5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/bfec558574a0ce1b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c00d832ea903c6b6
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c0afc5ec6a4435df
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c0eb8a3bdca2990a
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c0f033672632e320
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c1b467e3796f4775
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c31fda6c6821b979
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c492c7e2ddc3dcd6
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c657a362d04d077b
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c7d52283449db1df
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c7db73965c27bd00
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c908f0a8b8ed958c
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c90e56c8d6ff7fd0
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ca76bb035fabb17a
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cb31010082d0f9ca
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cd5d973a118b540c
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cd6f88b3f5a646f7
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ce4b8e3da3bd4378
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cec6d33d480a81c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cf9d347a029f0c4c
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d197a4566a9aeb60
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d2d267fd74594e2b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d305c95ff130f87a
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d3b50f2bd146c177
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d421acad960b4b1d
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d42337bba7e72aa2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d541581fe3c63f5b
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d694971b4d6e1708
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d782ea9dfb88a52b
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d89f6a905ffeb903
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d8bbf3c13b622b23
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d8f0c9ea00f7d767
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d955d31049876a9e
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/dcdbcc59efe7feb8
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/dd5a06354ad32b52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/dd606e7425a82b27
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/df64d7830e598803
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e594e679f8c51a75
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e6e171d221302e2f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e832b40f0167219d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e8422fbc9844014
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e91ae7e7dfb71ee9
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e9d43a4ab7777f4b
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/eb93428e64dfc11d
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ebf6d3e0e21cd288
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ec4e0461e9f0bb0a
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ed90c1891d1c4c28
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/edf638e5425bc575
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ee5c67b2c7b04b78
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ee5d8217eb6b77ce
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f0092ea403d607dd
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f0dba3adf8827dcd
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f2ebff90091264a9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f380f7e060fff472
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f3b226ff878e709b
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f4cf21d861535529
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f6b3728a298392a6
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f821074c685e8812
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f8c4de0113634448
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f966030a24ff0426
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fa7aa006d1768adf
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fc4989c1ceacb12c
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fd2e452f49df5be2
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fd8e2a019a79dee8
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fd92e20ca5a2e7f
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fd9f160121419046
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fe2baf07747246f2
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ff2d2a2e93c4719
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 django_marina-23.4/.vscode/configurationCache.log
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.vscode/dryrun.log
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 django_marina-23.4/.vscode/settings.json
--rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 django_marina-23.4/.vscode/targets.log
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_marina-23.4/docs/changelog.rst
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 django_marina-23.4/docs/conf.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 django_marina-23.4/docs/contributing.rst
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_marina-23.4/docs/db.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 django_marina-23.4/docs/index.rst
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_marina-23.4/docs/requirements.txt
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 django_marina-23.4/docs/test.rst
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 django_marina-23.4/example/README.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/__about__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/db/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/db/migrations.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/db/models.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/test/__init__.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/test/clients.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/test/test_cases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_marina-23.4/tests/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 django_marina-23.4/tests/models.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_db.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_extended_client.py
--rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_extended_test_case.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_imports.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_version.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_marina-23.4/tests/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_marina-23.4/tests/app/__init__.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 django_marina-23.4/tests/app/settings.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 django_marina-23.4/tests/app/urls.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 django_marina-23.4/tests/app/views.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 django_marina-23.4/.gitignore
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 django_marina-23.4/LICENSE
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_marina-23.4/README.md
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 django_marina-23.4/pyproject.toml
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 django_marina-23.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 django_marina-23.5/.DS_Store
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 django_marina-23.5/.readthedocs.yml
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 django_marina-23.5/CHANGELOG.md
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 django_marina-23.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 django_marina-23.5/Makefile
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/manage.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 django_marina-23.5/.github/dependabot.yml
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 django_marina-23.5/.github/workflows/dependabot-auto-approve-and-merge.yml
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 django_marina-23.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1024c46eeebfddd9
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/11c104e958fca970
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/11f1cbea2e7c1ef3
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/11f70c0dd6e655e2
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/13083e3d792d3151
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/133247f993b34e0d
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/142785e97b4cf74f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/143e80cb705de0b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/154ac96b7a9c4c26
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/15d1a8f69df6395
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/18d06dc21b74bfd2
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/190b08956f165527
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/19a968c1275adfdf
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1abea56c7d1ab303
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1b1308a706406783
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1b53ba39e1f57e58
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1bb1eb28ecbe1fd
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1c70287f931fd26f
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1d0678cc684da9de
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1d5212aad6aa1740
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1e7643c29d4d410
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/1fc507464a0e6288
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/221f399498345b28
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/22d256aa42f4eeda
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2543204f398cb739
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/254d7829f97b85e6
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2623a935f18c2389
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/26cb16652fde39d7
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/27bf07d792f63194
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2a86af9fbe9f5871
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2ac6b5f709e2223a
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2ad7e8df3f10e03
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2b90dd378c3d45bb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2cd00f2b457dca82
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2d486d58c50ef5d7
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2d9464ac3cccc68b
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2d9b1f2723f75b46
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/2e2d73549bcbd61e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/30cac57ee17b54d1
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/33869e8b2a934d4
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/33fbb16a8b89fbcc
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/3486a583c5aae9c7
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/36e6efd54df5afda
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/36f56c23a36b0c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/3867c51af477cf8d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/398b3cd46b054c5f
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/3d59ae216a1c8181
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/3ed6018cf5986c69
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/3f0a57d8e69fb2da
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/41e0cb6bd3f98ee7
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/426cc96891369f10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/42c20bab2f436d88
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/4313e83d0210a742
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/44097d4abe3025ec
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/44942ac379b31cf6
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/45ce23f60dd162f5
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/46a11b89a78d7ffd
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/472c3f1f2242535d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/47443eca57e44398
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/47594234b4ccf212
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/480bf6ada218a25
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/480cc16ccd1404aa
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/487962ffa1611e85
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/497399ebe720f9f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/49a09ccc457b7f8b
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/4a09de738e609540
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/4b66ca14605f82bd
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/4cf1f7dc83495933
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/4e3954633a0bf2c7
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/5146d8a06953ab21
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/515c8d28fb372ac5
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/51dc5c6c713b9817
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/52250ca9a5c62bef
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/5486c94fca9b1c86
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/55430fc79027d1a4
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/5594aca919406ac5
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/55dd803e72f04fe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/56c1a9758a8f943b
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/56f9652bf17b47c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/578c047a3a0f989d
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/583248f9f63239ea
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/5878ea8c01a175da
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/58c51b85d06e4d50
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/5abb45f46cb2832b
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/5b557057006ee4c8
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/5bf79e77047465ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/5cd5ffb8cf153388
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/602da119750b3c0f
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/608f1cb6c8d08d58
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/612cc2c4101efdd3
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/619e52f91b053290
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/630db95a305be885
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/630fe3444c7a9094
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6482a66319d710a8
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/64c23f13928d78e5
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/65afbecf5a75a81f
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/67b3a5b865e402f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/68b8f5d7044e15db
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/68b9472faaa1823f
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/69641bc8de3b442
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/69c186f16cb5d261
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6a3063597a8f25f5
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6cb371e95d06ba12
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6df151341fbfb8fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6e212e1d6037d4e9
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6e87d3cd8e10064c
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6f068a2700da29d6
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6faf75218bac593c
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/6fe58ded543446d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/7099ef80a1047a93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/72063909866fadb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/73da658a4784702c
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/73e7a5b4e3ea202b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/74fd2e3339bcf92c
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/75b4b597d009513b
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/76f0cbdaaae53850
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/77489570a19c7986
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/77d1b83bbba6912e
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/797af1fa82c5ae92
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/7a556dfd6c4b2fb
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/7ac66889f8779e3d
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/7bd79d720f2a2380
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/7c39318cadfc4952
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/7d149554663b0573
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/7f6beb0d17265650
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/81920bc911181e1d
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/829977667da261ed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/82a0d542c75229cc
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/82a4358a6d1b4eda
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/830bb9643cae8f59
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/857794017ccd3c9a
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/85d8fe88d14c01ed
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/8aff278ff88851fc
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/8c720e348bd5351
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/8cecabf7e2e19ce0
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/8de8c7f68e3bd5e8
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/8ebd74a1c0aa90ef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/8f67a558c3de3d82
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/8f701c80389b53e5
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/915d0a3fd2d99117
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/91883a456f61783b
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/91faf7bebf5a0364
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/9208aef60c2e233d
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/92293a3e521c27c2
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/93357306a59c700
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/933b6c3b6533ae7d
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/94e658d64ad183ca
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/95862bd589a59374
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/97353516d8c365c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/97a2fe8e0165782a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/984410d645d90d0f
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/9c0c889ee7eadadf
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/9c25e661e2484ef9
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/9d74f5d5028ef03e
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/9ef744015358e12d
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/9ff597d08d64ba20
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a040d7c9218123ca
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a04c25f87109c873
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a156d024a5d30cab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a313e9f602097400
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a42fb8397a68c523
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a4cdec6301ee4304
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a5790219187b8cd3
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a57a669de607793f
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a62363bb26f41068
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a6e737e20f342efd
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a85868f8fbb6c1ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a951830ea8bdeb48
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/a953ddeea5a097b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/abe363314a4cd4c3
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ac3e240235fba862
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ace934c109ecdcbc
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ad78c14c4521b7e3
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ae55027ec67feed3
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ae7d2ea132c983db
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/aec4a4843275828b
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/aed55d37c0eca6f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b07b696460410c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b0eb3a72a03e2dce
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b13e7fe605f50044
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b176e5c537beec8f
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b28fa1841f276735
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b2c1c0a97e5c5a2d
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b2e33bf0db76941f
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b3836daea2af04d4
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b3ee4610a623f211
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b7d63c347a5fe5f4
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/b9c6cb6048b64e78
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ba0e2ad2cf9080ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/bb6c759e4234e819
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/bba357a2a553736b
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/bcd30fab31815a22
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/be51610ec1a12bc5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/bfec558574a0ce1b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c00d832ea903c6b6
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c0afc5ec6a4435df
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c0eb8a3bdca2990a
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c0f033672632e320
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c1b467e3796f4775
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c20b8d5ee3b1e1f7
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c31fda6c6821b979
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c492c7e2ddc3dcd6
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c657a362d04d077b
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c72fc4a092c3bc14
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c7d52283449db1df
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c7db73965c27bd00
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c908f0a8b8ed958c
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c90e56c8d6ff7fd0
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/c9d87330408fee3b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ca528a4e183171ac
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ca76bb035fabb17a
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/cb31010082d0f9ca
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/cd5d973a118b540c
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/cd6f88b3f5a646f7
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ce4b8e3da3bd4378
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/cec6d33d480a81c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/cf9d347a029f0c4c
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d197a4566a9aeb60
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d2d267fd74594e2b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d305c95ff130f87a
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d3b50f2bd146c177
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d421acad960b4b1d
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d42337bba7e72aa2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d541581fe3c63f5b
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d694971b4d6e1708
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d782ea9dfb88a52b
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d89f6a905ffeb903
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d8bbf3c13b622b23
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d8f0c9ea00f7d767
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d955d31049876a9e
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d97c2fd762b4e13
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/d98edb5026e83292
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/dcdbcc59efe7feb8
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/dd5a06354ad32b52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/dd606e7425a82b27
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/df64d7830e598803
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e4bb8bb613f4f8dc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e52a4e9432b1d6dc
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e594e679f8c51a75
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e6e171d221302e2f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e832b40f0167219d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e8422fbc9844014
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e8dd2cf487f9f102
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e91ae7e7dfb71ee9
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/e9d43a4ab7777f4b
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/eb93428e64dfc11d
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ebf6d3e0e21cd288
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ec4e0461e9f0bb0a
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ed90c1891d1c4c28
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/edf638e5425bc575
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ee5c67b2c7b04b78
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ee5d8217eb6b77ce
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f0092ea403d607dd
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f0dba3adf8827dcd
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f2ebff90091264a9
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f30a52484b9f6917
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f380f7e060fff472
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f3b226ff878e709b
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f4cf21d861535529
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f6b3728a298392a6
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f821074c685e8812
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f8c4de0113634448
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/f966030a24ff0426
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/fa7aa006d1768adf
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/fc4989c1ceacb12c
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/fd2e452f49df5be2
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/fd8e2a019a79dee8
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/fd92e20ca5a2e7f
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/fd9f160121419046
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/fe2baf07747246f2
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.5/.ruff_cache/content/ff2d2a2e93c4719
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_marina-23.5/.vscode/configurationCache.log
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.5/.vscode/dryrun.log
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 django_marina-23.5/.vscode/settings.json
+-rw-r--r--   0        0        0    10058 2020-02-02 00:00:00.000000 django_marina-23.5/.vscode/targets.log
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 django_marina-23.5/docs/.DS_Store
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_marina-23.5/docs/changelog.rst
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 django_marina-23.5/docs/conf.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 django_marina-23.5/docs/contributing.rst
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_marina-23.5/docs/db.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 django_marina-23.5/docs/index.rst
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 django_marina-23.5/docs/test.rst
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 django_marina-23.5/example/README.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_marina-23.5/src/django_marina/__about__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 django_marina-23.5/src/django_marina/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 django_marina-23.5/src/django_marina/db/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 django_marina-23.5/src/django_marina/db/migrations.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 django_marina-23.5/src/django_marina/db/models.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 django_marina-23.5/src/django_marina/test/__init__.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 django_marina-23.5/src/django_marina/test/clients.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 django_marina-23.5/src/django_marina/test/test_cases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_marina-23.5/tests/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 django_marina-23.5/tests/models.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 django_marina-23.5/tests/test_db.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 django_marina-23.5/tests/test_extended_client.py
+-rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 django_marina-23.5/tests/test_extended_test_case.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 django_marina-23.5/tests/test_imports.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 django_marina-23.5/tests/test_version.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_marina-23.5/tests/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_marina-23.5/tests/app/__init__.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 django_marina-23.5/tests/app/settings.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 django_marina-23.5/tests/app/urls.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 django_marina-23.5/tests/app/views.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 django_marina-23.5/.gitignore
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 django_marina-23.5/LICENSE
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_marina-23.5/README.md
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 django_marina-23.5/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 django_marina-23.5/PKG-INFO
```

### Comparing `django_marina-23.4/.DS_Store` & `django_marina-23.5/.DS_Store`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0005  ................
 00000050: 0000 0001 0000 1000 6473 636c 626f 6f6c  ........dsclbool
 00000060: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,34 +26,34 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00000200: 0000 0000 0000 0000 0000 0005 0000 0004  ................
 00000210: 0064 0069 0073 0074 6473 636c 626f 6f6c  .d.i.s.tdsclbool
 00000220: 0100 0000 0400 6400 6900 7300 7476 5372  ......d.i.s.tvSr
 00000230: 6e6c 6f6e 6700 0000 0100 0000 0400 6400  nlong.........d.
 00000240: 6f00 6300 7362 7773 7062 6c6f 6200 0000  o.c.sbwspblob...
-00000250: b962 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+00000250: ba62 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
 00000260: 0707 0907 0b07 5d53 686f 7753 7461 7475  ......]ShowStatu
 00000270: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
 00000280: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
 00000290: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
 000002a0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
 000002b0: 5b53 686f 7753 6964 6562 6172 0909 0809  [ShowSidebar....
-000002c0: 5f10 197b 7b37 3231 2c20 3330 327d 2c20  _..{{721, 302}, 
-000002d0: 7b31 3438 322c 2038 3939 7d7d 0908 1523  {1482, 899}}...#
-000002e0: 2f3b 525f 6b6c 6d6e 6f8b 0000 0000 0000  /;R_klmno.......
-000002f0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 008c 0000 0004 0064  ...............d
-00000310: 006f 0063 0073 7653 726e 6c6f 6e67 0000  .o.c.svSrnlong..
-00000320: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 5f10 1a7b 7b31 3238 352c 2032 3037 7d2c  _..{{1285, 207},
+000002d0: 207b 3131 3537 2c20 3635 307d 7d09 0815   {1157, 650}}...
+000002e0: 232f 3b52 5f6b 6c6d 6e6f 8c00 0000 0000  #/;R_klmno......
+000002f0: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 8d00 0000 0400  ................
+00000310: 6400 6f00 6300 7364 7363 6c62 6f6f 6c01  d.o.c.sdsclbool.
+00000320: 0000 0004 0064 006f 0063 0073 7653 726e  .....d.o.c.svSrn
+00000330: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `django_marina-23.4/CHANGELOG.md` & `django_marina-23.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## 23.5 (2023-06-02)
+
+- Improve and fix CI on GitHub Axctions (#367, #374, #378).
+- Reinstate coveralls (#369).
+- Fix Read the Docs integration (#368).
+- Update Sphinx and switch to Furo theme (#373).
+- Remove references to tox and requirements (#383).
+- Requirements in pyproject.toml (#380).
+
 ## 23.4 (2023-05-20)
 
 - Switch build system to Hatch (#365).
 
 ## 23.3 (2023-04-28)
 
 - Use ruff for linting and reformatting (#341).
```

### Comparing `django_marina-23.4/CONTRIBUTING.md` & `django_marina-23.5/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -41,49 +41,41 @@
 
 ## Get Started!
 
 Ready to contribute? Here\'s how to set up `django-marina` for local development.
 
 You will need some knowledge of git, github, and Python/Django development. Using a Python virtual environment is advised.
 
+This project uses [Hatch](https://github.com/pypa/hatch) for environments and builds.
+
 ### Local installation
 
 This section assumes you know about local Python versions and virtual environments.
 
 To clone the repository and install the requirements for local development:
 
 ```console
 git clone git://github.com/zostera/django-marina.git
 cd django-marina
+pip install -U pip hatch
 pip install -e .
-pip install -U pip -r requirements-dev.txt
-```
-
-### Running the example app
-
-You can run the example app:
-
-```console
-cd example && python manage.py runserver
 ```
 
 ### Running the tests
 
-The test suite requires tox to be installed.
-
-To run the complete test suite:
+To run the tests:
 
 ```console
-make tox
+make test
 ```
 
-To run the tests in your current environment:
+To run the tests on all supported Python/Django combinations:
 
 ```console
-make test
+make tests
 ```
 
 ## Pull Request Guidelines
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests for new or changed functionality, and pass all tests.
```

### Comparing `django_marina-23.4/Makefile` & `django_marina-23.5/Makefile`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = $(shell hatch version)
+VERSION := $(shell hatch version)
 
 .PHONY: test
 test:
 	hatch run test
 
 .PHONY: tests
 tests:
@@ -14,16 +14,15 @@
 
 .PHONY: lint
 lint:
 	hatch run lint:style
 
 .PHONY: docs
 docs:
-	rm -rf docs/_build
-	cd docs && sphinx-build -b html -d _build/doctrees . _build/html
+	hatch run docs:build
 
 .PHONY: porcelain
 porcelain:
 ifeq ($(shell git status --porcelain),)
 	@echo "Working directory is clean."
 else
 	@echo "Error - working directory is dirty. Commit those changes!";
```

### Comparing `django_marina-23.4/.github/workflows/dependabot-auto-approve-and-merge.yml` & `django_marina-23.5/.github/workflows/dependabot-auto-approve-and-merge.yml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # PRs but also ensures that it only does work for Dependabot PRs.
     if: ${{ github.actor == 'dependabot[bot]' }}
     steps:
       # This first step will fail if there's no metadata and so the approval
       # will not occur.
       - name: Dependabot metadata
         id: dependabot-metadata
-        uses: dependabot/fetch-metadata@v1.4.0
+        uses: dependabot/fetch-metadata@v1.5.1
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
       # Here the PR gets approved.
       - name: Approve a PR
         run: gh pr review --approve "$PR_URL"
         env:
           PR_URL: ${{ github.event.pull_request.html_url }}
```

### Comparing `django_marina-23.4/.ruff_cache/content/26cb16652fde39d7` & `django_marina-23.5/.ruff_cache/content/26cb16652fde39d7`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/.ruff_cache/content/3d59ae216a1c8181` & `django_marina-23.5/.ruff_cache/content/3d59ae216a1c8181`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/.ruff_cache/content/45ce23f60dd162f5` & `django_marina-23.5/.ruff_cache/content/45ce23f60dd162f5`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/.ruff_cache/content/4b66ca14605f82bd` & `django_marina-23.5/.ruff_cache/content/4b66ca14605f82bd`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/.ruff_cache/content/73e7a5b4e3ea202b` & `django_marina-23.5/.ruff_cache/content/73e7a5b4e3ea202b`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/.ruff_cache/content/a42fb8397a68c523` & `django_marina-23.5/.ruff_cache/content/a42fb8397a68c523`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/.vscode/targets.log` & `django_marina-23.5/.vscode/targets.log`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # PARTICULAR PURPOSE.
 
 # This program built for i386-apple-darwin11.3.0
  
 make: *** No rule to make target `all'.  Stop.
 
 
-# Make data base, printed on Sat May 20 07:56:48 2023
+# Make data base, printed on Thu Jun  1 07:02:36 2023
 
 # Variables
 
 # automatic
 <D = $(patsubst %/,%,$(dir $<))
 # automatic
 ?F = $(notdir $?)
@@ -34,19 +34,18 @@
 CURDIR := /Users/dylan/Projects/django-marina
 # makefile
 SHELL = /bin/sh
 # environment
 VSCODE_NLS_CONFIG = {"locale":"nl","osLocale":"nl-nl","availableLanguages":{},"_languagePackSupport":true}
 # environment
 _ = /usr/bin/make
- 
 # environment
-STARSHIP_SESSION_KEY = 1268320338256262
+STARSHIP_SESSION_KEY = 3137324323265096
 # makefile (from `Makefile', line 1)
-VERSION = $(shell hatch version)
+VERSION := 23.4
 # environment
 __CFBundleIdentifier = com.microsoft.VSCode
 # environment
 INFOPATH = /opt/homebrew/share/info:
 # environment
 VSCODE_CWD = /Users/dylan/Projects/django-marina
 # environment
@@ -64,15 +63,15 @@
 # environment
 PYENV_ROOT = /Users/dylan/.pyenv
 # environment
 LDFLAGS = -L/opt/homebrew/opt/zlib/lib -L/opt/homebrew/opt/bzip2/lib -L/opt/homebrew/opt/sqlite/lib
 # default
 .FEATURES := target-specific order-only second-expansion else-if archives jobserver check-symlink
 # environment
-SSH_AUTH_SOCK = /private/tmp/com.apple.launchd.2sJr06OsY9/Listeners
+SSH_AUTH_SOCK = /private/tmp/com.apple.launchd.MICTSh2NiG/Listeners
 # automatic
 %F = $(notdir $%)
 # environment
 PWD = /Users/dylan/Projects/django-marina
 # environment
 HOMEBREW_CELLAR = /opt/homebrew/Cellar
 # environment
@@ -111,26 +110,28 @@
 COLORTERM = truecolor
 # default
 MAKE = $(MAKE_COMMAND)
 # environment
 LC_TERMINAL = iTerm2
 # environment
 SHLVL = 3
+# environment
+VSCODE_CRASH_REPORTER_SANDBOXED_HINT = 1
 # default
 MAKE_VERSION := 3.81
 # environment
 USER = dylan
 # makefile
 .DEFAULT_GOAL := test
 # default
 MAKECMDGOALS := all
 # environment
-TERM_SESSION_ID = w0t0p0:7E0ECFF0-3796-4507-A114-034771033E82
+TERM_SESSION_ID = w0t0p0:96C4C83E-8C7D-4AC4-B37E-99382C9092B9
 # environment
-DBUS_LAUNCHD_SESSION_BUS_SOCKET = /private/tmp/com.apple.launchd.9jUHnvuaZy/unix_domain_listener
+DBUS_LAUNCHD_SESSION_BUS_SOCKET = /private/tmp/com.apple.launchd.divrm1ujIP/unix_domain_listener
 # environment
 LESS = -R
 # automatic
 %D = $(patsubst %/,%,$(dir $%))
 # default
 MAKE_COMMAND := /Library/Developer/CommandLineTools/usr/bin/make
 # environment
@@ -150,39 +151,38 @@
 # environment
 MFLAGS = -Rrqp
 # automatic
 *D = $(patsubst %/,%,$(dir $*))
 # environment
 TERM_PROGRAM_VERSION = 3.4.19
 # environment
-XPC_SERVICE_NAME = application.com.microsoft.VSCode.204881173.204881179.8354167F-95BD-4E6E-96A5-6213B984D01B
+XPC_SERVICE_NAME = application.com.microsoft.VSCode.204881173.204881179.2D7C9981-4F78-4DF3-BC0C-01B2D682A799
 # environment
 LC_TERMINAL_VERSION = 3.4.19
 # environment
 HOMEBREW_PREFIX = /opt/homebrew
 # automatic
 +D = $(patsubst %/,%,$(dir $+))
-# environment
-VSCODE_L10N_BUNDLE_LOCATION = 
 # automatic
 +F = $(notdir $+)
 # environment
-ITERM_SESSION_ID = w0t0p0:7E0ECFF0-3796-4507-A114-034771033E82
+ITERM_SESSION_ID = w0t0p0:96C4C83E-8C7D-4AC4-B37E-99382C9092B9
 # environment
 HOMEBREW_REPOSITORY = /opt/homebrew
 # environment
 COLORFGBG = 15;0
 # environment
 __CF_USER_TEXT_ENCODING = 0x1F5:0:0
 # environment
 COMMAND_MODE = unix2003
 # default
 MAKEFILES := 
 # automatic
 <F = $(notdir $<)
+ 
 # environment
 ITERM_PROFILE = Default
 # environment
 PGUSER = postgres
 # environment
 EDITOR = code -w
 # environment
@@ -202,27 +202,27 @@
 # environment
 MAKELEVEL := 0
 # environment
 LANG = C
 # environment
 TERM = xterm-256color
 # environment
-VSCODE_PID = 89731
+VSCODE_PID = 71470
 # environment
 STARSHIP_SHELL = zsh
 # variable set hash-table stats:
-# Load=97/1024=9%, Rehash=0, Collisions=9/125=7%
+# Load=97/1024=9%, Rehash=0, Collisions=9/126=7%
 
 # Pattern-specific Variable Values
 
 # No pattern-specific variable values.
 
 # Directories
 
-# . (device 16777230, inode 2720904): 27 files, no impossibilities.
+# . (device 16777233, inode 2720904): 27 files, no impossibilities.
 
 # 27 files, no impossibilities in 1 directories.
 
 # Implicit Rules
 
 # No implicit rules.
 
@@ -233,15 +233,15 @@
 #  Command-line target.
 #  Implicit rule search has been done.
 #  File does not exist.
 #  File has not been updated.
 # variable set hash-table stats:
 # Load=0/32=0%, Rehash=0, Collisions=0/0=0%
 
-.PHONY: test tests reformat lint docs porcelain branch version build publish
+.PHONY: test tests reformat lint docs porcelain branch build publish
 #  Implicit rule search has not been done.
 #  Modification time never checked.
 #  File has not been updated.
 
 reformat:
 #  Phony target (prerequisite of .PHONY).
 #  Implicit rule search has not been done.
@@ -252,14 +252,17 @@
 	
 
 tests:
 #  Phony target (prerequisite of .PHONY).
 #  Implicit rule search has not been done.
 #  File does not exist.
 #  File has not been updated.
+#  commands to execute (from `Makefile', line 9):
+	hatch run all:test
+	
 
 porcelain:
 #  Phony target (prerequisite of .PHONY).
 #  Implicit rule search has not been done.
 #  File does not exist.
 #  File has not been updated.
 #  commands to execute (from `Makefile', line 26):
@@ -271,15 +274,15 @@
 #  Implicit rule search has not been done.
 #  Modification time never checked.
 #  File has not been updated.
 
 # Not a target:
 Makefile:
 #  Implicit rule search has been done.
-#  Last modified 2023-05-19 12:24:52
+#  Last modified 2023-05-28 09:08:10
 #  File has been updated.
 #  Successfully updated.
 # variable set hash-table stats:
 # Load=0/32=0%, Rehash=0, Collisions=0/0=0%
 
 branch:
 #  Phony target (prerequisite of .PHONY).
@@ -301,82 +304,63 @@
 	
 
 build: docs
 #  Phony target (prerequisite of .PHONY).
 #  Implicit rule search has not been done.
 #  File does not exist.
 #  File has not been updated.
-#  commands to execute (from `Makefile', line 52):
+#  commands to execute (from `Makefile', line 43):
 	rm -rf build dist src/*.egg-info
 	hatch build
 	
 
-version:
-#  Phony target (prerequisite of .PHONY).
-#  Implicit rule search has not been done.
-#  File does not exist.
-#  File has not been updated.
-#  commands to execute (from `Makefile', line 46):
-	@echo "Version ${VERSION} doens't look like a production version."
-	@exit 1;
-	
-
 # Not a target:
 .DEFAULT:
 #  Implicit rule search has not been done.
 #  Modification time never checked.
 #  File has not been updated.
 
-publish: porcelain branch version build
+publish: porcelain branch build
 #  Phony target (prerequisite of .PHONY).
 #  Implicit rule search has not been done.
 #  File does not exist.
 #  File has not been updated.
-#  commands to execute (from `Makefile', line 57):
- 
+#  commands to execute (from `Makefile', line 48):
 	hatch publish
 	git tag -a v${VERSION} -m "Release ${VERSION}"
 	git push origin --tags
 	
 
 docs:
 #  Phony target (prerequisite of .PHONY).
 #  Implicit rule search has not been done.
 #  File does not exist.
 #  File has not been updated.
 #  commands to execute (from `Makefile', line 21):
-	cd docs && sphinx-build -b html -d _build/doctrees . _build/html
+	hatch run docs:build
 	
 
 lint:
 #  Phony target (prerequisite of .PHONY).
 #  Implicit rule search has not been done.
 #  File does not exist.
 #  File has not been updated.
 #  commands to execute (from `Makefile', line 17):
 	hatch run lint:style
 	
 
-tox:
-#  Implicit rule search has not been done.
-#  Modification time never checked.
-#  File has not been updated.
-#  commands to execute (from `Makefile', line 9):
-	hatch run all:test
-	
-
 # files hash-table stats:
-# Load=16/1024=2%, Rehash=0, Collisions=0/52=0%
+# Load=14/1024=1%, Rehash=0, Collisions=0/47=0%
 # VPATH Search Paths
 
 # No `vpath' search paths.
 
 # No general (`VPATH' variable) search path.
 
 # # of strings in strcache: 1
 # # of strcache buffers: 1
 # strcache size: total = 4096 / max = 4096 / min = 4096 / avg = 4096
 # strcache free: total = 4087 / max = 4087 / min = 4087 / avg = 4087
 
-# Finished Make data base on Sat May 20 07:56:48 2023
+# Finished Make data base on Thu Jun  1 07:02:36 2023
```

### Comparing `django_marina-23.4/docs/conf.py` & `django_marina-23.5/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 copyright = f"{year} {authors}"
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx_mdinclude",
 ]
-pygments_style = "sphinx"
+
 htmlhelp_basename = f"{project}-doc"
-html_theme = "sphinx_rtd_theme"
+html_theme = "furo"
+pygments_style = "sphinx"
```

### Comparing `django_marina-23.4/src/django_marina/db/migrations.py` & `django_marina-23.5/src/django_marina/db/migrations.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/src/django_marina/db/models.py` & `django_marina-23.5/src/django_marina/db/models.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/src/django_marina/test/clients.py` & `django_marina-23.5/src/django_marina/test/clients.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/src/django_marina/test/test_cases.py` & `django_marina-23.5/src/django_marina/test/test_cases.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/models.py` & `django_marina-23.5/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/test_db.py` & `django_marina-23.5/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/test_extended_client.py` & `django_marina-23.5/tests/test_extended_client.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/test_extended_test_case.py` & `django_marina-23.5/tests/test_extended_test_case.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/test_imports.py` & `django_marina-23.5/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/urls.py` & `django_marina-23.5/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/app/settings.py` & `django_marina-23.5/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/app/urls.py` & `django_marina-23.5/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/tests/app/views.py` & `django_marina-23.5/tests/app/views.py`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/LICENSE` & `django_marina-23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/README.md` & `django_marina-23.5/README.md`

 * *Files identical despite different names*

### Comparing `django_marina-23.4/pyproject.toml` & `django_marina-23.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 Source = "https://github.com/zostera/django-marina"
 
 [tool.hatch.version]
 path = "src/django_marina/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
-  "coverage[toml]>=6.5",
+  "coverage[toml]>=7.2.6",
 ]
 matrix-name-format = "dj{value}"
 
 [tool.hatch.envs.default.scripts]
 cov = [
   "test-cov",
   "cov-report",
@@ -88,27 +88,32 @@
   {value = "django~=4.0.0", if = ["4.0"]},
   {value = "django~=4.1.0", if = ["4.1"]},
   {value = "django @ git+https://github.com/django/django.git", if = ["main"]},
 ]
 
 [tool.hatch.envs.docs]
 dependencies = [
-  "sphinx==6.2.1",
-  "sphinx_rtd_theme==1.2.0",
-  "sphinx-mdinclude==0.5.3",
+  "sphinx>=7.0.1",
+  "sphinx-mdinclude>=0.5.3",
+  "furo>=2023.05.20",
 ]
 python = "3.11"
+template = "docs"
 
 [tool.hatch.envs.docs.scripts]
-build = "rm -rf docs/_build; cd docs && sphinx-build -b html -d _build/doctrees . _build/html"
+build = [
+  "clean",
+  "cd docs && sphinx-build -b html -d _build/doctrees . _build/html",
+]
+clean = "rm -rf docs/_build"
 
 [tool.hatch.envs.lint]
 dependencies = [
-  "black>=23.1.0",
-  "ruff>=0.0.243",
+  "black>=23.3.0",
+  "ruff>=0.0.270",
 ]
 detached = true
 
 [tool.hatch.envs.lint.scripts]
 all = [
   "style",
 ]
@@ -157,16 +162,15 @@
 [tool.ruff.isort]
 known-first-party = ["django_marina", "app"]
 known-third-party = ["django"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
-source = ["src", "tests"]
+source = ["src"]
 
 [tool.coverage.paths]
 package = ["src/django_marina", "*/django_marina/src/django_marina"]
-tests = ["tests", "*/django_marina/tests"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
```

### Comparing `django_marina-23.4/PKG-INFO` & `django_marina-23.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-marina
-Version: 23.4
+Version: 23.5
 Summary: Django extensions by Zostera
 Project-URL: Changelog, https://github.com/zostera/django-marina/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://django-marina.readthedocs.io/
 Project-URL: Homepage, https://github.com/zostera/django-marina
 Project-URL: Issues, https://github.com/zostera/django-marina/issues
 Project-URL: Source, https://github.com/zostera/django-marina
 Author-email: Dylan Verheul <dylan@dyve.net>
```

