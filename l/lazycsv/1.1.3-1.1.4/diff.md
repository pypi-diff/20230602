# Comparing `tmp/lazycsv-1.1.3.tar.gz` & `tmp/lazycsv-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycsv-1.1.3.tar", last modified: Wed May 10 14:34:35 2023, max compression
+gzip compressed data, was "lazycsv-1.1.4.tar", last modified: Fri Jun  2 20:32:32 2023, max compression
```

## Comparing `lazycsv-1.1.3.tar` & `lazycsv-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/
--rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.3/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     9944 2023-05-10 14:34:35.581540 lazycsv-1.1.3/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     8893 2023-05-10 14:32:51.000000 lazycsv-1.1.3/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-10 14:34:35.581540 lazycsv-1.1.3/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2400 2023-05-10 14:34:21.000000 lazycsv-1.1.3/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/src/lazycsv/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.3/src/lazycsv/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    39709 2023-05-10 14:16:18.000000 lazycsv-1.1.3/src/lazycsv/lazycsv.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/src/lazycsv.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     9944 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       66 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    24486 2023-05-10 14:24:35.000000 lazycsv-1.1.3/tests/test_lazycsv.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-02 20:32:32.671516 lazycsv-1.1.4/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.4/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     9944 2023-06-02 20:32:32.668182 lazycsv-1.1.4/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     8893 2023-05-10 14:32:51.000000 lazycsv-1.1.4/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-02 20:32:32.671516 lazycsv-1.1.4/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2400 2023-06-02 19:44:06.000000 lazycsv-1.1.4/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-02 20:32:32.668182 lazycsv-1.1.4/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-02 20:32:32.668182 lazycsv-1.1.4/src/lazycsv/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.4/src/lazycsv/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    39919 2023-06-02 20:30:25.000000 lazycsv-1.1.4/src/lazycsv/lazycsv.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-02 20:32:32.668182 lazycsv-1.1.4/src/lazycsv.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     9944 2023-06-02 20:32:32.000000 lazycsv-1.1.4/src/lazycsv.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-06-02 20:32:32.000000 lazycsv-1.1.4/src/lazycsv.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-02 20:32:32.000000 lazycsv-1.1.4/src/lazycsv.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       66 2023-06-02 20:32:32.000000 lazycsv-1.1.4/src/lazycsv.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-06-02 20:32:32.000000 lazycsv-1.1.4/src/lazycsv.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-02 20:32:32.668182 lazycsv-1.1.4/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    24480 2023-06-02 16:19:26.000000 lazycsv-1.1.4/tests/test_lazycsv.py
```

### Comparing `lazycsv-1.1.3/LICENSE` & `lazycsv-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lazycsv-1.1.3/PKG-INFO` & `lazycsv-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.1.3
+Version: 1.1.4
 Summary: an fast, memory efficient csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `lazycsv-1.1.3/README.md` & `lazycsv-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lazycsv-1.1.3/setup.py` & `lazycsv-1.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="lazycsv",
-    version="1.1.3",
+    version="1.1.4",
     author="Michael Green, Chris Perkins",
     author_email="dev@crunch.io",
     description="an fast, memory efficient csv parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     extras_require={
```

### Comparing `lazycsv-1.1.3/src/lazycsv/lazycsv.c` & `lazycsv-1.1.4/src/lazycsv/lazycsv.c`

 * *Files 4% similar despite different names*

