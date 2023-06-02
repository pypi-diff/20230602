# Comparing `tmp/xircuits-1.8.2.tar.gz` & `tmp/xircuits-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xircuits-1.8.2.tar", last modified: Thu Jun  1 09:39:57 2023, max compression
+gzip compressed data, was "xircuits-1.8.3.tar", last modified: Fri Jun  2 21:53:15 2023, max compression
```

## Comparing `xircuits-1.8.2.tar` & `xircuits-1.8.3.tar`

### file list

```diff
@@ -1,243 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:57.013994 xircuits-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-01 09:37:30.000000 xircuits-1.8.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-01 09:37:30.000000 xircuits-1.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-01 09:37:30.000000 xircuits-1.8.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 09:37:30.000000 xircuits-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-01 09:37:30.000000 xircuits-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-01 09:39:57.013994 xircuits-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-01 09:37:30.000000 xircuits-1.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-01 09:37:30.000000 xircuits-1.8.2/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-01 09:37:30.000000 xircuits-1.8.2/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.973993 xircuits-1.8.2/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.977993 xircuits-1.8.2/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 09:37:30.000000 xircuits-1.8.2/jupyter-config/nb-config/xircuits.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.977993 xircuits-1.8.2/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 09:37:30.000000 xircuits-1.8.2/jupyter-config/server-config/xircuits.json
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-01 09:37:30.000000 xircuits-1.8.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-01 09:37:30.000000 xircuits-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-01 09:37:30.000000 xircuits-1.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:39:57.013994 xircuits-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-01 09:37:30.000000 xircuits-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.981993 xircuits-1.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.981993 xircuits-1.8.2/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/commands/CustomActionEvent.tsx
--rw-r--r--   0 runner    (1001) docker     (123)    33587 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/commands/NodeActionCommands.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.981993 xircuits-1.8.2/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/CustomNodeFactory.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/CustomNodeModel.ts
--rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/CustomNodeWidget.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/DragNewLinkState.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/RunSwitcher.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/XircuitsApp.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.981993 xircuits-1.8.2/src/components/link/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/link/CustomLinkFactory.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/link/CustomLinkModel.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.981993 xircuits-1.8.2/src/components/port/
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/port/CustomPortLabel.tsx
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/port/CustomPortModel.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.981993 xircuits-1.8.2/src/components/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/state/CustomDiagramState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/state/DefaultState.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/state/DragDiagramItemsState.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/state/DragNewLinkState.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/state/MoveItemsState.ts
--rw-r--r--   0 runner    (1001) docker     (123)    34261 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/components/xircuitBodyWidget.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.981993 xircuits-1.8.2/src/context-menu/
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/context-menu/ComponentsPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/context-menu/NodeActionsPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/context-menu/TrayItemPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/context-menu/TrayPanel.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.981993 xircuits-1.8.2/src/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/dialog/CommentDialog.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/dialog/FormDialog.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/dialog/LiteralInputDialog.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/dialog/RunDialog.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/dialog/formDialogwidget.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.985993 xircuits-1.8.2/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/helpers/DemoCanvasWidget.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/helpers/DemoWorkspaceWidget.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/helpers/Helper.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/helpers/InputSanitizer.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/helpers/index.css
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/index.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.985993 xircuits-1.8.2/src/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/kernel/RunOutput.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/kernel/panel.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.985993 xircuits-1.8.2/src/log/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/log/LogLevelSwitcher.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/log/LogPlugin.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.985993 xircuits-1.8.2/src/server/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/server/handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/svg.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.985993 xircuits-1.8.2/src/tray_library/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/tray_library/AdvanceComponentLib.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/tray_library/Component.tsx
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/tray_library/GeneralComponentLib.tsx
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/tray_library/Sidebar.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/tray_library/TrayItemWidget.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/tray_library/TrayWidget.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.985993 xircuits-1.8.2/src/ui-components/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/ui-components/icons.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/xircuitFactory.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-01 09:37:30.000000 xircuits-1.8.2/src/xircuitWidget.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.985993 xircuits-1.8.2/style/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/Comment.css
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/ComponentInfo.css
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/ComponentsPanel.css
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/NodeActionPanel.css
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/Sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)    19174 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/description-markdown.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.989993 xircuits-1.8.2/style/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/3-vertical-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/breakpoint.svg
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/component-library.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/debugger.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/lock-nodes.svg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/next.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/reload-all.svg
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/revert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   489893 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/xpress-loading-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)   262062 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/xpress-loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)   127132 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/xpress-logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/icons/xpress-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-01 09:37:30.000000 xircuits-1.8.2/style/toggle.css
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-01 09:37:30.000000 xircuits-1.8.2/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.989993 xircuits-1.8.2/xai_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.989993 xircuits-1.8.2/xai_components/xai_controlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_controlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_controlflow/branches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.989993 xircuits-1.8.2/xai_components/xai_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_pytorch/quickstart.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_pytorch/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_pytorch/torch_nn_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.989993 xircuits-1.8.2/xai_components/xai_spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_spark/pyspark_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_spark/pyspark_mllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_spark/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_spark/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.989993 xircuits-1.8.2/xai_components/xai_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_template/example_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_template/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_template/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.993993 xircuits-1.8.2/xai_components/xai_tensorflow_keras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_tensorflow_keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_tensorflow_keras/keras_transfer_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_tensorflow_keras/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_tensorflow_keras/tf_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_tensorflow_keras/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.993993 xircuits-1.8.2/xai_components/xai_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-01 09:37:30.000000 xircuits-1.8.2/xai_components/xai_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.993993 xircuits-1.8.2/xircuits/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.993993 xircuits-1.8.2/xircuits/.xircuits/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-01 09:39:56.000000 xircuits-1.8.2/xircuits/.xircuits/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/.xircuits/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.993993 xircuits-1.8.2/xircuits/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/compiler/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/compiler/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/compiler/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/compiler/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.993993 xircuits-1.8.2/xircuits/compiler/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/compiler/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/compiler/vendor/unparse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.997994 xircuits-1.8.2/xircuits/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/handlers/compile_xircuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/handlers/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/handlers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/handlers/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/handlers/request_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/handlers/request_submodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/handlers/spark_submit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.997994 xircuits-1.8.2/xircuits/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-01 09:39:24.000000 xircuits-1.8.2/xircuits/labextension/build_log.json
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:57.009994 xircuits-1.8.2/xircuits/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   262062 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/bc25618efe3bea59255b942449ba5922365f0aad8cfb91b8096790363ff0ac9b.gif
--rw-r--r--   0 runner    (1001) docker     (123)   361350 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/lib_index_js.e3c375749eca37176102.js
--rw-r--r--   0 runner    (1001) docker     (123)   450477 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/lib_index_js.e3c375749eca37176102.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0.e5e08421993e8b0d6940.js
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0.e5e08421993e8b0d6940.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1.69771b4348e185a22e47.js
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1.69771b4348e185a22e47.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c0.a1fe7d758d8bfd1fcb6d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c0.a1fe7d758d8bfd1fcb6d.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c1.4158a663778b2cc4558a.js
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c1.4158a663778b2cc4558a.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    62894 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/remoteEntry.3aab60af2c2340b392f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/remoteEntry.3aab60af2c2340b392f7.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-01 09:39:24.000000 xircuits-1.8.2/xircuits/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)   114764 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js
--rw-r--r--   0 runner    (1001) docker     (123)   115185 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js
--rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   411695 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js
--rw-r--r--   0 runner    (1001) docker     (123)   407959 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   110571 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.339ba20fba041bb86e74.js
--rw-r--r--   0 runner    (1001) docker     (123)   104002 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.339ba20fba041bb86e74.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    37911 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.63a1ec84812da57c0fc4.js
--rw-r--r--   0 runner    (1001) docker     (123)    34045 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.63a1ec84812da57c0fc4.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7.6237bb7955064b6be43a.js
--rw-r--r--   0 runner    (1001) docker     (123)    40767 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7.6237bb7955064b6be43a.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    78456 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_marked_lib_marked_esm_js.f8b1654d24f4d8a9ebb1.js
--rw-r--r--   0 runner    (1001) docker     (123)    96369 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_marked_lib_marked_esm_js.f8b1654d24f4d8a9ebb1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    91107 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_pathfinding_index_js.57d527803f5ef363858c.js
--rw-r--r--   0 runner    (1001) docker     (123)   101513 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_pathfinding_index_js.57d527803f5ef363858c.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   558946 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_geometry_dist_index_js.6d56ef20c085cca0afc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   692762 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_geometry_dist_index_js.6d56ef20c085cca0afc6.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    80823 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-canvas-core_dist_index_js.fedff644cad1098d8bcb.js
--rw-r--r--   0 runner    (1001) docker     (123)   110591 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-canvas-core_dist_index_js.fedff644cad1098d8bcb.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   105669 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js.23c3c2a475ea57fe7938.js
--rw-r--r--   0 runner    (1001) docker     (123)   144789 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js.23c3c2a475ea57fe7938.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    37033 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js.7dc9f640385f857c0d8d.js
--rw-r--r--   0 runner    (1001) docker     (123)    46494 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js.7dc9f640385f857c0d8d.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    61726 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js.274da3f6f09bc30ae8a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    86658 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js.274da3f6f09bc30ae8a5.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    39451 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_prop-types_index_js.ecaf55d6e3a49828fd03.js
--rw-r--r--   0 runner    (1001) docker     (123)    44610 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_prop-types_index_js.ecaf55d6e3a49828fd03.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-accessible-accordion_dist_es_index_js.e27e21540f362d2400f1.js
--rw-r--r--   0 runner    (1001) docker     (123)    33663 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-accessible-accordion_dist_es_index_js.e27e21540f362d2400f1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    50019 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-image-gallery_build_image-gallery_js.54c6b2ee4f593bcd3578.js
--rw-r--r--   0 runner    (1001) docker     (123)    58384 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-image-gallery_build_image-gallery_js.54c6b2ee4f593bcd3578.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    38684 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-numeric-input_index_js.7e201324b89725af60a3.js
--rw-r--r--   0 runner    (1001) docker     (123)    45998 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-numeric-input_index_js.7e201324b89725af60a3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-portal-tooltip_lib_index_js.13053d183ec1bf6fe8b1.js
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-portal-tooltip_lib_index_js.13053d183ec1bf6fe8b1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    20526 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-switch_index_js.a2a55561dfbed639ad75.js
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-switch_index_js.a2a55561dfbed639ad75.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-toggle_dist_component_index_js.e801abe36cc813fe2470.js
--rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-toggle_dist_component_index_js.e801abe36cc813fe2470.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    93056 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-tooltip_dist_index_es_js.917868bea13b4ea0b7c0.js
--rw-r--r--   0 runner    (1001) docker     (123)   171088 2023-06-01 09:39:27.000000 xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-tooltip_dist_index_es_js.917868bea13b4ea0b7c0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-01 09:37:30.000000 xircuits-1.8.2/xircuits/start_xircuits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:39:56.993993 xircuits-1.8.2/xircuits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-01 09:39:56.000000 xircuits-1.8.2/xircuits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-06-01 09:39:56.000000 xircuits-1.8.2/xircuits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:39:56.000000 xircuits-1.8.2/xircuits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 09:39:56.000000 xircuits-1.8.2/xircuits.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:38:29.000000 xircuits-1.8.2/xircuits.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-01 09:39:56.000000 xircuits-1.8.2/xircuits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 09:39:56.000000 xircuits-1.8.2/xircuits.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.490049 xircuits-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-02 21:51:04.000000 xircuits-1.8.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 21:51:04.000000 xircuits-1.8.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-02 21:51:04.000000 xircuits-1.8.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 21:51:04.000000 xircuits-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-02 21:51:04.000000 xircuits-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-02 21:53:15.490049 xircuits-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-02 21:51:04.000000 xircuits-1.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-02 21:51:04.000000 xircuits-1.8.3/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-02 21:51:04.000000 xircuits-1.8.3/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.454048 xircuits-1.8.3/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 21:51:04.000000 xircuits-1.8.3/jupyter-config/nb-config/xircuits.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-02 21:51:04.000000 xircuits-1.8.3/jupyter-config/server-config/xircuits.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-02 21:51:04.000000 xircuits-1.8.3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 21:51:04.000000 xircuits-1.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 21:51:04.000000 xircuits-1.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:53:15.490049 xircuits-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-02 21:51:04.000000 xircuits-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/commands/CustomActionEvent.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    33587 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/commands/NodeActionCommands.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/CustomNodeFactory.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/CustomNodeModel.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/CustomNodeWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/DragNewLinkState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/RunSwitcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/XircuitsApp.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/src/components/link/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/link/CustomLinkFactory.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/link/CustomLinkModel.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/src/components/port/
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/port/CustomPortLabel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/port/CustomPortModel.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/src/components/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/state/CustomDiagramState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/state/DefaultState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/state/DragDiagramItemsState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/state/DragNewLinkState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/state/MoveItemsState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    34261 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/components/xircuitBodyWidget.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/src/context-menu/
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/context-menu/ComponentsPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/context-menu/NodeActionsPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/context-menu/TrayItemPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/context-menu/TrayPanel.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.462048 xircuits-1.8.3/src/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/dialog/CommentDialog.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/dialog/FormDialog.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/dialog/LiteralInputDialog.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/dialog/RunDialog.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/dialog/formDialogwidget.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.466048 xircuits-1.8.3/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/helpers/DemoCanvasWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/helpers/DemoWorkspaceWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/helpers/Helper.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/helpers/InputSanitizer.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/helpers/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/index.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.466048 xircuits-1.8.3/src/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/kernel/RunOutput.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/kernel/panel.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.466048 xircuits-1.8.3/src/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/log/LogLevelSwitcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/log/LogPlugin.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.466048 xircuits-1.8.3/src/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/server/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/svg.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.466048 xircuits-1.8.3/src/tray_library/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/tray_library/AdvanceComponentLib.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/tray_library/Component.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/tray_library/GeneralComponentLib.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/tray_library/Sidebar.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/tray_library/TrayItemWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/tray_library/TrayWidget.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.466048 xircuits-1.8.3/src/ui-components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/ui-components/icons.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/xircuitFactory.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-02 21:51:04.000000 xircuits-1.8.3/src/xircuitWidget.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.466048 xircuits-1.8.3/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/Comment.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/ComponentInfo.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/ComponentsPanel.css
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/NodeActionPanel.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/Sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)    19174 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/description-markdown.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.470048 xircuits-1.8.3/style/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/3-vertical-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/breakpoint.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/component-library.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/debugger.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/lock-nodes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/next.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/reload-all.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/revert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   489893 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/xpress-loading-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   262062 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/xpress-loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   127132 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/xpress-logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/icons/xpress-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-02 21:51:04.000000 xircuits-1.8.3/style/toggle.css
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-02 21:51:04.000000 xircuits-1.8.3/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.470048 xircuits-1.8.3/xai_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.470048 xircuits-1.8.3/xai_components/xai_controlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_controlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_controlflow/branches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.470048 xircuits-1.8.3/xai_components/xai_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_pytorch/quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_pytorch/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_pytorch/torch_nn_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.470048 xircuits-1.8.3/xai_components/xai_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_sklearn/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_sklearn/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_sklearn/sklearn_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.470048 xircuits-1.8.3/xai_components/xai_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_spark/pyspark_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_spark/pyspark_mllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_spark/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_spark/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.470048 xircuits-1.8.3/xai_components/xai_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_template/example_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_template/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_template/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xai_components/xai_tensorflow_keras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_tensorflow_keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_tensorflow_keras/keras_transfer_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_tensorflow_keras/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_tensorflow_keras/tf_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_tensorflow_keras/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xai_components/xai_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xai_components/xai_xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_xgboost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xai_components/xai_xgboost/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_xgboost/examples/XGBoostClassifier.xircuits
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_xgboost/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_xgboost/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-02 21:51:04.000000 xircuits-1.8.3/xai_components/xai_xgboost/xgboost_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xircuits/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xircuits/.xircuits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-02 21:53:14.000000 xircuits-1.8.3/xircuits/.xircuits/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/.xircuits/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xircuits/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/compiler/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/compiler/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/compiler/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/compiler/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xircuits/compiler/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/compiler/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/compiler/vendor/unparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.478048 xircuits-1.8.3/xircuits/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/handlers/compile_xircuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/handlers/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/handlers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/handlers/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/handlers/request_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/handlers/request_submodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/handlers/spark_submit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.478048 xircuits-1.8.3/xircuits/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-02 21:52:45.000000 xircuits-1.8.3/xircuits/labextension/build_log.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.490049 xircuits-1.8.3/xircuits/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   262062 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/bc25618efe3bea59255b942449ba5922365f0aad8cfb91b8096790363ff0ac9b.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   361350 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/lib_index_js.e3c375749eca37176102.js
+-rw-r--r--   0 runner    (1001) docker     (123)   450477 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/lib_index_js.e3c375749eca37176102.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0.e5e08421993e8b0d6940.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0.e5e08421993e8b0d6940.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1.69771b4348e185a22e47.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1.69771b4348e185a22e47.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c0.a1fe7d758d8bfd1fcb6d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c0.a1fe7d758d8bfd1fcb6d.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c1.4158a663778b2cc4558a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c1.4158a663778b2cc4558a.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    62894 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/remoteEntry.e8c33c4dca473d62d6b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/remoteEntry.e8c33c4dca473d62d6b4.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-02 21:52:45.000000 xircuits-1.8.3/xircuits/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114764 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   115185 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   411695 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js
+-rw-r--r--   0 runner    (1001) docker     (123)   407959 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   110571 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.339ba20fba041bb86e74.js
+-rw-r--r--   0 runner    (1001) docker     (123)   104002 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.339ba20fba041bb86e74.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    37911 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.63a1ec84812da57c0fc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34045 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.63a1ec84812da57c0fc4.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7.6237bb7955064b6be43a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40767 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7.6237bb7955064b6be43a.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    78456 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_marked_lib_marked_esm_js.f8b1654d24f4d8a9ebb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    96369 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_marked_lib_marked_esm_js.f8b1654d24f4d8a9ebb1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    91107 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_pathfinding_index_js.57d527803f5ef363858c.js
+-rw-r--r--   0 runner    (1001) docker     (123)   101513 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_pathfinding_index_js.57d527803f5ef363858c.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   558946 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_geometry_dist_index_js.6d56ef20c085cca0afc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   692762 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_geometry_dist_index_js.6d56ef20c085cca0afc6.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    80823 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-canvas-core_dist_index_js.fedff644cad1098d8bcb.js
+-rw-r--r--   0 runner    (1001) docker     (123)   110591 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-canvas-core_dist_index_js.fedff644cad1098d8bcb.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   105669 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js.23c3c2a475ea57fe7938.js
+-rw-r--r--   0 runner    (1001) docker     (123)   144789 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js.23c3c2a475ea57fe7938.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    37033 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js.7dc9f640385f857c0d8d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    46494 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js.7dc9f640385f857c0d8d.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    61726 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js.274da3f6f09bc30ae8a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86658 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js.274da3f6f09bc30ae8a5.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    39451 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_prop-types_index_js.ecaf55d6e3a49828fd03.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44610 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_prop-types_index_js.ecaf55d6e3a49828fd03.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-accessible-accordion_dist_es_index_js.e27e21540f362d2400f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33663 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-accessible-accordion_dist_es_index_js.e27e21540f362d2400f1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50019 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-image-gallery_build_image-gallery_js.54c6b2ee4f593bcd3578.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58384 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-image-gallery_build_image-gallery_js.54c6b2ee4f593bcd3578.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    38684 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-numeric-input_index_js.7e201324b89725af60a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45998 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-numeric-input_index_js.7e201324b89725af60a3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-portal-tooltip_lib_index_js.13053d183ec1bf6fe8b1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-portal-tooltip_lib_index_js.13053d183ec1bf6fe8b1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    20526 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-switch_index_js.a2a55561dfbed639ad75.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-switch_index_js.a2a55561dfbed639ad75.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-toggle_dist_component_index_js.e801abe36cc813fe2470.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-toggle_dist_component_index_js.e801abe36cc813fe2470.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    93056 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-tooltip_dist_index_es_js.917868bea13b4ea0b7c0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   171088 2023-06-02 21:52:48.000000 xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-tooltip_dist_index_es_js.917868bea13b4ea0b7c0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-02 21:51:04.000000 xircuits-1.8.3/xircuits/start_xircuits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:15.474048 xircuits-1.8.3/xircuits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-02 21:53:14.000000 xircuits-1.8.3/xircuits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-02 21:53:15.000000 xircuits-1.8.3/xircuits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:53:14.000000 xircuits-1.8.3/xircuits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-02 21:53:14.000000 xircuits-1.8.3/xircuits.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:51:55.000000 xircuits-1.8.3/xircuits.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-02 21:53:14.000000 xircuits-1.8.3/xircuits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 21:53:14.000000 xircuits-1.8.3/xircuits.egg-info/top_level.txt
```

### Comparing `xircuits-1.8.2/.gitmodules` & `xircuits-1.8.3/.gitmodules`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/CONTRIBUTING.md` & `xircuits-1.8.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/LICENSE` & `xircuits-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/MANIFEST.in` & `xircuits-1.8.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/PKG-INFO` & `xircuits-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xircuits
-Version: 1.8.2
+Version: 1.8.3
 Summary: A JupyterLab extension for rendering and editing xircuit files.
 Home-page: https://github.com/XpressAI/xircuits
 Author: Xpress AI
 Author-email: eduardo@xpress.ai
 License: Apache-2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -19,18 +19,20 @@
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: spark
+Provides-Extra: template
 Provides-Extra: tensorflow_keras
 Provides-Extra: pytorch
-Provides-Extra: template
+Provides-Extra: sklearn
+Provides-Extra: xgboost
+Provides-Extra: spark
 Provides-Extra: full
 License-File: LICENSE
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/68586800/151280601-7ff2b7b2-10e5-4544-b3df-aa6a5a654dae.png" width="450"/>
 </p>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: xircuits Version: 1.8.2 Summary: A JupyterLab
+Metadata-Version: 2.1 Name: xircuits Version: 1.8.3 Summary: A JupyterLab
 extension for rendering and editing xircuit files. Home-page: https://
 github.com/XpressAI/xircuits Author: Xpress AI Author-email: eduardo@xpress.ai
 License: Apache-2.0 Keywords: Jupyter,JupyterLab,JupyterLab3 Platform: Linux
 Platform: Mac OS X Platform: Windows Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab Classifier: Framework :: Jupyter
 :: JupyterLab :: 3 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-spark Provides-Extra: tensorflow_keras Provides-Extra: pytorch Provides-Extra:
-template Provides-Extra: full License-File: LICENSE
+template Provides-Extra: tensorflow_keras Provides-Extra: pytorch Provides-
+Extra: sklearn Provides-Extra: xgboost Provides-Extra: spark Provides-Extra:
+full License-File: LICENSE
  [https://user-images.githubusercontent.com/68586800/151280601-7ff2b7b2-10e5-
                           4544-b3df-aa6a5a654dae.png]
 Docs â¢ Install â¢ Tutorials â¢ Developer_Guides â¢ Contribute â¢ Blog â¢
                                    Discord
                    Component_Libraries â¢ Project_Templates
               [GitHub] [GitHub_release] [Documentation] [Python]
 ![xircuits-frontpage](https://user-images.githubusercontent.com/68586800/
```

