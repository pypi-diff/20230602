# Comparing `tmp/gregory_online-0.2.3.tar.gz` & `tmp/gregory_online-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.2.3.tar", last modified: Thu Apr 20 14:09:29 2023, max compression
+gzip compressed data, was "gregory_online-0.2.4.tar", last modified: Fri Jun  2 15:19:40 2023, max compression
```

## Comparing `gregory_online-0.2.3.tar` & `gregory_online-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 14:09:29.125568 gregory_online-0.2.3/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      392 2023-04-20 14:09:29.125568 gregory_online-0.2.3/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      177 2023-03-15 09:15:19.000000 gregory_online-0.2.3/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 14:09:29.121568 gregory_online-0.2.3/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    48177 2023-04-20 14:09:16.000000 gregory_online-0.2.3/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 14:09:29.125568 gregory_online-0.2.3/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.2.3/gregory_online/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-15 09:15:19.000000 gregory_online-0.2.3/gregory_online/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12154 2023-04-19 12:12:40.000000 gregory_online-0.2.3/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 08:56:38.000000 gregory_online-0.2.3/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3955 2023-03-17 13:02:18.000000 gregory_online-0.2.3/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      779 2023-03-16 17:25:56.000000 gregory_online-0.2.3/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12830 2023-03-15 13:27:27.000000 gregory_online-0.2.3/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-03-17 14:35:05.000000 gregory_online-0.2.3/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.2.3/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-19 12:17:44.000000 gregory_online-0.2.3/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.2.3/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2635 2023-03-15 09:15:19.000000 gregory_online-0.2.3/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-20 14:09:28.000000 gregory_online-0.2.3/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 14:09:29.125568 gregory_online-0.2.3/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      392 2023-04-20 14:09:29.000000 gregory_online-0.2.3/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-04-20 14:09:29.000000 gregory_online-0.2.3/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-20 14:09:29.000000 gregory_online-0.2.3/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       53 2023-04-20 14:09:29.000000 gregory_online-0.2.3/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-04-20 14:09:29.000000 gregory_online-0.2.3/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-20 14:09:29.125568 gregory_online-0.2.3/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1186 2023-03-15 13:31:42.000000 gregory_online-0.2.3/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-02 15:19:40.124060 gregory_online-0.2.4/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-02 15:19:40.124060 gregory_online-0.2.4/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:19:34.000000 gregory_online-0.2.4/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-02 15:19:40.120060 gregory_online-0.2.4/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    49972 2023-06-02 15:19:37.000000 gregory_online-0.2.4/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-02 15:19:40.120060 gregory_online-0.2.4/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.2.4/gregory_online/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-17 17:33:40.000000 gregory_online-0.2.4/gregory_online/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12282 2023-06-02 13:02:37.000000 gregory_online-0.2.4/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 14:10:17.000000 gregory_online-0.2.4/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3955 2023-03-17 17:33:40.000000 gregory_online-0.2.4/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      779 2023-03-17 17:33:40.000000 gregory_online-0.2.4/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-05-31 13:39:18.000000 gregory_online-0.2.4/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-03-17 17:33:40.000000 gregory_online-0.2.4/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.2.4/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-20 14:10:17.000000 gregory_online-0.2.4/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.2.4/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2853 2023-06-02 14:03:44.000000 gregory_online-0.2.4/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-02 15:19:39.000000 gregory_online-0.2.4/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-02 15:19:40.124060 gregory_online-0.2.4/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       65 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-02 15:19:40.124060 gregory_online-0.2.4/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1200 2023-06-01 12:16:03.000000 gregory_online-0.2.4/setup.py
```

### Comparing `gregory_online-0.2.3/bin/gregory_online` & `gregory_online-0.2.4/bin/gregory_online`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 import csv
 # import array
 
 import fastnumbers # cor calib, let it crash here
 
 from tdb_io.influx import influxwrite
 
+
+import math
+
 HOSTNAME = socket.gethostname()
 
 #----------------------------global variables
 # histograms = {} # moved to container
 # canvases = {} # c will be dir
 
 
@@ -86,15 +89,15 @@
 cala = 1
 calb = 0
 cala_bg = 1
 calb_bg = 0
 h1np = None
 h1np_diff = None # last poll
 h1np_old = None # define 60 sec eg
-h1np_old_age = 20
+h1np_last_interval = 20
 h1np_substr = None # h1np - backg
 #----load separately
 h1np_backg = None
 h1np_backg_lt = 100  # background livetime
 
 
 # global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
@@ -230,33 +233,38 @@
     #print( len(a),"X" ,len(b),  f" 6 -->  {6*sca+shi}" )
     #print( len(a),"X" ,len(b),  f" 22 -->  {22*sca+shi}" )
     return spectrumb
 
 
 
 
-def main( timeold = None , debug=False, server = None, histogram = None, polltime = None):
+def main( timeold = None , debug=False, server = None, histogram = None, polltime = None, OFFLINE = False):
     '''
     Main function of the project
     Config is settled in the beginning
     '''
+    #OFFLINE = True
+    #online
+    #if online:
+    #OFFLINE = False
+
     #======== DEFINE THE CONFIG FILE HERE ========
     print("i... OVERRIDE the CONFIG with")
     print("i... -s 127.0.0.1 -h b0c01")
     print("i... ")
 
     # ---------------- container stuff
     global histograms, canvases, range_and_peaks
     global gregory_started
     global last_fit_res
     global ECALIB, ECALIBa, ECALIBb # calibrations
     #
     # --------------    other stuff
     #global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt
-    global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
+    global h1np,h1np_diff,h1np_old,h1np_last_interval,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
 
     cmd = "" # no key command
 
     gregory_started = None # dt.datetime.now()
 
     config.CONFIG['filename'] = "~/.config/gregory_online/cfg.json"
     config.CONFIG["poll_time"] = 2
@@ -293,14 +301,16 @@
     print("_"*10, TITLE ,"_"*10)
     print("_"*(len(TITLE)+22) )
 
 
     # INIT HISOGRAM AND SET STEP, PRESETIME
 
     b0c01 = fetchnp.Histogram( serverc, spectrumname )
+
+
     if polltime is not None:
         config.CONFIG["poll_time"] = float(polltime)
     b0c01.set_step( config.CONFIG["poll_time"])
 
 
     # #   - SET THE RUNTIME ON AGE ??????  AGE will stand only for diffage spectrum
     # arg = time2seconds(age)
@@ -309,15 +319,15 @@
     # #time.sleep(1)
     # -------  timeold will work for server that doesnot use TITLE:  rt=123.4s
     if timeold is not None:
         arg = time2seconds(timeold)
         print(f"i... measurement time (current spectrum age) is set to {timeold} == {arg} s ") #
         b0c01.set_started_before( arg)
 
-    OFFLINE = True
+    #OFFLINE = True
     thr = threading.Thread( target=b0c01.start2collect , args=() )
     if not OFFLINE:
         thr.start()
 
 
     top = topbar.Topbar( bgcolor = bg.blue)
     top2 = top.add(bgcolor = bg.black)
@@ -337,49 +347,56 @@
     lenhistos = 0
 
     # ### backg_np = None
     # h1np = None
     # h1np_diff = None
     # h1np_substr = None
     # h1np_backg = None
-    dage = 0
+    d_last_interval = 0.0
     warn_del = fg.default
     unwarn_del = fg.default
+
     while thr.is_alive() or OFFLINE:
 
         if  b0c01.fetch_flag():
-            # if fetched - get values
+            # if fetched - get values ==========================
+
             h1np = b0c01.get_h1np()
             h1np_diff = b0c01.get_h1np_diff()
             deltat = b0c01.get_deltat()
-            runtime = b0c01.get_runtime()
+            runtime = b0c01.get_runtime() # total histogram time/age; NOT last_interval
             gregory_started = b0c01.get_started()
             #if runtime.total_seconds()<=0:
             #    runtime = 1#dt.datetime.now()-dt.datetime.now()
             lenhistos = b0c01.get_lenhistos()
             #print(runtime)
 
-            h1np_old, dage = b0c01.get_old_histo( h1np_old_age) # get 20sec old
+            h1np_old, d_last_interval = b0c01.get_partial_time_histo( h1np_last_interval) # get 20sec old
 
             # - if the age differs more than 1%, show in red on topbar
-            if dage/h1np_old_age>0.01:
-                # print(f"{fg.cyan}i...                    delta in age={dage:.2f} s, demanded age={h1np_old_age} s{fg.default}")
+            if d_last_interval/h1np_last_interval>0.01:
+                # print(f"{fg.cyan}i...                    delta in age={d_last_interval:.2f} s, demanded age={h1np_old_age} s{fg.default}")
                 warn_del = f"{fg.white}{bg.red}"
             else:
                 warn_del = f"{fg.default}{bg.default}"
             unwarn_del = f"{fg.default}{bg.blue}"
 
             limits_calib = b0c01.get_limits_calib()
 
-            rate= h1np_diff.sum()/deltat
+            rate= h1np_diff.sum()/deltat # does sum contain underflow? ->Integral() doesnot
+            # I like to have underflow there...
+
 
+            # print(h1np_diff[0], h1np_diff[1]) # underflow and 1st bin #1
             #------------------------- ending the small calc
 
 
 
+
+
             #-----------------------------  DISPLAY AND UPDATE HISTO SECION ------------
             #-----------------------------  DISPLAY AND UPDATE HISTO SECION ------------
             #-----------------------------  DISPLAY AND UPDATE HISTO SECION ------------
             #-----------------------------  DISPLAY AND UPDATE HISTO SECION ------------
             #-----------------------------  DISPLAY AND UPDATE HISTO SECION ------------
             #  histograms that need to be updated online
 
@@ -391,31 +408,49 @@
                 fill_h_with_np(h1np,"rat",runtime.total_seconds(), limits_calib=limits_calib,title=spectrumname)  #
 
             if ROOT.gDirectory.FindObject("diff"):
                 fill_h_with_np(h1np_diff,"diff",deltat, limits_calib=limits_calib, title=spectrumname)  #
 
 
             if ROOT.gDirectory.FindObject("last"):
-                fill_h_with_np(h1np - h1np_old,"last", h1np_old_age,
+                fill_h_with_np(h1np - h1np_old,"last", h1np_last_interval,
                                limits_calib=limits_calib,
-                               title = f"last {h1np_old_age:.1f}s as rate {spectrumname}")  #
+                               title = f"last {h1np_last_interval:.1f}s as rate {spectrumname}")  #
 
             if ROOT.gDirectory.FindObject("sub"):
                 h1np_substr = h1np/runtime.total_seconds() - h1np_backg/h1np_backg_lt
                 errors = np.square( np.sqrt( h1np )/runtime.total_seconds() ) + np.square( np.sqrt(h1np_backg)/h1np_backg_lt )
                 errors = np.sqrt(errors)
                 fill_h_with_np(h1np_substr,"sub",None, errors=errors , limits_calib=limits_calib, title=spectrumname)  #
                 ##display_np( h1np_substr,  "substr", "c_substr", 1, errors)
 
 
             #if ROOT.gDirectory.FindObject("backg"):
             #    fill_h_with_np(histograms["backg"],"backg")  # No livetime here
 
+
+            INFLUX = True
+            if INFLUX and len(h1np_diff)>2:
+                just_spesum = h1np_diff[1:-1].sum()
+                # print(just_spesum, h1np_diff)
+                deadt = 0
+                if  just_spesum !=0:
+                    deadt = h1np_diff[0]/just_spesum*100
+                if is_float(rate) and is_float(deadt):
+                    infvals = f"rate_{spectrumname}={rate:.1f},deadt_{spectrumname}={deadt:.1f}"
+                    #print(infvals)
+                    influxwrite("test", f"greg",  infvals ) # hostname added automat
+
+
+
+
             # IN ANY CASE... REFRESH ALL CANVASES
             refresh_canvases()
+
+        # it was if fetch_flag............__________________________________________
         elif OFFLINE:
             refresh_canvases()
 
 
             #     print(f"i... new fetch: rate= {h1np_diff.sum()/deltat:.2f} (dt={deltat:.2f})")
 
             #--------------------------- influx stuff ---------------
@@ -441,15 +476,15 @@
             #if rate>0: # DONT SEND in the beginning (what about LARGE values?)
             #    if runtime.total_seconds()>1:
             #        msg = compose_udp( spectrumname, rate )
             #        udpsend( msg )
 
 
 
-
+        #=================================== FETCHING OR REFRESH IS DONE ==========
         # -- drop closed canvases:  name changes to c1, c1_n4... or somethnig
         for i in list(canvases.keys()):
             if i!=canvases[i].GetName():
                 canvases.pop(i,None)
 
         #---------------- HANDLE KEYBOARD -----------------------
         # the concept is
@@ -475,20 +510,23 @@
             #arg = key.split()[-1] # the last? NO. take all
             arg = " ".join(key.split()[1:]) # the last? NO. take all
             if cmd == arg:
                 arg=""
 
         # nospace multiletter cmd  d    v q
         if (arg=="") and (len(cmd)>0):
-            if cmd == "d": cmd = "dt"
-            if cmd[0] == "d": # for display
+            if cmd == "d":
+                #??
+                cmd = "d"  # total is default display
+                arg = "t"  # total is default display
+            elif cmd[0] == "d": # for display
                 arg = cmd[0:]
                 cmd = "d"
             if cmd[0] == "l": # for load
-                arg = cmd[1:]
+                arg = cmd[0:]
                 cmd = "l"
             print(f"i... cmd = {cmd} arg={arg}")
 
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
@@ -504,15 +542,15 @@
             nx=f"{fg.default}"
 
             yg=f"{bg.green}{fg.white}"
             ng=f"{bg.default}{fg.default}"
             print(f"""{yg}----HELP---------------------------------------{ng}
  {yy}h{ny} ... this help
  {yy}t{ny} ... set time of real spectrum: 't 1:59:59'
- {yy}a{ny} ... define age for the last histogram display 'a 3600'
+ {yy}a{ny} ... age AKA last_interval for the "last" histo : e.g. "a 3600"
  {yy}r{ny} ... range,pk search    {yy}R{ny} ... Record range, pks to DISK
  {yy}f{ny} ... fit
  {yy}c{ny} ... calib (energy)
  {yy}i{ny} ... info               {yy}v{ny} ... view histo details
  {yy}u{ny} ... unzoom             {yy}z{ny} ... zoom
  {yy}n{ny} ... next               {yy}p{ny} ... previous
  {yy}w{ny} ... window width
@@ -817,15 +855,15 @@
                     print("X... zoom's  energy is not float")
                 if middle is not None:
                     is_zoomed =[ True, middle ]
                     for i in histograms.keys():
                         histo_zoomenergy( histograms[i] ,
                                       is_zoomed[1] - config.CONFIG["window"]/2,
                                       is_zoomed[1] + config.CONFIG["window"]/2 )
-            elif is_zoomed[0]:
+            elif "is_zoomed" in globals() and is_zoomed[0]:
                 config.CONFIG["window"] = config.CONFIG["window"]/2
                 for i in histograms.keys():
                     histo_zoomenergy( histograms[i] ,
                                       is_zoomed[1] - config.CONFIG["window"]/2,
                                       is_zoomed[1] + config.CONFIG["window"]/2 )
 
 
@@ -884,15 +922,15 @@
                 #histo_details( histograms[ spectrumname] )
             print(f"i... canvases  : {list(canvases.keys())}")
             print(f"i... histograms:{list(histograms.keys())}")
 
 
         elif cmd == "t":   # ***CMD***  TIME ========== t time from start
             if  arg=="":
-                print("i... cmd t needs time")
+                print("i... cmd t needs time from start 3600s 1h 1:00:00")
                 continue
             arg = time2seconds(arg)
             print(f"i... arg: seconds == {arg} ")
             b0c01.set_started_before( arg) # ON "T" time
 
         elif cmd == "s":   # ***CMD*** #============= s save
             print("i... just save total")
@@ -905,26 +943,30 @@
 
         elif cmd == "a":   # ***CMD***  AGE ========== a age_of_diff histo
             if  arg=="":
                 print("i... cmd a needs time")
                 continue
             arg = time2seconds(arg)
             print(f"i... arg: seconds == {arg} / LAST {arg} seconds histogram ")
-            h1np_old_age = arg
+            h1np_last_interval = arg
 
 
         elif cmd == "d":   # ***CMD***  DISPL ============= d
             first_h = True # more histograms on the same canvas
 
+            # i blindly try
+            ROOT.gStyle.SetOptStat(1111111) # WORKS
+
             for ic in arg: # plot one by one
                 print("   i... interpretting display argument:",ic)
                 if "t" in ic: # TOTAL
                     display_np( h1np, "tot", "c_tot" , None , limits_calib=limits_calib)
                     first_h = False
 
+                # fast way to displ hists one by one
                 for ii in range(1,10):
                     if f"{ii}" in ic: #
                         #display_np( h1np, "s{ii}", "c_s{ii}" , None , limits_calib=limits_calib)
                         display_h_name(f"s{ii}", cname=f"c_s{ii}" , filled = True, color = ii+39)
                         first_h = False
 
 
@@ -969,26 +1011,26 @@
                         histograms["diff"].SetMarkerColor(8) # green2
                         histograms["diff"].SetMarkerStyle(7)
                         histograms["diff"].Draw("same EX0")
 
                 if "l" in ic: # RAte last
                     if first_h:
                         print("i... RATELAST histogram FIRST")
-                        display_np( h1np - h1np_old,  "last", "c_last", h1np_old_age,
+                        display_np( h1np - h1np_old,  "last", "c_last", h1np_last_interval,
                                     limits_calib=limits_calib, \
                                     filled=True, color = 46)
                         histograms["last"].SetLineColor(16)
                         histograms["last"].SetMarkerColor(46) # dark red
                         histograms["last"].SetMarkerStyle(7)
                         first_h = False
                     else:
                         print("i... RATELAST histogram ALSO")
-                        fill_h_with_np(h1np - h1np_old,"last", h1np_old_age,
+                        fill_h_with_np(h1np - h1np_old,"last", h1np_last_interval,
                                        limits_calib=limits_calib,
-                                       title = f"last {h1np_old_age:.1f}s as rate {spectrumname}")
+                                       title = f"last {h1np_last_interval:.1f}s as rate {spectrumname}")
                         #display_np( h1np_diff,  "diff", "c_diff", deltat)
                         histograms["last"].SetLineColor(16)
                         histograms["last"].SetMarkerColor(46) # green2
                         histograms["last"].SetMarkerStyle(7)
                         histograms["last"].Draw("same EX0")
 
 
@@ -1066,15 +1108,16 @@
 
 
         elif  cmd == "l":  # ***CMD***  LOAD ====== l
             if arg=="":
                 select_histo_to_load(  ) # load_txt()
                 print(f"i.. {fg.cyan} LOAD WITH NUMBER like:    l1  l2 l3 ...  {fg.default}")
             else:
-                select_histo_to_load( arg[0] ) # load_txt()
+                for ii in arg:
+                    select_histo_to_load( ii ) # load_txt() # all that are given in argument l67
             #continue # arg="bg"
             # #-------------standard manipulation:  _lt...txt
             # lis = glob.glob(f"{arg}_lt*_a*_b*.txt")
             # filename = ""
             # print(lis)
             # if len(lis)>0:
             #     filename = lis[0]
@@ -1132,27 +1175,33 @@
         #=============================================================END OF COMMMANDS==========
         #=============================================================END OF COMMMANDS==========
         #=============================================================END OF COMMMANDS==========
 
         # why here?
         top.place()
 
+        # total histogram time
         rdays = runtime.days# floor(runtime.total_seconds()/3600/24)
         rhours = floor(runtime.seconds/3600)
         rminsec = runtime.total_seconds() - (rdays*24+rhours)*3600
         rminu = floor(rminsec/60)
         rsec = int(rminsec - rminu*60)
+
+        # total histogram time
         rditime = f"{rdays*24+rhours:03d}:{rminu:02d}:{rsec:02d}"
         # was ....RUN= str(runtime)[0:10]
 
-        prima = str(dt.datetime.now())[:-5]
-        prima = f"{bg.green}{fg.white}{fx.bold}{spectrumname}{fg.default}{bg.blue}"
+        # prima = str(dt.datetime.now())[:-5]
+        if OFFLINE:
+            prima = f"{bg.green}{fg.white}{fx.bold}OFFLINE{fg.default}{bg.blue}"
+        else:
+            prima = f"{bg.green}{fg.white}{fx.bold}{spectrumname}{fg.default}{bg.blue}"
 
 
-        top.print_to( 0, f" {prima} {fg.white}{fx.bold} dt={deltat:.2f} sec. {fg.yellow} rate={rate:7.1f} {fg.white} RUN={rditime} MEM={lenhistos:4}  D[{h1np_old_age:.0f}s]={warn_del} {dage:.2f} {unwarn_del} {fg.default}" )
+        top.print_to( 0, f" {prima} {fg.white}{fx.bold} dt={deltat:.2f} sec. {fg.yellow} rate={rate:7.1f} {fg.white} RUN={rditime} MEM={lenhistos:4}  D[{h1np_last_interval:.0f}s]={warn_del} {d_last_interval:.2f} {unwarn_del} {fg.default}" )
 
         if len(key)==0:
             top2.print_to( 0, f"{fg.cyan}{bg.black}{' '*80}{bg.black}")
         else:
             top2.print_to( 0, f"{fg.white}{bg.red} > {fx.bold}{a_abc}{fg.yellow}_{fg.white}{b_abc}{fx.default}{fg.default}{bg.default} ")
         #top.place()
```