```diff
@@ -118,70 +118,71 @@
     size_t position;
     size_t stop;
     size_t step;
     char reversed;
 } LazyCSV_Iter;
 
 
-static inline void _BufferWrite(int fd, LazyCSV_Buffer *buffer, void *data,
-                                size_t size) {
+static inline void LazyCSV_BufferWrite(int fd, LazyCSV_Buffer *buffer,
+                                       void *data, size_t size) {
 
     if (buffer->size + size >= buffer->capacity) {
         write(fd, buffer->data, buffer->size);
         buffer->size = 0;
     }
     memcpy(&buffer->data[buffer->size], data, size);
     buffer->size += size;
 }
 
 
-static inline void _BufferCache(LazyCSV_Buffer *buffer, void *data,
-                                size_t size) {
+static inline void LazyCSV_BufferCache(LazyCSV_Buffer *buffer, void *data,
+                                       size_t size) {
 
     if (size == 0) return;
 
     if (buffer->size + size >= buffer->capacity) {
         buffer->capacity *= 1.5;
         buffer->data = realloc(buffer->data, buffer->capacity);
     }
     memcpy(&buffer->data[buffer->size], data, size);
     buffer->size += size;
 }
 
 
-static inline void _BufferFlush(int comma_file, LazyCSV_Buffer* buffer) {
+static inline void LazyCSV_BufferFlush(int comma_file, LazyCSV_Buffer *buffer) {
     write(comma_file, buffer->data, buffer->size);
     buffer->size = 0;
     fsync(comma_file);
 }
 
 
-static inline void _Value_ToDisk(size_t value, LazyCSV_RowIndex *ridx,
-                                 LazyCSV_AnchorPoint *apnt, size_t col_index,
-                                 int cfile, LazyCSV_Buffer *cbuf, int afile,
-                                 LazyCSV_Buffer *abuf) {
+static inline void LazyCSV_ValueToDisk(size_t value, LazyCSV_RowIndex *ridx,
+                                       LazyCSV_AnchorPoint *apnt,
+                                       size_t col_index, int cfile,
+                                       LazyCSV_Buffer *cbuf, int afile,
+                                       LazyCSV_Buffer *abuf) {
 
     size_t target = value - apnt->value;
 
     if (target > INDEX_DTYPE_MAX) {
         *apnt = (LazyCSV_AnchorPoint){.value = value, .col = col_index+1};
-        _BufferWrite(afile, abuf, apnt, sizeof(LazyCSV_AnchorPoint));
+        LazyCSV_BufferWrite(afile, abuf, apnt, sizeof(LazyCSV_AnchorPoint));
         ridx->count += 1;
         target = 0;
     }
 
     INDEX_DTYPE item = target;
 
-    _BufferWrite(cfile, cbuf, &item, sizeof(INDEX_DTYPE));
+    LazyCSV_BufferWrite(cfile, cbuf, &item, sizeof(INDEX_DTYPE));
 }
 
 
-static inline size_t _AnchorValue_FromValue(size_t value,
-                                            LazyCSV_AnchorPoint *amap,
-                                            LazyCSV_RowIndex *ridx) {
+static inline size_t LazyCSV_AnchorValueFromValue(size_t value,
+                                                  LazyCSV_AnchorPoint *amap,
+                                                  LazyCSV_RowIndex *ridx) {
 
     LazyCSV_AnchorPoint *apnt = amap + ridx->count - 1;
 
     if (value >= apnt->col) {
         // we hit this if there is only one anchor point, or we're iterating
         // over the last anchor point.
         return apnt->value;
@@ -206,25 +207,29 @@
         else {
             return apnt->value;
         }
     }
     return SIZE_MAX;
 }
 
-static inline size_t _Value_FromIndex(size_t value, LazyCSV_RowIndex *ridx,
-                                      char *cmap, char *amap) {
 
-    size_t cval = *(INDEX_DTYPE*)(cmap+(value*sizeof(INDEX_DTYPE)));
-    size_t aval = _AnchorValue_FromValue(value, (LazyCSV_AnchorPoint*)amap, ridx);
+static inline size_t LazyCSV_ValueFromIndex(size_t value,
+                                            LazyCSV_RowIndex *ridx, char *cmap,
+                                            char *amap) {
+
+    size_t cval = *(INDEX_DTYPE *)(cmap + (value * sizeof(INDEX_DTYPE)));
+    size_t aval =
+        LazyCSV_AnchorValueFromValue(value, (LazyCSV_AnchorPoint *)amap, ridx);
     return aval == SIZE_MAX ? aval : cval + aval;
 }
 
 
 static inline void LazyCSV_IterCol(LazyCSV_Iter *iter, size_t *offset,
                                    size_t *len) {
+
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
     if (iter->position < iter->stop) {
         size_t position =
             iter->reversed
                 ? lazy->rows - 1 - iter->position + !lazy->_skip_headers
                 : iter->position + !lazy->_skip_headers;
@@ -238,16 +243,16 @@
         LazyCSV_RowIndex* ridx =
             (LazyCSV_RowIndex*)
             (newlines + position*sizeof(LazyCSV_RowIndex));
 
         char* aidx = anchors+ridx->index;
         char* cidx = commas+((lazy->cols+1)*position*sizeof(INDEX_DTYPE));
 
-        size_t cs = _Value_FromIndex(iter->col, ridx, cidx, aidx);
-        size_t ce = _Value_FromIndex(iter->col + 1, ridx, cidx, aidx);
+        size_t cs = LazyCSV_ValueFromIndex(iter->col, ridx, cidx, aidx);
+        size_t ce = LazyCSV_ValueFromIndex(iter->col + 1, ridx, cidx, aidx);
 
         *len = ce - cs - 1;
         *offset = cs;
     }
 }
 
 
@@ -271,22 +276,23 @@
         LazyCSV_RowIndex* ridx =
             (LazyCSV_RowIndex*)
             (newlines + row*sizeof(LazyCSV_RowIndex));
 
         char *aidx = anchors + ridx->index;
         char *cidx = commas + ((lazy->cols + 1) * row * sizeof(INDEX_DTYPE));
 
-        size_t cs = _Value_FromIndex(position, ridx, cidx, aidx);
-        size_t ce = _Value_FromIndex(position + 1, ridx, cidx, aidx);
+        size_t cs = LazyCSV_ValueFromIndex(position, ridx, cidx, aidx);
+        size_t ce = LazyCSV_ValueFromIndex(position + 1, ridx, cidx, aidx);
 
         *len = ce - cs - 1;
         *offset = cs;
     }
 }
 
+
 static inline PyObject *PyBytes_FromOffsetAndLen(LazyCSV *lazy, size_t offset,
                                                  size_t len) {
 
     PyObject* result;
     char* addr;
 
     switch (len) {
@@ -430,16 +436,16 @@
         case SIZE_MAX:
             LazyCSV_IterRow(iter, &offset, &len);
             break;
         default:
             LazyCSV_IterCol(iter, &offset, &len);
         }
         addr = lazy->_data->data + offset;
-        _BufferCache(&buffer, &len, sizeof(size_t));
-        _BufferCache(&buffer, addr, len);
+        LazyCSV_BufferCache(&buffer, &len, sizeof(size_t));
+        LazyCSV_BufferCache(&buffer, addr, len);
         max_len = len > max_len ? len : max_len;
     }
 
     npy_intp const dimensions[1] = {size, };
     npy_intp const strides[1] = {max_len, };
 
     PyArrayObject *arr =
@@ -516,87 +522,73 @@
     .tp_doc = "LazyCSV iterable",
     .tp_methods = LazyCSV_IterMethods,
     .tp_iter = LazyCSV_IterSelf,
     .tp_iternext = LazyCSV_IterNext,
 };
 
 
-static inline void _TempDir_AsString(PyObject** tempdir, char** dirname) {
-    PyObject* tempfile = PyImport_ImportModule("tempfile");
-    PyObject* tempdir_obj = PyObject_GetAttrString(
-        tempfile, "TemporaryDirectory"
-    );
+static inline void LazyCSV_TempDirAsString(PyObject **tempdir, char **dirname) {
+    PyObject *tempfile = PyImport_ImportModule("tempfile");
+    PyObject *tempdir_obj =
+        PyObject_GetAttrString(tempfile, "TemporaryDirectory");
 
     *tempdir = PyObject_CallObject(tempdir_obj, NULL);
     PyObject* dirname_obj = PyObject_GetAttrString(*tempdir, "name");
     PyObject* dirstring = PyUnicode_AsUTF8String(dirname_obj);
     *dirname = PyBytes_AsString(dirstring);
 
     Py_DECREF(tempfile);
     Py_DECREF(tempdir_obj);
     Py_DECREF(dirname_obj);
     Py_DECREF(dirstring);
 }
 
 
-static inline void _FullName_FromName(PyObject *name, PyObject **fullname_obj,
-                                      char **fullname) {
+static inline void LazyCSV_FullNameFromName(PyObject *name,
+                                            PyObject **fullname_obj,
+                                            char **fullname) {
 
     PyObject *os_path = PyImport_ImportModule("os.path");
-    PyObject *builtins = PyImport_ImportModule("builtins");
+    PyObject *isfile = PyObject_CallMethod(os_path, "isfile", "O", name);
 
+    PyObject *builtins = PyImport_ImportModule("builtins");
     PyObject* global_vars = PyObject_CallMethod(builtins, "globals", NULL);
 
-    PyObject* _dirname;
-
     // borrowed ref
     PyObject* __file__ = PyDict_GetItemString(global_vars, "__file__");
 
-    if (!__file__) {
-        // if run in say, the python shell, there is no __file__, so use cwd
-        // of the interpreter
-        PyObject *os = PyImport_ImportModule("os");
-        _dirname = PyObject_CallMethod(os, "getcwd", NULL);
-        Py_DECREF(os);
-    }
-
-    else {
-        _dirname = PyObject_CallMethod(os_path, "dirname", "O", __file__);
+    if (isfile == Py_True) {
+        // owned reference which we keep
+        *fullname_obj = PyObject_CallMethod(os_path, "abspath", "O", name);
+        *fullname = PyBytes_AsString(*fullname_obj);
     }
 
-    PyObject *dirname = PyUnicode_AsUTF8String(_dirname);
-    Py_DECREF(_dirname);
-
-    PyObject *abspath = PyObject_CallMethod(os_path, "abspath", "O", name);
-
-    PyObject *bytes = PyObject_GetAttrString(builtins, "bytes");
-    PyObject *startswith =
-        PyObject_CallMethod(bytes, "startswith", "OO", abspath, dirname);
+    else if (__file__) {
+        // also check to see if file is relative to the caller if not
+        // previously found
+        PyObject *_dirname =
+            PyObject_CallMethod(os_path, "dirname", "O", __file__);
 
-    if (startswith == Py_True) {
-        *fullname_obj = abspath;
-        Py_INCREF(abspath);
-        *fullname = PyBytes_AsString(abspath);
-    }
+        PyObject *dirname = PyUnicode_AsUTF8String(_dirname);
 
-    else {
         PyObject *joined =
             PyObject_CallMethod(os_path, "join", "(OO)", dirname, name);
+
         *fullname_obj = PyObject_CallMethod(os_path, "abspath", "O", joined);
         *fullname = PyBytes_AsString(*fullname_obj);
+
         Py_DECREF(joined);
+        Py_DECREF(_dirname);
+        Py_DECREF(dirname);
     }
 
     Py_DECREF(os_path);
+    Py_DECREF(isfile);
     Py_DECREF(builtins);
     Py_DECREF(global_vars);
-    Py_DECREF(dirname);
-    Py_DECREF(abspath);
-    Py_DECREF(bytes);
-    Py_DECREF(startswith);
 }
 
 
 static PyObject *LazyCSV_New(PyTypeObject *type, PyObject *args,
                              PyObject *kwargs) {
 
     PyObject* name;
@@ -643,15 +635,15 @@
         );
         Py_DECREF(name);
         return NULL;
     }
 
     PyObject* fullname_obj;
     char* fullname;
-    _FullName_FromName(name, &fullname_obj, &fullname);
+    LazyCSV_FullNameFromName(name, &fullname_obj, &fullname);
 
     Py_DECREF(name);
 
     int ufd = open(fullname, O_RDONLY);
     if (ufd == -1) {
         PyErr_SetString(
             PyExc_FileNotFoundError,
@@ -674,15 +666,15 @@
     size_t file_len = ust.st_size;
 
     int mmap_flags = PROT_READ;
     char* file = mmap(NULL, file_len, mmap_flags, MAP_PRIVATE, ufd, 0);
 
     PyObject* tempdir = NULL;
     if (!dirname) {
-        _TempDir_AsString(&tempdir, &dirname);
+        LazyCSV_TempDirAsString(&tempdir, &dirname);
     }
 
     char* comma_index = tempnam(dirname, "LzyC_");
     char* anchor_index = tempnam(dirname, "LzyA_");
     char* newline_index = tempnam(dirname, "LzyN_");
 
     int file_flags = O_WRONLY|O_CREAT|O_EXCL;
@@ -734,32 +726,32 @@
             && cm2 != CARRIAGE_RETURN) {
             size_t val = (
                 newline == (CARRIAGE_RETURN+LINE_FEED)
             ) ? i + 1 : i;
 
             apnt = (LazyCSV_AnchorPoint){.value = val, .col = col_index};
 
-            _BufferWrite(anchor_file, &anchor_buffer, &apnt,
-                         sizeof(LazyCSV_AnchorPoint));
+            LazyCSV_BufferWrite(anchor_file, &anchor_buffer, &apnt,
+                                sizeof(LazyCSV_AnchorPoint));
 
             ridx.index += ridx.count*sizeof(LazyCSV_AnchorPoint);
             ridx.count = 1;
 
-            _Value_ToDisk(val, &ridx, &apnt, col_index, comma_file,
-                          &comma_buffer, anchor_file, &anchor_buffer);
+            LazyCSV_ValueToDisk(val, &ridx, &apnt, col_index, comma_file,
+                                &comma_buffer, anchor_file, &anchor_buffer);
         }
 
         if (c == *quotechar) {
             quoted = !quoted;
         }
 
         else if (!quoted && c == *delimiter) {
             size_t val = i + 1;
-            _Value_ToDisk(val, &ridx, &apnt, col_index, comma_file,
-                          &comma_buffer, anchor_file, &anchor_buffer);
+            LazyCSV_ValueToDisk(val, &ridx, &apnt, col_index, comma_file,
+                                &comma_buffer, anchor_file, &anchor_buffer);
             if (cols == SIZE_MAX || col_index < cols) {
                 col_index += 1;
             }
             else {
                 overflow_warning =
                     "column overflow encountered while parsing CSV, "
                     "extra values will be truncated!";
@@ -780,62 +772,63 @@
             // no-op, don't match next block for \r\n
         }
 
         else if (!quoted && (c == CARRIAGE_RETURN || c == LINE_FEED)) {
             size_t val = i + 1;
 
             if (overflow == SIZE_MAX) {
-                _Value_ToDisk(val, &ridx, &apnt, col_index, comma_file,
-                              &comma_buffer, anchor_file, &anchor_buffer);
+                LazyCSV_ValueToDisk(val, &ridx, &apnt, col_index, comma_file,
+                                    &comma_buffer, anchor_file, &anchor_buffer);
             }
             else {
                 overflow = SIZE_MAX;
             }
 
             if (row_index == 0) {
                 cols = col_index;
             }
 
             else if (col_index < cols) {
                 underflow_warning =
                     "column underflow encountered while parsing CSV, "
                     "missing values will be filled with the empty bytestring!";
                 while (col_index < cols) {
-                    _Value_ToDisk(val, &ridx, &apnt, col_index, comma_file,
-                                  &comma_buffer, anchor_file, &anchor_buffer);
-                    col_index += 1;
+                  LazyCSV_ValueToDisk(val, &ridx, &apnt, col_index, comma_file,
+                                      &comma_buffer, anchor_file,
+                                      &anchor_buffer);
+                  col_index += 1;
                 }
             }
 
             if (newline == -1) {
                 newline = (c == CARRIAGE_RETURN && file[i + 1] == LINE_FEED)
                               ? LINE_FEED + CARRIAGE_RETURN
                               : c;
             }
 
-            _BufferWrite(newline_file, &newline_buffer, &ridx,
-                         sizeof(LazyCSV_RowIndex));
+            LazyCSV_BufferWrite(newline_file, &newline_buffer, &ridx,
+                                sizeof(LazyCSV_RowIndex));
 
             col_index = 0;
             row_index += 1;
         }
 
         cm2 = cm1;
         cm1 = c;
     }
 
     char last_char = file[file_len - 1];
     char overcount = last_char == CARRIAGE_RETURN || last_char == LINE_FEED;
 
     if (!overcount) {
-        _Value_ToDisk(file_len + 1, &ridx, &apnt, col_index, comma_file,
-                      &comma_buffer, anchor_file, &anchor_buffer);
+        LazyCSV_ValueToDisk(file_len + 1, &ridx, &apnt, col_index, comma_file,
+                            &comma_buffer, anchor_file, &anchor_buffer);
 
-        _BufferWrite(newline_file, &newline_buffer, &ridx,
-                     sizeof(LazyCSV_RowIndex));
+        LazyCSV_BufferWrite(newline_file, &newline_buffer, &ridx,
+                            sizeof(LazyCSV_RowIndex));
     }
 
     if (overflow_warning)
         PyErr_WarnEx(
             PyExc_RuntimeWarning,
             overflow_warning,
             1
@@ -847,17 +840,17 @@
             underflow_warning,
             1
         );
 
     rows = row_index - overcount + skip_headers;
     cols = cols + 1;
 
-    _BufferFlush(comma_file, &comma_buffer);
-    _BufferFlush(anchor_file, &anchor_buffer);
-    _BufferFlush(newline_file, &newline_buffer);
+    LazyCSV_BufferFlush(comma_file, &comma_buffer);
+    LazyCSV_BufferFlush(anchor_file, &anchor_buffer);
+    LazyCSV_BufferFlush(newline_file, &newline_buffer);
 
     close(comma_file);
     close(anchor_file);
     close(newline_file);
 
     free(comma_buffer.data);
     free(anchor_buffer.data);
@@ -904,18 +897,19 @@
 
     if (!skip_headers) {
         headers = PyTuple_New(cols);
         LazyCSV_RowIndex* ridx = (LazyCSV_RowIndex*)newline_memmap;
 
         size_t cs, ce;
         size_t len;
-        char* addr;
+        char *addr;
         for (size_t i = 0; i < cols; i++) {
-            cs = _Value_FromIndex(i, ridx, comma_memmap, anchor_memmap);
-            ce = _Value_FromIndex(i+1, ridx, comma_memmap, anchor_memmap);
+            cs = LazyCSV_ValueFromIndex(i, ridx, comma_memmap, anchor_memmap);
+            ce = LazyCSV_ValueFromIndex(i + 1, ridx, comma_memmap,
+                                        anchor_memmap);
 
             if (ce - cs == 1) {
                 PyTuple_SET_ITEM(headers, i, PyBytes_FromString(""));
             }
             else {
                 addr = file + cs;
 
@@ -1179,16 +1173,16 @@
     LazyCSV_RowIndex* ridx =
         (LazyCSV_RowIndex*)
         (newlines + row*sizeof(LazyCSV_RowIndex));
 
     char* aidx = anchors+ridx->index;
     char* cidx = commas+((lazy->cols+1)*row*sizeof(INDEX_DTYPE));
 
-    size_t cs = _Value_FromIndex((size_t)col, ridx, cidx, aidx);
-    size_t ce = _Value_FromIndex((size_t)col + 1, ridx, cidx, aidx);
+    size_t cs = LazyCSV_ValueFromIndex((size_t)col, ridx, cidx, aidx);
+    size_t ce = LazyCSV_ValueFromIndex((size_t)col + 1, ridx, cidx, aidx);
 
     size_t len = ce - cs - 1;
 
     return PyBytes_FromOffsetAndLen(lazy, cs, len);
 }
```

### Comparing `lazycsv-1.1.3/src/lazycsv.egg-info/PKG-INFO` & `lazycsv-1.1.4/src/lazycsv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.1.3
+Version: 1.1.4
 Summary: an fast, memory efficient csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `lazycsv-1.1.3/tests/test_lazycsv.py` & `lazycsv-1.1.4/tests/test_lazycsv.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
                     " LAZYCSV_INCLUDE_NUMPY=1 as an env variable to compile"
                     " extension with numpy support."
                 )
 
 
 class TestLazyCSVOptions:
     def test_custom_quotechar_and_delimiter(self):
-        lazy = lazycsv.LazyCSV("tests/fixtures/file_delimiter_and_quotechar.csv", quotechar="|", delimiter="\t")
+        lazy = lazycsv.LazyCSV("fixtures/file_delimiter_and_quotechar.csv", quotechar="|", delimiter="\t")
         actual = list(list(lazy.sequence(row=i)) for i in range(lazy.rows))
         expected = [[b'0', b'A'], [b'1', b'B']]
         assert actual == expected
 
     def test_custom_quotechar_unquote_false(self):
         data = "INDEX,ATTR\n0,|A|\n1,|B|\n"
         with prepped_file(data.encode()) as tempf:
```

