# Comparing `tmp/napari-chatgpt-2023.5.2.tar.gz` & `tmp/napari-chatgpt-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-chatgpt-2023.5.2.tar", last modified: Wed May  3 00:41:13 2023, max compression
+gzip compressed data, was "napari-chatgpt-2023.6.2.tar", last modified: Fri Jun  2 19:20:53 2023, max compression
```

## Comparing `napari-chatgpt-2023.5.2.tar` & `napari-chatgpt-2023.6.2.tar`

### file list

```diff
@@ -1,161 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.678624 napari-chatgpt-2023.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.646624 napari-chatgpt-2023.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.650624 napari-chatgpt-2023.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.github/workflows/just_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.650624 napari-chatgpt-2023.5.2/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20605 2023-05-03 00:41:13.678624 napari-chatgpt-2023.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-03 00:41:13.678624 napari-chatgpt-2023.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.650624 napari-chatgpt-2023.5.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.654624 napari-chatgpt-2023.5.2/src/napari_chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/conv_agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/enumerate_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/enumerate_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/gtts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/lanchain_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/playwright_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/tts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/whisper_cpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/callback_handle_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/callback_handler_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/chat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/chat_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/chat.js
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/prism.css
--rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/prism.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.662624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/memory/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/napari_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.662624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.662624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/async_base_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/demo/tools_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/file_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/functions_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/google_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/human_input_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/math_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_base_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_file_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_viewer_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_viewer_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_widget_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/cell_nuclei_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/cellpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/google_search_tool_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tool_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/web_image_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/web_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/wikipedia_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/wikipedia_search_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/api_key_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/api_key_vault_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/browser_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/camel_case_to_normal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/api_key_vault_dialog_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/browser_widget_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/open_zarr_in_napari_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/dynamic_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/exception_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/extract_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/filter_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/find_function_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/installed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/missing_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/missing_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/open_in_napari.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/openai_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/scrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.678624 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/api_key_vault_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/download_files_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/duckduckgo_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/dynamic_import_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/exception_guard_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/extract_code_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/extract_url_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/filter_lines_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/find_function_name_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/google_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/inspection_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/installed_packages_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/missing_imports_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/missing_libraries_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/run_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/scrapper_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/summarizer_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/wikipedia_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.654624 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20605 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.005091 napari-chatgpt-2023.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.969090 napari-chatgpt-2023.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.973090 napari-chatgpt-2023.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.github/workflows/just_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.973090 napari-chatgpt-2023.6.2/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-02 19:20:53.005091 napari-chatgpt-2023.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-02 19:20:53.005091 napari-chatgpt-2023.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.973090 napari-chatgpt-2023.6.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.973090 napari-chatgpt-2023.6.2/src/napari_chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/bard_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/conv_agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/enumerate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/enumerate_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/gpt4all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/gtts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/lanchain_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/openai_list_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/playwright_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/tts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/whisper_cpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/chat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/chat_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.981090 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/_tailwind.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/chat.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/marked-highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/prism.css
+-rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/prism.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight.dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/tailwind.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/llms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/.pytest_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/bard_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/memory/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/napari_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/async_base_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/demo/tools_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari_base_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/web_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/file_download_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/human_input_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/async_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/async_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/async_utils/run_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/gpt4all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/test/download_files_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/test/summarizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/open_in_napari.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/dynamic_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/exception_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/exception_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/installed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/missing_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/python_lang_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/required_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/exception_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/exception_guard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/installed_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/required_imports_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/download_file_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/qt_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/segmentation/cellpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/extract_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/filter_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/find_function_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/python_code_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/extract_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/extract_url_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/system/folders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/metasearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/scrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.005091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/google_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/metasearch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/scrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/wikipedia_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/tox.ini
```

### Comparing `napari-chatgpt-2023.5.2/.github/workflows/just_deploy.yml` & `napari-chatgpt-2023.6.2/.github/workflows/just_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/.github/workflows/test_and_deploy.yml` & `napari-chatgpt-2023.6.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/.gitignore` & `napari-chatgpt-2023.6.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -78,7 +78,8 @@
 .python-version
 
 # OS
 .DS_Store
 
 # written by setuptools_scm
 **/_version.py
+/src/napari_chatgpt/llm/test/.pytest_cache/README.md
```

### Comparing `napari-chatgpt-2023.5.2/.napari-hub/config.yml` & `napari-chatgpt-2023.6.2/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/.pre-commit-config.yaml` & `napari-chatgpt-2023.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/LICENSE` & `napari-chatgpt-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/PKG-INFO` & `napari-chatgpt-2023.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.5.2
+Version: 2023.6.2
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
@@ -23,98 +23,138 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# napari-chatgpt, home of _Omega_, a napari-aware autonomous LLM-based agent.
+# napari-chatgpt
+
+## Home of
+_Omega_, a napari-aware autonomous LLM-based agent specialised in image processing and analysis.
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
 