### Comparing `xircuits-1.8.2/README.md` & `xircuits-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/RELEASE.md` & `xircuits-1.8.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/package.json` & `xircuits-1.8.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'1.8.3'"}*

```diff
@@ -116,9 +116,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.8.2"
+    "version": "1.8.3"
 }
```

### Comparing `xircuits-1.8.2/pyproject.toml` & `xircuits-1.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/setup.py` & `xircuits-1.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/commands/CustomActionEvent.tsx` & `xircuits-1.8.3/src/commands/CustomActionEvent.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/commands/NodeActionCommands.tsx` & `xircuits-1.8.3/src/commands/NodeActionCommands.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/CustomNodeFactory.tsx` & `xircuits-1.8.3/src/components/CustomNodeFactory.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/CustomNodeModel.ts` & `xircuits-1.8.3/src/components/CustomNodeModel.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/CustomNodeWidget.tsx` & `xircuits-1.8.3/src/components/CustomNodeWidget.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/DragNewLinkState.ts` & `xircuits-1.8.3/src/components/DragNewLinkState.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/RunSwitcher.tsx` & `xircuits-1.8.3/src/components/RunSwitcher.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/XircuitsApp.ts` & `xircuits-1.8.3/src/components/XircuitsApp.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/link/CustomLinkFactory.tsx` & `xircuits-1.8.3/src/components/link/CustomLinkFactory.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/link/CustomLinkModel.ts` & `xircuits-1.8.3/src/components/link/CustomLinkModel.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/port/CustomPortLabel.tsx` & `xircuits-1.8.3/src/components/port/CustomPortLabel.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/port/CustomPortModel.ts` & `xircuits-1.8.3/src/components/port/CustomPortModel.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/state/CustomDiagramState.ts` & `xircuits-1.8.3/src/components/state/CustomDiagramState.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/state/DefaultState.ts` & `xircuits-1.8.3/src/components/state/DefaultState.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/state/DragDiagramItemsState.ts` & `xircuits-1.8.3/src/components/state/DragDiagramItemsState.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/state/DragNewLinkState.ts` & `xircuits-1.8.3/src/components/state/DragNewLinkState.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/state/MoveItemsState.ts` & `xircuits-1.8.3/src/components/state/MoveItemsState.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/components/xircuitBodyWidget.tsx` & `xircuits-1.8.3/src/components/xircuitBodyWidget.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/context-menu/ComponentsPanel.tsx` & `xircuits-1.8.3/src/context-menu/ComponentsPanel.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/context-menu/NodeActionsPanel.tsx` & `xircuits-1.8.3/src/context-menu/NodeActionsPanel.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/context-menu/TrayItemPanel.tsx` & `xircuits-1.8.3/src/context-menu/TrayItemPanel.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/dialog/CommentDialog.tsx` & `xircuits-1.8.3/src/dialog/CommentDialog.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/dialog/FormDialog.tsx` & `xircuits-1.8.3/src/dialog/FormDialog.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/dialog/LiteralInputDialog.tsx` & `xircuits-1.8.3/src/dialog/LiteralInputDialog.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/dialog/RunDialog.tsx` & `xircuits-1.8.3/src/dialog/RunDialog.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/dialog/formDialogwidget.tsx` & `xircuits-1.8.3/src/dialog/formDialogwidget.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/helpers/DemoCanvasWidget.tsx` & `xircuits-1.8.3/src/helpers/DemoCanvasWidget.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/helpers/DemoWorkspaceWidget.tsx` & `xircuits-1.8.3/src/helpers/DemoWorkspaceWidget.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/helpers/Helper.tsx` & `xircuits-1.8.3/src/helpers/Helper.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/helpers/InputSanitizer.tsx` & `xircuits-1.8.3/src/helpers/InputSanitizer.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/index.tsx` & `xircuits-1.8.3/src/index.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/kernel/panel.ts` & `xircuits-1.8.3/src/kernel/panel.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/log/LogLevelSwitcher.tsx` & `xircuits-1.8.3/src/log/LogLevelSwitcher.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/log/LogPlugin.ts` & `xircuits-1.8.3/src/log/LogPlugin.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/server/handler.ts` & `xircuits-1.8.3/src/server/handler.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/tray_library/AdvanceComponentLib.tsx` & `xircuits-1.8.3/src/tray_library/AdvanceComponentLib.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/tray_library/Component.tsx` & `xircuits-1.8.3/src/tray_library/Component.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/tray_library/GeneralComponentLib.tsx` & `xircuits-1.8.3/src/tray_library/GeneralComponentLib.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/tray_library/Sidebar.tsx` & `xircuits-1.8.3/src/tray_library/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/tray_library/TrayItemWidget.tsx` & `xircuits-1.8.3/src/tray_library/TrayItemWidget.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/ui-components/icons.tsx` & `xircuits-1.8.3/src/ui-components/icons.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/xircuitFactory.ts` & `xircuits-1.8.3/src/xircuitFactory.ts`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/src/xircuitWidget.tsx` & `xircuits-1.8.3/src/xircuitWidget.tsx`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/ComponentInfo.css` & `xircuits-1.8.3/style/ComponentInfo.css`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/ComponentsPanel.css` & `xircuits-1.8.3/style/ComponentsPanel.css`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/Sidebar.css` & `xircuits-1.8.3/style/Sidebar.css`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/base.css` & `xircuits-1.8.3/style/base.css`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/description-markdown.css` & `xircuits-1.8.3/style/description-markdown.css`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/icons/debugger.svg` & `xircuits-1.8.3/style/icons/debugger.svg`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/icons/lock.svg` & `xircuits-1.8.3/style/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/icons/reload-all.svg` & `xircuits-1.8.3/style/icons/reload-all.svg`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/icons/revert.svg` & `xircuits-1.8.3/style/icons/revert.svg`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/icons/xpress-loading-2.gif` & `xircuits-1.8.3/style/icons/xpress-loading-2.gif`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/icons/xpress-loading.gif` & `xircuits-1.8.3/style/icons/xpress-loading.gif`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/icons/xpress-logo.ico` & `xircuits-1.8.3/style/icons/xpress-logo.ico`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/icons/xpress-logo.svg` & `xircuits-1.8.3/style/icons/xpress-logo.svg`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/style/toggle.css` & `xircuits-1.8.3/style/toggle.css`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/tsconfig.json` & `xircuits-1.8.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/base.py` & `xircuits-1.8.3/xai_components/base.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/readme.md` & `xircuits-1.8.3/xai_components/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 <div align="center">
 
 | Name     | Description                                                                                    |                                                                                                                                                            |
 | -------- | ---------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Tensorflow Keras | Deep learning related components using Tensorflow Keras.                                       | [Link](https://github.com/XpressAI/xircuits/tree/master/xai_components/xai_tensorflow_keras) |
 | Pytorch  | Components that use Pytorch's ML library.                                                      | [Link](https://github.com/XpressAI/xircuits/tree/master/xai_components/xai_pytorch)   |
 | Spark    | Components built using the Pyspark library. Run these components with the Xircuits Remote Run! | [Link](https://github.com/XpressAI/xircuits/tree/master/xai_components/xai_spark)       |
+| SKlearn | Scikit learn components. | [Link](https://github.com/XpressAI/xircuits/tree/master/xai_components/xai_sklearn) |
+| XGBoost |  Optimized distributed gradient boosting library. | [Link](https://github.com/XpressAI/xircuits/tree/master/xai_components/xai_xgboost) |
 | Template | Great components for new learners and to experiment outputs.                                   | [Link](https://github.com/XpressAI/xircuits/tree/master/xai_components/xai_template) |
 | Utils    | Commonly used components for day-to-day workflows.                                             | [Link](https://github.com/XpressAI/xircuits/tree/master/xai_components/xai_utils)       |
 | Controlflow | Components to enable ifs and loops. | [Link](https://github.com/XpressAI/xircuits/tree/master/xai_components/xai_controlflow) |
 
 </div>
```

### Comparing `xircuits-1.8.2/xai_components/xai_controlflow/branches.py` & `xircuits-1.8.3/xai_components/xai_controlflow/branches.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_pytorch/quickstart.py` & `xircuits-1.8.3/xai_components/xai_pytorch/quickstart.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_pytorch/torch_nn_layers.py` & `xircuits-1.8.3/xai_components/xai_pytorch/torch_nn_layers.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_spark/pyspark_core.py` & `xircuits-1.8.3/xai_components/xai_spark/pyspark_core.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_spark/pyspark_mllib.py` & `xircuits-1.8.3/xai_components/xai_spark/pyspark_mllib.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_spark/readme.md` & `xircuits-1.8.3/xai_components/xai_spark/readme.md`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_template/example_components.py` & `xircuits-1.8.3/xai_components/xai_template/example_components.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_tensorflow_keras/keras_transfer_learning.py` & `xircuits-1.8.3/xai_components/xai_tensorflow_keras/keras_transfer_learning.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_tensorflow_keras/tf_keras.py` & `xircuits-1.8.3/xai_components/xai_tensorflow_keras/tf_keras.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_tensorflow_keras/training.py` & `xircuits-1.8.3/xai_components/xai_tensorflow_keras/training.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xai_components/xai_utils/utils.py` & `xircuits-1.8.3/xai_components/xai_utils/utils.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/.xircuits/.gitmodules` & `xircuits-1.8.3/xircuits/.xircuits/.gitmodules`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/.xircuits/config.ini` & `xircuits-1.8.3/xircuits/.xircuits/config.ini`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/__init__.py` & `xircuits-1.8.3/xircuits/__init__.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/compiler/compiler.py` & `xircuits-1.8.3/xircuits/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/compiler/generator.py` & `xircuits-1.8.3/xircuits/compiler/generator.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/compiler/parser.py` & `xircuits-1.8.3/xircuits/compiler/parser.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/compiler/vendor/unparse.py` & `xircuits-1.8.3/xircuits/compiler/vendor/unparse.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/handlers/__init__.py` & `xircuits-1.8.3/xircuits/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/handlers/compile_xircuits.py` & `xircuits-1.8.3/xircuits/handlers/compile_xircuits.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/handlers/components.py` & `xircuits-1.8.3/xircuits/handlers/components.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/handlers/config.py` & `xircuits-1.8.3/xircuits/handlers/config.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/handlers/debugger.py` & `xircuits-1.8.3/xircuits/handlers/debugger.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/handlers/request_folder.py` & `xircuits-1.8.3/xircuits/handlers/request_folder.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/handlers/request_submodule.py` & `xircuits-1.8.3/xircuits/handlers/request_submodule.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/handlers/spark_submit.py` & `xircuits-1.8.3/xircuits/handlers/spark_submit.py`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/build_log.json` & `xircuits-1.8.3/xircuits/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999994326434276%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'xircuits': {'version': '1.8.3'}}}}}}"}*

```diff
@@ -635,15 +635,15 @@
                         "react-switch": {},
                         "react-textarea-autosize": {},
                         "react-toggle": {},
                         "react-tooltip": {},
                         "xircuits": {
                             "import": "/home/runner/work/xircuits/xircuits/lib/index.js",
                             "singleton": true,
-                            "version": "1.8.2"
+                            "version": "1.8.3"
                         },
                         "yjs": {
                             "import": false,
                             "requiredVersion": "^13.5.17",
                             "singleton": true
                         }
                     }
```

### Comparing `xircuits-1.8.2/xircuits/labextension/package.json` & `xircuits-1.8.3/xircuits/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9731359649122806%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e8c33c4dca473d62d6b4.js'}}",*

 * * "'version'": "'1.8.3'"}*

```diff
@@ -67,15 +67,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/XpressAI/xircuits",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3aab60af2c2340b392f7.js",
+            "load": "static/remoteEntry.e8c33c4dca473d62d6b4.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "xircuits"
                 },
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.8.2"
+    "version": "1.8.3"
 }
```

### Comparing `xircuits-1.8.2/xircuits/labextension/static/bc25618efe3bea59255b942449ba5922365f0aad8cfb91b8096790363ff0ac9b.gif` & `xircuits-1.8.3/xircuits/labextension/static/bc25618efe3bea59255b942449ba5922365f0aad8cfb91b8096790363ff0ac9b.gif`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/lib_index_js.e3c375749eca37176102.js` & `xircuits-1.8.3/xircuits/labextension/static/lib_index_js.e3c375749eca37176102.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/lib_index_js.e3c375749eca37176102.js.map` & `xircuits-1.8.3/xircuits/labextension/static/lib_index_js.e3c375749eca37176102.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0.e5e08421993e8b0d6940.js` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0.e5e08421993e8b0d6940.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0.e5e08421993e8b0d6940.js.map` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0.e5e08421993e8b0d6940.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1.69771b4348e185a22e47.js` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1.69771b4348e185a22e47.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1.69771b4348e185a22e47.js.map` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1.69771b4348e185a22e47.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c0.a1fe7d758d8bfd1fcb6d.js` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c0.a1fe7d758d8bfd1fcb6d.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c0.a1fe7d758d8bfd1fcb6d.js.map` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c0.a1fe7d758d8bfd1fcb6d.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c1.4158a663778b2cc4558a.js` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c1.4158a663778b2cc4558a.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c1.4158a663778b2cc4558a.js.map` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_krc-pagination_lib_index_js-_9b3c1.4158a663778b2cc4558a.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js.map` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js.map` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js.map` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js.map` & `xircuits-1.8.3/xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/remoteEntry.3aab60af2c2340b392f7.js` & `xircuits-1.8.3/xircuits/labextension/static/remoteEntry.e8c33c4dca473d62d6b4.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -519,15 +519,15 @@
                     /******/
                     register("react-textarea-autosize", "8.3.3", () => (Promise.all([__webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910")]).then(() => (() => (__webpack_require__( /*! ./node_modules/react-textarea-autosize/dist/react-textarea-autosize.browser.esm.js */ "./node_modules/react-textarea-autosize/dist/react-textarea-autosize.browser.esm.js"))))));
                     /******/
                     register("react-toggle", "4.1.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_prop-types_index_js"), __webpack_require__.e("vendors-node_modules_react-toggle_dist_component_index_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ./node_modules/react-toggle/dist/component/index.js */ "./node_modules/react-toggle/dist/component/index.js"))))));
                     /******/
                     register("react-tooltip", "4.2.21", () => (Promise.all([__webpack_require__.e("vendors-node_modules_prop-types_index_js"), __webpack_require__.e("vendors-node_modules_react-tooltip_dist_index_es_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ./node_modules/react-tooltip/dist/index.es.js */ "./node_modules/react-tooltip/dist/index.es.js"))))));
                     /******/
-                    register("xircuits", "1.8.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_projectstorm_geometry_dist_index_js"), __webpack_require__.e("vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js"), __webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("webpack_sharing_consume_default_emotion_styled_emotion_styled"), __webpack_require__.e("webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("xircuits", "1.8.3", () => (Promise.all([__webpack_require__.e("vendors-node_modules_projectstorm_geometry_dist_index_js"), __webpack_require__.e("vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js"), __webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("webpack_sharing_consume_default_emotion_styled_emotion_styled"), __webpack_require__.e("webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1364,8 +1364,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/xircuits");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).xircuits = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.3aab60af2c2340b392f7.js.map
+//# sourceMappingURL=remoteEntry.e8c33c4dca473d62d6b4.js.map
```

### Comparing `xircuits-1.8.2/xircuits/labextension/static/remoteEntry.3aab60af2c2340b392f7.js.map` & `xircuits-1.8.3/xircuits/labextension/static/remoteEntry.e8c33c4dca473d62d6b4.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9214285714285715%*

 * *Differences: {"'file'": "'remoteEntry.e8c33c4dca473d62d6b4.js'",*

 * * "'sourcesContent'": "{insert: [(11, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.3aab60af2c2340b392f7.js",
+    "file": "remoteEntry.e8c33c4dca473d62d6b4.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC/BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8qHAA8qH;WAC5sH;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;;;;;WCJA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7DA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCjRA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://xircuits/webpack/container-entry",
         "webpack://xircuits/webpack/bootstrap",
         "webpack://xircuits/webpack/runtime/compat get default export",
@@ -32,15 +32,15 @@
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_projectstorm_geometry_dist_index_js\":\"6d56ef20c085cca0afc6\",\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\":\"23c3c2a475ea57fe7938\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"60f4ca1c03a44b1a935c\",\"vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7\":\"6237bb7955064b6be43a\",\"webpack_sharing_consume_default_react\":\"f1fb04fd62b3f8f8252f\",\"webpack_sharing_consume_default_emotion_styled_emotion_styled\":\"c31a1efdeaeffdfd56e8\",\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\":\"c638ad11c8a027ab64dc\",\"lib_index_js\":\"e3c375749eca37176102\",\"style_index_js\":\"8d65101c7953569e67b2\",\"vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js\":\"339ba20fba041bb86e74\",\"node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0\":\"e5e08421993e8b0d6940\",\"vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js\":\"63a1ec84812da57c0fc4\",\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\":\"2532571945c143a4fd75\",\"webpack_sharing_consume_default_emotion_react_emotion_react-_1cec\":\"42a10740f3031f0ec641\",\"vendors-node_modules_projectstorm_react-canvas-core_dist_index_js\":\"fedff644cad1098d8bcb\",\"vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js\":\"7dc9f640385f857c0d8d\",\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\":\"0d77f52057fa78293be3\",\"webpack_sharing_consume_default_emotion_react_emotion_react-webpack_sharing_consume_default_e-2f734f\":\"9563dc6d7211dc99b182\",\"vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js\":\"274da3f6f09bc30ae8a5\",\"webpack_sharing_consume_default_projectstorm_react-diagrams-defaults_projectstorm_react-diagr-28113e\":\"2060371fe5102686c3c9\",\"webpack_sharing_consume_default_dagre_dagre-webpack_sharing_consume_default_pathfinding_pathfinding\":\"852c66b9d6def7f7f01e\",\"webpack_sharing_consume_default_projectstorm_react-diagrams-routing_projectstorm_react-diagra-ba726c\":\"05faed0a2b3f78808c42\",\"node_modules_projectstorm_react-diagrams_dist_index_js-_718a0\":\"20f9ad52b47a17ffea59\",\"vendors-node_modules_dagre_index_js\":\"bb0a10362365f9062b66\",\"node_modules_krc-pagination_lib_index_js-_9b3c0\":\"a1fe7d758d8bfd1fcb6d\",\"vendors-node_modules_marked_lib_marked_esm_js\":\"f8b1654d24f4d8a9ebb1\",\"vendors-node_modules_pathfinding_index_js\":\"57d527803f5ef363858c\",\"vendors-node_modules_react-accessible-accordion_dist_es_index_js\":\"e27e21540f362d2400f1\",\"vendors-node_modules_react-image-gallery_build_image-gallery_js\":\"54c6b2ee4f593bcd3578\",\"vendors-node_modules_prop-types_index_js\":\"ecaf55d6e3a49828fd03\",\"vendors-node_modules_react-numeric-input_index_js\":\"7e201324b89725af60a3\",\"vendors-node_modules_react-portal-tooltip_lib_index_js\":\"13053d183ec1bf6fe8b1\",\"webpack_sharing_consume_default_react-dom\":\"671382a00e45b65a6bb6\",\"vendors-node_modules_react-switch_index_js\":\"a2a55561dfbed639ad75\",\"node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910\":\"14aefefbf127229080e9\",\"vendors-node_modules_react-toggle_dist_component_index_js\":\"e801abe36cc813fe2470\",\"vendors-node_modules_react-tooltip_dist_index_es_js\":\"917868bea13b4ea0b7c0\",\"node_modules_projectstorm_react-diagrams_dist_index_js-_718a1\":\"2b02758ec1fa9eb3a339\",\"node_modules_krc-pagination_lib_index_js-_9b3c1\":\"4158a663778b2cc4558a\",\"node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911\":\"b80b22a56a58ba2f0de3\",\"node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1\":\"69771b4348e185a22e47\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"xircuits:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.nmd = (module) => {\n\tmodule.paths = [];\n\tif (!module.children) module.children = [];\n\treturn module;\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"xircuits\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@emotion/react\", \"11.7.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@emotion/react/dist/emotion-react.browser.esm.js */ \"./node_modules/@emotion/react/dist/emotion-react.browser.esm.js\"))))));\n\t\t\tregister(\"@emotion/styled\", \"11.6.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_1cec\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@emotion/styled/dist/emotion-styled.browser.esm.js */ \"./node_modules/@emotion/styled/dist/emotion-styled.browser.esm.js\"))))));\n\t\t\tregister(\"@projectstorm/react-canvas-core\", \"6.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-canvas-core_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@projectstorm/react-canvas-core/dist/index.js */ \"./node_modules/@projectstorm/react-canvas-core/dist/index.js\"))))));\n\t\t\tregister(\"@projectstorm/react-diagrams-defaults\", \"6.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-webpack_sharing_consume_default_e-2f734f\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@projectstorm/react-diagrams-defaults/dist/index.js */ \"./node_modules/@projectstorm/react-diagrams-defaults/dist/index.js\"))))));\n\t\t\tregister(\"@projectstorm/react-diagrams-routing\", \"6.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-diagrams-defaults_projectstorm_react-diagr-28113e\"), __webpack_require__.e(\"webpack_sharing_consume_default_dagre_dagre-webpack_sharing_consume_default_pathfinding_pathfinding\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@projectstorm/react-diagrams-routing/dist/index.js */ \"./node_modules/@projectstorm/react-diagrams-routing/dist/index.js\"))))));\n\t\t\tregister(\"@projectstorm/react-diagrams\", \"6.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-diagrams-defaults_projectstorm_react-diagr-28113e\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-diagrams-routing_projectstorm_react-diagra-ba726c\"), __webpack_require__.e(\"node_modules_projectstorm_react-diagrams_dist_index_js-_718a0\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@projectstorm/react-diagrams/dist/index.js */ \"./node_modules/@projectstorm/react-diagrams/dist/index.js\"))))));\n\t\t\tregister(\"dagre\", \"0.8.5\", () => (__webpack_require__.e(\"vendors-node_modules_dagre_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/dagre/index.js */ \"./node_modules/dagre/index.js\"))))));\n\t\t\tregister(\"krc-pagination\", \"1.0.1\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"node_modules_krc-pagination_lib_index_js-_9b3c0\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/krc-pagination/lib/index.js */ \"./node_modules/krc-pagination/lib/index.js\"))))));\n\t\t\tregister(\"marked\", \"4.0.18\", () => (__webpack_require__.e(\"vendors-node_modules_marked_lib_marked_esm_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/marked/lib/marked.esm.js */ \"./node_modules/marked/lib/marked.esm.js\"))))));\n\t\t\tregister(\"pathfinding\", \"0.4.18\", () => (__webpack_require__.e(\"vendors-node_modules_pathfinding_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/pathfinding/index.js */ \"./node_modules/pathfinding/index.js\"))))));\n\t\t\tregister(\"react-accessible-accordion\", \"4.0.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_react-accessible-accordion_dist_es_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-accessible-accordion/dist/es/index.js */ \"./node_modules/react-accessible-accordion/dist/es/index.js\"))))));\n\t\t\tregister(\"react-image-gallery\", \"1.2.7\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_react-image-gallery_build_image-gallery_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-image-gallery/build/image-gallery.js */ \"./node_modules/react-image-gallery/build/image-gallery.js\"))))));\n\t\t\tregister(\"react-numeric-input\", \"2.2.3\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-numeric-input_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-numeric-input/index.js */ \"./node_modules/react-numeric-input/index.js\"))))));\n\t\t\tregister(\"react-portal-tooltip\", \"2.4.7\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-portal-tooltip_lib_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_react-dom\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-portal-tooltip/lib/index.js */ \"./node_modules/react-portal-tooltip/lib/index.js\"))))));\n\t\t\tregister(\"react-switch\", \"6.0.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-switch_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-switch/index.js */ \"./node_modules/react-switch/index.js\"))))));\n\t\t\tregister(\"react-textarea-autosize\", \"8.3.3\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-textarea-autosize/dist/react-textarea-autosize.browser.esm.js */ \"./node_modules/react-textarea-autosize/dist/react-textarea-autosize.browser.esm.js\"))))));\n\t\t\tregister(\"react-toggle\", \"4.1.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-toggle_dist_component_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-toggle/dist/component/index.js */ \"./node_modules/react-toggle/dist/component/index.js\"))))));\n\t\t\tregister(\"react-tooltip\", \"4.2.21\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-tooltip_dist_index_es_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-tooltip/dist/index.es.js */ \"./node_modules/react-tooltip/dist/index.es.js\"))))));\n\t\t\tregister(\"xircuits\", \"1.8.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"xircuits\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@emotion/react\", \"11.7.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b0\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@emotion/react/dist/emotion-react.browser.esm.js */ \"./node_modules/@emotion/react/dist/emotion-react.browser.esm.js\"))))));\n\t\t\tregister(\"@emotion/styled\", \"11.6.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_1cec\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@emotion/styled/dist/emotion-styled.browser.esm.js */ \"./node_modules/@emotion/styled/dist/emotion-styled.browser.esm.js\"))))));\n\t\t\tregister(\"@projectstorm/react-canvas-core\", \"6.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-canvas-core_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@projectstorm/react-canvas-core/dist/index.js */ \"./node_modules/@projectstorm/react-canvas-core/dist/index.js\"))))));\n\t\t\tregister(\"@projectstorm/react-diagrams-defaults\", \"6.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-webpack_sharing_consume_default_e-2f734f\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@projectstorm/react-diagrams-defaults/dist/index.js */ \"./node_modules/@projectstorm/react-diagrams-defaults/dist/index.js\"))))));\n\t\t\tregister(\"@projectstorm/react-diagrams-routing\", \"6.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-diagrams-defaults_projectstorm_react-diagr-28113e\"), __webpack_require__.e(\"webpack_sharing_consume_default_dagre_dagre-webpack_sharing_consume_default_pathfinding_pathfinding\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@projectstorm/react-diagrams-routing/dist/index.js */ \"./node_modules/@projectstorm/react-diagrams-routing/dist/index.js\"))))));\n\t\t\tregister(\"@projectstorm/react-diagrams\", \"6.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-diagrams-defaults_projectstorm_react-diagr-28113e\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-diagrams-routing_projectstorm_react-diagra-ba726c\"), __webpack_require__.e(\"node_modules_projectstorm_react-diagrams_dist_index_js-_718a0\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@projectstorm/react-diagrams/dist/index.js */ \"./node_modules/@projectstorm/react-diagrams/dist/index.js\"))))));\n\t\t\tregister(\"dagre\", \"0.8.5\", () => (__webpack_require__.e(\"vendors-node_modules_dagre_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/dagre/index.js */ \"./node_modules/dagre/index.js\"))))));\n\t\t\tregister(\"krc-pagination\", \"1.0.1\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"node_modules_krc-pagination_lib_index_js-_9b3c0\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/krc-pagination/lib/index.js */ \"./node_modules/krc-pagination/lib/index.js\"))))));\n\t\t\tregister(\"marked\", \"4.0.18\", () => (__webpack_require__.e(\"vendors-node_modules_marked_lib_marked_esm_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/marked/lib/marked.esm.js */ \"./node_modules/marked/lib/marked.esm.js\"))))));\n\t\t\tregister(\"pathfinding\", \"0.4.18\", () => (__webpack_require__.e(\"vendors-node_modules_pathfinding_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/pathfinding/index.js */ \"./node_modules/pathfinding/index.js\"))))));\n\t\t\tregister(\"react-accessible-accordion\", \"4.0.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_react-accessible-accordion_dist_es_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-accessible-accordion/dist/es/index.js */ \"./node_modules/react-accessible-accordion/dist/es/index.js\"))))));\n\t\t\tregister(\"react-image-gallery\", \"1.2.7\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_react-image-gallery_build_image-gallery_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-image-gallery/build/image-gallery.js */ \"./node_modules/react-image-gallery/build/image-gallery.js\"))))));\n\t\t\tregister(\"react-numeric-input\", \"2.2.3\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-numeric-input_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-numeric-input/index.js */ \"./node_modules/react-numeric-input/index.js\"))))));\n\t\t\tregister(\"react-portal-tooltip\", \"2.4.7\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-portal-tooltip_lib_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_react-dom\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-portal-tooltip/lib/index.js */ \"./node_modules/react-portal-tooltip/lib/index.js\"))))));\n\t\t\tregister(\"react-switch\", \"6.0.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-switch_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-switch/index.js */ \"./node_modules/react-switch/index.js\"))))));\n\t\t\tregister(\"react-textarea-autosize\", \"8.3.3\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-textarea-autosize/dist/react-textarea-autosize.browser.esm.js */ \"./node_modules/react-textarea-autosize/dist/react-textarea-autosize.browser.esm.js\"))))));\n\t\t\tregister(\"react-toggle\", \"4.1.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-toggle_dist_component_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-toggle/dist/component/index.js */ \"./node_modules/react-toggle/dist/component/index.js\"))))));\n\t\t\tregister(\"react-tooltip\", \"4.2.21\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-tooltip_dist_index_es_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/react-tooltip/dist/index.es.js */ \"./node_modules/react-tooltip/dist/index.es.js\"))))));\n\t\t\tregister(\"xircuits\", \"1.8.3\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_geometry_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js\"), __webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_styled_emotion_styled\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@emotion/styled/@emotion/styled?ffb9\": () => (loadFallback(\"default\", \"@emotion/styled\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_1cec\")]).then(() => (() => (__webpack_require__(/*! @emotion/styled */ \"./node_modules/@emotion/styled/dist/emotion-styled.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@projectstorm/react-canvas-core/@projectstorm/react-canvas-core?4a30\": () => (loadStrictVersionCheckFallback(\"default\", \"@projectstorm/react-canvas-core\", [1,6,6,1], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_react-canvas-core_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\")]).then(() => (() => (__webpack_require__(/*! @projectstorm/react-canvas-core */ \"./node_modules/@projectstorm/react-canvas-core/dist/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/docmanager\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/translation\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/translation\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/rendermime\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\": () => (loadVersionCheck(\"default\", \"@jupyterlab/docregistry\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@projectstorm/react-diagrams/@projectstorm/react-diagrams\": () => (loadStrictVersionCheckFallback(\"default\", \"@projectstorm/react-diagrams\", [1,6,6,1], () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-diagrams-defaults_projectstorm_react-diagr-28113e\"), __webpack_require__.e(\"webpack_sharing_consume_default_projectstorm_react-diagrams-routing_projectstorm_react-diagra-ba726c\"), __webpack_require__.e(\"node_modules_projectstorm_react-diagrams_dist_index_js-_718a1\")]).then(() => (() => (__webpack_require__(/*! @projectstorm/react-diagrams */ \"./node_modules/@projectstorm/react-diagrams/dist/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@emotion/styled/@emotion/styled?2715\": () => (loadStrictVersionCheckFallback(\"default\", \"@emotion/styled\", [1,11,3,0], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_1cec\")]).then(() => (() => (__webpack_require__(/*! @emotion/styled */ \"./node_modules/@emotion/styled/dist/emotion-styled.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/react-image-gallery/react-image-gallery\": () => (loadStrictVersionCheckFallback(\"default\", \"react-image-gallery\", [1,1,2,7], () => (__webpack_require__.e(\"vendors-node_modules_react-image-gallery_build_image-gallery_js\").then(() => (() => (__webpack_require__(/*! react-image-gallery */ \"./node_modules/react-image-gallery/build/image-gallery.js\"))))))),\n\t\"webpack/sharing/consume/default/react-portal-tooltip/react-portal-tooltip\": () => (loadStrictVersionCheckFallback(\"default\", \"react-portal-tooltip\", [1,2,4,7], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-portal-tooltip_lib_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react-dom\")]).then(() => (() => (__webpack_require__(/*! react-portal-tooltip */ \"./node_modules/react-portal-tooltip/lib/index.js\"))))))),\n\t\"webpack/sharing/consume/default/krc-pagination/krc-pagination\": () => (loadStrictVersionCheckFallback(\"default\", \"krc-pagination\", [1,1,0,1], () => (__webpack_require__.e(\"node_modules_krc-pagination_lib_index_js-_9b3c1\").then(() => (() => (__webpack_require__(/*! krc-pagination */ \"./node_modules/krc-pagination/lib/index.js\"))))))),\n\t\"webpack/sharing/consume/default/react-toggle/react-toggle\": () => (loadStrictVersionCheckFallback(\"default\", \"react-toggle\", [1,4,1,2], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-toggle_dist_component_index_js\")]).then(() => (() => (__webpack_require__(/*! react-toggle */ \"./node_modules/react-toggle/dist/component/index.js\"))))))),\n\t\"webpack/sharing/consume/default/react-tooltip/react-tooltip\": () => (loadStrictVersionCheckFallback(\"default\", \"react-tooltip\", [1,4,2,21], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-tooltip_dist_index_es_js\")]).then(() => (() => (__webpack_require__(/*! react-tooltip */ \"./node_modules/react-tooltip/dist/index.es.js\"))))))),\n\t\"webpack/sharing/consume/default/marked/marked\": () => (loadStrictVersionCheckFallback(\"default\", \"marked\", [1,4,0,18], () => (__webpack_require__.e(\"vendors-node_modules_marked_lib_marked_esm_js\").then(() => (() => (__webpack_require__(/*! marked */ \"./node_modules/marked/lib/marked.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@lumino/messaging\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/messaging\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,37,2])),\n\t\"webpack/sharing/consume/default/react-textarea-autosize/react-textarea-autosize\": () => (loadStrictVersionCheckFallback(\"default\", \"react-textarea-autosize\", [1,8,3,3], () => (__webpack_require__.e(\"node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911\").then(() => (() => (__webpack_require__(/*! react-textarea-autosize */ \"./node_modules/react-textarea-autosize/dist/react-textarea-autosize.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/logconsole\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/logconsole\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,6,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,6,4])),\n\t\"webpack/sharing/consume/default/react-numeric-input/react-numeric-input\": () => (loadStrictVersionCheckFallback(\"default\", \"react-numeric-input\", [1,2,2,3], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-numeric-input_index_js\")]).then(() => (() => (__webpack_require__(/*! react-numeric-input */ \"./node_modules/react-numeric-input/index.js\"))))))),\n\t\"webpack/sharing/consume/default/react-switch/react-switch\": () => (loadStrictVersionCheckFallback(\"default\", \"react-switch\", [1,6,0,0], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_prop-types_index_js\"), __webpack_require__.e(\"vendors-node_modules_react-switch_index_js\")]).then(() => (() => (__webpack_require__(/*! react-switch */ \"./node_modules/react-switch/index.js\"))))))),\n\t\"webpack/sharing/consume/default/react-accessible-accordion/react-accessible-accordion\": () => (loadStrictVersionCheckFallback(\"default\", \"react-accessible-accordion\", [1,4,0,0], () => (__webpack_require__.e(\"vendors-node_modules_react-accessible-accordion_dist_es_index_js\").then(() => (() => (__webpack_require__(/*! react-accessible-accordion */ \"./node_modules/react-accessible-accordion/dist/es/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@emotion/react/@emotion/react?9405\": () => (loadStrictVersionCheckFallback(\"default\", \"@emotion/react\", [1,11,4,1], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js\"), __webpack_require__.e(\"node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1\")]).then(() => (() => (__webpack_require__(/*! @emotion/react */ \"./node_modules/@emotion/react/dist/emotion-react.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/outputarea\": () => (loadVersionCheck(\"default\", \"@jupyterlab/outputarea\", [1,3,6,4])),\n\t\"webpack/sharing/consume/default/@emotion/react/@emotion/react?8f22\": () => (loadFallback(\"default\", \"@emotion/react\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js\"), __webpack_require__.e(\"node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1\")]).then(() => (() => (__webpack_require__(/*! @emotion/react */ \"./node_modules/@emotion/react/dist/emotion-react.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@emotion/react/@emotion/react?1cec\": () => (loadStrictVersionCheckFallback(\"default\", \"@emotion/react\", [1,11,0,0,,\"rc\",0], () => (__webpack_require__.e(\"vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js\").then(() => (() => (__webpack_require__(/*! @emotion/react */ \"./node_modules/@emotion/react/dist/emotion-react.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@projectstorm/react-canvas-core/@projectstorm/react-canvas-core?4cd6\": () => (loadFallback(\"default\", \"@projectstorm/react-canvas-core\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_react-canvas-core_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\")]).then(() => (() => (__webpack_require__(/*! @projectstorm/react-canvas-core */ \"./node_modules/@projectstorm/react-canvas-core/dist/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@emotion/styled/@emotion/styled?c8aa\": () => (loadStrictVersionCheckFallback(\"default\", \"@emotion/styled\", [1,11], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-_1cec\")]).then(() => (() => (__webpack_require__(/*! @emotion/styled */ \"./node_modules/@emotion/styled/dist/emotion-styled.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@emotion/react/@emotion/react?6062\": () => (loadStrictVersionCheckFallback(\"default\", \"@emotion/react\", [1,11], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js\"), __webpack_require__.e(\"node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_hash_dist_hash_browser-6cd86b1\")]).then(() => (() => (__webpack_require__(/*! @emotion/react */ \"./node_modules/@emotion/react/dist/emotion-react.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@projectstorm/react-diagrams-defaults/@projectstorm/react-diagrams-defaults\": () => (loadStrictVersionCheckFallback(\"default\", \"@projectstorm/react-diagrams-defaults\", [1,6,6,1], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_emotion_react_emotion_react-webpack_sharing_consume_default_e-2f734f\")]).then(() => (() => (__webpack_require__(/*! @projectstorm/react-diagrams-defaults */ \"./node_modules/@projectstorm/react-diagrams-defaults/dist/index.js\"))))))),\n\t\"webpack/sharing/consume/default/pathfinding/pathfinding\": () => (loadStrictVersionCheckFallback(\"default\", \"pathfinding\", [2,0,4,18], () => (__webpack_require__.e(\"vendors-node_modules_pathfinding_index_js\").then(() => (() => (__webpack_require__(/*! pathfinding */ \"./node_modules/pathfinding/index.js\"))))))),\n\t\"webpack/sharing/consume/default/dagre/dagre\": () => (loadStrictVersionCheckFallback(\"default\", \"dagre\", [2,0,8,5], () => (__webpack_require__.e(\"vendors-node_modules_dagre_index_js\").then(() => (() => (__webpack_require__(/*! dagre */ \"./node_modules/dagre/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@projectstorm/react-diagrams-routing/@projectstorm/react-diagrams-routing\": () => (loadStrictVersionCheckFallback(\"default\", \"@projectstorm/react-diagrams-routing\", [1,6,6,1], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_dagre_dagre-webpack_sharing_consume_default_pathfinding_pathfinding\")]).then(() => (() => (__webpack_require__(/*! @projectstorm/react-diagrams-routing */ \"./node_modules/@projectstorm/react-diagrams-routing/dist/index.js\"))))))),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,17,0,1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\"\n\t],\n\t\"webpack_sharing_consume_default_emotion_styled_emotion_styled\": [\n\t\t\"webpack/sharing/consume/default/@emotion/styled/@emotion/styled?ffb9\"\n\t],\n\t\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4a30\": [\n\t\t\"webpack/sharing/consume/default/@projectstorm/react-canvas-core/@projectstorm/react-canvas-core?4a30\"\n\t],\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/translation\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@projectstorm/react-diagrams/@projectstorm/react-diagrams\",\n\t\t\"webpack/sharing/consume/default/@emotion/styled/@emotion/styled?2715\",\n\t\t\"webpack/sharing/consume/default/react-image-gallery/react-image-gallery\",\n\t\t\"webpack/sharing/consume/default/react-portal-tooltip/react-portal-tooltip\",\n\t\t\"webpack/sharing/consume/default/krc-pagination/krc-pagination\",\n\t\t\"webpack/sharing/consume/default/react-toggle/react-toggle\",\n\t\t\"webpack/sharing/consume/default/react-tooltip/react-tooltip\",\n\t\t\"webpack/sharing/consume/default/marked/marked\",\n\t\t\"webpack/sharing/consume/default/@lumino/messaging\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/react-textarea-autosize/react-textarea-autosize\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/logconsole\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react-numeric-input/react-numeric-input\",\n\t\t\"webpack/sharing/consume/default/react-switch/react-switch\",\n\t\t\"webpack/sharing/consume/default/react-accessible-accordion/react-accessible-accordion\",\n\t\t\"webpack/sharing/consume/default/@emotion/react/@emotion/react?9405\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/outputarea\"\n\t],\n\t\"webpack_sharing_consume_default_emotion_react_emotion_react-_8f22\": [\n\t\t\"webpack/sharing/consume/default/@emotion/react/@emotion/react?8f22\"\n\t],\n\t\"webpack_sharing_consume_default_emotion_react_emotion_react-_1cec\": [\n\t\t\"webpack/sharing/consume/default/@emotion/react/@emotion/react?1cec\"\n\t],\n\t\"webpack_sharing_consume_default_projectstorm_react-canvas-core_projectstorm_react-canvas-core-_4cd6\": [\n\t\t\"webpack/sharing/consume/default/@projectstorm/react-canvas-core/@projectstorm/react-canvas-core?4cd6\"\n\t],\n\t\"webpack_sharing_consume_default_emotion_react_emotion_react-webpack_sharing_consume_default_e-2f734f\": [\n\t\t\"webpack/sharing/consume/default/@emotion/styled/@emotion/styled?c8aa\",\n\t\t\"webpack/sharing/consume/default/@emotion/react/@emotion/react?6062\"\n\t],\n\t\"webpack_sharing_consume_default_projectstorm_react-diagrams-defaults_projectstorm_react-diagr-28113e\": [\n\t\t\"webpack/sharing/consume/default/@projectstorm/react-diagrams-defaults/@projectstorm/react-diagrams-defaults\"\n\t],\n\t\"webpack_sharing_consume_default_dagre_dagre-webpack_sharing_consume_default_pathfinding_pathfinding\": [\n\t\t\"webpack/sharing/consume/default/pathfinding/pathfinding\",\n\t\t\"webpack/sharing/consume/default/dagre/dagre\"\n\t],\n\t\"webpack_sharing_consume_default_projectstorm_react-diagrams-routing_projectstorm_react-diagra-ba726c\": [\n\t\t\"webpack/sharing/consume/default/@projectstorm/react-diagrams-routing/@projectstorm/react-diagrams-routing\"\n\t],\n\t\"webpack_sharing_consume_default_react-dom\": [\n\t\t\"webpack/sharing/consume/default/react-dom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"xircuits\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(!/^webpack_sharing_consume_default_(emotion_(react_emotion_react\\-(_1cec|_8f22|webpack_sharing_consume_default_e\\-2f734f)|styled_emotion_styled)|projectstorm_react\\-(canvas\\-core_projectstorm_react\\-canvas\\-core\\-_4(a30|cd6)|diagrams\\-(defaults_projectstorm_react\\-diagr\\-28113e|routing_projectstorm_react\\-diagra\\-ba726c))|react(|\\-dom)|dagre_dagre\\-webpack_sharing_consume_default_pathfinding_pathfinding)$/.test(chunkId)) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkxircuits\"] = self[\"webpackChunkxircuits\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/xircuits\");\n",
         ""
```

### Comparing `xircuits-1.8.2/xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js` & `xircuits-1.8.3/xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js.map` & `xircuits-1.8.3/xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.339ba20fba041bb86e74.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.339ba20fba041bb86e74.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.339ba20fba041bb86e74.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.339ba20fba041bb86e74.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.63a1ec84812da57c0fc4.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.63a1ec84812da57c0fc4.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.63a1ec84812da57c0fc4.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.63a1ec84812da57c0fc4.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7.6237bb7955064b6be43a.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7.6237bb7955064b6be43a.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7.6237bb7955064b6be43a.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_krc-pagination_styles_css-node_modules_rc-dialog_assets_bootstrap_css-no-49e9b7.6237bb7955064b6be43a.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_marked_lib_marked_esm_js.f8b1654d24f4d8a9ebb1.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_marked_lib_marked_esm_js.f8b1654d24f4d8a9ebb1.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_marked_lib_marked_esm_js.f8b1654d24f4d8a9ebb1.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_marked_lib_marked_esm_js.f8b1654d24f4d8a9ebb1.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_pathfinding_index_js.57d527803f5ef363858c.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_pathfinding_index_js.57d527803f5ef363858c.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_pathfinding_index_js.57d527803f5ef363858c.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_pathfinding_index_js.57d527803f5ef363858c.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_geometry_dist_index_js.6d56ef20c085cca0afc6.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_geometry_dist_index_js.6d56ef20c085cca0afc6.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_geometry_dist_index_js.6d56ef20c085cca0afc6.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_geometry_dist_index_js.6d56ef20c085cca0afc6.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-canvas-core_dist_index_js.fedff644cad1098d8bcb.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-canvas-core_dist_index_js.fedff644cad1098d8bcb.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-canvas-core_dist_index_js.fedff644cad1098d8bcb.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-canvas-core_dist_index_js.fedff644cad1098d8bcb.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js.23c3c2a475ea57fe7938.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js.23c3c2a475ea57fe7938.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js.23c3c2a475ea57fe7938.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-core_dist_index_js.23c3c2a475ea57fe7938.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js.7dc9f640385f857c0d8d.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js.7dc9f640385f857c0d8d.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js.7dc9f640385f857c0d8d.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-defaults_dist_index_js.7dc9f640385f857c0d8d.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js.274da3f6f09bc30ae8a5.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js.274da3f6f09bc30ae8a5.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js.274da3f6f09bc30ae8a5.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_projectstorm_react-diagrams-routing_dist_index_js.274da3f6f09bc30ae8a5.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_prop-types_index_js.ecaf55d6e3a49828fd03.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_prop-types_index_js.ecaf55d6e3a49828fd03.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_prop-types_index_js.ecaf55d6e3a49828fd03.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_prop-types_index_js.ecaf55d6e3a49828fd03.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-accessible-accordion_dist_es_index_js.e27e21540f362d2400f1.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-accessible-accordion_dist_es_index_js.e27e21540f362d2400f1.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-accessible-accordion_dist_es_index_js.e27e21540f362d2400f1.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-accessible-accordion_dist_es_index_js.e27e21540f362d2400f1.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-image-gallery_build_image-gallery_js.54c6b2ee4f593bcd3578.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-image-gallery_build_image-gallery_js.54c6b2ee4f593bcd3578.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-image-gallery_build_image-gallery_js.54c6b2ee4f593bcd3578.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-image-gallery_build_image-gallery_js.54c6b2ee4f593bcd3578.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-numeric-input_index_js.7e201324b89725af60a3.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-numeric-input_index_js.7e201324b89725af60a3.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-numeric-input_index_js.7e201324b89725af60a3.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-numeric-input_index_js.7e201324b89725af60a3.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-portal-tooltip_lib_index_js.13053d183ec1bf6fe8b1.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-portal-tooltip_lib_index_js.13053d183ec1bf6fe8b1.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-portal-tooltip_lib_index_js.13053d183ec1bf6fe8b1.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-portal-tooltip_lib_index_js.13053d183ec1bf6fe8b1.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-switch_index_js.a2a55561dfbed639ad75.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-switch_index_js.a2a55561dfbed639ad75.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-switch_index_js.a2a55561dfbed639ad75.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-switch_index_js.a2a55561dfbed639ad75.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-toggle_dist_component_index_js.e801abe36cc813fe2470.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-toggle_dist_component_index_js.e801abe36cc813fe2470.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-toggle_dist_component_index_js.e801abe36cc813fe2470.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-toggle_dist_component_index_js.e801abe36cc813fe2470.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-tooltip_dist_index_es_js.917868bea13b4ea0b7c0.js` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-tooltip_dist_index_es_js.917868bea13b4ea0b7c0.js`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/labextension/static/vendors-node_modules_react-tooltip_dist_index_es_js.917868bea13b4ea0b7c0.js.map` & `xircuits-1.8.3/xircuits/labextension/static/vendors-node_modules_react-tooltip_dist_index_es_js.917868bea13b4ea0b7c0.js.map`

 * *Files identical despite different names*

### Comparing `xircuits-1.8.2/xircuits/start_xircuits.py` & `xircuits-1.8.3/xircuits/start_xircuits.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # coding: utf-8
 """A wrapper to start xircuits and offer to start to XAI-components"""
 
 from pathlib import Path
-from urllib import request
 import os
 import argparse
 import pkg_resources
 import shutil
 from .handlers.request_folder import request_folder
 from .handlers.request_submodule import get_submodule_config, request_submodule_library
+import subprocess
+import sys
 
 def init_xircuits():
 
     package_name = 'xircuits'
     copy_from_installed_wheel(package_name, 
                               resource='.xircuits', 
                               dest_path='.xircuits')
@@ -64,16 +65,15 @@
     args = parser.parse_args()
     request_submodule_library(args.submodule_library)
 
     if not args.no_install:
         submodule_path, _ = get_submodule_config(args.submodule_library)
 
         print("Installing " + args.submodule_library + "...")
-        install_cmd = "cmd /c pip install -r " + submodule_path + "/requirements.txt"
-        os.system(install_cmd)
+        subprocess.run([sys.executable, "-m", "pip", "install", "-r",  submodule_path + "/requirements.txt"], check=True)
 
 def main():
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--branch', nargs='?', help='pull files from a xircuits branch')
 
     parsed, extra_args = parser.parse_known_args()
```

### Comparing `xircuits-1.8.2/xircuits.egg-info/PKG-INFO` & `xircuits-1.8.3/xircuits.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xircuits
-Version: 1.8.2
+Version: 1.8.3
 Summary: A JupyterLab extension for rendering and editing xircuit files.
 Home-page: https://github.com/XpressAI/xircuits
 Author: Xpress AI
 Author-email: eduardo@xpress.ai
 License: Apache-2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -19,18 +19,20 @@
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: spark
+Provides-Extra: template
 Provides-Extra: tensorflow_keras
 Provides-Extra: pytorch
-Provides-Extra: template
+Provides-Extra: sklearn
+Provides-Extra: xgboost
+Provides-Extra: spark
 Provides-Extra: full
 License-File: LICENSE
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/68586800/151280601-7ff2b7b2-10e5-4544-b3df-aa6a5a654dae.png" width="450"/>
 </p>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: xircuits Version: 1.8.2 Summary: A JupyterLab
+Metadata-Version: 2.1 Name: xircuits Version: 1.8.3 Summary: A JupyterLab
 extension for rendering and editing xircuit files. Home-page: https://
 github.com/XpressAI/xircuits Author: Xpress AI Author-email: eduardo@xpress.ai
 License: Apache-2.0 Keywords: Jupyter,JupyterLab,JupyterLab3 Platform: Linux
 Platform: Mac OS X Platform: Windows Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab Classifier: Framework :: Jupyter
 :: JupyterLab :: 3 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-spark Provides-Extra: tensorflow_keras Provides-Extra: pytorch Provides-Extra:
-template Provides-Extra: full License-File: LICENSE
+template Provides-Extra: tensorflow_keras Provides-Extra: pytorch Provides-
+Extra: sklearn Provides-Extra: xgboost Provides-Extra: spark Provides-Extra:
+full License-File: LICENSE
  [https://user-images.githubusercontent.com/68586800/151280601-7ff2b7b2-10e5-
                           4544-b3df-aa6a5a654dae.png]
 Docs â¢ Install â¢ Tutorials â¢ Developer_Guides â¢ Contribute â¢ Blog â¢
                                    Discord
                    Component_Libraries â¢ Project_Templates
               [GitHub] [GitHub_release] [Documentation] [Python]
 ![xircuits-frontpage](https://user-images.githubusercontent.com/68586800/
```

### Comparing `xircuits-1.8.2/xircuits.egg-info/SOURCES.txt` & `xircuits-1.8.3/xircuits.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -90,14 +90,18 @@
 xai_components/readme.md
 xai_components/xai_controlflow/__init__.py
 xai_components/xai_controlflow/branches.py
 xai_components/xai_pytorch/__init__.py
 xai_components/xai_pytorch/quickstart.py
 xai_components/xai_pytorch/requirements.txt
 xai_components/xai_pytorch/torch_nn_layers.py
+xai_components/xai_sklearn/__init__.py
+xai_components/xai_sklearn/readme.md
+xai_components/xai_sklearn/requirements.txt
+xai_components/xai_sklearn/sklearn_components.py
 xai_components/xai_spark/__init__.py
 xai_components/xai_spark/pyspark_core.py
 xai_components/xai_spark/pyspark_mllib.py
 xai_components/xai_spark/readme.md
 xai_components/xai_spark/requirements.txt
 xai_components/xai_template/__init__.py
 xai_components/xai_template/example_components.py
@@ -106,14 +110,19 @@
 xai_components/xai_tensorflow_keras/__init__.py
 xai_components/xai_tensorflow_keras/keras_transfer_learning.py
 xai_components/xai_tensorflow_keras/requirements.txt
 xai_components/xai_tensorflow_keras/tf_keras.py
 xai_components/xai_tensorflow_keras/training.py
 xai_components/xai_utils/__init__.py
 xai_components/xai_utils/utils.py
+xai_components/xai_xgboost/__init__.py
+xai_components/xai_xgboost/readme.md
+xai_components/xai_xgboost/requirements.txt
+xai_components/xai_xgboost/xgboost_components.py
+xai_components/xai_xgboost/examples/XGBoostClassifier.xircuits
 xircuits/__init__.py
 xircuits/_version.py
 xircuits/start_xircuits.py
 xircuits.egg-info/PKG-INFO
 xircuits.egg-info/SOURCES.txt
 xircuits.egg-info/dependency_links.txt
 xircuits.egg-info/entry_points.txt
@@ -155,16 +164,16 @@
 xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a0.20f9ad52b47a17ffea59.js.map
 xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js
 xircuits/labextension/static/node_modules_projectstorm_react-diagrams_dist_index_js-_718a1.2b02758ec1fa9eb3a339.js.map
 xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js
 xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d910.14aefefbf127229080e9.js.map
 xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js
 xircuits/labextension/static/node_modules_react-textarea-autosize_dist_react-textarea-autosize_browser_esm_js-_7d911.b80b22a56a58ba2f0de3.js.map
-xircuits/labextension/static/remoteEntry.3aab60af2c2340b392f7.js
-xircuits/labextension/static/remoteEntry.3aab60af2c2340b392f7.js.map
+xircuits/labextension/static/remoteEntry.e8c33c4dca473d62d6b4.js
+xircuits/labextension/static/remoteEntry.e8c33c4dca473d62d6b4.js.map
 xircuits/labextension/static/style.js
 xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js
 xircuits/labextension/static/style_index_js.8d65101c7953569e67b2.js.map
 xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js
 xircuits/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.60f4ca1c03a44b1a935c.js.map
 xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js
 xircuits/labextension/static/vendors-node_modules_dagre_index_js.bb0a10362365f9062b66.js.map
```