### Comparing `gregory_online-0.2.3/gregory_online/config.py` & `gregory_online-0.2.4/gregory_online/config.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.3/gregory_online/fetchnp.py` & `gregory_online-0.2.4/gregory_online/fetchnp.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     def get_lenhistos(self):
         return len(self.histos)
 
     def get_limits_calib(self):
         return self.xmin,self.xmax
 
 
-    def get_old_histo(self, age):
+    def get_partial_time_histo(self, age):
         ele=None
         dist=999999
         #print(f"D... demanded age = {age}")
         for k in self.histos.keys():
             if ele is None: ele = k
             agedif = abs(self.histos[k][0] - age)
             #print(f"D... {k} - histo = {self.histos[k]}")
@@ -127,14 +127,15 @@
 
     def get_runtime(self):
         #print( "D... get runtime:", self.runtime, type(self.runtime)  )
         # print(f"D... realtime in get_runtime  = {self.realtime}")
         if type(self.runtime) is dt.timedelta:
             if self.runtime.total_seconds()<=0:
                 self.runtime = dt.timedelta(seconds=1)
+
         if self.realtime is not None: # TITLE is used .....
             #print( "D... realtime=", self.realtime  ,   self.runtime )
             if abs(self.realtime  -self.runtime.total_seconds() )>15: # DEIFFERENCE 15 seconds ........
                 print(f"{fg.red}START TIME RESET !!!!!!!!!!{fg.default}")
                 self.set_started_before( self.realtime ) # RESET RUNTIME, SINCE THERE IS A 15s difference
             return dt.timedelta( seconds=self.realtime ) # taken from TITLE
         else:
@@ -187,29 +188,33 @@
         if not ok :
             print(f"!... no connection {self.url}")
             return False
 
         jhis = json.loads(jhis)
         # dict_keys(['_typename', 'fUniqueID', 'fBits', 'fName', 'fTitle', 'fLineColor', 'fLineStyle', 'fLineWidth', 'fFillColor', 'fFillStyle', 'fMarkerColor', 'fMarkerStyle', 'fMarkerSize', 'fNcells', 'fXaxis', 'fYaxis', 'fZaxis', 'fBarOffset', 'fBarWidth', 'fEntries', 'fTsumw', 'fTsumw2', 'fTsumwx', 'fTsumwx2', 'fMaximum', 'fMinimum', 'fNormFactor', 'fContour', 'fSumw2', 'fOption', 'fFunctions', 'fBufferSize', 'fBuffer', 'fBinStatErrOpt', 'fStatOverflows', 'fArray'])
 
+
         #print(jhis.keys() )
-        #print( jhis["fTitle"])
-        grp = re.search(r'rt=([\d\.]+)$',jhis["fTitle"])
-        # print(grp)
 
+        # print( jhis["fTitle"])
+
+        grp = re.search(r'rt=([\d\.]+)$',jhis["fTitle"])  # rt=3600 at the END of title ...
+        # print(grp)
         if grp is not None and len(grp.groups())>0:
             self.realtime = float(grp.groups()[0].split("=")[-1])
             #print( f" realtime from title grp ={self.realtime}" )
 
         self.xmin = jhis['fXaxis']['fXmin']
         self.xmax = jhis['fXaxis']['fXmax']
 