-A [napari](napari.org) plugin that levegares OpenAI's Large Language Model ChatGPT to implement _Omega_ 
-a napari-aware agent capable of performing image processing and analysis tasks in a conversational manner.
-
-This repository was created as a 'week-end project' by [Loic A. Royer](https://twitter.com/loicaroyer) 
-who leads a [research group](https://royerlab.org) at the [Chan Zuckerberg Biohub](https://czbiohub.org/sf/). It levegages [OpenAI](https://openai.com)'s ChatGPT API via the [LangChain](https://python.langchain.com/en/latest/index.html) Python library, as well as [napari](https://napari.org), a fast, interactive, multi-dimensional 
-image viewer for Python, [another](https://ilovesymposia.com/2019/10/24/introducing-napari-a-fast-n-dimensional-image-viewer-in-python/) 
+A [napari](napari.org) plugin that levegares OpenAI's Large Language Model
+ChatGPT to implement _Omega_
+a napari-aware agent capable of performing image processing and analysis tasks
+in a conversational manner.
+
+This repository was created as a 'week-end project'
+by [Loic A. Royer](https://twitter.com/loicaroyer)
+who leads a [research group](https://royerlab.org) at
+the [Chan Zuckerberg Biohub](https://czbiohub.org/sf/). It
+levegages [OpenAI](https://openai.com)'s ChatGPT API via
+the [LangChain](https://python.langchain.com/en/latest/index.html) Python
+library, as well as [napari](https://napari.org), a fast, interactive,
+multi-dimensional
+image viewer for
+Python, [another](https://ilovesymposia.com/2019/10/24/introducing-napari-a-fast-n-dimensional-image-viewer-in-python/)
 of Loic's week-end projects.
 
 # What is Omega?
 
-Omega is a LLM-based and tool-armed autonomous agent that demonstrates the potential for Large Language Models (LLMs) to be applied to image processing, analysis and visualisation. 
-Can LLM-based agents write image processing code and napari widgets, correct its coding mistakes, perform 
+Omega is a LLM-based and tool-armed autonomous agent that demonstrates the
+potential for Large Language Models (LLMs) to be applied to image processing,
+analysis and visualisation.
+Can LLM-based agents write image processing code and napari widgets, correct its
+coding mistakes, perform
 follow-up analysis, and control the napari viewer? The answer appears to be yes.
 
 #### In this video I ask Omega to segment an image using the [SLIC](https://www.iro.umontreal.ca/~mignotte/IFT6150/Articles/SLIC_Superpixels.pdf) algorithm. It makes a first attempt using the implementation in scikit-image, but fails because of an inexistant 'multichannel' parameter. Realising that, Omega tries again, and this time, succeeds:
+
 https://user-images.githubusercontent.com/1870994/235768559-ca8bfa84-21f5-47b6-b2bd-7fcc07cedd92.mp4
 
-#### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:   
-https://user-images.githubusercontent.com/1870994/235769990-a281a118-1369-47aa-834a-b491f706bd48.mp4
+#### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:
 
+https://user-images.githubusercontent.com/1870994/235769990-a281a118-1369-47aa-834a-b491f706bd48.mp4
 
-As LLMs continue to improve, Omega will become even more adept at handling complex 
-image processing and analysis tasks. The current version of ChatGPT, 3.5, 
-has a cutoff date of 2021, which means that it lacks nearly two years of knowledge 
-on the napari API and usage, as well as the latest versions of popular libraries 
-like scikit-image, OpenCV, numpy, scipy, etc... Despite this, you can see in the videos below 
-that it is quite capable. While ChatGPT 4.0 is a significant upgrade, it is not yet widely 
+As LLMs continue to improve, Omega will become even more adept at handling
+complex
+image processing and analysis tasks. The current version of ChatGPT, 3.5,
+has a cutoff date of 2021, which means that it lacks nearly two years of
+knowledge
+on the napari API and usage, as well as the latest versions of popular libraries
+like scikit-image, OpenCV, numpy, scipy, etc... Despite this, you can see in the
+videos below
+that it is quite capable. While ChatGPT 4.0 is a significant upgrade, it is not
+yet widely
 available.
 
-Omega could eventually help non-experts process and analyse images, especially in the bioimage domain. 
-It is also potentially valuable for educative purposes as it could 
-assist in teaching image processing and analysis, making it more accessible. 
-Although ChatGPT, which powers Omega, may not be yet on par with an expert image analyst or computer vision 
+Omega could eventually help non-experts process and analyse images, especially
+in the bioimage domain.
+It is also potentially valuable for educative purposes as it could
+assist in teaching image processing and analysis, making it more accessible.
+Although ChatGPT, which powers Omega, may not be yet on par with an expert image
+analyst or computer vision
 expert, it is just a matter of time...
 
-Omega holds a conversation with the user and uses the following tools to acheive answer questions, 
+Omega holds a conversation with the user and uses the following tools to acheive
+answer questions,
 download and operate on images, write widgets for napari, and more:
 
 ### napari related tools:
-- napari viewer control: 
-    Gives Omega the ability to control all aspects of the napari viewer.
-  
+
+- napari viewer control:
+  Gives Omega the ability to control all aspects of the napari viewer.
+
 - napari query:
-    Gives Omega the ability to query information about the state of the viewer, of its layers, and their contents.
+  Gives Omega the ability to query information about the state of the viewer, of
+  its layers, and their contents.
 
 - napari widget maker:
-    Gives Omega the ability to make napari functional widgets that take layers as input and return a new layer.
+  Gives Omega the ability to make napari functional widgets that take layers as
+  input and return a new layer.
+
+### cell segmentation tools:
 
-### cell segmentation tools: 
 - cell and nuclei segmentation:
-    This tool specialises in segmenting cells and nuclei in images using some predefined segmentation algorithms. Right now only cellpose is implemented. 
+  This tool specialises in segmenting cells and nuclei in images using some
+  predefined segmentation algorithms. Right now only cellpose is implemented.
 
 ### Generic python installation queries:
+
 - python function signature query:
-    Lets Omega query the signature of function when it is unsure how to call a function and what the names and type of the parameters are.
+  Lets Omega query the signature of function when it is unsure how to call a
+  function and what the names and type of the parameters are.
 
 ### web search related tools:
+
 - web search:
-    Usefull to give Omega access to the knowledge accessible through the web
+  Usefull to give Omega access to the knowledge accessible through the web
 
 - web image serach:
-    Streamlined path to search the web for images and open them in napari  
+  Streamlined path to search the web for images and open them in napari
 
 - wikipedia search:
-    Gives Omega access to the whole wikipedia
-
+  Gives Omega access to the whole wikipedia
 
 ----------------------------------
 
-## Installation:
+## Installation from within napari:
+
+You can install `napari-chatgpt` directly from within napari in the Plugins>
+Install/Uninstall Plugins menu.
+(Please note that the Omega agent will hapilly install packages in the
+corresponding environment).
+
+IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the
+latest one!
 
-You can also install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
-(Please note that the Omega agent will hapilly install packages in the corresponding environment)
+## Installation in an new conda environment (RECOMMENDED):
 
-Create environment: 
+Make sure you have an anaocnda/miniconda installation on your system.
+Ask ChatGPT what is that all about if you are unsure ;-)
+
+Create environment:
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
     conda activate napari-chatgpt 
 
@@ -122,238 +162,328 @@
 
     conda install -c conda-forge napari     
 
 Install the repo in enbvironment:
 
     pip install napari-chatgpt
 
-
 ## Installation variations:
 
 To install latest development version :
 
     git clone https://github.com/royerlab/napari-chatgpt.git
     cd napari-chatgpt
     pip install -e .
 
 or:
 
     pip install git+https://github.com/royerlab/napari-chatgpt.git
 
-
 ## Requirements:
 
 You need an OpenAI key, there is no way around this, unless we add some other,
-potentially local LLMs compatible to LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar models come to mind). However, this will likely be at the cost of cognitive performance,
+potentially local LLMs compatible to
+LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar
+models come to mind). However, this will likely be at the cost of cognitive
+performance,
 which I am not sure is worth it at this point. Please prove me wrong.
-You can get your OpenAI key by signing up [here](https://openai.com/blog/openai-api).
-Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5 is very
-reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A bargain.
-Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop, hopefully.
-
-Note: you can limit the burn-rate to a certain amount of dollars per month, just in case you let
-Omega thinking over the week end and forget to stop it (don't worry, this is actually not possible). 
-
+You can get your OpenAI key by signing
+up [here](https://openai.com/blog/openai-api).
+Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5
+is very
+reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
+bargain.
+Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
+hopefully.
+
+Note: you can limit the burn-rate to a certain amount of dollars per month, just
+in case you let
+Omega thinking over the week end and forget to stop it (don't worry, this is
+actually not possible).
 
 ## Usage:
 
 Once all is installed, and if it is not already running, start napari:
 
     napari
-    
+
 You can then the Omega napari plugin via the plugins menu:
 
 <img width="498" alt="image" src="https://user-images.githubusercontent.com/1870994/235790134-1d87fd50-583f-4fd9-ade2-c64497b91331.png">
 
 
 You just opened the plugin as a widget, you now need to actually start Omega:
 
 <img width="104" alt="image" src="https://user-images.githubusercontent.com/1870994/235811111-9e468785-9562-410a-8e9a-c63cb03fb765.png">
 
 
-If you have not set the 'OPENAI_API_KEY' environment variable as is typicall done,
-Omega will ask you for your OpenAI API key, and will store it _safely_ in an _encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
+If you have not set the 'OPENAI_API_KEY' environment variable as is typicall
+done,
+Omega will ask you for your OpenAI API key, and will store it _safely_ in an
+_encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
 
 <img width="293" alt="image" src="https://user-images.githubusercontent.com/1870994/235793528-9e892c5e-d8ca-43e1-9020-f2dfab45b32d.png">
 
 
 Just enter an encryption/decription key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
-(The idea is that you might not be able to remember your openAI key by heart, but you might be able to do so with your own password or passphrase)
+(The idea is that you might not be able to remember your openAI key by heart,
+but you might be able to do so with your own password or passphrase)
 
-You can then direct your browser to: [http://0.0.0.0:9000/](http://0.0.0.0:9000/)
+You can then direct your browser
+to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
 and start having an hopefully nice chat with Omega.
 
-
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
 - What is your name?
 - What tools do you have available?
 - Make me a Gaussian blur widget with sigma parameter
-- Open this tiff file in napari: https://people.math.sc.edu/Burkardt/data/tif/at3_1m4_03.tif
-- Make a widget that applies the transformation: y = x^alpha + y^beta with alpha and beta two parameters.
+- Open this tiff file in
+  napari: https://people.math.sc.edu/Burkardt/data/tif/at3_1m4_03.tif
+- Make a widget that applies the transformation: y = x^alpha + y^beta with alpha
+  and beta two parameters.
 - Create a widget to multiply two images
 - Can you open in napari a photo of Albert Einstein?
 - Downscale by a factor 3x the image on layer named 'img'
 - Rename selected layer to 'downscaled_image'
-- Upscale image 'downscaled_image' by a factor 3 using some smart interpolation scheme of your choice (not nearest-neighboor)
+- Upscale image 'downscaled_image' by a factor 3 using some smart interpolation
+  scheme of your choice (not nearest-neighboor)
 - Caveat: makes a plugin instead of actually doing teh job
 - How many channels has the image on layer 0
 - Make a image sharpening filter widget, expose relevant parameters
-- Can you open this file in napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
-- Split the two channels of the first layer (first axis) into two separate layers
+- Can you open this file in
+  napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
+- Split the two channels of the first layer (first axis) into two separate
+  layers
 - Switch viewer to 3d
-- Create a napari widget for a function that takes two image layers and returns a 3D image stack of n images where each 2D image corresponds to a linear blending of the two layer images between 0 and 1.
-- [Loaded the ‘cell’ sample image] there is one cell in the image on the first layer, it is roughly circular and brighter than its surroundings, ca you write segmentation code that returns a labels layer for it?
+- Create a napari widget for a function that takes two image layers and returns
+  a 3D image stack of n images where each 2D image corresponds to a linear
+  blending of the two layer images between 0 and 1.
+- [Loaded the ‘cell’ sample image] there is one cell in the image on the first
+  layer, it is roughly circular and brighter than its surroundings, ca you write
+  segmentation code that returns a labels layer for it?
 - Can you create a widget to blend two images?
 - Can you tell me more about the 'guided Canny edge filter' ?
 - Write a configurable RGB to grayscale widget, ensure weights sum to 1
 
 ## Video Demos:
 
-Not everyone will want, or can, get an API key for the latest and best LLM models, 
-so here are videos showcasing what's possible. You will notice that Omega sometimes 
-fails on its first attempt, typically because of mistaken parameters for functions,
-or other syntax errors. But it also often recovers by having access to the error message,
-and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can do, imagine
+Not everyone will want, or can, get an API key for the latest and best LLM
+models,
+so here are videos showcasing what's possible. You will notice that Omega
+sometimes
+fails on its first attempt, typically because of mistaken parameters for
+functions,
+or other syntax errors. But it also often recovers by having access to the error
+message,
+and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can
+do, imagine
 what will be possible with 4.0 and future more capable models...
 
 ##
-In this first video, I ask Omega to make a napari widget to convert images from RGB to grayscale:
+
+In this first video, I ask Omega to make a napari widget to convert images from
+RGB to grayscale:
 
 https://user-images.githubusercontent.com/1870994/235769895-23cfc7ed-622a-47f9-95aa-4be77efc0f78.mp4
 
 ##
-Of course Omega is capable of holding a conversation, it sort of knows 'who it is', can search the web
-and wikipedia. Eventually I imagine it could leverage the ability to search for improving its responses,
+
+Of course Omega is capable of holding a conversation, it sort of knows 'who it
+is', can search the web
+and wikipedia. Eventually I imagine it could leverage the ability to search for
+improving its responses,
 and I have seen doing it a few times:
 
 https://user-images.githubusercontent.com/1870994/235769920-86b02d9d-1196-4339-a8d9-9a028bcd4607.mp4
 
 ##
-Following-up from the previous video, I ask Omega to create a new labels layer containing just the largest segment. The script that Omega writes as another rookie mistake: it confuses layers and images. The error message then confuses Omega into thinking that it got the name of the layer wrong, setting it off in a quest
-to find the name of the labels layer. It succeeds at writting code that searches for the labels layer, and uses that name to write a script that then does extracts te largest segment into its own layer. Not bad: 
+
+Following-up from the previous video, I ask Omega to create a new labels layer
+containing just the largest segment. The script that Omega writes as another
+rookie mistake: it confuses layers and images. The error message then confuses
+Omega into thinking that it got the name of the layer wrong, setting it off in a
+quest
+to find the name of the labels layer. It succeeds at writting code that searches
+for the labels layer, and uses that name to write a script that then does
+extracts te largest segment into its own layer. Not bad:
 
 https://user-images.githubusercontent.com/1870994/235770741-d8905afd-0a9b-4eb7-a075-481979ab7b01.mp4
 
 ##
-In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific. The answer is a vanilla yet effective widget that uses the Otsu approach to threshold the image and then finds the connected components.
-Note that when you ask Omega to make a widget, it won't know of any runtime issues with the code because
-it is not running the code itself, yet. It can tell if there is a syntax problem though... Nevertheless, the widget ends up working just fine:
+
+In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific.
+The answer is a vanilla yet effective widget that uses the Otsu approach to
+threshold the image and then finds the connected components.
+Note that when you ask Omega to make a widget, it won't know of any runtime
+issues with the code because
+it is not running the code itself, yet. It can tell if there is a syntax problem
+though... Nevertheless, the widget ends up working just fine:
 
 https://user-images.githubusercontent.com/1870994/235770794-90091bfe-b546-4dd0-bd9c-3895bfc33a1d.mp4
 
 ##
-Now it gets more interesting. Following up on the previous video, can we ask Omega to do some follow-
-up analysis on the segments themselves? I ask Omega to list the 10 largest segments and compute their 
-areas and centroids. No problem: 
+
+Now it gets more interesting. Following up on the previous video, can we ask
+Omega to do some follow-
+up analysis on the segments themselves? I ask Omega to list the 10 largest
+segments and compute their
+areas and centroids. No problem:
 
 https://user-images.githubusercontent.com/1870994/235770828-0f829f76-1f3d-44b8-b8e8-89fcbcde6e11.mp4
 
-Note: You could even ask for it in markdown format, which would look better (not shown here).
+Note: You could even ask for it in markdown format, which would look better (not
+shown here).
 
 ##
-Next I ask Omega to make a widget that lets me filter segments by area. And it works beautifully.
-Arguably it is not rocket science, but the thought-to-widget time ratio must be in the hundreds when comparing Omega to an average user trying to write their own widget:
+
+Next I ask Omega to make a widget that lets me filter segments by area. And it
+works beautifully.
+Arguably it is not rocket science, but the thought-to-widget time ratio must be
+in the hundreds when comparing Omega to an average user trying to write their
+own widget:
 
 https://user-images.githubusercontent.com/1870994/235770860-4287e6a3-dae3-4c6d-a588-dea2bb1f69b7.mp4
 
 ##
-This is an example of a failed widget. I ask for a widget that can do dilations and erosions. The widget
-is created but is 'broken' because Omega made the mistake of using floats for the number of dilations
+
+This is an example of a failed widget. I ask for a widget that can do dilations
+and erosions. The widget
+is created but is 'broken' because Omega made the mistake of using floats for
+the number of dilations
 and erosions: (In the next video I tell Omega to fix it)
 
 https://user-images.githubusercontent.com/1870994/235770896-819f394d-9785-46e8-a31a-a135b19316bf.mp4
 
 ##
-Following up from previous video, I explain that I want the two parameters (number erosions and dilations)
-to be integers. Notice that I exploit the conversational nature of the agent by assuming that it remembers
+
+Following up from previous video, I explain that I want the two parameters (
+number erosions and dilations)
+to be integers. Notice that I exploit the conversational nature of the agent by
+assuming that it remembers
 what the widget is about:
 
 https://user-images.githubusercontent.com/1870994/235770914-90991ac4-337e-4dcd-a04c-dd44b5e8be3e.mp4
 
 ##
-This video demos a specialised 'cell and nuclei segmentation tool' which leverages [cellpose 2.0](https://www.cellpose.org/) to segment cell cytoplasms or nuclei. In general, we can't assume that
-LLMs know about every single image processing library, especially for specific domains. So it can be 
-a good strategy to provide such specialised tools. After Omega successfully segments the nuclei, I ask
-from it to count the nuclei. Answer: 340. Notice that the code generated 'searches' the layer with name 'segmented' with a loop. Cute:
+
+This video demos a specialised 'cell and nuclei segmentation tool' which
+leverages [cellpose 2.0](https://www.cellpose.org/) to segment cell cytoplasms
+or nuclei. In general, we can't assume that
+LLMs know about every single image processing library, especially for specific
+domains. So it can be
+a good strategy to provide such specialised tools. After Omega successfully
+segments the nuclei, I ask
+from it to count the nuclei. Answer: 340. Notice that the code generated '
+searches' the layer with name 'segmented' with a loop. Cute:
 
 https://user-images.githubusercontent.com/1870994/235770933-07f5cbe6-2224-4dcd-b378-e81cc4e66500.mov
 
 ##
-Enough with cells. Aparently The 'memory' of ChatGPT is filled with unescessary information, it knows the url of Albert Einstein's photo on wikipedia, and combined with the 'napari file open' tool it can therefore open that photo in napari:
+
+Enough with cells. Aparently The 'memory' of ChatGPT is filled with unescessary
+information, it knows the url of Albert Einstein's photo on wikipedia, and
+combined with the 'napari file open' tool it can therefore open that photo in
+napari:
 
 https://user-images.githubusercontent.com/1870994/235770959-406e8173-8416-4100-bcb6-7f0b617ce234.mp4
 
-## 
-You can ask for rather incongruous widgets, widgets you would probably never write because you just need them once or something. Here I ask for a widget that applies a rather odd non-linear transformation to each
-pixel. The result is predictably boring, but it works, and I don't think that the answer was 'copy pasted'
+##  
+
+You can ask for rather incongruous widgets, widgets you would probably never
+write because you just need them once or something. Here I ask for a widget that
+applies a rather odd non-linear transformation to each
+pixel. The result is predictably boring, but it works, and I don't think that
+the answer was 'copy pasted'
 from somewhere else...
 
 https://user-images.githubusercontent.com/1870994/235770984-c88c8eac-d3b2-47d7-81b1-48fbe4429e90.mp4
 
 ##
-In this one, starting again from our beloved Albert, I ask to rename that layer to 'Einstein' which looks
-better than just 'array'. Then I ask Omega to apply a Canny edge filter. Predictably it uses scikit-image:
+
+In this one, starting again from our beloved Albert, I ask to rename that layer
+to 'Einstein' which looks
+better than just 'array'. Then I ask Omega to apply a Canny edge filter.
+Predictably it uses scikit-image:
 
 https://user-images.githubusercontent.com/1870994/235771000-89dba0db-e710-4f76-b271-e9dcf65239b1.mp4
 
-## 
-Then I ask for a 'Canny edge detection widget'. It happily makes the widget and offers relevant parameters:
+##  
+
+Then I ask for a 'Canny edge detection widget'. It happily makes the widget and
+offers relevant parameters:
 
 https://user-images.githubusercontent.com/1870994/235771031-d978b652-2e28-4178-aa7e-dbdfd2e21c2d.mp4
 
 ##
-Following up on previous video, I play with dilations on the edge image. 
-Omega has some trouble when I ask to 'do it again'. Fine, sometimes you have a bit more explicit:
+
+Following up on previous video, I play with dilations on the edge image.
+Omega has some trouble when I ask to 'do it again'. Fine, sometimes you have a
+bit more explicit:
 
 https://user-images.githubusercontent.com/1870994/235771066-adc7f0bb-0b8e-415c-8e89-6107182cd5b1.mp4
 
 ##
-You can also experiment with more classic 'numpy' code by creating and manipulating arrays and visualising 
+
+You can also experiment with more classic 'numpy' code by creating and
+manipulating arrays and visualising
 the output live:
 
 https://user-images.githubusercontent.com/1870994/235771093-85a751c8-cc5a-4685-b40a-acdf81f0e5c9.mp4
 
 ##
-This video demonstrates that Omega understand many aspects of the napari viewer API. It can switch viewing modes, translate layers, etc... :
+
+This video demonstrates that Omega understand many aspects of the napari viewer
+API. It can switch viewing modes, translate layers, etc... :
 
 https://user-images.githubusercontent.com/1870994/235771129-db095c1f-56f7-4bb9-9bff-ef57ce66387b.mp4
 
 ##
-I never thought this one would work: I ask Omega to open in napari a mp4 video from a URL and then use OpenCV to detect people. It does it. But the one thing that Omega does not know is that creating a layer for each frame of the video is not a practical approach. Not clear what happened to the colors though. Probably an RGB ordering or format issue:
 
-https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
+I never thought this one would work: I ask Omega to open in napari a mp4 video
+from a URL and then use OpenCV to detect people. It does it. But the one thing
+that Omega does not know is that creating a layer for each frame of the video is
+not a practical approach. Not clear what happened to the colors though. Probably
+an RGB ordering or format issue:
 
+https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
 
 ## Disclaimer:
 
 Do not use this software lightly, it will download libaries by its own volition,
-write any code that it deems nescessary, it might actually do what you ask, even if
-it is a bad idea. Also, beware that it might _misundertand_ what you ask and then do
-something bad. For example, it is unwise to use Omega to delete 'some' files from your system,
+write any code that it deems nescessary, it might actually do what you ask, even
+if
+it is a bad idea. Also, beware that it might _misundertand_ what you ask and
+then do
+something bad. For example, it is unwise to use Omega to delete 'some' files
+from your system,
 it might end up deleteing more than that if you are unclear in your request.  
-To be 100% safe, we recommend that you use this software from within a sandboxed virtual machine. 
+To be 100% safe, we recommend that you use this software from within a sandboxed
+virtual machine.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
-INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR 
-PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE 
-FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
-TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE 
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED,
+INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR
+PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+BE LIABLE
+FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
+THE
 USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-
 ## Contributing
 
-Contributions are very welcome. Tests can be run with [tox], please ensure
+Contributions are extremely welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-chatgpt" is free and open source software
```

### Comparing `napari-chatgpt-2023.5.2/README.md` & `napari-chatgpt-2023.6.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,131 @@
-# napari-chatgpt, home of _Omega_, a napari-aware autonomous LLM-based agent.
+# napari-chatgpt
+
+## Home of
+_Omega_, a napari-aware autonomous LLM-based agent specialised in image processing and analysis.
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
 
-A [napari](napari.org) plugin that levegares OpenAI's Large Language Model ChatGPT to implement _Omega_ 
-a napari-aware agent capable of performing image processing and analysis tasks in a conversational manner.
-
-This repository was created as a 'week-end project' by [Loic A. Royer](https://twitter.com/loicaroyer) 
-who leads a [research group](https://royerlab.org) at the [Chan Zuckerberg Biohub](https://czbiohub.org/sf/). It levegages [OpenAI](https://openai.com)'s ChatGPT API via the [LangChain](https://python.langchain.com/en/latest/index.html) Python library, as well as [napari](https://napari.org), a fast, interactive, multi-dimensional 
-image viewer for Python, [another](https://ilovesymposia.com/2019/10/24/introducing-napari-a-fast-n-dimensional-image-viewer-in-python/) 
+A [napari](napari.org) plugin that levegares OpenAI's Large Language Model
+ChatGPT to implement _Omega_
+a napari-aware agent capable of performing image processing and analysis tasks
+in a conversational manner.
+
+This repository was created as a 'week-end project'
+by [Loic A. Royer](https://twitter.com/loicaroyer)
+who leads a [research group](https://royerlab.org) at
+the [Chan Zuckerberg Biohub](https://czbiohub.org/sf/). It
+levegages [OpenAI](https://openai.com)'s ChatGPT API via
+the [LangChain](https://python.langchain.com/en/latest/index.html) Python
+library, as well as [napari](https://napari.org), a fast, interactive,
+multi-dimensional
+image viewer for
+Python, [another](https://ilovesymposia.com/2019/10/24/introducing-napari-a-fast-n-dimensional-image-viewer-in-python/)
 of Loic's week-end projects.
 
 # What is Omega?
 
-Omega is a LLM-based and tool-armed autonomous agent that demonstrates the potential for Large Language Models (LLMs) to be applied to image processing, analysis and visualisation. 
-Can LLM-based agents write image processing code and napari widgets, correct its coding mistakes, perform 
+Omega is a LLM-based and tool-armed autonomous agent that demonstrates the
+potential for Large Language Models (LLMs) to be applied to image processing,
+analysis and visualisation.
+Can LLM-based agents write image processing code and napari widgets, correct its
+coding mistakes, perform
 follow-up analysis, and control the napari viewer? The answer appears to be yes.
 
 #### In this video I ask Omega to segment an image using the [SLIC](https://www.iro.umontreal.ca/~mignotte/IFT6150/Articles/SLIC_Superpixels.pdf) algorithm. It makes a first attempt using the implementation in scikit-image, but fails because of an inexistant 'multichannel' parameter. Realising that, Omega tries again, and this time, succeeds:
+
 https://user-images.githubusercontent.com/1870994/235768559-ca8bfa84-21f5-47b6-b2bd-7fcc07cedd92.mp4
 
-#### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:   
-https://user-images.githubusercontent.com/1870994/235769990-a281a118-1369-47aa-834a-b491f706bd48.mp4
+#### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:
 
+https://user-images.githubusercontent.com/1870994/235769990-a281a118-1369-47aa-834a-b491f706bd48.mp4
 
-As LLMs continue to improve, Omega will become even more adept at handling complex 
-image processing and analysis tasks. The current version of ChatGPT, 3.5, 
-has a cutoff date of 2021, which means that it lacks nearly two years of knowledge 
-on the napari API and usage, as well as the latest versions of popular libraries 
-like scikit-image, OpenCV, numpy, scipy, etc... Despite this, you can see in the videos below 
-that it is quite capable. While ChatGPT 4.0 is a significant upgrade, it is not yet widely 
+As LLMs continue to improve, Omega will become even more adept at handling
+complex
+image processing and analysis tasks. The current version of ChatGPT, 3.5,
+has a cutoff date of 2021, which means that it lacks nearly two years of
+knowledge
+on the napari API and usage, as well as the latest versions of popular libraries
+like scikit-image, OpenCV, numpy, scipy, etc... Despite this, you can see in the
+videos below
+that it is quite capable. While ChatGPT 4.0 is a significant upgrade, it is not
+yet widely
 available.
 
-Omega could eventually help non-experts process and analyse images, especially in the bioimage domain. 
-It is also potentially valuable for educative purposes as it could 
-assist in teaching image processing and analysis, making it more accessible. 
-Although ChatGPT, which powers Omega, may not be yet on par with an expert image analyst or computer vision 
+Omega could eventually help non-experts process and analyse images, especially
+in the bioimage domain.
+It is also potentially valuable for educative purposes as it could
+assist in teaching image processing and analysis, making it more accessible.
+Although ChatGPT, which powers Omega, may not be yet on par with an expert image
+analyst or computer vision
 expert, it is just a matter of time...
 
-Omega holds a conversation with the user and uses the following tools to acheive answer questions, 
+Omega holds a conversation with the user and uses the following tools to acheive
+answer questions,
 download and operate on images, write widgets for napari, and more:
 
 ### napari related tools:
-- napari viewer control: 
-    Gives Omega the ability to control all aspects of the napari viewer.
-  
+
+- napari viewer control:
+  Gives Omega the ability to control all aspects of the napari viewer.
+
 - napari query:
-    Gives Omega the ability to query information about the state of the viewer, of its layers, and their contents.
+  Gives Omega the ability to query information about the state of the viewer, of
+  its layers, and their contents.
 
 - napari widget maker:
-    Gives Omega the ability to make napari functional widgets that take layers as input and return a new layer.
+  Gives Omega the ability to make napari functional widgets that take layers as
+  input and return a new layer.
+
+### cell segmentation tools:
 
-### cell segmentation tools: 
 - cell and nuclei segmentation:
-    This tool specialises in segmenting cells and nuclei in images using some predefined segmentation algorithms. Right now only cellpose is implemented. 
+  This tool specialises in segmenting cells and nuclei in images using some
+  predefined segmentation algorithms. Right now only cellpose is implemented.
 
 ### Generic python installation queries:
+
 - python function signature query:
-    Lets Omega query the signature of function when it is unsure how to call a function and what the names and type of the parameters are.
+  Lets Omega query the signature of function when it is unsure how to call a
+  function and what the names and type of the parameters are.
 
 ### web search related tools:
+
 - web search:
-    Usefull to give Omega access to the knowledge accessible through the web
+  Usefull to give Omega access to the knowledge accessible through the web
 
 - web image serach:
-    Streamlined path to search the web for images and open them in napari  
+  Streamlined path to search the web for images and open them in napari
 
 - wikipedia search:
-    Gives Omega access to the whole wikipedia
-
+  Gives Omega access to the whole wikipedia
 
 ----------------------------------
 
-## Installation:
+## Installation from within napari:
+
+You can install `napari-chatgpt` directly from within napari in the Plugins>
+Install/Uninstall Plugins menu.
+(Please note that the Omega agent will hapilly install packages in the
+corresponding environment).
+
+IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the
+latest one!
 
-You can also install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
-(Please note that the Omega agent will hapilly install packages in the corresponding environment)
+## Installation in an new conda environment (RECOMMENDED):
 
-Create environment: 
+Make sure you have an anaocnda/miniconda installation on your system.
+Ask ChatGPT what is that all about if you are unsure ;-)
+
+Create environment:
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
     conda activate napari-chatgpt 
 
@@ -93,238 +133,328 @@
 
     conda install -c conda-forge napari     
 
 Install the repo in enbvironment:
 
     pip install napari-chatgpt
 
-
 ## Installation variations:
 
 To install latest development version :
 
     git clone https://github.com/royerlab/napari-chatgpt.git
     cd napari-chatgpt
     pip install -e .
 
 or:
 
     pip install git+https://github.com/royerlab/napari-chatgpt.git
 
-
 ## Requirements:
 
 You need an OpenAI key, there is no way around this, unless we add some other,
-potentially local LLMs compatible to LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar models come to mind). However, this will likely be at the cost of cognitive performance,
+potentially local LLMs compatible to
+LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar
+models come to mind). However, this will likely be at the cost of cognitive
+performance,
 which I am not sure is worth it at this point. Please prove me wrong.
-You can get your OpenAI key by signing up [here](https://openai.com/blog/openai-api).
-Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5 is very
-reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A bargain.
-Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop, hopefully.
-
-Note: you can limit the burn-rate to a certain amount of dollars per month, just in case you let
-Omega thinking over the week end and forget to stop it (don't worry, this is actually not possible). 
-
+You can get your OpenAI key by signing
+up [here](https://openai.com/blog/openai-api).
+Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5
+is very
+reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
+bargain.
+Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
+hopefully.
+
+Note: you can limit the burn-rate to a certain amount of dollars per month, just
+in case you let
+Omega thinking over the week end and forget to stop it (don't worry, this is
+actually not possible).
 
 ## Usage:
 
 Once all is installed, and if it is not already running, start napari:
 
     napari
-    
+
 You can then the Omega napari plugin via the plugins menu:
 
 <img width="498" alt="image" src="https://user-images.githubusercontent.com/1870994/235790134-1d87fd50-583f-4fd9-ade2-c64497b91331.png">
 
 
 You just opened the plugin as a widget, you now need to actually start Omega:
 
 <img width="104" alt="image" src="https://user-images.githubusercontent.com/1870994/235811111-9e468785-9562-410a-8e9a-c63cb03fb765.png">
 
 
-If you have not set the 'OPENAI_API_KEY' environment variable as is typicall done,
-Omega will ask you for your OpenAI API key, and will store it _safely_ in an _encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
+If you have not set the 'OPENAI_API_KEY' environment variable as is typicall
+done,
+Omega will ask you for your OpenAI API key, and will store it _safely_ in an
+_encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
 
 <img width="293" alt="image" src="https://user-images.githubusercontent.com/1870994/235793528-9e892c5e-d8ca-43e1-9020-f2dfab45b32d.png">
 
 
 Just enter an encryption/decription key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
-(The idea is that you might not be able to remember your openAI key by heart, but you might be able to do so with your own password or passphrase)
+(The idea is that you might not be able to remember your openAI key by heart,
+but you might be able to do so with your own password or passphrase)
 
-You can then direct your browser to: [http://0.0.0.0:9000/](http://0.0.0.0:9000/)
+You can then direct your browser
+to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
 and start having an hopefully nice chat with Omega.
 
-
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
 - What is your name?
 - What tools do you have available?
 - Make me a Gaussian blur widget with sigma parameter
-- Open this tiff file in napari: https://people.math.sc.edu/Burkardt/data/tif/at3_1m4_03.tif
-- Make a widget that applies the transformation: y = x^alpha + y^beta with alpha and beta two parameters.
+- Open this tiff file in
+  napari: https://people.math.sc.edu/Burkardt/data/tif/at3_1m4_03.tif
+- Make a widget that applies the transformation: y = x^alpha + y^beta with alpha
+  and beta two parameters.
 - Create a widget to multiply two images
 - Can you open in napari a photo of Albert Einstein?
 - Downscale by a factor 3x the image on layer named 'img'
 - Rename selected layer to 'downscaled_image'
-- Upscale image 'downscaled_image' by a factor 3 using some smart interpolation scheme of your choice (not nearest-neighboor)
+- Upscale image 'downscaled_image' by a factor 3 using some smart interpolation
+  scheme of your choice (not nearest-neighboor)
 - Caveat: makes a plugin instead of actually doing teh job
 - How many channels has the image on layer 0
 - Make a image sharpening filter widget, expose relevant parameters
-- Can you open this file in napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
-- Split the two channels of the first layer (first axis) into two separate layers
+- Can you open this file in
+  napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
+- Split the two channels of the first layer (first axis) into two separate
+  layers
 - Switch viewer to 3d
-- Create a napari widget for a function that takes two image layers and returns a 3D image stack of n images where each 2D image corresponds to a linear blending of the two layer images between 0 and 1.
-- [Loaded the ‘cell’ sample image] there is one cell in the image on the first layer, it is roughly circular and brighter than its surroundings, ca you write segmentation code that returns a labels layer for it?
+- Create a napari widget for a function that takes two image layers and returns
+  a 3D image stack of n images where each 2D image corresponds to a linear
+  blending of the two layer images between 0 and 1.
+- [Loaded the ‘cell’ sample image] there is one cell in the image on the first
+  layer, it is roughly circular and brighter than its surroundings, ca you write
+  segmentation code that returns a labels layer for it?
 - Can you create a widget to blend two images?
 - Can you tell me more about the 'guided Canny edge filter' ?
 - Write a configurable RGB to grayscale widget, ensure weights sum to 1
 
 ## Video Demos:
 
-Not everyone will want, or can, get an API key for the latest and best LLM models, 
-so here are videos showcasing what's possible. You will notice that Omega sometimes 
-fails on its first attempt, typically because of mistaken parameters for functions,
-or other syntax errors. But it also often recovers by having access to the error message,
-and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can do, imagine
+Not everyone will want, or can, get an API key for the latest and best LLM
+models,
+so here are videos showcasing what's possible. You will notice that Omega
+sometimes
+fails on its first attempt, typically because of mistaken parameters for
+functions,
+or other syntax errors. But it also often recovers by having access to the error
+message,
+and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can
+do, imagine
 what will be possible with 4.0 and future more capable models...
 
 ##
-In this first video, I ask Omega to make a napari widget to convert images from RGB to grayscale:
+
+In this first video, I ask Omega to make a napari widget to convert images from
+RGB to grayscale:
 
 https://user-images.githubusercontent.com/1870994/235769895-23cfc7ed-622a-47f9-95aa-4be77efc0f78.mp4
 
 ##
-Of course Omega is capable of holding a conversation, it sort of knows 'who it is', can search the web
-and wikipedia. Eventually I imagine it could leverage the ability to search for improving its responses,
+
+Of course Omega is capable of holding a conversation, it sort of knows 'who it
+is', can search the web
+and wikipedia. Eventually I imagine it could leverage the ability to search for
+improving its responses,
 and I have seen doing it a few times:
 
 https://user-images.githubusercontent.com/1870994/235769920-86b02d9d-1196-4339-a8d9-9a028bcd4607.mp4
 
 ##
-Following-up from the previous video, I ask Omega to create a new labels layer containing just the largest segment. The script that Omega writes as another rookie mistake: it confuses layers and images. The error message then confuses Omega into thinking that it got the name of the layer wrong, setting it off in a quest
-to find the name of the labels layer. It succeeds at writting code that searches for the labels layer, and uses that name to write a script that then does extracts te largest segment into its own layer. Not bad: 
+
+Following-up from the previous video, I ask Omega to create a new labels layer
+containing just the largest segment. The script that Omega writes as another
+rookie mistake: it confuses layers and images. The error message then confuses
+Omega into thinking that it got the name of the layer wrong, setting it off in a
+quest
+to find the name of the labels layer. It succeeds at writting code that searches
+for the labels layer, and uses that name to write a script that then does
+extracts te largest segment into its own layer. Not bad:
 
 https://user-images.githubusercontent.com/1870994/235770741-d8905afd-0a9b-4eb7-a075-481979ab7b01.mp4
 
 ##
-In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific. The answer is a vanilla yet effective widget that uses the Otsu approach to threshold the image and then finds the connected components.
-Note that when you ask Omega to make a widget, it won't know of any runtime issues with the code because
-it is not running the code itself, yet. It can tell if there is a syntax problem though... Nevertheless, the widget ends up working just fine:
+
+In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific.
+The answer is a vanilla yet effective widget that uses the Otsu approach to
+threshold the image and then finds the connected components.
+Note that when you ask Omega to make a widget, it won't know of any runtime
+issues with the code because
+it is not running the code itself, yet. It can tell if there is a syntax problem
+though... Nevertheless, the widget ends up working just fine:
 
 https://user-images.githubusercontent.com/1870994/235770794-90091bfe-b546-4dd0-bd9c-3895bfc33a1d.mp4
 
 ##
-Now it gets more interesting. Following up on the previous video, can we ask Omega to do some follow-
-up analysis on the segments themselves? I ask Omega to list the 10 largest segments and compute their 
-areas and centroids. No problem: 
+
+Now it gets more interesting. Following up on the previous video, can we ask
+Omega to do some follow-
+up analysis on the segments themselves? I ask Omega to list the 10 largest
+segments and compute their
+areas and centroids. No problem:
 
 https://user-images.githubusercontent.com/1870994/235770828-0f829f76-1f3d-44b8-b8e8-89fcbcde6e11.mp4
 
-Note: You could even ask for it in markdown format, which would look better (not shown here).
+Note: You could even ask for it in markdown format, which would look better (not
+shown here).
 
 ##
-Next I ask Omega to make a widget that lets me filter segments by area. And it works beautifully.
-Arguably it is not rocket science, but the thought-to-widget time ratio must be in the hundreds when comparing Omega to an average user trying to write their own widget:
+
+Next I ask Omega to make a widget that lets me filter segments by area. And it
+works beautifully.
+Arguably it is not rocket science, but the thought-to-widget time ratio must be
+in the hundreds when comparing Omega to an average user trying to write their
+own widget:
 
 https://user-images.githubusercontent.com/1870994/235770860-4287e6a3-dae3-4c6d-a588-dea2bb1f69b7.mp4
 
 ##
-This is an example of a failed widget. I ask for a widget that can do dilations and erosions. The widget
-is created but is 'broken' because Omega made the mistake of using floats for the number of dilations
+
+This is an example of a failed widget. I ask for a widget that can do dilations
+and erosions. The widget
+is created but is 'broken' because Omega made the mistake of using floats for
+the number of dilations
 and erosions: (In the next video I tell Omega to fix it)
 
 https://user-images.githubusercontent.com/1870994/235770896-819f394d-9785-46e8-a31a-a135b19316bf.mp4
 
 ##
-Following up from previous video, I explain that I want the two parameters (number erosions and dilations)
-to be integers. Notice that I exploit the conversational nature of the agent by assuming that it remembers
+
+Following up from previous video, I explain that I want the two parameters (
+number erosions and dilations)
+to be integers. Notice that I exploit the conversational nature of the agent by
+assuming that it remembers
 what the widget is about:
 
 https://user-images.githubusercontent.com/1870994/235770914-90991ac4-337e-4dcd-a04c-dd44b5e8be3e.mp4
 
 ##
-This video demos a specialised 'cell and nuclei segmentation tool' which leverages [cellpose 2.0](https://www.cellpose.org/) to segment cell cytoplasms or nuclei. In general, we can't assume that
-LLMs know about every single image processing library, especially for specific domains. So it can be 
-a good strategy to provide such specialised tools. After Omega successfully segments the nuclei, I ask
-from it to count the nuclei. Answer: 340. Notice that the code generated 'searches' the layer with name 'segmented' with a loop. Cute:
+
+This video demos a specialised 'cell and nuclei segmentation tool' which
+leverages [cellpose 2.0](https://www.cellpose.org/) to segment cell cytoplasms
+or nuclei. In general, we can't assume that
+LLMs know about every single image processing library, especially for specific
+domains. So it can be
+a good strategy to provide such specialised tools. After Omega successfully
+segments the nuclei, I ask
+from it to count the nuclei. Answer: 340. Notice that the code generated '
+searches' the layer with name 'segmented' with a loop. Cute:
 
 https://user-images.githubusercontent.com/1870994/235770933-07f5cbe6-2224-4dcd-b378-e81cc4e66500.mov
 
 ##
-Enough with cells. Aparently The 'memory' of ChatGPT is filled with unescessary information, it knows the url of Albert Einstein's photo on wikipedia, and combined with the 'napari file open' tool it can therefore open that photo in napari:
+
+Enough with cells. Aparently The 'memory' of ChatGPT is filled with unescessary
+information, it knows the url of Albert Einstein's photo on wikipedia, and
+combined with the 'napari file open' tool it can therefore open that photo in
+napari:
 
 https://user-images.githubusercontent.com/1870994/235770959-406e8173-8416-4100-bcb6-7f0b617ce234.mp4
 
-## 
-You can ask for rather incongruous widgets, widgets you would probably never write because you just need them once or something. Here I ask for a widget that applies a rather odd non-linear transformation to each
-pixel. The result is predictably boring, but it works, and I don't think that the answer was 'copy pasted'
+##  
+
+You can ask for rather incongruous widgets, widgets you would probably never
+write because you just need them once or something. Here I ask for a widget that
+applies a rather odd non-linear transformation to each
+pixel. The result is predictably boring, but it works, and I don't think that
+the answer was 'copy pasted'
 from somewhere else...
 
 https://user-images.githubusercontent.com/1870994/235770984-c88c8eac-d3b2-47d7-81b1-48fbe4429e90.mp4
 
 ##
-In this one, starting again from our beloved Albert, I ask to rename that layer to 'Einstein' which looks
-better than just 'array'. Then I ask Omega to apply a Canny edge filter. Predictably it uses scikit-image:
+
+In this one, starting again from our beloved Albert, I ask to rename that layer
+to 'Einstein' which looks
+better than just 'array'. Then I ask Omega to apply a Canny edge filter.
+Predictably it uses scikit-image:
 
 https://user-images.githubusercontent.com/1870994/235771000-89dba0db-e710-4f76-b271-e9dcf65239b1.mp4
 
-## 
-Then I ask for a 'Canny edge detection widget'. It happily makes the widget and offers relevant parameters:
+##  
+
+Then I ask for a 'Canny edge detection widget'. It happily makes the widget and
+offers relevant parameters:
 
 https://user-images.githubusercontent.com/1870994/235771031-d978b652-2e28-4178-aa7e-dbdfd2e21c2d.mp4
 
 ##
-Following up on previous video, I play with dilations on the edge image. 
-Omega has some trouble when I ask to 'do it again'. Fine, sometimes you have a bit more explicit:
+
+Following up on previous video, I play with dilations on the edge image.
+Omega has some trouble when I ask to 'do it again'. Fine, sometimes you have a
+bit more explicit:
 
 https://user-images.githubusercontent.com/1870994/235771066-adc7f0bb-0b8e-415c-8e89-6107182cd5b1.mp4
 
 ##
-You can also experiment with more classic 'numpy' code by creating and manipulating arrays and visualising 
+
+You can also experiment with more classic 'numpy' code by creating and
+manipulating arrays and visualising
 the output live:
 
 https://user-images.githubusercontent.com/1870994/235771093-85a751c8-cc5a-4685-b40a-acdf81f0e5c9.mp4
 
 ##
-This video demonstrates that Omega understand many aspects of the napari viewer API. It can switch viewing modes, translate layers, etc... :
+
+This video demonstrates that Omega understand many aspects of the napari viewer
+API. It can switch viewing modes, translate layers, etc... :
 
 https://user-images.githubusercontent.com/1870994/235771129-db095c1f-56f7-4bb9-9bff-ef57ce66387b.mp4
 
 ##
-I never thought this one would work: I ask Omega to open in napari a mp4 video from a URL and then use OpenCV to detect people. It does it. But the one thing that Omega does not know is that creating a layer for each frame of the video is not a practical approach. Not clear what happened to the colors though. Probably an RGB ordering or format issue:
 
-https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
+I never thought this one would work: I ask Omega to open in napari a mp4 video
+from a URL and then use OpenCV to detect people. It does it. But the one thing
+that Omega does not know is that creating a layer for each frame of the video is
+not a practical approach. Not clear what happened to the colors though. Probably
+an RGB ordering or format issue:
 
+https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
 
 ## Disclaimer:
 
 Do not use this software lightly, it will download libaries by its own volition,
-write any code that it deems nescessary, it might actually do what you ask, even if
-it is a bad idea. Also, beware that it might _misundertand_ what you ask and then do
-something bad. For example, it is unwise to use Omega to delete 'some' files from your system,
+write any code that it deems nescessary, it might actually do what you ask, even
+if
+it is a bad idea. Also, beware that it might _misundertand_ what you ask and
+then do
+something bad. For example, it is unwise to use Omega to delete 'some' files
+from your system,
 it might end up deleteing more than that if you are unclear in your request.  
-To be 100% safe, we recommend that you use this software from within a sandboxed virtual machine. 
+To be 100% safe, we recommend that you use this software from within a sandboxed
+virtual machine.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
-INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR 
-PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE 
-FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
-TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE 
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED,
+INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR
+PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+BE LIABLE
+FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
+THE
 USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-
 ## Contributing
 
-Contributions are very welcome. Tests can be run with [tox], please ensure
+Contributions are extremely welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-chatgpt" is free and open source software
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/conv_agent_demo.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/conv_agent_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from langchain.agents import initialize_agent
 from langchain.agents.load_tools import _get_llm_math
 from langchain.chat_models import ChatOpenAI
 from langchain.memory import ConversationBufferMemory
 from langchain.tools.python.tool import PythonREPLTool
 from langchain.tools.wikipedia.tool import WikipediaQueryRun
 
-from napari_chatgpt.omega.tools.google_search_tool import GoogleSearchTool
+from napari_chatgpt.omega.tools.search.web_search_tool import WebSearchTool
 
 llm = ChatOpenAI(temperature=0)
 
 memory = ConversationBufferMemory(memory_key="chat_history",
                                   return_messages=True)
 
 wiki = WikipediaQueryRun(api_wrapper=WikipediaAPIWrapper())
-tools = [wiki, GoogleSearchTool(), _get_llm_math(llm), PythonREPLTool()]
+tools = [wiki, WebSearchTool(), _get_llm_math(llm), PythonREPLTool()]
 
 system_message = """Omega is a large language model trained by OpenAI.
 
 Omega is designed to be able to assist with a wide range of tasks, 
 from answering simple questions to providing in-depth explanations and 
 discussions on a wide range of topics. As a language model, Omega is 
 able to generate human-like text based on the input it receives, allowing
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/enumerate_functions.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/enumerate_functions.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/lanchain_openai.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/lanchain_openai.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/playwright_sandbox.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/playwright_sandbox.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/speech_recognition_demo.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/speech_recognition_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/terminal.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/terminal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/tts_demo.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/tts_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/whisper_cpp.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/whisper_cpp.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/_tests/test_widget.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/_tests/test_widget.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
     viewer.add_image(np.random.random((100, 100)))
 
     # create our widget, passing in the viewer
     my_widget = OmegaQWidget(viewer)
 
-    # call our widget method
-    my_widget._on_click()
-
-    # read captured output and check that it's as we expected
-    captured = capsys.readouterr()
-    assert 'Omega' in captured.out
+    # # call our widget method
+    # my_widget._on_click()
+    #
+    # # read captured output and check that it's as we expected
+    # captured = capsys.readouterr()
+    # assert 'Omega' in captured.out
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/callback_handle_chat.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,50 @@
 import asyncio
-from typing import Any, Dict, Union, List
+from pprint import pprint
+from typing import Any, Dict, Union, List, Optional
+from uuid import UUID
 
 from arbol import aprint
 from langchain.callbacks.base import AsyncCallbackHandler
-from langchain.schema import AgentFinish, AgentAction, LLMResult
+from langchain.schema import AgentFinish, AgentAction, LLMResult, BaseMessage
 
 from napari_chatgpt.chat_server.chat_response import ChatResponse
-from napari_chatgpt.utils.camel_case_to_normal import camel_case_to_lower_case
+from napari_chatgpt.omega.omega_agent.agent_output_parser import parse_command
+from napari_chatgpt.utils.strings.camel_case_to_normal import \
+    camel_case_to_lower_case
 
 
 class ChatCallbackHandler(AsyncCallbackHandler):
     """Callback handler for chat responses."""
 
-    def __init__(self, websocket):
+    def __init__(self, websocket, verbose: bool = False):
         self.websocket = websocket
+        self.verbose = verbose
+        self.last_tool_used = ''
+        self.last_tool_input = ''
+
+    async def on_chat_model_start(
+            self,
+            serialized: Dict[str, Any],
+            messages: List[List[BaseMessage]],
+            *,
+            run_id: UUID,
+            parent_run_id: Optional[UUID] = None,
+            **kwargs: Any,
+    ) -> Any:
+        """Run when a chat model starts running."""
+        if self.verbose:
+            aprint(
+                f"CHAT on_chat_model_start: serialized={serialized},  messages={messages}, run_id={run_id}, parent_run_id={parent_run_id}, kwargs={kwargs}")
 
     async def on_llm_start(
             self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> Any:
         """Run when LLM starts running."""
+        pprint(prompts)
         resp = ChatResponse(sender="agent", message='', type="typing")
         await self.websocket.send_json(resp.dict())
 
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> Any:
         """Run on new LLM token. Only available when streaming is enabled."""
 
     async def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
@@ -34,65 +56,76 @@
         """Run when LLM errors."""
 
     async def on_chain_start(
             self, serialized: Dict[str, Any], inputs: Dict[str, Any],
             **kwargs: Any
     ) -> Any:
         """Run when chain starts running."""
-        aprint(
-            f"CHAT on_chain_start: serialized={serialized},  inputs={inputs}")
+        if self.verbose:
+            aprint(
+                f"CHAT on_chain_start: serialized={serialized},  inputs={inputs}")
 
     async def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
         """Run when chain ends running."""
-        aprint(f"CHAT on_chain_end: {outputs}")
+        if self.verbose:
+            aprint(f"CHAT on_chain_end: {outputs}")
 
     async def on_chain_error(
             self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when chain errors."""
-        aprint(f"CHAT on_chain_error: {error}")
+        if self.verbose:
+            aprint(f"CHAT on_chain_error: {error}")
 
     async def on_tool_start(
             self, serialized: Dict[str, Any], input_str: str, **kwargs: Any
     ) -> Any:
         """Run when tool starts running."""
-        aprint(
-            f"CHAT on_tool_start: serialized={serialized}, input_str={input_str}")
+        if self.verbose:
+            aprint(
+                f"CHAT on_tool_start: serialized={serialized}, input_str={input_str}")
 
     async def on_tool_end(self, output: str, **kwargs: Any) -> Any:
         """Run when tool ends running."""
-        aprint(f"CHAT on_tool_end: output={output}")
+        if self.verbose:
+            aprint(f"CHAT on_tool_end: output={output}")
 
     async def on_tool_error(
             self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when tool errors."""
-        aprint(f"CHAT on_tool_error: {error}")
+        if self.verbose:
+            aprint(f"CHAT on_tool_error: {error}")
         error_type = type(error).__name__
         error_message = ', '.join(error.args)
         message = f"Failed because:\n'{error_message}'\nException: '{error_type}'\n"
         resp = ChatResponse(sender="agent", message=message, type="error")
         asyncio.run(self.websocket.send_json(resp.dict()))
 
     async def on_text(self, text: str, **kwargs: Any) -> Any:
         """Run on arbitrary text."""
-        pass
-        aprint(f"CHAT on_text: {text}")
+        if self.verbose:
+            aprint(f"CHAT on_text: {text}")
 
     async def on_agent_action(self, action: AgentAction, **kwargs: Any) -> Any:
         """Run on agent action."""
-        aprint(f"CHAT on_agent_action: {action}")
+        if self.verbose:
+            aprint(f"CHAT on_agent_action: {action}")
         tool = camel_case_to_lower_case(action.tool)
         message = f"I am using the {tool} to tackle your request: '{action.tool_input}'"
 
-        if not 'Action:' in action.log and not 'Input:' in action.log:
+        self.last_tool_used = tool
+        self.last_tool_input = action.tool_input
+
+        if not parse_command([action.tool],action.log):
             message += f"\n {action.log}"
 
         resp = ChatResponse(sender="agent", message=message, type="action")
         await self.websocket.send_json(resp.dict())
 
     async def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
         """Run on agent end."""
-        aprint(f"CHAT on_agent_finish: {finish}")
+        if self.verbose:
+            aprint(f"CHAT on_agent_finish: {finish}")
         # message = finish.return_values['output']
         # resp = ChatResponse(sender="agent", message=message, type="finish")
         # await self.websocket.send_json(resp.dict())
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/callback_handler_tool.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from typing import Any, Dict, Union, List
 
 from arbol import aprint
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.schema import AgentFinish, AgentAction, LLMResult
 
 from napari_chatgpt.chat_server.chat_response import ChatResponse
-from napari_chatgpt.utils.tests.run_async import run_async
+from napari_chatgpt.utils.async_utils.run_async import run_async
 
 
 class ToolCallbackHandler(BaseCallbackHandler):
     """Callback handler for tool responses."""
 
-    def __init__(self, websocket):
+    def __init__(self, websocket, verbose: bool = False):
         self.websocket = websocket
+        self.verbose = verbose
+        self.last_internal_tool_response = None
 
     async def on_llm_start(
             self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> Any:
         """Run when LLM starts running."""
         pass
 
@@ -35,62 +37,74 @@
         pass
 
     def on_chain_start(
             self, serialized: Dict[str, Any], inputs: Dict[str, Any],
             **kwargs: Any
     ) -> Any:
         """Run when chain starts running."""
-        aprint(
-            f"TOOL on_chain_start: serialized={serialized},  inputs={inputs}")
+        if self.verbose:
+            aprint(
+                f"TOOL on_chain_start: serialized={serialized},  inputs={inputs}")
 
     def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
         """Run when chain ends running."""
-        message = outputs['text']
-        aprint(f"TOOL on_chain_end: {message}")
-        resp = ChatResponse(sender="agent", message=message, type="tool_result")
+        self.last_internal_tool_response = outputs['text']
+        if self.verbose:
+            aprint(f"TOOL on_chain_end: {self.last_internal_tool_response}")
+        resp = ChatResponse(sender="agent",
+                            message=self.last_internal_tool_response,
+                            type="tool_result")
         run_async(self.websocket.send_json, resp.dict())
 
     def on_chain_error(
             self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when chain errors."""
-        aprint(f"TOOL on_chain_error: {error}")
+        if self.verbose:
+            aprint(f"TOOL on_chain_error: {error}")
 
     def on_tool_start(
             self, serialized: Dict[str, Any], input_str: str, **kwargs: Any
     ) -> Any:
         """Run when tool starts running."""
-        aprint(
-            f"TOOL on_tool_start: serialized={serialized}, input_str={input_str}")
+        if self.verbose:
+            aprint(
+                f"TOOL on_tool_start: serialized={serialized}, input_str={input_str}")
+
+        self.last_internal_tool_response = None
+
         # tool = camel_case_to_lower_case(serialized['name'])
         # message = f"The {tool} received this request: '{input_str}'"
         # resp = ChatResponse(sender="agent", message=message, type="tool_start")
         # asyncio.run(self.websocket.send_json(resp.dict()))
 
     def on_tool_end(self, output: str, **kwargs: Any) -> Any:
         """Run when tool ends running."""
-        aprint(f"TOOL on_tool_end: {output}")
+        if self.verbose:
+            aprint(f"TOOL on_tool_end: {output}")
         if 'Exception' in output or 'Failure' in output:
             resp = ChatResponse(sender="agent", message=output, type="error")
             run_async(self.websocket.send_json, resp.dict())
 
     def on_tool_error(
             self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when tool errors."""
-        aprint(f"TOOL on_tool_error: {error}")
+        if self.verbose:
+            aprint(f"TOOL on_tool_error: {error}")
         error_type = type(error).__name__
         error_message = ', '.join(error.args)
         message = f"Failed because:\n'{error_message}'\nException: '{error_type}'\n"
         resp = ChatResponse(sender="agent", message=message, type="error")
         run_async(self.websocket.send_json, resp.dict())
 
     def on_text(self, text: str, **kwargs: Any) -> Any:
         """Run on arbitrary text."""
-        aprint(f"TOOL on_text: {text}")
+        if self.verbose:
+            aprint(f"TOOL on_text: {text}")
 
     def on_agent_action(self, action: AgentAction, **kwargs: Any) -> Any:
         """Run on agent action."""
         pass
 
     async def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
         """Run on agent end."""
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/chat.js` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/chat.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,56 @@
+//import {markedHighlight} from "marked-highlight";
+
+marked.use(markedHighlight({
+    langPrefix: 'language-',
+    highlight(code, lang) {
+
+        var highlighter = new Sunlight.Highlighter();
+
+        //first argument is the text to highlight, second is the language id
+        var context = highlighter.highlight(code, lang);
+        var nodes = context.getNodes(); //array of DOM nodes
+
+        //the following will convert it to an HTML string
+        var dummyElement = document.createElement("div");
+        for (var i = 0; i < nodes.length; i++) {
+            dummyElement.appendChild(nodes[i]);
+        }
+
+        var rawHtml = dummyElement.innerHTML + '<br>';
+
+        console.log(rawHtml)
+
+        return rawHtml
+    }
+}));
+
+//marked.use(markedHighlight({
+//  langPrefix: 'hljs language-',
+//  highlight(code, lang) {
+//    const language = hljs.getLanguage(lang) ? lang : 'plaintext';
+//    return hljs.highlight(code, { language }).value;
+//  }
+//}));
+
 function escapeHTML(unsafeText) {
     let div = document.createElement('div');
     div.innerText = unsafeText;
     return div.innerHTML;
 }
 
+function parse_markdown(str) {
+    // Parse Markdown to HTML:
+    str = marked.parse(str);
+
+    // Make sure that ordered lists show up as ordered with numbers:
+    str = str.replace("<ol>", '<ol class="list-decimal">');
+    return str;
+}
+
 // Endpoint for websocket:
 var endpoint = "ws://localhost:9000/chat";
 var ws = new WebSocket(endpoint);
 
 // Default subtitle:
 default_subtitle = " Ask a question, ask for a widget, ask to process images, or control the napari viewer ! ";
 
@@ -28,29 +71,29 @@
 
     // Message received from agent:
     if (data.sender === "agent") {
         // start message:
         if (data.type === "start") {
             // Set subtitle:
             var header = document.getElementById('header');
-            header.innerHTML = "Thinking...";
+            header.innerHTML = "Thinking... please wait!";
 
         }
         // agent is typing:
         else if (data.type === "typing") {
             // Set subtitle:
             var header = document.getElementById('header');
             header.innerHTML = 'Typing...';
         }
         // action message:
         else if (data.type === "action") {
 
             // Set subtitle:
             var header = document.getElementById('header');
-            header.innerHTML = "Using a tool...";
+            header.innerHTML = "Using a tool... please wait!";
 
             // Create a new message entry:
             var div = document.createElement('div');
             div.className = 'server-message';
             var p = document.createElement('p');
 
             // Add this new message into message list:
@@ -75,25 +118,25 @@
             // Set background color:
             //p.parentElement.className = 'server-message';
 
             // markdown:
             message = data.message
 
             // Parse markdown and render as HTML:
-            p.innerHTML += marked.parse(data.message)
+            p.innerHTML += parse_markdown(data.message)
 
         }
         // action message:
         else if (data.type === "tool_result") {
 
             // Current (last) message:
             var p = messages.lastChild.lastChild;
 
             // Parse markdown and render as HTML:
-            p.innerHTML += "<br>" + marked.parse(data.message);
+            p.innerHTML += "<br>" + parse_markdown(data.message);
         }
         // end message, this is sent once the agent has a final response:
         else if (data.type === "final") {
             // Create a new message entry:
             var div = document.createElement('div');
             div.className = 'server-message';
             var p = document.createElement('p');
@@ -105,15 +148,15 @@
             // Current (last) message:
             var p = messages.lastChild.lastChild;
 
             // Set background color:
             p.parentElement.className = 'server-message';
 
             // Parse markdown and render as HTML:
-            p.innerHTML = "<strong>" + "Omega: " + "</strong>" + marked.parse(data.message)
+            p.innerHTML = "<strong>" + "Omega: " + "</strong>" + parse_markdown(data.message)
 
             // Reset subtitle:
             var header = document.getElementById('header');
             header.innerHTML = default_subtitle;
 
             // Reset button text and state:
             var button = document.getElementById('send');
@@ -138,30 +181,30 @@
 
             // Add message to message list:
             div.appendChild(p);
             messages.appendChild(div);
 
             // Display error message:
             var p = messages.lastChild.lastChild;
-            p.innerHTML = "<strong>" + "Omega: " + "</strong>" + marked.parse(data.message)
+            p.innerHTML = "<strong>" + "Omega: " + "</strong>" + parse_markdown(data.message)
 
             // Set background color:
             p.parentElement.className = 'error-message';
         }
     }
     // Message received from user:
     else if (data.sender === "user") {
         // Create new message entry:
         var div = document.createElement('div');
         div.className = 'client-message';
         var p = document.createElement('p');
 
         // Set default (empty) message:
         p.innerHTML = "<strong>" + "You: " + "</strong>";
-        p.innerHTML += marked.parse(data.message);
+        p.innerHTML += parse_markdown(data.message);
 
         // Add message to message list:
         div.appendChild(p);
         messages.appendChild(div);
     }
     // Scroll to the bottom of the chat
     messages.scrollTop = messages.scrollHeight;
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/prism.css` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/prism.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/prism.js` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/prism.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/memory/memory.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/memory/memory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type
 
+from langchain.base_language import BaseLanguageModel
 from langchain.chains.llm import LLMChain
 from langchain.memory.chat_memory import BaseChatMemory
 from langchain.memory.prompt import SUMMARY_PROMPT
 from langchain.prompts.base import BasePromptTemplate
 from langchain.schema import (
-    BaseLanguageModel,
     BaseMessage,
     SystemMessage,
     get_buffer_string,
 )
 from pydantic import BaseModel, root_validator
 
 
@@ -35,35 +35,48 @@
             new_lines = new_lines[
                         :self.newlines_max_length - len(post_fix)] + post_fix
 
         chain = LLMChain(llm=self.llm, prompt=self.prompt)
         return chain.predict(summary=existing_summary, new_lines=new_lines)
 
 
-class OmegaConversationSummaryMemory(BaseChatMemory, SummarizerMixin):
-    """Conversation summarizer to memory."""
+class OmegaMemory(BaseChatMemory, SummarizerMixin):
+    """Buffer with summarizer for storing conversation memory."""
 
-    buffer: str = ""
-    memory_key: str = "history"  #: :meta private:
+    max_token_limit: int = 2000
+    moving_summary_buffer: str = ""
+    memory_key: str = "history"
+
+    @property
+    def buffer(self) -> List[BaseMessage]:
+        return self.chat_memory.messages
 
     @property
     def memory_variables(self) -> List[str]:
         """Will always return list of memory variables.
 
         :meta private:
         """
         return [self.memory_key]
 
     def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """Return history buffer."""
+        buffer = self.buffer
+        if self.moving_summary_buffer != "":
+            first_messages: List[BaseMessage] = [
+                self.summary_message_cls(content=self.moving_summary_buffer)
+            ]
+            buffer = first_messages + buffer
         if self.return_messages:
-            buffer: Any = [self.summary_message_cls(content=self.buffer)]
+            final_buffer: Any = buffer
         else:
-            buffer = self.buffer
-        return {self.memory_key: buffer}
+            final_buffer = get_buffer_string(
+                buffer, human_prefix=self.human_prefix, ai_prefix=self.ai_prefix
+            )
+        return {self.memory_key: final_buffer}
 
     @root_validator()
     def validate_prompt_input_variables(cls, values: Dict) -> Dict:
         """Validate that prompt input variables are consistent."""
         prompt_variables = values["prompt"].input_variables
         expected_keys = {"summary", "new_lines"}
         if expected_keys != set(prompt_variables):
@@ -73,15 +86,27 @@
             )
         return values
 
     def save_context(self, inputs: Dict[str, Any],
                      outputs: Dict[str, str]) -> None:
         """Save context from this conversation to buffer."""
         super().save_context(inputs, outputs)
-        self.buffer = self.predict_new_summary(
-            self.chat_memory.messages[-2:], self.buffer
-        )
+        self.prune()
+
+    def prune(self) -> None:
+        """Prune buffer if it exceeds max token limit"""
+        buffer = self.chat_memory.messages
+        curr_buffer_length = self.llm.get_num_tokens_from_messages(buffer)
+        if curr_buffer_length > self.max_token_limit:
+            pruned_memory = []
+            while curr_buffer_length > self.max_token_limit:
+                pruned_memory.append(buffer.pop(0))
+                curr_buffer_length = self.llm.get_num_tokens_from_messages(
+                    buffer)
+            self.moving_summary_buffer = self.predict_new_summary(
+                pruned_memory, self.moving_summary_buffer
+            )
 
     def clear(self) -> None:
         """Clear memory contents."""
         super().clear()
-        self.buffer = ""
+        self.moving_summary_buffer = ""
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/napari_bridge.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/napari_bridge.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 import napari
 import napari.viewer
 from arbol import aprint, asection
 from napari import Viewer
 from napari.qt.threading import thread_worker
 
-from napari_chatgpt.utils.exception_guard import ExceptionGuard
+from napari_chatgpt.omega.tools.special.exception_catcher_tool import \
+    enqueue_exception
+from napari_chatgpt.utils.python.exception_guard import ExceptionGuard
 
 
 class NapariBridge():
 
     def __init__(self, viewer: Viewer):
         self.viewer = viewer
 
@@ -23,18 +25,19 @@
             with asection(f"qt_code_executor received delegated function."):
                 with ExceptionGuard() as guard:
                     aprint("Executing now!")
                     result = fun(viewer)
                     aprint(result)
                     self.from_napari_queue.put(result)
 
-                if guard.exception_type:
+                if guard.exception:
                     aprint(
-                        f"Error while executing on napari's QT thread:\n{guard.error_string}")
-                    self.from_napari_queue.put(guard.error_string)
+                        f"Exception while executing on napari's QT thread:\n{guard.exception_description}")
+                    self.from_napari_queue.put(guard)
+                    enqueue_exception(guard.exception_value)
 
         @thread_worker(connect={'yielded': qt_code_executor})
         def omega_napari_worker(to_napari_queue: Queue,
                                 from_napari_queue: Queue):
             while True:
                 code = to_napari_queue.get()
                 if code is None:
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,82 @@
 import re
 import traceback
-from typing import Union
+from typing import Union, List
 
 from langchain.agents import AgentOutputParser
 from langchain.schema import AgentAction, AgentFinish
 
 from napari_chatgpt.omega.omega_agent.prompts import \
     OMEGA_FORMAT_INSTRUCTIONS
 
 
 class OmegaAgentOutputParser(AgentOutputParser):
+
+    tool_names: List[str]
+
     def get_format_instructions(self) -> str:
         return OMEGA_FORMAT_INSTRUCTIONS
 
     def parse(self, text: str) -> Union[AgentAction, AgentFinish]:
 
         try:
+            # Clean up output:
             cleaned_output = text.strip()
 
-            # lines = cleaned_output.splitlines(keepends=True)
-            words = re.split(r'(\s+)', cleaned_output)
-
-            # Simple state machine to robustly parse output:
-            action = ''
-            input = ''
-            state = 'start'
-            for word in words:
-                normalised_line = word.strip().lower()
-                if 'action:' == normalised_line:
-                    state = 'action'
-                    continue
-                elif 'input:' == normalised_line:
-                    state = 'input'
-                    continue
-
-                if state == 'action':
-                    action += word
-                elif state == 'input':
-                    input += word
+            # Add FinalAnswer as a special tool/action:
+            tool_names = self.tool_names+['FinalAnswer']
 
-            action = action.strip()
-            input = input.strip()
+            # Parse:
+            result = parse_command(tool_names, cleaned_output)
 
-            if action.lower() == "finalanswer":
-                return AgentFinish({"output": input}, text)
+            if not result:
+                result = AgentFinish({"output": cleaned_output}, cleaned_output)
             else:
-                return AgentAction(action, input, text)
+                action_str, input_str = result
+
+                if action_str.lower() == "finalanswer":
+                    result = AgentFinish({"output": input_str}, cleaned_output)
+                else:
+                    result = AgentAction(action_str, input_str, cleaned_output)
+
+            return result
 
         except Exception as e:
             traceback.print_exc()
-            raise e
+            return AgentFinish({"output": cleaned_output}, cleaned_output)
+
+
+def parse_command(tool_names: List[str], command_string: str):
+
+    # Convert to lower case for more robust substring finding:
+    command_string_lower_case = command_string.lower()
+
+    for tool_name in tool_names:
+        tool_name_sc = tool_name.lower()+':'
+        if tool_name_sc in command_string_lower_case:
+
+            # action/tool name is:
+            action_str = tool_name
+
+            # Position:
+            index = command_string_lower_case.find(tool_name_sc)
+
+            # get the input:
+            input_str = command_string[index + len(tool_name_sc):]
+
+            # Cleanup:
+            action_str = action_str.strip()
+            input_str = input_str.strip()
+
+            return action_str, input_str
+
+    return None
+
+
+    # pattern = r'^([a-zA-Z]+):(.*)'
+    # match = re.match(pattern, command_string, re.DOTALL | re.MULTILINE)
+    # if match:
+    #     action_str = match.group(1).strip()
+    #     input_str = match.group(2).strip()
+    #     return action_str, input_str
+    # else:
+    #     return None
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/async_base_tool.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/async_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/demo/tools_demo.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/demo/tools_demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from langchain import OpenAI, WikipediaAPIWrapper
 from langchain.agents import initialize_agent
 from langchain.tools.wikipedia.tool import WikipediaQueryRun
 
-from napari_chatgpt.omega.tools.google_search_tool import GoogleSearchTool
+from napari_chatgpt.omega.tools.search.web_search_tool import WebSearchTool
 
 llm = OpenAI(temperature=0)
 
 # tools = [GoogleSearchTool()]
 # agent = initialize_agent(tools,
 #                          llm,
 #                          agent="zero-shot-react-description",
 #                          verbose=True)
 # result = agent.run("What is zebrahub? ")
 
 
 wiki = WikipediaQueryRun(api_wrapper=WikipediaAPIWrapper())
 
-tools = [wiki, GoogleSearchTool()]
+tools = [wiki, WebSearchTool()]
 agent = initialize_agent(tools,
                          llm,
                          agent="conversational-react-description",
                          verbose=True)
 result = agent.run("Who is Albert Einstein? ")
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/functions_info.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/functions_info_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 """A tool for running python code in a REPL."""
 import traceback
 
+from arbol import asection, aprint
+
 from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
-from napari_chatgpt.utils.inspection import extract_package_path, \
+from napari_chatgpt.utils.llm.summarizer import summarize
+from napari_chatgpt.utils.python.python_lang_utils import extract_package_path, \
     get_function_info
-from napari_chatgpt.utils.summarizer import summarize
 
 
 class PythonFunctionsInfoTool(AsyncBaseTool):
     """A tool for querying the signature and docstrings of python functions."""
 
     name = "PythonFunctionsInfoTool"
     description = (
-        "A tool for querying the signature and docstrings of python functions from their fully qualified name. "
+        "Use this tool for querying the signature and docstrings of python functions from their fully qualified name. "
         "For example, send: scipy.ndimage.convolve and this tool will returns the full signature of this function "
         "with all its parameters and if possible corresponding type hints. "
-        "You can use this tool to check the correct signature of functions before writting python code. "
+        "You can use this tool to check the correct signature of functions before writing python code. "
         "If you want the whole docstring to get a better understanding of the function, its parameters, "
         "and example usages, please prefix your request with the single star character '*'."
     )
 
     def _run(self, query: str) -> str:
         """Use the tool."""
 
-        add_docstrings = False
+        with asection(f"PythonFunctionsInfoTool: query= {query} "):
+
+            add_docstrings = False
+
+            if '*' in query:
+                query = query.replace('*', '')
+                add_docstrings = True
+                aprint('Agent asked for docstrings!')
+
+            try:
+                function_path_and_name = extract_package_path(query)
+                if function_path_and_name:
+                    function_info = get_function_info(function_path_and_name,
+                                                      add_docstrings=add_docstrings)
+
+                    if len(function_info) > 512:
+                        function_info = summarize(function_info)
 
-        if '*' in query:
-            query = query.replace('*', '')
-            add_docstrings = True
-
-        try:
-            function_path_and_name = extract_package_path(query)
-            if function_path_and_name:
-                function_info = get_function_info(function_path_and_name,
-                                                  add_docstrings=add_docstrings)
+                    result = f"Here is the information you requested about function {function_path_and_name}:\n{function_info}\n"
 
-                if len(function_info) > 512:
-                    function_info = summarize(function_info)
+                else:
+                    result = "Error: there is no qualified function name in the request!"
 
-                result = f"Here is the information you requested about function {function_path_and_name}:\n{function_info}\n"
+                aprint(result)
                 return result
-            else:
-                return "Error: there is no qualified function name in the request!"
 
-        except Exception as e:
-            error_info = f"Error: {type(e).__name__} occured while trying to get information about: '{function_path_and_name}'."
-            traceback.print_exc()
-            return error_info
+            except Exception as e:
+                error_info = f"Error: {type(e).__name__} with message: '{str(e)}' occured while trying to get information about: '{function_path_and_name}'."
+                traceback.print_exc()
+                return error_info
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/human_input_tool.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/human_input_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     print("\n")
     print(text)
 
 
 class HumanInputTool(AsyncBaseTool):
     """Tool that adds the capability to ask user for input."""
 
-    name = "Human"
+    name = "HumanInputTool"
     description = (
         "You can ask a human for guidance when you think you "
         "got stuck or you are not sure what to do next. "
         "The input should be a question for the human."
     )
     prompt_func: Callable[[str], None] = Field(
         default_factory=lambda: _print_func)
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_viewer_control.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,100 @@
 """A tool for controlling a napari instance."""
 from contextlib import redirect_stdout
 from io import StringIO
 
+from arbol import asection, aprint
 from napari import Viewer
 
 from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
 
 _napari_viewer_control_prompt = """
 "
-Task:
-Given a plain text request, you competently write python code to control an already instantiated napari viewer instance.
-The napari viewer instance is immediately available by using the variable: 'viewer'. 
-For example, you can directly write: viewer.add_image(np.zeros((10,10))) without preamble. 
-Therefore, DO NOT use 'napari.Viewer()' or 'with napari.gui_qt():' in your code. 
-DO NOT CREATE A NEW INSTANCE OF A NAPARI VIEWER, use the one provided in the variable: 'viewer'.
-Make sure the calls to the viewer are correct.
+**Task:**
 
-{generic_codegen_instructions}
+Your task is to write Python code to control an already instantiated napari viewer instance based on a plain text request. The viewer instance is accessible using the variable `viewer`, so you can directly use methods like `viewer.add_image(np.zeros((10,10)))` without any preamble.
+
+**Please note the following instructions for your code:**
+- Do not create a new instance of `napari.Viewer()`. Use the existing instance provided in the variable `viewer`.
+- Ensure that your calls to the viewer's methods are correct.
+
+**Please keep the following notes in mind:**
+- If you need to add images, labels, points, shapes, surfaces, tracks, vectors, or any other type of layer that is not stored as an array, you may need additional code to read files from disk or download from a URL.
+- Unless explicitly stated in the request, the result of operations on layers should be a new layer in napari and not modify the existing layers.
+- Convert arrays to the float type before processing. Intermediate or local arrays should be of type float. Constants like `np.full()`, `np.ones()`, `np.zeros()`, etc., should be floats (e.g., 1.0).
+- If the request mentions "this," "that," or "the image/layer," it most likely refers to the last added image/layer.
+- If you are unsure about the layer being referred to, assume it is the last layer of the type most appropriate for the request.
+- If the request mentions the 'selected image', it most likely refers to the active or selected image layer.
+- To get the selected layer use: viewer.layers.selection.active
+- Important: At the end of your code add a print statement that states clearly and concisely what has been, or not, achieved. 
 
-Only use existing methods of the napari viewer:
+{generic_codegen_instructions}
 
-viewer.add_layer(layer: Layer)
-viewer.add_image(data: ArrayLike, rgb:bool=None, colormap='gray', contrast_limits=None, gamma=1, interpolation2d='nearest', interpolation3d='linear', rendering='mip', iso_threshold=0.5, attenuation=0.05, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', visible=True, multiscale=None, cache=True, depiction='volume', plane=None, experimental_clipping_planes=None)
-viewer.add_labels(data: ArrayLike, num_colors:int=50, features=None, properties=None, color=None, seed=0.5, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', rendering='iso_categorical', depiction='volume', visible=True, multiscale=None, cache=True, plane=None, experimental_clipping_planes=None)
-viewer.add_points(data: ArrayLike=None, ndim:int=None, features=None, properties=None, text=None, symbol='o', size=10, edge_width=0.05, edge_width_is_relative=True, edge_color='dimgray', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, face_color='white', face_color_cycle=None, face_colormap='viridis', face_contrast_limits=None, out_of_slice_display=False, n_dimensional=None, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', visible=True, cache=True, property_choices=None, experimental_clipping_planes=None, shading='none', canvas_size_limits=(2, 10000), antialiasing=1, shown=True)
-viewer.add_shapes(data: ArrayLike=None, ndim:int=None, features=None, properties=None, property_choices=None, text=None, shape_type='rectangle', edge_width=1, edge_color='#777777', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, face_color='white', face_color_cycle=None, face_colormap='viridis', face_contrast_limits=None, z_index=0, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', visible=True, cache=True, experimental_clipping_planes=None)
-viewer.add_surface(data: ArrayLike, colormap='gray', contrast_limits=None, gamma=1, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', shading='flat', visible=True, cache=True, experimental_clipping_planes=None, wireframe=None, normals=None)
-viewer.add_tracks(data: ArrayLike, features=None, properties=None, graph=None, tail_width=2, tail_length=30, head_length=0, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='additive', visible=True, colormap='turbo', color_by='track_id', colormaps_dict=None, cache=True, experimental_clipping_planes=None)
-viewer.add_vectors(data: ArrayLike=None, ndim=None, features=None, properties=None, property_choices=None, edge_width=1, edge_color='red', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, out_of_slice_display=False, length=1, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', visible=True, cache=True, experimental_clipping_planes=None)
-
-Note 1: To add images, labels, points, shapes, surfaces, tracks, vectors or any other type of layer, that are not stored as an array, you might need to write additional code to read files from disk or download from url.
-Note 2: The result of operations on layers (for example applying a filter, etc.) should be a new layer in napari, unless the requests states explicitly that it be in-place.
-Note 3: Convert arrays  to float type before processing. Intermediate or local arrays should be of type float. Constants for: np.full(), np.ones(), np.zeros(), ... should be floats (for example 1.0).
-Note 4: If the request mentions 'this/that/the image/layer' then most likely it refers to the last added image/layer.
+{last_generated_code}
 
-Request: 
+**Request:**
 {input}
 
-Answer in markdown:
+**Answer in markdown:**
 """
 
+"""
+**Use the existing methods of the `napari` viewer, which are as follows:**
+- `viewer.add_layer(layer: Layer)`
+- `viewer.add_image(data: ArrayLike, rgb:bool=None, colormap='gray', contrast_limits=None, gamma=1, interpolation2d='nearest', interpolation3d='linear', rendering='mip', iso_threshold=0.5, attenuation=0.05, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', visible=True, multiscale=None, cache=True, depiction='volume', plane=None, experimental_clipping_planes=None)`
+- `viewer.add_labels(data: ArrayLike, num_colors:int=50, features=None, properties=None, color=None, seed=0.5, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', rendering='iso_categorical', depiction='volume', visible=True, multiscale=None, cache=True, plane=None, experimental_clipping_planes=None)`
+- `viewer.add_points(data: ArrayLike=None, ndim:int=None, features=None, properties=None, text=None, symbol='o', size=10, edge_width=0.05, edge_width_is_relative=True, edge_color='dimgray', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, face_color='white', face_color_cycle=None, face_colormap='viridis', face_contrast_limits=None, out_of_slice_display=False, n_dimensional=None, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', visible=True, cache=True, property_choices=None, experimental_clipping_planes=None, shading='none', canvas_size_limits=(2, 10000), antialiasing=1, shown=True)`
+- `viewer.add_shapes(data: ArrayLike=None, ndim:int=None, features=None, properties=None, property_choices=None, text=None, shape_type='rectangle', edge_width=1, edge_color='#777777', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, face_color='white', face_color_cycle=None, face_colormap='viridis', face_contrast_limits=None, z_index=0, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', visible=True, cache=True, experimental_clipping_planes=None)`
+- `viewer.add_surface(data: ArrayLike, colormap='gray', contrast_limits=None, gamma=1, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', shading='flat', visible=True, cache=True, experimental_clipping_planes=None, wireframe=None, normals=None)`
+- `viewer.add_tracks(data: ArrayLike, features=None, properties=None, graph=None, tail_width=2, tail_length=30, head_length=0, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='additive', visible=True, colormap='turbo', color_by='track_id', colormaps_dict=None, cache=True, experimental_clipping_planes=None)`
+- `viewer.add_vectors(data: ArrayLike=None, ndim=None, features=None, properties=None, property_choices=None, edge_width=1, edge_color='red', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, out_of_slice_display=False, length=1, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', visible=True, cache=True, experimental_clipping_planes=None)`
+
+"""
+
+_code_prefix = \
+"""
+import napari
+"""
 
 class NapariViewerControlTool(NapariBaseTool):
     """A tool for running python code in a REPL."""
 
     name = "NapariViewerControlTool"
     description = (
-        "Forward plain text requests to this tool when you need to control, operate, "
-        "act, or set parameters of a napari viewer instance. "
-        "Requests must be a plain text description (no code) of what must be done with "
-        "the viewer, its layers, or parameters."
+        "Use this tool when you want to control, operate, perform actions, "
+        "or adjust parameters of a napari viewer instance or its layers "
+        "(images, labels, points, tracks, shapes, and meshes). "
+        "Input must be a plain text description of what you want to do. "
+        "The input must not assume knowledge of our conversation and must be explicit about what is asked."
+        "For instance, you can request to 'apply a Gaussian filter to the selected image'. "
+        "Do NOT include code in your input."
     )
     prompt = _napari_viewer_control_prompt
+    code_prefix = _code_prefix
+    save_last_generated_code = False
 
     def _run_code(self, request: str, code: str, viewer: Viewer) -> str:
-        code = super()._prepare_code(code)
 
-        # Redirect output:
-        f = StringIO()
-        with redirect_stdout(f):
-            # Running code:
-            exec(code, globals(), {**locals(), 'viewer': viewer})
+        with asection(f"NapariViewerControlTool: request= {request} "):
+
+            # Prepare code:
+            code = super()._prepare_code(code, do_fix_bad_calls=True)
+
+            # Redirect output:
+            f = StringIO()
+            with redirect_stdout(f):
+                # Running code:
+                exec(code, globals(), {**locals(), 'viewer': viewer})
+
+            # Get captured stdout:
+            captured_output = f.getvalue().strip()
+
+            # Message:
+            if len(captured_output) > 0:
+                message = f"Tool completed task successfully: {captured_output}"
+            else:
+                message = f"Tool completed task successfully"
 
-        captured_output = f.getvalue()
+            with asection(f"Message:"):
+                aprint(message)
 
-        return f"Success: request '{request}' satisfied:\n{captured_output}"
+            return message
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_widget_maker.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 """A tool for making a napari widget."""
+import traceback
 
+from arbol import asection, aprint
 from napari import Viewer
 
 from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
-from napari_chatgpt.utils.dynamic_import import dynamic_import
-from napari_chatgpt.utils.filter_lines import filter_lines
-from napari_chatgpt.utils.find_function_name import find_function_name
+from napari_chatgpt.utils.python.dynamic_import import dynamic_import
+from napari_chatgpt.utils.strings.filter_lines import filter_lines
+from napari_chatgpt.utils.strings.find_function_name import find_function_name
 
 _napari_widget_maker_prompt = """
-Task:
-You competently write image processing and image analysis functions in python given a plain text request. 
-The function should be pure, self-contained, effective, well-written, syntactically correct.
-The function should work on 2D and 3D images, and images of any number of dimensions (nD), 
-unless the request is explicit about the number of dimensions. 
-The widget should do all and everything that is asked, but nothing else or superfluous.
+**Task:**
+Your task is to competently write image processing and image analysis functions in Python based on a plain text request. The functions should meet the following criteria:
+- The functions should be pure, self-contained, effective, well-written, and syntactically correct.
+- The functions should work on 2D and 3D images, and ideally on images of any number of dimensions (nD), unless the request explicitly specifies the number of dimensions.
+- The functions should perform all the required tasks precisely as requested, without adding any extra or unnecessary functionality.
 
-Instructions for manipulating arrays from Images layers:
-- Convert arrays to float type before processing.
+**Instructions for manipulating arrays from Image layers:**
+- Convert arrays to the float type before processing.
 - Any intermediate or locally created image array should also be of type float.
-- Images arrays created with: np.full(), np.ones(), np.zeros(), ... should use float parameters (for example 1.0).
-- DO NOT clip (np.clip) the resulting image.
+- When creating image arrays using functions like np.full(), np.ones(), np.zeros(), etc., use float parameters (e.g., 1.0).
+- Do NOT clip (np.clip) the resulting image unless explicitly instructed.
 
-Instructions for manipulating arrays from Labels layers:
-- DO NOT convert to float arrays originating from labels layers, instead cast to np.uint32.
+**Instructions for manipulating arrays from Label layers:**
+- Do NOT convert arrays originating from label layers to float. Instead, cast them to np.uint32.
 
-Instructions for Function Signature:
-- Integers, floats, boolean, or any other type accepted by the magicgui library.
-- Decorate the function with the magicgui decorator: '@magicgui(call_button='Run')' where <function_name> is the name of the function that you wrote.
-- DO NOT CREATE A NEW INSTANCE OF A NAPARI VIEWER, use the one provided in the variable: 'viewer'.
-- DO NOT write code to add the widget to the napari window by calling viewer.window.add_dock_widget().
-
-You have two mutually exclusive options for passing data:
-
-    (i) The first kind of function signature must be typed with any of the following type hints:
-    napari layer data types: ImageData, LabelsData, PointsData, ShapesData, 
-    SurfaceData, TracksData, VectorsData. These types must be imported with import 
-    statements such as: 'from napari.types import ImageData' 
-    
-    (ii) The second type of function signature must be typed with any of the following type hints:
-    napari layer types: Data, Labels, Points, Shapes, Surface, Tracks, Vectors. 
-    These types must be imported with import statements such as: 'from napari.layers import Image' 
-    
-The function code must be consistent: if you use layers then you access the data via: 'layer.data', otherwise you can directly operate on the arrays.
+**Instructions for function parameters and magicgui decorator:**
+- Accept integers, floats, booleans, or any other type that is compatible with the magicgui library.
+- Decorate the function with the magicgui decorator: '@magicgui(call_button='Run')'. 
+- Ideally, replace the call_button text 'Run' with a few short words that more explicit describe the action of the widget.
+- Set 'result_widget=True' in the decorator, if and only if, the widget function returns a string, or a single int, float, list or tuple.
+- Set 'result_widget=False' in the decorator, if the widget function returns an array or a napari layer.
+- To expose a float parameter as a slider, include <parameter_name>={{"widget_type": "FloatSlider", 'min':<min_value>, 'max': <max_value>}} in the decorator.
+- To expose a string parameter as dropdown choice, include <parameter_name>={{"choices": ['first', 'second', 'third']}}.
+- Do NOT create a new instance of a napari viewer. Use the one provided in the variable 'viewer'.
+- Do NOT manually add the widget to the napari window by calling viewer.window.add_dock_widget().
+- Do NOT add layers to the viewer within the function. Instead, use a return statement to return the result.
+- Do NOT use tuples for widget function parameters.
+- Do NOT expose *args and **kwargs as widget function parameters.
+- Pay attention to the data types required by the library functions you use, for example: convert a float to an int before passing to a function that requires an int.
+
+**There are two mutually exclusive options for passing data:**
+
+(i) The first kind of function signature should be typed with any of the following type hints:
+    - napari layer data types: ImageData, LabelsData, PointsData, ShapesData, SurfaceData, TracksData, VectorsData.
+    - Import these types using statements like: 'from napari.types import ImageData'
+
+(ii) The second kind of function signature should be typed with any of the following type hints:
+    - napari layer types: Data, Labels, Points, Shapes, Surface, Tracks, Vectors.
+    - Import these types using statements like: 'from napari.layers import Image'
+
+The function code must be consistent: if you use layers, access the data via 'layer.data'. Otherwise, you can directly operate on the arrays.
 Do not mix these two options for the function parameters.
-The function signature should have a type hint for the return, e.g.  -> ImageData or -> Image
+The function signature should include a type hint for the return value, such as '-> ImageData' or '-> Image'.
 
 {generic_codegen_instructions}
 
-Request:  
+{last_generated_code}
+
+**Request:**
 {input}
 
-Answer in markdown:
+**Answer in markdown:**
 """
 #
 # Important: all import statements must be inside of the function except for those needed for magicgui and for type hints.
 # All import statements required by function calls within the function must be within the function.
 
 
 _code_prefix = """
@@ -66,42 +77,67 @@
 
 
 class NapariWidgetMakerTool(NapariBaseTool):
     """A tool for making napari widgets"""
 
     name = "NapariWidgetMakerTool"
     description = (
-        "Forward plain text requests to this tool when you need to make napari function widgets from function descriptions. "
-        "Requests must be a plain text description (no code) of an image processing or analysis function. "
-        "For example, you can ask for 'a gaussian filter widget with sigma parameter'. "
-        "This tool does not process or analyse images, it makes widget that then do that. "
-        "ONLY use this tool when the word 'widget' is mentioned. "
+        "Use this tool to make a napari widget. " # from the plain text description of a function, ""or to modify a previously generated widget
+        "Input must be a plain text description of the requested function and its parameters. "
+        "The input must not assume knowledge of our conversation. "
+        "For instance, if the input is for a 'Gaussian filter with a sigma parameter', "
+        "this tool will make the corresponding widget. "
+        "Another example: if the input is to 'add a mean parameter to the Gaussian filter with a sigma parameter widget', "
+        "this tool will make a new version of the previosuly generated widget, but with mean parameter. "
+        "Another example: if the input is to 'remove the inexistent parameter num_cores from the Gaussian filter with a sigma parameter widget', "
+        "this tool will make a new version of the previosuly generated widget, but without the offending parameter. "
+        "Important: The input must fully describe the widget every time, and in addition describe the modifications or fixes. "
+        "This tool only makes widgets from function descriptions, "
+        "it does not directly process or analyse images or other napari layers. "
+        "Only use this tool when you need to make, modify, or fix a widget, not to answer questions! "
+        "Do NOT include code in the input."
     )
     code_prefix = _code_prefix
     prompt = _napari_widget_maker_prompt
+    save_last_generated_code = False
+    return_direct: bool = True
 
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
 
-        code = super()._prepare_code(code)
+        with asection(f"NapariWidgetMakerTool: query= {query} "):
+
+            # Prepare code:
+            code = super()._prepare_code(code)
+
+            # Extracts function name:
+            function_name = find_function_name(code)
+
+            # If the function exists:
+            if function_name:
+
+                # Remove any viewer add_dock_widget code:
+                code = filter_lines(code, ['viewer = napari.Viewer(', 'viewer.window.add_dock_widget(', 'napari.run(', 'viewer.add_image('])
+
+                try:
 
-        # Extracts function name:
-        function_name = find_function_name(code)
+                    # Load the code as module:
+                    loaded_module = dynamic_import(code)
 
-        # If the function exists:
-        if function_name:
+                    # get the function:
+                    function = getattr(loaded_module, function_name)
 
-            # Remove any viewer add_dock_widget code:
-            code = filter_lines(code, ['viewer.window.add_dock_widget('])
+                    # Load the widget in the viewer:
+                    viewer.window.add_dock_widget(function, name=function_name)
 
-            # Load the code as module:
-            loaded_module = dynamic_import(code)
+                    message = f"The requested widget has been successfully created and registered to the viewer."
 
-            # get the function:
-            function = getattr(loaded_module, function_name)
+                except Exception as e:
+                    traceback.print_exc()
+                    raise e
 
-            # Load the widget in the viewer:
-            viewer.window.add_dock_widget(function)
+            else:
+                message = f"Could not create or register the requested widget to the viewer."
 
-            return "Success: widget was created and registered to the viewer."
+            with asection(f"Message:"):
+                aprint(message)
 
-        else:
-            return "Failure: function could not be found in provided code."
+            return message
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/cell_nuclei_segmentation.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """A tool for controlling a napari instance."""
 from pathlib import Path
 
+from arbol import asection, aprint
 from napari import Viewer
 
 from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
-from napari_chatgpt.utils.dynamic_import import dynamic_import
+from napari_chatgpt.utils.python.dynamic_import import dynamic_import
 
 _cell_segmentation_prompt = """
 "
-Task:
+**Task:**
 Given a plain text request, you competently write a python function segment(viewer) that calls the cellpose_segmentation() function.
 Segmentation is performed on images present as layers of the instantiated napari viewer.
 The napari viewer instance is immediately available by using the variable: 'viewer'. 
 For example, you can directly write: viewer.add_image(np.zeros((10,10))) without preamble. 
 Therefore, DO NOT use 'napari.Viewer()' or 'with napari.gui_qt():' in your code. 
 DO NOT CREATE A NEW INSTANCE OF A NAPARI VIEWER, use the one provided in the variable: 'viewer'.
 Make sure the calls to the viewer are correct.
 
 {generic_codegen_instructions}
 
-Notes: 
+**Notes:** 
 - Convert arrays to float type before processing. Intermediate or local arrays should be of type float. Constants for: np.full(), np.ones(), np.zeros(), ... should be floats (for example 1.0).
 - If the request mentions 'this/that/the image/layer' then most likely it refers to the last added image/layer.
 - Convert the segmented image to np.uint32 before returning the segmentation.
 
-
-ONLY AVAILABLE SEGMENTATION FUNCTION(S):
+**ONLY AVAILABLE SEGMENTATION FUNCTION(S):**
 The only segmentation function that you can use is cellpose_segmentation():
 
 def cellpose_segmentation( image: ArrayLike,
                            model_type: str = 'cyto',
                            channel: Optional[Sequence[int]] = None,
                            diameter: Optional[float] = None) -> ArrayLike:
 
@@ -57,23 +57,25 @@
             diameter can be a list or a single number for all images
 
 This function returns the segmented image as a labels array.
 To use function cellpose_segmentation() simply import it:
 
 from napari_chatgpt.omega.tools.segmentation.cellpose import cellpose_segmentation
 
-IMPORTANT INSTRUCTIONS: 
+**IMPORTANT INSTRUCTIONS:**
 - DO NOT include code for the function 'cellpose_segmentation()' in your answer.
 - INSTEAD, DIRECTLY call the segmentation function 'cellpose_segmentation()' provided above after import.
 - Assume that the function 'cellpose_segmentation()' is available and within scope of your code.
 - DO NOT add the segmentation to the napari viewer.
 - DO NOT directly use the Cellpose API: models.cellpose(...
 - Response is only the python function: segment(viewer)->ArrayLike.
 - The image input array to cellpose_segmentation() must be a float, therefore convert to float if needed!
 
+{last_generated_code}
+
 Request: 
 {input}
 
 Answer in markdown with a single function segment(viewer)->ArrayLike that takes the viewer and returns the segmented image.
 """
 
 
@@ -98,37 +100,49 @@
 # _cell_segmentation_prompt = _cell_segmentation_prompt.replace('*cellpose*', _get_seg_code('cellpose', signature=True))
 
 class CellNucleiSegmentationTool(NapariBaseTool):
     """A tool for segmenting cells in images using different algorithms."""
 
     name = "CellAndNucleiSegmentationTool"
     description = (
-        "Forward plain text requests to this tool when you need to segment cells or segment nuclei in images (or layers). "
-        "This tool operates on image layers present in the already instantiated napari viewer."
-        "This tool has the highest priority when the request pertains to cell or nuclei segmentation."
+        "Use this tool when you need to segment cells or nuclei in images (or layers). "
+        "Input must be a plain text request that must mention 'cellpose'. "
+        "For example, you can ask: 'to segment nuclei in selected layer with cellpose'. "
+        "This tool operates on image layers present in the already instantiated napari viewer. "
     )
     prompt = _cell_segmentation_prompt
+    save_last_generated_code = False
 
     # generic_codegen_instructions: str = ''
 
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
-        # prepare code:
-        code = super()._prepare_code(code)
+        with asection(f"CellNucleiSegmentationTool: query= {query} "):
+            # prepare code:
+            code = super()._prepare_code(code)
+
+            cellpose_code = _get_seg_code('cellpose')
+
+            # combine generated code and functions:
+            code = cellpose_code + '\n\n' + code
+
+            with asection(f"Code:"):
+                aprint(code)
+
+            # Load the code as module:
+            loaded_module = dynamic_import(code)
 
-        # cellpose_code = _get_seg_code('cellpose')
-        #
-        # # combine generated code and functions:
-        # code = cellpose_code +'\n\n' + code
+            # get the function:
+            segment = getattr(loaded_module, 'segment')
 
-        # Load the code as module:
-        loaded_module = dynamic_import(code)
+            # Run segmentation:
+            with asection(f"Running segmentation..."):
+                segmented_image = segment(viewer)
 
-        # get the function:
-        segment = getattr(loaded_module, 'segment')
+            # Add to viewer:
+            viewer.add_labels(segmented_image, name='segmented')
 
-        # Run segmentation:
-        segmented_image = segment(viewer)
+            # Message:
+            message = f"Success: segmentation succeeded!"
 
-        # Add to viewer:
-        viewer.add_labels(segmented_image, name='segmented')
+            aprint(f"Message: {message}")
 
-        return f"Success: segmentation succeeded!"
+            return message
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/cellpose.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/segmentation/cellpose.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/wikipedia_query_tool.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,31 @@
+from arbol import asection, aprint
 from langchain import WikipediaAPIWrapper
 
 from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
 
 _api_wrapper = WikipediaAPIWrapper()
 
 
 class WikipediaQueryTool(AsyncBaseTool):
     """Tool that adds the capability to search using the Wikipedia API."""
 
-    name = "Wikipedia"
+    name = "WikipediaQueryTool"
     description = (
-        "A wrapper around Wikipedia. "
-        "Useful for when you need to answer general questions on topics covered by an encyclopedia. "
-        "Input should be a search query."
+        "Use this tool to answer general questions on topics covered by an encyclopedia "
+        "such as historical events, scientific concepts, geography... "
+        "for which you don't already have the answer. "
+        "Input must be a plain text wikipedia search query. "
+        "Do NOT use this tool if you already have the answer."
     )
 
     def _run(self, query: str) -> str:
         """Use the Wikipedia tool."""
-        return _api_wrapper.run(query)
+
+        with asection(f"WikipediaQueryTool: query= {query} "):
+            # Run wikipedia query:
+            result = _api_wrapper.run(query)
+
+            with asection(f"Result:"):
+                aprint(result)
+
+            return result
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/api_key_vault.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/api_key_vault_dialog.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from PyQt5.QtWidgets import QDialog, QLabel, QLineEdit, QPushButton
 from arbol import aprint
-from cryptography.fernet import InvalidToken
 
-from napari_chatgpt.utils.api_key_vault import KeyVault
+from napari_chatgpt.utils.api_keys.api_key_vault import KeyVault
 
 
 class APIKeyDialog(QDialog):
     def __init__(self, api_key_name: str, parent=None):
         super().__init__(parent)
 
         self.api_key = None
@@ -52,14 +51,15 @@
 
         # Connect the button to a slot
         self.button.clicked.connect(self.button_clicked)
 
     def button_clicked(self):
 
         if self.key_vault.is_key_present():
+            from cryptography.fernet import InvalidToken
             try:
                 password = self.password_textbox.text()
 
                 # Decrypt API key:
                 self.api_key = self.key_vault.read_api_key(password=password)
 
                 # Close the dialog box
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/camel_case_to_normal.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/camel_case_to_normal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/api_key_vault_dialog_demo.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from PyQt5.QtWidgets import QApplication, QMainWindow, QPushButton
 
-from napari_chatgpt.utils.api_key_vault_dialog import \
+from napari_chatgpt.utils.api_keys.api_key_vault_dialog import \
     request_if_needed_api_key_dialog
 
 
 class MainWindow(QMainWindow):
     def __init__(self):
         super().__init__()
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/download_files.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/download_files.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/duckduckgo.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/duckduckgo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 import traceback
 
 from duckduckgo_search import ddg, ddg_images
 
-from napari_chatgpt.utils.summarizer import summarize
-
+from napari_chatgpt.utils.llm.summarizer import summarize
+from napari_chatgpt.utils.python.missing_packages import \
+    pip_install_single_package
+
+# Make sure we have the latest version installed:
+try:
+    pip_install_single_package('duckduckgo_search', upgrade=True)
+except Exception as e:
+    traceback.print_exc()
 
 def summary_ddg(query: str,
                 num_results: int = 3,
-                lang: str = "us-en",
+                lang: str = "en",
                 do_summarize: bool = True,
                 ) -> str:
     try:
+
         results = search_ddg(query=query,
                              num_results=num_results,
                              lang=lang)
 
+        # Are there any results?
+        if len(results) == 0:
+            return "No results."
+
         text = f"The following results were found for the web search query: '{query}'"
 
         for result in results:
             text += f"Title: {result['title']}\n Description: {result['body']}\n URL: {result['href']}\n\n "
 
-        text += "How do the results inform the query ?"
-
         if do_summarize:
+            # summary prompt:
+            text += "Please summarise these results and list facts and information that help answer the query:"
             text = summarize(text)
 
         return text
 
     except Exception as e:
         traceback.format_exc()
         return f"Web search failed for: '{query}'"
 
 
 def search_ddg(query: str,
                num_results: int = 3,
-               lang: str = "us-en",
+               lang: str = "en",
                safesearch: str = 'moderate'
                ) -> str:
+    lang = 'en-us' if lang == 'en' else lang
+
     results = ddg(query,
                   region=lang,
                   time='h_',
                   safesearch=safesearch,
                   max_results=num_results)
 
     if results:
@@ -49,17 +63,19 @@
         results = []
 
     return results
 
 
 def search_images_ddg(query: str,
                       num_results: int = 3,
-                      lang: str = "us-en",
+                      lang: str = "en",
                       safesearch: str = 'moderate'
                       ) -> str:
+    lang = 'en-us' if lang == 'en' else lang
+
     results = ddg_images(query,
                          region=lang,
                          safesearch=safesearch,
                          size=None,
                          color=None,
                          type_image=None,
                          layout=None,
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/dynamic_import.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/extract_urls.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/extract_urls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/filter_lines.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/filter_lines.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/google.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Code vendored from: https://github.com/Nv7-GitHub/googlesearch/blob/master/googlesearch/__init__.py
 
 import random
 
-from napari_chatgpt.utils.headers import _scrapping_request_headers
-from napari_chatgpt.utils.scrapper import text_from_url
+from napari_chatgpt.utils.web.headers import _scrapping_request_headers
+from napari_chatgpt.utils.web.scrapper import text_from_url
 
 _useragent_list = [
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0) Gecko/20100101 Firefox/66.0',
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
     'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36',
     'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
@@ -55,15 +55,15 @@
         return f"SearchResult(url={self.url}, title={self.title}, description={self.description})"
 
 
 def search_overview(query: str,
                     num_results: int = 3,
                     lang: str = "en",
                     max_text_snippets: int = 5,
-                    max_query_freq_hz: float = 1.0) -> str:
+                    max_query_freq_hz: float = 0.5) -> str:
     url = f"https://www.google.com/search?q={query}&num={num_results}&hl={lang}"
     text = text_from_url(url,
                          max_text_snippets=max_text_snippets,
                          max_query_freq_hz=max_query_freq_hz)
     return text
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/headers.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/headers.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/installed_packages.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/installed_packages.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,7 +65,13 @@
                             not line.startswith('#')]
 
         return package_list
 
     except Exception as e:
         print(traceback.format_exc())
         return []
+
+
+def is_package_installed(package_name: str):
+    from pkgutil import find_loader
+    loader = find_loader(package_name)
+    return loader is not None
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/open_in_napari.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/open_in_napari.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 'mov') or url.endswith('avi') or url.endswith('m4v')):
             return False
 
         # temp folder:
         temp_folder = tempfile.gettempdir()
 
         # Download video file:
-        from napari_chatgpt.utils.download_files import download_files
+        from napari_chatgpt.utils.download.download_files import download_files
         files = download_files(urls=[url], path=temp_folder)
         file = files[0]
 
         # make full path:
         file_path = os.path.join(temp_folder, file)
 
         # open video:
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/scrapper.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/scrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from typing import Optional
 
 from bs4 import BeautifulSoup
 from bs4.element import Comment
 from requests import Session
 
-from napari_chatgpt.utils.headers import _scrapping_request_headers
+from napari_chatgpt.utils.web.headers import _scrapping_request_headers
 
 
 def _tag_visible(element):
     if element.parent.name in ['style', 'script', 'head', 'title', 'meta',
                                '[document]']:
         return False
     if isinstance(element, Comment):
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/summarizer.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/summarizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from langchain.chains.summarize import load_summarize_chain
 from langchain.chat_models import ChatOpenAI
 from langchain.docstore.document import Document
 from langchain.llms import BaseLLM
 from langchain.text_splitter import CharacterTextSplitter
 
-from napari_chatgpt.utils.openai_key import set_openai_key
-
 
 def summarize(text: str, llm: BaseLLM = None):
-    # Ensure that OpenAI key is set:
-    set_openai_key()
+    # Clean up text:
+    text = text.strip()
+
+    # Is there anything to summarise?
+    if len(text) == 0:
+        return text
 
     # Instantiates LLM if needed:
     llm = llm or ChatOpenAI(model_name='gpt-3.5-turbo', temperature=0)
 
     # Splits the text:
     text_splitter = CharacterTextSplitter()
     texts = text_splitter.split_text(text)
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/api_key_vault_tests.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from napari_chatgpt.utils.api_key_vault import KeyVault, _encode64, _decode64
+from napari_chatgpt.utils.api_keys.api_key_vault import KeyVault, _encode64, \
+    _decode64
 
 
 def test_b64_encode_decode():
     plain = '1234'
     encoded = _encode64(plain)
     decoded = _decode64(encoded)
     assert plain == decoded
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/download_files_tests.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/test/download_files_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tempfile
 
 from arbol import aprint
 
-from src.napari_chatgpt.utils.download_files import download_files
-from src.napari_chatgpt.utils.extract_urls import extract_urls
+from napari_chatgpt.utils.download.download_files import download_files
+from napari_chatgpt.utils.strings.extract_urls import extract_urls
 
 
 def test_download_files():
     # Example string with urls:
     text = "Check out my website at https://www.example.com! " \
            "For more information, visit http://en.wikipedia.org/wiki/URL."
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/extract_code_tests.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/extract_code_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from napari_chatgpt.utils.extract_code import extract_code_from_markdown
+from napari_chatgpt.utils.strings.extract_code import extract_code_from_markdown
 
 markdown = """
 ```python
 # some python code
 from napari_chatgpt.utils.extract_code import extract_code_from_markdown
 
 def filter_lines(text:str, filter_out: List[str]=None) -> str:
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/filter_lines_tests.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/filter_lines_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from napari_chatgpt.utils.filter_lines import filter_lines
+from napari_chatgpt.utils.strings.filter_lines import filter_lines
 
 ___text = """
 from magicgui import magicgui
 from typing import Union
 from napari.types import ImageData
 from magicgui import magicgui
 import numpy as np
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/wikipedia.py` & `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/wikipedia.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Code vendored from: https://github.com/Nv7-GitHub/googlesearch/blob/master/googlesearch/__init__.py
 from langchain.llms import BaseLLM
 
-from napari_chatgpt.utils.duckduckgo import search_ddg
-from napari_chatgpt.utils.summarizer import summarize
+from napari_chatgpt.utils.llm.summarizer import summarize
+from napari_chatgpt.utils.web.duckduckgo import search_ddg
 
 
 def search_wikipedia(query: str,
                      num_results: int = 3,
                      max_text_length: int = 4000,
                      do_summarize: bool = False,
                      llm: BaseLLM = None) -> str:
```

### Comparing `napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/PKG-INFO` & `napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.5.2
+Version: 2023.6.2
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
@@ -23,98 +23,138 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# napari-chatgpt, home of _Omega_, a napari-aware autonomous LLM-based agent.
+# napari-chatgpt
+
+## Home of
+_Omega_, a napari-aware autonomous LLM-based agent specialised in image processing and analysis.
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
 
-A [napari](napari.org) plugin that levegares OpenAI's Large Language Model ChatGPT to implement _Omega_ 
-a napari-aware agent capable of performing image processing and analysis tasks in a conversational manner.
-
-This repository was created as a 'week-end project' by [Loic A. Royer](https://twitter.com/loicaroyer) 
-who leads a [research group](https://royerlab.org) at the [Chan Zuckerberg Biohub](https://czbiohub.org/sf/). It levegages [OpenAI](https://openai.com)'s ChatGPT API via the [LangChain](https://python.langchain.com/en/latest/index.html) Python library, as well as [napari](https://napari.org), a fast, interactive, multi-dimensional 
-image viewer for Python, [another](https://ilovesymposia.com/2019/10/24/introducing-napari-a-fast-n-dimensional-image-viewer-in-python/) 
+A [napari](napari.org) plugin that levegares OpenAI's Large Language Model
+ChatGPT to implement _Omega_
+a napari-aware agent capable of performing image processing and analysis tasks
+in a conversational manner.
+
+This repository was created as a 'week-end project'
+by [Loic A. Royer](https://twitter.com/loicaroyer)
+who leads a [research group](https://royerlab.org) at
+the [Chan Zuckerberg Biohub](https://czbiohub.org/sf/). It
+levegages [OpenAI](https://openai.com)'s ChatGPT API via
+the [LangChain](https://python.langchain.com/en/latest/index.html) Python
+library, as well as [napari](https://napari.org), a fast, interactive,
+multi-dimensional
+image viewer for
+Python, [another](https://ilovesymposia.com/2019/10/24/introducing-napari-a-fast-n-dimensional-image-viewer-in-python/)
 of Loic's week-end projects.
 
 # What is Omega?
 
-Omega is a LLM-based and tool-armed autonomous agent that demonstrates the potential for Large Language Models (LLMs) to be applied to image processing, analysis and visualisation. 
-Can LLM-based agents write image processing code and napari widgets, correct its coding mistakes, perform 
+Omega is a LLM-based and tool-armed autonomous agent that demonstrates the
+potential for Large Language Models (LLMs) to be applied to image processing,
+analysis and visualisation.
+Can LLM-based agents write image processing code and napari widgets, correct its
+coding mistakes, perform
 follow-up analysis, and control the napari viewer? The answer appears to be yes.
 
 #### In this video I ask Omega to segment an image using the [SLIC](https://www.iro.umontreal.ca/~mignotte/IFT6150/Articles/SLIC_Superpixels.pdf) algorithm. It makes a first attempt using the implementation in scikit-image, but fails because of an inexistant 'multichannel' parameter. Realising that, Omega tries again, and this time, succeeds:
+
 https://user-images.githubusercontent.com/1870994/235768559-ca8bfa84-21f5-47b6-b2bd-7fcc07cedd92.mp4
 
-#### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:   
-https://user-images.githubusercontent.com/1870994/235769990-a281a118-1369-47aa-834a-b491f706bd48.mp4
+#### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:
 
+https://user-images.githubusercontent.com/1870994/235769990-a281a118-1369-47aa-834a-b491f706bd48.mp4
 
-As LLMs continue to improve, Omega will become even more adept at handling complex 
-image processing and analysis tasks. The current version of ChatGPT, 3.5, 
-has a cutoff date of 2021, which means that it lacks nearly two years of knowledge 
-on the napari API and usage, as well as the latest versions of popular libraries 
-like scikit-image, OpenCV, numpy, scipy, etc... Despite this, you can see in the videos below 
-that it is quite capable. While ChatGPT 4.0 is a significant upgrade, it is not yet widely 
+As LLMs continue to improve, Omega will become even more adept at handling
+complex
+image processing and analysis tasks. The current version of ChatGPT, 3.5,
+has a cutoff date of 2021, which means that it lacks nearly two years of
+knowledge
+on the napari API and usage, as well as the latest versions of popular libraries
+like scikit-image, OpenCV, numpy, scipy, etc... Despite this, you can see in the
+videos below
+that it is quite capable. While ChatGPT 4.0 is a significant upgrade, it is not
+yet widely
 available.
 
-Omega could eventually help non-experts process and analyse images, especially in the bioimage domain. 
-It is also potentially valuable for educative purposes as it could 
-assist in teaching image processing and analysis, making it more accessible. 
-Although ChatGPT, which powers Omega, may not be yet on par with an expert image analyst or computer vision 
+Omega could eventually help non-experts process and analyse images, especially
+in the bioimage domain.
+It is also potentially valuable for educative purposes as it could
+assist in teaching image processing and analysis, making it more accessible.
+Although ChatGPT, which powers Omega, may not be yet on par with an expert image
+analyst or computer vision
 expert, it is just a matter of time...
 
-Omega holds a conversation with the user and uses the following tools to acheive answer questions, 
+Omega holds a conversation with the user and uses the following tools to acheive
+answer questions,
 download and operate on images, write widgets for napari, and more:
 
 ### napari related tools:
-- napari viewer control: 
-    Gives Omega the ability to control all aspects of the napari viewer.
-  
+
+- napari viewer control:
+  Gives Omega the ability to control all aspects of the napari viewer.
+
 - napari query:
-    Gives Omega the ability to query information about the state of the viewer, of its layers, and their contents.
+  Gives Omega the ability to query information about the state of the viewer, of
+  its layers, and their contents.
 
 - napari widget maker:
-    Gives Omega the ability to make napari functional widgets that take layers as input and return a new layer.
+  Gives Omega the ability to make napari functional widgets that take layers as
+  input and return a new layer.
+
+### cell segmentation tools:
 
-### cell segmentation tools: 
 - cell and nuclei segmentation:
-    This tool specialises in segmenting cells and nuclei in images using some predefined segmentation algorithms. Right now only cellpose is implemented. 
+  This tool specialises in segmenting cells and nuclei in images using some
+  predefined segmentation algorithms. Right now only cellpose is implemented.
 
 ### Generic python installation queries:
+
 - python function signature query:
-    Lets Omega query the signature of function when it is unsure how to call a function and what the names and type of the parameters are.
+  Lets Omega query the signature of function when it is unsure how to call a
+  function and what the names and type of the parameters are.
 
 ### web search related tools:
+
 - web search:
-    Usefull to give Omega access to the knowledge accessible through the web
+  Usefull to give Omega access to the knowledge accessible through the web
 
 - web image serach:
-    Streamlined path to search the web for images and open them in napari  
+  Streamlined path to search the web for images and open them in napari
 
 - wikipedia search:
-    Gives Omega access to the whole wikipedia
-
+  Gives Omega access to the whole wikipedia
 
 ----------------------------------
 
-## Installation:
+## Installation from within napari:
+
+You can install `napari-chatgpt` directly from within napari in the Plugins>
+Install/Uninstall Plugins menu.
+(Please note that the Omega agent will hapilly install packages in the
+corresponding environment).
+
+IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the
+latest one!
 
-You can also install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
-(Please note that the Omega agent will hapilly install packages in the corresponding environment)
+## Installation in an new conda environment (RECOMMENDED):
 
-Create environment: 
+Make sure you have an anaocnda/miniconda installation on your system.
+Ask ChatGPT what is that all about if you are unsure ;-)
+
+Create environment:
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
     conda activate napari-chatgpt 
 
@@ -122,238 +162,328 @@
 
     conda install -c conda-forge napari     
 
 Install the repo in enbvironment:
 
     pip install napari-chatgpt
 
-
 ## Installation variations:
 
 To install latest development version :
 
     git clone https://github.com/royerlab/napari-chatgpt.git
     cd napari-chatgpt
     pip install -e .
 
 or:
 
     pip install git+https://github.com/royerlab/napari-chatgpt.git
 
-
 ## Requirements:
 
 You need an OpenAI key, there is no way around this, unless we add some other,
-potentially local LLMs compatible to LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar models come to mind). However, this will likely be at the cost of cognitive performance,
+potentially local LLMs compatible to
+LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar
+models come to mind). However, this will likely be at the cost of cognitive
+performance,
 which I am not sure is worth it at this point. Please prove me wrong.
-You can get your OpenAI key by signing up [here](https://openai.com/blog/openai-api).
-Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5 is very
-reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A bargain.
-Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop, hopefully.
-
-Note: you can limit the burn-rate to a certain amount of dollars per month, just in case you let
-Omega thinking over the week end and forget to stop it (don't worry, this is actually not possible). 
-
+You can get your OpenAI key by signing
+up [here](https://openai.com/blog/openai-api).
+Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5
+is very
+reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
+bargain.
+Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
+hopefully.
+
+Note: you can limit the burn-rate to a certain amount of dollars per month, just
+in case you let
+Omega thinking over the week end and forget to stop it (don't worry, this is
+actually not possible).
 
 ## Usage:
 
 Once all is installed, and if it is not already running, start napari:
 
     napari
-    
+
 You can then the Omega napari plugin via the plugins menu:
 
 <img width="498" alt="image" src="https://user-images.githubusercontent.com/1870994/235790134-1d87fd50-583f-4fd9-ade2-c64497b91331.png">
 
 
 You just opened the plugin as a widget, you now need to actually start Omega:
 
 <img width="104" alt="image" src="https://user-images.githubusercontent.com/1870994/235811111-9e468785-9562-410a-8e9a-c63cb03fb765.png">
 
 
-If you have not set the 'OPENAI_API_KEY' environment variable as is typicall done,
-Omega will ask you for your OpenAI API key, and will store it _safely_ in an _encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
+If you have not set the 'OPENAI_API_KEY' environment variable as is typicall
+done,
+Omega will ask you for your OpenAI API key, and will store it _safely_ in an
+_encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
 
 <img width="293" alt="image" src="https://user-images.githubusercontent.com/1870994/235793528-9e892c5e-d8ca-43e1-9020-f2dfab45b32d.png">
 
 
 Just enter an encryption/decription key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
-(The idea is that you might not be able to remember your openAI key by heart, but you might be able to do so with your own password or passphrase)
+(The idea is that you might not be able to remember your openAI key by heart,
+but you might be able to do so with your own password or passphrase)
 
-You can then direct your browser to: [http://0.0.0.0:9000/](http://0.0.0.0:9000/)
+You can then direct your browser
+to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
 and start having an hopefully nice chat with Omega.
 
-
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
 - What is your name?
 - What tools do you have available?
 - Make me a Gaussian blur widget with sigma parameter
-- Open this tiff file in napari: https://people.math.sc.edu/Burkardt/data/tif/at3_1m4_03.tif
-- Make a widget that applies the transformation: y = x^alpha + y^beta with alpha and beta two parameters.
+- Open this tiff file in
+  napari: https://people.math.sc.edu/Burkardt/data/tif/at3_1m4_03.tif
+- Make a widget that applies the transformation: y = x^alpha + y^beta with alpha
+  and beta two parameters.
 - Create a widget to multiply two images
 - Can you open in napari a photo of Albert Einstein?
 - Downscale by a factor 3x the image on layer named 'img'
 - Rename selected layer to 'downscaled_image'
-- Upscale image 'downscaled_image' by a factor 3 using some smart interpolation scheme of your choice (not nearest-neighboor)
+- Upscale image 'downscaled_image' by a factor 3 using some smart interpolation
+  scheme of your choice (not nearest-neighboor)
 - Caveat: makes a plugin instead of actually doing teh job
 - How many channels has the image on layer 0
 - Make a image sharpening filter widget, expose relevant parameters
-- Can you open this file in napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
-- Split the two channels of the first layer (first axis) into two separate layers
+- Can you open this file in
+  napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
+- Split the two channels of the first layer (first axis) into two separate
+  layers
 - Switch viewer to 3d
-- Create a napari widget for a function that takes two image layers and returns a 3D image stack of n images where each 2D image corresponds to a linear blending of the two layer images between 0 and 1.
-- [Loaded the ‘cell’ sample image] there is one cell in the image on the first layer, it is roughly circular and brighter than its surroundings, ca you write segmentation code that returns a labels layer for it?
+- Create a napari widget for a function that takes two image layers and returns
+  a 3D image stack of n images where each 2D image corresponds to a linear
+  blending of the two layer images between 0 and 1.
+- [Loaded the ‘cell’ sample image] there is one cell in the image on the first
+  layer, it is roughly circular and brighter than its surroundings, ca you write
+  segmentation code that returns a labels layer for it?
 - Can you create a widget to blend two images?
 - Can you tell me more about the 'guided Canny edge filter' ?
 - Write a configurable RGB to grayscale widget, ensure weights sum to 1
 
 ## Video Demos:
 
-Not everyone will want, or can, get an API key for the latest and best LLM models, 
-so here are videos showcasing what's possible. You will notice that Omega sometimes 
-fails on its first attempt, typically because of mistaken parameters for functions,
-or other syntax errors. But it also often recovers by having access to the error message,
-and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can do, imagine
+Not everyone will want, or can, get an API key for the latest and best LLM
+models,
+so here are videos showcasing what's possible. You will notice that Omega
+sometimes
+fails on its first attempt, typically because of mistaken parameters for
+functions,
+or other syntax errors. But it also often recovers by having access to the error
+message,
+and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can
+do, imagine
 what will be possible with 4.0 and future more capable models...
 
 ##
-In this first video, I ask Omega to make a napari widget to convert images from RGB to grayscale:
+
+In this first video, I ask Omega to make a napari widget to convert images from
+RGB to grayscale:
 
 https://user-images.githubusercontent.com/1870994/235769895-23cfc7ed-622a-47f9-95aa-4be77efc0f78.mp4
 
 ##
-Of course Omega is capable of holding a conversation, it sort of knows 'who it is', can search the web
-and wikipedia. Eventually I imagine it could leverage the ability to search for improving its responses,
+
+Of course Omega is capable of holding a conversation, it sort of knows 'who it
+is', can search the web
+and wikipedia. Eventually I imagine it could leverage the ability to search for
+improving its responses,
 and I have seen doing it a few times:
 
 https://user-images.githubusercontent.com/1870994/235769920-86b02d9d-1196-4339-a8d9-9a028bcd4607.mp4
 
 ##
-Following-up from the previous video, I ask Omega to create a new labels layer containing just the largest segment. The script that Omega writes as another rookie mistake: it confuses layers and images. The error message then confuses Omega into thinking that it got the name of the layer wrong, setting it off in a quest
-to find the name of the labels layer. It succeeds at writting code that searches for the labels layer, and uses that name to write a script that then does extracts te largest segment into its own layer. Not bad: 
+
+Following-up from the previous video, I ask Omega to create a new labels layer
+containing just the largest segment. The script that Omega writes as another
+rookie mistake: it confuses layers and images. The error message then confuses
+Omega into thinking that it got the name of the layer wrong, setting it off in a
+quest
+to find the name of the labels layer. It succeeds at writting code that searches
+for the labels layer, and uses that name to write a script that then does
+extracts te largest segment into its own layer. Not bad:
 
 https://user-images.githubusercontent.com/1870994/235770741-d8905afd-0a9b-4eb7-a075-481979ab7b01.mp4
 
 ##
-In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific. The answer is a vanilla yet effective widget that uses the Otsu approach to threshold the image and then finds the connected components.
-Note that when you ask Omega to make a widget, it won't know of any runtime issues with the code because
-it is not running the code itself, yet. It can tell if there is a syntax problem though... Nevertheless, the widget ends up working just fine:
+
+In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific.
+The answer is a vanilla yet effective widget that uses the Otsu approach to
+threshold the image and then finds the connected components.
+Note that when you ask Omega to make a widget, it won't know of any runtime
+issues with the code because
+it is not running the code itself, yet. It can tell if there is a syntax problem
+though... Nevertheless, the widget ends up working just fine:
 
 https://user-images.githubusercontent.com/1870994/235770794-90091bfe-b546-4dd0-bd9c-3895bfc33a1d.mp4
 
 ##
-Now it gets more interesting. Following up on the previous video, can we ask Omega to do some follow-
-up analysis on the segments themselves? I ask Omega to list the 10 largest segments and compute their 
-areas and centroids. No problem: 
+
+Now it gets more interesting. Following up on the previous video, can we ask
+Omega to do some follow-
+up analysis on the segments themselves? I ask Omega to list the 10 largest
+segments and compute their
+areas and centroids. No problem:
 
 https://user-images.githubusercontent.com/1870994/235770828-0f829f76-1f3d-44b8-b8e8-89fcbcde6e11.mp4
 
-Note: You could even ask for it in markdown format, which would look better (not shown here).
+Note: You could even ask for it in markdown format, which would look better (not
+shown here).
 
 ##
-Next I ask Omega to make a widget that lets me filter segments by area. And it works beautifully.
-Arguably it is not rocket science, but the thought-to-widget time ratio must be in the hundreds when comparing Omega to an average user trying to write their own widget:
+
+Next I ask Omega to make a widget that lets me filter segments by area. And it
+works beautifully.
+Arguably it is not rocket science, but the thought-to-widget time ratio must be
+in the hundreds when comparing Omega to an average user trying to write their
+own widget:
 
 https://user-images.githubusercontent.com/1870994/235770860-4287e6a3-dae3-4c6d-a588-dea2bb1f69b7.mp4
 
 ##
-This is an example of a failed widget. I ask for a widget that can do dilations and erosions. The widget
-is created but is 'broken' because Omega made the mistake of using floats for the number of dilations
+
+This is an example of a failed widget. I ask for a widget that can do dilations
+and erosions. The widget
+is created but is 'broken' because Omega made the mistake of using floats for
+the number of dilations
 and erosions: (In the next video I tell Omega to fix it)
 
 https://user-images.githubusercontent.com/1870994/235770896-819f394d-9785-46e8-a31a-a135b19316bf.mp4
 
 ##
-Following up from previous video, I explain that I want the two parameters (number erosions and dilations)
-to be integers. Notice that I exploit the conversational nature of the agent by assuming that it remembers
+
+Following up from previous video, I explain that I want the two parameters (
+number erosions and dilations)
+to be integers. Notice that I exploit the conversational nature of the agent by
+assuming that it remembers
 what the widget is about:
 
 https://user-images.githubusercontent.com/1870994/235770914-90991ac4-337e-4dcd-a04c-dd44b5e8be3e.mp4
 
 ##
-This video demos a specialised 'cell and nuclei segmentation tool' which leverages [cellpose 2.0](https://www.cellpose.org/) to segment cell cytoplasms or nuclei. In general, we can't assume that
-LLMs know about every single image processing library, especially for specific domains. So it can be 
-a good strategy to provide such specialised tools. After Omega successfully segments the nuclei, I ask
-from it to count the nuclei. Answer: 340. Notice that the code generated 'searches' the layer with name 'segmented' with a loop. Cute:
+
+This video demos a specialised 'cell and nuclei segmentation tool' which
+leverages [cellpose 2.0](https://www.cellpose.org/) to segment cell cytoplasms
+or nuclei. In general, we can't assume that
+LLMs know about every single image processing library, especially for specific
+domains. So it can be
+a good strategy to provide such specialised tools. After Omega successfully
+segments the nuclei, I ask
+from it to count the nuclei. Answer: 340. Notice that the code generated '
+searches' the layer with name 'segmented' with a loop. Cute:
 
 https://user-images.githubusercontent.com/1870994/235770933-07f5cbe6-2224-4dcd-b378-e81cc4e66500.mov
 
 ##
-Enough with cells. Aparently The 'memory' of ChatGPT is filled with unescessary information, it knows the url of Albert Einstein's photo on wikipedia, and combined with the 'napari file open' tool it can therefore open that photo in napari:
+
+Enough with cells. Aparently The 'memory' of ChatGPT is filled with unescessary
+information, it knows the url of Albert Einstein's photo on wikipedia, and
+combined with the 'napari file open' tool it can therefore open that photo in
+napari:
 
 https://user-images.githubusercontent.com/1870994/235770959-406e8173-8416-4100-bcb6-7f0b617ce234.mp4
 
-## 
-You can ask for rather incongruous widgets, widgets you would probably never write because you just need them once or something. Here I ask for a widget that applies a rather odd non-linear transformation to each
-pixel. The result is predictably boring, but it works, and I don't think that the answer was 'copy pasted'
+##  
+
+You can ask for rather incongruous widgets, widgets you would probably never
+write because you just need them once or something. Here I ask for a widget that
+applies a rather odd non-linear transformation to each
+pixel. The result is predictably boring, but it works, and I don't think that
+the answer was 'copy pasted'
 from somewhere else...
 
 https://user-images.githubusercontent.com/1870994/235770984-c88c8eac-d3b2-47d7-81b1-48fbe4429e90.mp4
 
 ##
-In this one, starting again from our beloved Albert, I ask to rename that layer to 'Einstein' which looks
-better than just 'array'. Then I ask Omega to apply a Canny edge filter. Predictably it uses scikit-image:
+
+In this one, starting again from our beloved Albert, I ask to rename that layer
+to 'Einstein' which looks
+better than just 'array'. Then I ask Omega to apply a Canny edge filter.
+Predictably it uses scikit-image:
 
 https://user-images.githubusercontent.com/1870994/235771000-89dba0db-e710-4f76-b271-e9dcf65239b1.mp4
 
-## 
-Then I ask for a 'Canny edge detection widget'. It happily makes the widget and offers relevant parameters:
+##  
+
+Then I ask for a 'Canny edge detection widget'. It happily makes the widget and
+offers relevant parameters:
 
 https://user-images.githubusercontent.com/1870994/235771031-d978b652-2e28-4178-aa7e-dbdfd2e21c2d.mp4
 
 ##
-Following up on previous video, I play with dilations on the edge image. 
-Omega has some trouble when I ask to 'do it again'. Fine, sometimes you have a bit more explicit:
+
+Following up on previous video, I play with dilations on the edge image.
+Omega has some trouble when I ask to 'do it again'. Fine, sometimes you have a
+bit more explicit:
 
 https://user-images.githubusercontent.com/1870994/235771066-adc7f0bb-0b8e-415c-8e89-6107182cd5b1.mp4
 
 ##
-You can also experiment with more classic 'numpy' code by creating and manipulating arrays and visualising 
+
+You can also experiment with more classic 'numpy' code by creating and
+manipulating arrays and visualising
 the output live:
 
 https://user-images.githubusercontent.com/1870994/235771093-85a751c8-cc5a-4685-b40a-acdf81f0e5c9.mp4
 
 ##
-This video demonstrates that Omega understand many aspects of the napari viewer API. It can switch viewing modes, translate layers, etc... :
+
+This video demonstrates that Omega understand many aspects of the napari viewer
+API. It can switch viewing modes, translate layers, etc... :
 
 https://user-images.githubusercontent.com/1870994/235771129-db095c1f-56f7-4bb9-9bff-ef57ce66387b.mp4
 
 ##
-I never thought this one would work: I ask Omega to open in napari a mp4 video from a URL and then use OpenCV to detect people. It does it. But the one thing that Omega does not know is that creating a layer for each frame of the video is not a practical approach. Not clear what happened to the colors though. Probably an RGB ordering or format issue:
 
-https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
+I never thought this one would work: I ask Omega to open in napari a mp4 video
+from a URL and then use OpenCV to detect people. It does it. But the one thing
+that Omega does not know is that creating a layer for each frame of the video is
+not a practical approach. Not clear what happened to the colors though. Probably
+an RGB ordering or format issue:
 
+https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
 
 ## Disclaimer:
 
 Do not use this software lightly, it will download libaries by its own volition,
-write any code that it deems nescessary, it might actually do what you ask, even if
-it is a bad idea. Also, beware that it might _misundertand_ what you ask and then do
-something bad. For example, it is unwise to use Omega to delete 'some' files from your system,
+write any code that it deems nescessary, it might actually do what you ask, even
+if
+it is a bad idea. Also, beware that it might _misundertand_ what you ask and
+then do
+something bad. For example, it is unwise to use Omega to delete 'some' files
+from your system,
 it might end up deleteing more than that if you are unclear in your request.  
-To be 100% safe, we recommend that you use this software from within a sandboxed virtual machine. 
+To be 100% safe, we recommend that you use this software from within a sandboxed
+virtual machine.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
-INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR 
-PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE 
-FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
-TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE 
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED,
+INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR
+PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+BE LIABLE
+FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
+THE
 USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-
 ## Contributing
 
-Contributions are very welcome. Tests can be run with [tox], please ensure
+Contributions are extremely welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-chatgpt" is free and open source software
```

### Comparing `napari-chatgpt-2023.5.2/tox.ini` & `napari-chatgpt-2023.6.2/tox.ini`

 * *Files identical despite different names*

