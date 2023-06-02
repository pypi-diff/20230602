# Comparing `tmp/chatllm-2023.6.2.9.16.4.tar.gz` & `tmp/chatllm-2023.6.2.9.16.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatllm-2023.6.2.9.16.4.tar", last modified: Fri Jun  2 01:16:04 2023, max compression
+gzip compressed data, was "chatllm-2023.6.2.9.16.47.tar", last modified: Fri Jun  2 01:16:47 2023, max compression
```

## Comparing `chatllm-2023.6.2.9.16.4.tar` & `chatllm-2023.6.2.9.16.47.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.482638 chatllm-2023.6.2.9.16.4/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.2.9.16.4/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.2.9.16.4/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     6663 2023-06-02 01:16:04.482435 chatllm-2023.6.2.9.16.4/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     5935 2023-05-31 01:20:56.000000 chatllm-2023.6.2.9.16.4/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.2.9.16.4/README.md.bak
--rw-r--r--   0 betterme   (501) staff       (20)      898 2023-05-31 01:32:50.000000 chatllm-2023.6.2.9.16.4/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.434204 chatllm-2023.6.2.9.16.4/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.436433 chatllm-2023.6.2.9.16.4/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.2.9.16.4/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.2.9.16.4/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.2.9.16.4/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.2.9.16.4/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.436812 chatllm-2023.6.2.9.16.4/chatllm/aigc/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.2.9.16.4/chatllm/aigc/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.2.9.16.4/chatllm/aigc/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.439179 chatllm-2023.6.2.9.16.4/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.2.9.16.4/chatllm/api/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.2.9.16.4/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      586 2023-06-01 01:41:38.000000 chatllm-2023.6.2.9.16.4/chatllm/api/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-05-31 03:52:51.000000 chatllm-2023.6.2.9.16.4/chatllm/api/config.py
--rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.2.9.16.4/chatllm/api/datamodels.py
--rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.2.9.16.4/chatllm/api/openai_client.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.440427 chatllm-2023.6.2.9.16.4/chatllm/api/routes/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.2.9.16.4/chatllm/api/routes/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.2.9.16.4/chatllm/api/routes/api.py
--rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2023.6.2.9.16.4/chatllm/api/routes/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     4696 2023-06-02 01:03:20.000000 chatllm-2023.6.2.9.16.4/chatllm/api/routes/completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-05-26 07:01:26.000000 chatllm-2023.6.2.9.16.4/chatllm/api/routes/embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3471 2023-05-31 08:27:43.000000 chatllm-2023.6.2.9.16.4/chatllm/api/routes/responses.py
--rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.2.9.16.4/chatllm/api/sse_api.py
--rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.2.9.16.4/chatllm/api/test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.444267 chatllm-2023.6.2.9.16.4/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/__chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2414 2023-05-31 06:03:52.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2395 2023-05-31 09:20:39.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.2.9.16.4/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.2.9.16.4/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.444863 chatllm-2023.6.2.9.16.4/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1281 2023-06-01 09:05:12.000000 chatllm-2023.6.2.9.16.4/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.2.9.16.4/chatllm/closeai.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.2.9.16.4/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.445671 chatllm-2023.6.2.9.16.4/chatllm/llms/
--rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-06-02 01:07:49.000000 chatllm-2023.6.2.9.16.4/chatllm/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2243 2023-06-02 01:09:41.000000 chatllm-2023.6.2.9.16.4/chatllm/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.2.9.16.4/chatllm/llms/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.2.9.16.4/chatllm/llms/llama.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.447182 chatllm-2023.6.2.9.16.4/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.2.9.16.4/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.2.9.16.4/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2336 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.4/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.2.9.16.4/chatllm/utils/gpu_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.2.9.16.4/chatllm/utils/nbce.py
--rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.2.9.16.4/chatllm/utils/nbce_test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.449163 chatllm-2023.6.2.9.16.4/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.2.9.16.4/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.4/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.2.9.16.4/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-05-15 11:46:17.000000 chatllm-2023.6.2.9.16.4/chatllm/webui/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.2.9.16.4/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.2.9.16.4/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 chatllm-2023.6.2.9.16.4/chatllm/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.2.9.16.4/chatllm/webui/visualglm_st.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.435322 chatllm-2023.6.2.9.16.4/chatllm.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     6663 2023-06-02 01:16:04.000000 chatllm-2023.6.2.9.16.4/chatllm.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     2640 2023-06-02 01:16:04.000000 chatllm-2023.6.2.9.16.4/chatllm.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-02 01:16:04.000000 chatllm-2023.6.2.9.16.4/chatllm.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-02 01:16:04.000000 chatllm-2023.6.2.9.16.4/chatllm.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-02 01:16:04.000000 chatllm-2023.6.2.9.16.4/chatllm.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-06-02 01:16:04.000000 chatllm-2023.6.2.9.16.4/chatllm.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-02 01:16:04.000000 chatllm-2023.6.2.9.16.4/chatllm.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.453605 chatllm-2023.6.2.9.16.4/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.465587 chatllm-2023.6.2.9.16.4/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.2.9.16.4/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.2.9.16.4/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.2.9.16.4/data/imgs/chatbox.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.2.9.16.4/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.2.9.16.4/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.2.9.16.4/data/imgs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.2.9.16.4/data/imgs/img_1.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.2.9.16.4/data/imgs/role.png
--rw-r--r--   0 betterme   (501) staff       (20)   443539 2023-05-26 00:55:04.000000 chatllm-2023.6.2.9.16.4/data/imgs/群.png
--rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.2.9.16.4/data/openai_keys.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.470022 chatllm-2023.6.2.9.16.4/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.2.9.16.4/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.2.9.16.4/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.4/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.4/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.4/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.2.9.16.4/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.4/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.480225 chatllm-2023.6.2.9.16.4/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      332 2023-05-31 10:28:33.000000 chatllm-2023.6.2.9.16.4/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.2.9.16.4/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.2.9.16.4/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.2.9.16.4/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.2.9.16.4/requirements_openai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.2.9.16.4/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.2.9.16.4/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-02 01:16:04.482701 chatllm-2023.6.2.9.16.4/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1700 2023-05-31 05:17:11.000000 chatllm-2023.6.2.9.16.4/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:04.480784 chatllm-2023.6.2.9.16.4/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.2.9.16.4/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.4/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.831497 chatllm-2023.6.2.9.16.47/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.2.9.16.47/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.2.9.16.47/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     6664 2023-06-02 01:16:47.831335 chatllm-2023.6.2.9.16.47/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     5935 2023-05-31 01:20:56.000000 chatllm-2023.6.2.9.16.47/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.2.9.16.47/README.md.bak
+-rw-r--r--   0 betterme   (501) staff       (20)      898 2023-05-31 01:32:50.000000 chatllm-2023.6.2.9.16.47/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.810805 chatllm-2023.6.2.9.16.47/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.812262 chatllm-2023.6.2.9.16.47/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.2.9.16.47/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.2.9.16.47/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.2.9.16.47/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.2.9.16.47/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.812562 chatllm-2023.6.2.9.16.47/chatllm/aigc/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.2.9.16.47/chatllm/aigc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.2.9.16.47/chatllm/aigc/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.813828 chatllm-2023.6.2.9.16.47/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.2.9.16.47/chatllm/api/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.2.9.16.47/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      586 2023-06-01 01:41:38.000000 chatllm-2023.6.2.9.16.47/chatllm/api/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-05-31 03:52:51.000000 chatllm-2023.6.2.9.16.47/chatllm/api/config.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.2.9.16.47/chatllm/api/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.2.9.16.47/chatllm/api/openai_client.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.814683 chatllm-2023.6.2.9.16.47/chatllm/api/routes/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4696 2023-06-02 01:03:20.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-05-26 07:01:26.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3471 2023-05-31 08:27:43.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/responses.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.2.9.16.47/chatllm/api/sse_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.2.9.16.47/chatllm/api/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.816616 chatllm-2023.6.2.9.16.47/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/__chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2414 2023-05-31 06:03:52.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2395 2023-05-31 09:20:39.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.2.9.16.47/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.816985 chatllm-2023.6.2.9.16.47/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1281 2023-06-01 09:05:12.000000 chatllm-2023.6.2.9.16.47/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.2.9.16.47/chatllm/closeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.2.9.16.47/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.817513 chatllm-2023.6.2.9.16.47/chatllm/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-06-02 01:07:49.000000 chatllm-2023.6.2.9.16.47/chatllm/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2243 2023-06-02 01:09:41.000000 chatllm-2023.6.2.9.16.47/chatllm/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.2.9.16.47/chatllm/llms/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.2.9.16.47/chatllm/llms/llama.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.818319 chatllm-2023.6.2.9.16.47/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2336 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/gpu_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/nbce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/nbce_test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.819315 chatllm-2023.6.2.9.16.47/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-05-15 11:46:17.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/visualglm_st.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.811743 chatllm-2023.6.2.9.16.47/chatllm.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     6664 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     2640 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.821978 chatllm-2023.6.2.9.16.47/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.824431 chatllm-2023.6.2.9.16.47/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.2.9.16.47/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.2.9.16.47/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.2.9.16.47/data/imgs/chatbox.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.2.9.16.47/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.2.9.16.47/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.2.9.16.47/data/imgs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.2.9.16.47/data/imgs/img_1.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.2.9.16.47/data/imgs/role.png
+-rw-r--r--   0 betterme   (501) staff       (20)   443539 2023-05-26 00:55:04.000000 chatllm-2023.6.2.9.16.47/data/imgs/群.png
+-rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.2.9.16.47/data/openai_keys.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.826919 chatllm-2023.6.2.9.16.47/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.2.9.16.47/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.2.9.16.47/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.47/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.47/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.47/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.2.9.16.47/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.47/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.830610 chatllm-2023.6.2.9.16.47/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      332 2023-05-31 10:28:33.000000 chatllm-2023.6.2.9.16.47/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.2.9.16.47/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.2.9.16.47/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.2.9.16.47/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.2.9.16.47/requirements_openai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.2.9.16.47/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.2.9.16.47/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-02 01:16:47.831558 chatllm-2023.6.2.9.16.47/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1700 2023-05-31 05:17:11.000000 chatllm-2023.6.2.9.16.47/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.831025 chatllm-2023.6.2.9.16.47/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.2.9.16.47/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/tox.ini
```

### Comparing `chatllm-2023.6.2.9.16.4/.gitignore` & `chatllm-2023.6.2.9.16.47/.gitignore`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/.travis.yml` & `chatllm-2023.6.2.9.16.47/.travis.yml`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/LICENSE` & `chatllm-2023.6.2.9.16.47/LICENSE`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/Makefile` & `chatllm-2023.6.2.9.16.47/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/PKG-INFO` & `chatllm-2023.6.2.9.16.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.2.9.16.4
+Version: 2023.6.2.9.16.47
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatllm-2023.6.2.9.16.4/README.md` & `chatllm-2023.6.2.9.16.47/README.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/README.md.bak` & `chatllm-2023.6.2.9.16.47/README.md.bak`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/TODO.md` & `chatllm-2023.6.2.9.16.47/TODO.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/_his/FaissANN.py` & `chatllm-2023.6.2.9.16.47/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/_his/_chatllm.py` & `chatllm-2023.6.2.9.16.47/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/_his/_qa.py` & `chatllm-2023.6.2.9.16.47/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/aigc/common.py` & `chatllm-2023.6.2.9.16.47/chatllm/aigc/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/app.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/app.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/config.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/config.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/datamodels.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/datamodels.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/openai_client.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/openai_client.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/routes/api.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/routes/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/routes/base.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/routes/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/routes/completions.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/routes/completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/routes/embeddings.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/routes/responses.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/routes/responses.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/sse_api.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/sse_api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/api/test.py` & `chatllm-2023.6.2.9.16.47/chatllm/api/test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/applications/Question2Answer.py` & `chatllm-2023.6.2.9.16.47/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/applications/__chatbase.py` & `chatllm-2023.6.2.9.16.47/chatllm/applications/__chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/applications/chatann.py` & `chatllm-2023.6.2.9.16.47/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/applications/chatbase.py` & `chatllm-2023.6.2.9.16.47/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/applications/chatcrawler.py` & `chatllm-2023.6.2.9.16.47/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/applications/chatpdf.py` & `chatllm-2023.6.2.9.16.47/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/applications/chatwhoosh.py` & `chatllm-2023.6.2.9.16.47/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/chatyuan.py` & `chatllm-2023.6.2.9.16.47/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/clis/cli.py` & `chatllm-2023.6.2.9.16.47/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/closeai.py` & `chatllm-2023.6.2.9.16.47/chatllm/closeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/embedding.py` & `chatllm-2023.6.2.9.16.47/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/llms/__init__.py` & `chatllm-2023.6.2.9.16.47/chatllm/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/llms/chatglm.py` & `chatllm-2023.6.2.9.16.47/chatllm/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/llms/demo.py` & `chatllm-2023.6.2.9.16.47/chatllm/llms/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/llms/llama.py` & `chatllm-2023.6.2.9.16.47/chatllm/llms/llama.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/utils/common.py` & `chatllm-2023.6.2.9.16.47/chatllm/utils/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/utils/gpu_utils.py` & `chatllm-2023.6.2.9.16.47/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/utils/nbce.py` & `chatllm-2023.6.2.9.16.47/chatllm/utils/nbce.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/utils/nbce_test.py` & `chatllm-2023.6.2.9.16.47/chatllm/utils/nbce_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/webui/chatbase.py` & `chatllm-2023.6.2.9.16.47/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/webui/chatpdf.py` & `chatllm-2023.6.2.9.16.47/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/webui/gradio_ui.py` & `chatllm-2023.6.2.9.16.47/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/webui/nice_ui.py` & `chatllm-2023.6.2.9.16.47/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm/webui/visualglm_st.py` & `chatllm-2023.6.2.9.16.47/chatllm/webui/visualglm_st.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/chatllm.egg-info/PKG-INFO` & `chatllm-2023.6.2.9.16.47/chatllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.2.9.16.4
+Version: 2023.6.2.9.16.47
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatllm-2023.6.2.9.16.4/chatllm.egg-info/SOURCES.txt` & `chatllm-2023.6.2.9.16.47/chatllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/LLM.drawio.png` & `chatllm-2023.6.2.9.16.47/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/LLM.png` & `chatllm-2023.6.2.9.16.47/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/chatbox.png` & `chatllm-2023.6.2.9.16.47/data/imgs/chatbox.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/chatpdf.gif` & `chatllm-2023.6.2.9.16.47/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/chatpdf_ann_df.png` & `chatllm-2023.6.2.9.16.47/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/img.png` & `chatllm-2023.6.2.9.16.47/data/imgs/img.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/img_1.png` & `chatllm-2023.6.2.9.16.47/data/imgs/img_1.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/role.png` & `chatllm-2023.6.2.9.16.47/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/imgs/群.png` & `chatllm-2023.6.2.9.16.47/data/imgs/群.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/openai_keys.md` & `chatllm-2023.6.2.9.16.47/data/openai_keys.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/医/500种中药现代研究.txt` & `chatllm-2023.6.2.9.16.47/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/医/古今医统大全.txt` & `chatllm-2023.6.2.9.16.47/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/姚明.txt` & `chatllm-2023.6.2.9.16.47/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/王治郅.txt` & `chatllm-2023.6.2.9.16.47/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/科比.txt` & `chatllm-2023.6.2.9.16.47/data/科比.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/data/财报.pdf` & `chatllm-2023.6.2.9.16.47/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/docs/Makefile` & `chatllm-2023.6.2.9.16.47/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/docs/conf.py` & `chatllm-2023.6.2.9.16.47/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/docs/make.bat` & `chatllm-2023.6.2.9.16.47/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/setup.py` & `chatllm-2023.6.2.9.16.47/setup.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/tests/test_llm4gpt.py` & `chatllm-2023.6.2.9.16.47/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.4/tests/内存型.ipynb` & `chatllm-2023.6.2.9.16.47/tests/内存型.ipynb`

 * *Files identical despite different names*

