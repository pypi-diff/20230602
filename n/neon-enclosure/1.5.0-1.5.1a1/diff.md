# Comparing `tmp/neon_enclosure-1.5.0-py3-none-any.whl.zip` & `tmp/neon_enclosure-1.5.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13786 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1831 b- defN 23-May-26 23:48 neon_enclosure/__init__.py
--rw-r--r--  2.0 unx     2832 b- defN 23-May-26 23:48 neon_enclosure/__main__.py
--rw-r--r--  2.0 unx     3152 b- defN 23-May-26 23:48 neon_enclosure/cli.py
--rw-r--r--  2.0 unx     3660 b- defN 23-May-26 23:48 neon_enclosure/service.py
--rw-r--r--  2.0 unx     1832 b- defN 23-May-26 23:48 neon_enclosure/admin/__init__.py
--rw-r--r--  2.0 unx     2839 b- defN 23-May-26 23:48 neon_enclosure/admin/__main__.py
--rw-r--r--  2.0 unx     2406 b- defN 23-May-26 23:48 neon_enclosure/admin/service.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2695 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      127 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1119 b- defN 23-May-26 23:49 neon_enclosure-1.5.0.dist-info/RECORD
-13 files, 24234 bytes uncompressed, 11902 bytes compressed:  50.9%
+Zip file size: 13847 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jun-02 18:09 neon_enclosure/__init__.py
+-rw-r--r--  2.0 unx     2828 b- defN 23-Jun-02 18:09 neon_enclosure/__main__.py
+-rw-r--r--  2.0 unx     3165 b- defN 23-Jun-02 18:09 neon_enclosure/cli.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-Jun-02 18:09 neon_enclosure/service.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-Jun-02 18:09 neon_enclosure/admin/__init__.py
+-rw-r--r--  2.0 unx     2841 b- defN 23-Jun-02 18:09 neon_enclosure/admin/__main__.py
+-rw-r--r--  2.0 unx     2406 b- defN 23-Jun-02 18:09 neon_enclosure/admin/service.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-02 18:09 neon_enclosure-1.5.1a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2785 b- defN 23-Jun-02 18:09 neon_enclosure-1.5.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 18:09 neon_enclosure-1.5.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-02 18:09 neon_enclosure-1.5.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-02 18:09 neon_enclosure-1.5.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1131 b- defN 23-Jun-02 18:09 neon_enclosure-1.5.1a1.dist-info/RECORD
+13 files, 24346 bytes uncompressed, 11939 bytes compressed:  51.0%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: neon_enclosure/admin/__main__.py
 Comment: 
 
 Filename: neon_enclosure/admin/service.py
 Comment: 
 
-Filename: neon_enclosure-1.5.0.dist-info/LICENSE.md
+Filename: neon_enclosure-1.5.1a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_enclosure-1.5.0.dist-info/METADATA
+Filename: neon_enclosure-1.5.1a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_enclosure-1.5.0.dist-info/WHEEL
+Filename: neon_enclosure-1.5.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_enclosure-1.5.0.dist-info/entry_points.txt
+Filename: neon_enclosure-1.5.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_enclosure-1.5.0.dist-info/top_level.txt
+Filename: neon_enclosure-1.5.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_enclosure-1.5.0.dist-info/RECORD
+Filename: neon_enclosure-1.5.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_enclosure/__main__.py

```diff
@@ -24,32 +24,31 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.log_utils import init_log
 from neon_utils.process_utils import start_malloc, snapshot_malloc, print_malloc
+from neon_utils.signal_utils import init_signal_bus, init_signal_handlers
 from ovos_utils.messagebus import get_mycroft_bus
 from ovos_utils.process_utils import reset_sigint_handler
 from ovos_utils.log import LOG
 from ovos_utils import wait_for_exit_signal
 
+from neon_enclosure.service import NeonHardwareAbstractionLayer
+
 
 def main(*args, **kwargs):
     init_log(log_name="enclosure")
     malloc_running = start_malloc(stack_depth=4)
     bus = get_mycroft_bus()
     kwargs["bus"] = bus
-    from neon_utils.signal_utils import init_signal_bus, \
-        init_signal_handlers
+
     init_signal_bus(bus)
     init_signal_handlers()
-
-    from .service import NeonHardwareAbstractionLayer
-
     reset_sigint_handler()
     service = NeonHardwareAbstractionLayer(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     if malloc_running:
         try:
             print_malloc(snapshot_malloc())
```

## neon_enclosure/cli.py

```diff
@@ -21,16 +21,14 @@
 # CONTRIBUTORS  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import os
-
 import click
 
 from click_default_group import DefaultGroup
 from neon_utils.packaging_utils import get_package_version_spec
 from neon_utils.configuration_utils import init_config_dir
 
 
@@ -53,15 +51,16 @@
     click.echo("Starting Enclosure Service")
     main()
     click.echo("Enclosure Service Shutdown")
 
 
 @neon_enclosure_cli.command(help="Start Neon Enclosure Admin module")
 def run_admin():
-    if os.geteuid() != 0:
+    from os import geteuid
+    if geteuid() != 0:
         click.echo("Admin enclosure must be started as `root`")
         exit(1)
     init_config_dir()
     from neon_enclosure.admin.__main__ import main
     click.echo("Starting Admin Enclosure Service")
     main()
     click.echo("Admin Enclosure Service Shutdown")
```