-
+        #print( jhis.keys() )
         helem = jhis['fArray']
 
+        #print(len(helem) , helem[0], helem[-1] )
+
         self.h1np_prev = 1.0*self.h1np # save  previous
         self.h1np = np.array( helem )
 
         #---------protection in case of  reset
         if self.h1np.sum()< self.h1np_prev.sum():
             print(f"i... {fg.red}RESET? I CLEAN THE PREV. HISTOGRAM{fg.default}")
             self.h1np_prev = self.h1np_prev*0
```

### Comparing `gregory_online-0.2.3/gregory_online/histo_analyze.py` & `gregory_online-0.2.4/gregory_online/histo_analyze.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.3/gregory_online/histo_displ.py` & `gregory_online-0.2.4/gregory_online/histo_displ.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.3/gregory_online/histo_global_cont.py` & `gregory_online-0.2.4/gregory_online/histo_global_cont.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.3/gregory_online/histo_io.py` & `gregory_online-0.2.4/gregory_online/histo_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 #!/usr/bin/env python3
 """
 load and save operations
 * load a textfile with LT A and B given in the filename
-* verify under/overfl
+* verify under/overfl bin present
+____
+* definition of .details file INSIDE save_hist_txt
+* real usage of .details file in     load_hist_txt with load_details
+ : these are used in load_hist_txt
+ - livetime
+ - a
+ - b
+ - entries
+ - rate
 """
 from fire import Fire
 
 import glob
 
 from gregory_online.histo_global_cont import histograms
 