## neon_enclosure/admin/__main__.py

```diff
@@ -24,33 +24,32 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.log_utils import init_log
 from neon_utils.process_utils import start_malloc, snapshot_malloc, print_malloc
+from neon_utils.signal_utils import init_signal_bus, init_signal_handlers
 from ovos_utils.messagebus import get_mycroft_bus
 from ovos_utils.process_utils import reset_sigint_handler
 from ovos_utils import wait_for_exit_signal
 from ovos_utils.log import LOG
 
+from neon_enclosure.admin.service import NeonAdminHardwareAbstractionLayer
+
 
 def main(*args, **kwargs):
     init_log(log_name="admin")
     malloc_running = start_malloc(stack_depth=4)
 
     bus = get_mycroft_bus()
     kwargs["bus"] = bus
-    from neon_utils.signal_utils import init_signal_bus, \
-        init_signal_handlers
+
     init_signal_bus(bus)
     init_signal_handlers()
-
-    from .service import NeonAdminHardwareAbstractionLayer
-
     reset_sigint_handler()
     service = NeonAdminHardwareAbstractionLayer(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     if malloc_running:
         try:
             print_malloc(snapshot_malloc())
```

## Comparing `neon_enclosure-1.5.0.dist-info/LICENSE.md` & `neon_enclosure-1.5.1a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_enclosure-1.5.0.dist-info/METADATA` & `neon_enclosure-1.5.1a1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.5.0
+Version: 1.5.1a1
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: ovos-PHAL (~=0.0.4)
-Requires-Dist: neon-utils[network] (~=1.3)
+Requires-Dist: neon-utils[network] (>=1.5.0a11,~=1.3)
 Requires-Dist: ovos-utils[extras] (~=0.0.32)
+Requires-Dist: click (~=8.0)
+Requires-Dist: click-default-group (~=1.2)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-backend-client (~=0.0.6)
 Provides-Extra: docker
 Requires-Dist: ovos-phal-plugin-homeassistant (~=0.0.1) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-notification-widgets (~=1.0.0) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-color-scheme-manager (~=1.0.0) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-configuration-provider (~=1.0.0) ; extra == 'docker'
@@ -51,9 +53,7 @@
 -e PULSE_SERVER=unix:${XDG_RUNTIME_DIR}/pulse/native \
 -e PULSE_COOKIE=/home/neon/.config/pulse/cookie \
 neon_enclosure
 ```
 
 >*Note:* The above example assumes Docker data is stored in the standard user locations `~/.local/share` and `~/.config`.
 > You may want to change these values to some other path to separate container and host system data.
-
-
```

## Comparing `neon_enclosure-1.5.0.dist-info/RECORD` & `neon_enclosure-1.5.1a1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 neon_enclosure/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
-neon_enclosure/__main__.py,sha256=v0iXqgiP-OXIHMoReuZ3v_3cCm7SVKsvlEyobaldfv0,2832
-neon_enclosure/cli.py,sha256=hrt0DltcdUypm-g08OFDG8ojbMXSANkgRw1OAVk_10g,3152
+neon_enclosure/__main__.py,sha256=NeBq4HEjYhMx5BGI3_nSxh7KVIbGahl8R6_QBaL4mq4,2828
+neon_enclosure/cli.py,sha256=qpmDg3KphuxhK5bB8f4q039L3xZeCJR_Cyvaz_BuYoI,3165
 neon_enclosure/service.py,sha256=ntd4ky4nfdtDEkWEKn8wRJkrqQFX1_N9l0HDXQwDcfI,3660
 neon_enclosure/admin/__init__.py,sha256=FCW9FTGwZxZm9BbxptD2ri02MXw5mq0YtuIfJ0Rm0SA,1832
-neon_enclosure/admin/__main__.py,sha256=bMiOyKwsqEyqXlgOSiy64lT1pqCw7hq5pvrTUXGVZdE,2839
+neon_enclosure/admin/__main__.py,sha256=dGregbob_X2K0h6v2Dh8Djug9Zfg9_csKz1YcvFqPa4,2841
 neon_enclosure/admin/service.py,sha256=UrD0RLVFi-27A0wnFFfQjVlmo-GHWxEyma1Q0W8TLqE,2406
-neon_enclosure-1.5.0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_enclosure-1.5.0.dist-info/METADATA,sha256=lkr-sTgG_zSqGRAx5KJOohphZDjTTyRmdyDO5_4_ysc,2695
-neon_enclosure-1.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_enclosure-1.5.0.dist-info/entry_points.txt,sha256=6Jj4lPTnz0a89img-7ynoJRUxlX7ye2o4hPVmwhC_hc,127
-neon_enclosure-1.5.0.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
-neon_enclosure-1.5.0.dist-info/RECORD,,
+neon_enclosure-1.5.1a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_enclosure-1.5.1a1.dist-info/METADATA,sha256=ZkK9B_AHieSEWz_QbDYyRy5VvDRHWbGIBLkh0my_v4k,2785
+neon_enclosure-1.5.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_enclosure-1.5.1a1.dist-info/entry_points.txt,sha256=xIujp8DylZvh005eOZ7canZhQr2JdIepZhoV2SXRnEI,126
+neon_enclosure-1.5.1a1.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
+neon_enclosure-1.5.1a1.dist-info/RECORD,,
```