@@ -165,21 +174,26 @@
         print("X... no spectrum selected")
     if num in avadisc.keys():
         load_hist_txt( avadisc[num] , f"s{num}" )
 
 
 # ----------------------------------- loading spectra/histogram
 
-def load_details(fname):
+def load_details(fname):   # used in load_hist_txt: where histograms[hname] is created
+                           # and rate interpretted
     res = None
     if os.path.exists(fname):
         with open(fname) as f:
             res = f.readlines()
         res = [ (x.strip().split(" ")[0],"_".join(x.strip().split(" ")[1:])) for x in res]
         res = dict(res)
+
+        # the following are gonna be converted and cause a crash if error
+        res["totaltime"] = float(res["totaltime"]) # not always needed?
+        # not floatres["started"] = float(res["started"]) # not always needed
         res["livetime"] = float(res["livetime"])
         res["a"] = float(res["a"])
         res["b"] = float(res["b"])
         res["entries"] = float(res["entries"])
         res["rate"] = float(res["rate"])
     return res
```

### Comparing `gregory_online-0.2.3/gregory_online/histo_np_ops.py` & `gregory_online-0.2.4/gregory_online/histo_np_ops.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.3/gregory_online/key_enter.py` & `gregory_online-0.2.4/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.3/gregory_online/topbar.py` & `gregory_online-0.2.4/gregory_online/topbar.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.3/gregory_online/utils.py` & `gregory_online-0.2.4/gregory_online/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,30 +7,38 @@
 from pyfromroot import  prun
 from console import fg,bg
 
 import os
 
 #
 #  taken from flashcam and stackoveerflow
+import math
 
 def is_int(n):
+    if n is None or math.isnan(n):
+        return False
     try:
         float_n = float(n)
         int_n = int(float_n)
     except ValueError:
         return False
     else:
         return float_n == int_n
 
 def is_float(n):
     try:
         float_n = float(n)
+        #print(n, float_n)
     except ValueError:
         return False
     else:
+        #print("true block", n)
+        if n is None or math.isnan(n):
+            #print("NONE")
+            return False
         return True
 
 def is_bool(n):
     if type(n) is str and n=="False": return True
     if type(n) is str and n=="True": return True
     return False
```

### Comparing `gregory_online-0.2.3/gregory_online.egg-info/SOURCES.txt` & `gregory_online-0.2.4/gregory_online.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.3/setup.py` & `gregory_online-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     license="GPL2",
     version=get_version("gregory_online/version.py"),
     packages=['gregory_online'],
     package_data={'gregory_online': ['data/*']},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     scripts = ['bin/gregory_online'],
-    install_requires = ['fire','scipy','pyfromroot','pytermgui','readchar','fastnumbers'],
+    install_requires = ['fire','scipy','pyfromroot','pytermgui','readchar','fastnumbers','sshkeyboard'],
 )
```

