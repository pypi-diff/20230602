# Comparing `tmp/dupechecker-0.2.0.tar.gz` & `tmp/dupechecker-0.2.1.tar.gz`

## Comparing `dupechecker-0.2.0.tar` & `dupechecker-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dupechecker-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 dupechecker-0.2.0/docs/dupechecker.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-0.2.0/docs/index.html
--rw-r--r--   0        0        0    23051 2020-02-02 00:00:00.000000 dupechecker-0.2.0/docs/search.js
--rw-r--r--   0        0        0   107454 2020-02-02 00:00:00.000000 dupechecker-0.2.0/docs/dupechecker/dupechecker.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dupechecker-0.2.0/src/dupechecker/__init__.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 dupechecker-0.2.0/src/dupechecker/dupechecker.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-0.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 dupechecker-0.2.0/README.md
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dupechecker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 dupechecker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dupechecker-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 dupechecker-0.2.1/docs/dupechecker.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-0.2.1/docs/index.html
+-rw-r--r--   0        0        0    23051 2020-02-02 00:00:00.000000 dupechecker-0.2.1/docs/search.js
+-rw-r--r--   0        0        0   110839 2020-02-02 00:00:00.000000 dupechecker-0.2.1/docs/dupechecker/dupechecker.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dupechecker-0.2.1/src/dupechecker/__init__.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 dupechecker-0.2.1/src/dupechecker/dupechecker.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 dupechecker-0.2.1/README.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dupechecker-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 dupechecker-0.2.1/PKG-INFO
```

### Comparing `dupechecker-0.2.0/docs/dupechecker.html` & `dupechecker-0.2.1/docs/dupechecker.html`

 * *Files identical despite different names*

### Comparing `dupechecker-0.2.0/docs/search.js` & `dupechecker-0.2.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `dupechecker-0.2.0/docs/dupechecker/dupechecker.html` & `dupechecker-0.2.1/docs/dupechecker/dupechecker.html`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
                         <label class="view-source-button" for="mod-dupechecker-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">filecmp</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">time</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">concurrent.futures</span> <span class="kn">import</span> <span class="n">ThreadPoolExecutor</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">itertools</span> <span class="kn">import</span> <span class="n">combinations</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">copy</span> <span class="kn">import</span> <span class="n">deepcopy</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">griddle</span> <span class="kn">import</span> <span class="n">griddy</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">printbuddies</span> <span class="kn">import</span> <span class="n">Spinner</span>
 </span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">younotyou</span> <span class="kn">import</span> <span class="n">younotyou</span>
 </span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
 </span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
@@ -147,77 +147,87 @@
 </span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
 </span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Gathering files...&quot;</span><span class="p">)</span>
 </span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
 </span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
 </span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>            <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
 </span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="p">)</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="n">younotyou</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span><span class="p">)</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="n">num_comparisons</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">combinations</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">,</span> <span class="mi">2</span><span class="p">)))</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Making </span><span class="si">{</span><span class="n">num_comparisons</span><span class="si">}</span><span class="s2"> comparisons between </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="p">)</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="p">]</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="n">dupechecker</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">younotyou</span><span class="p">(</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="p">)</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="p">]</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Comparing </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="p">)</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="p">]</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">deepcopy</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">))</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>                <span class="n">griddy</span><span class="p">(</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                    <span class="p">[[</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">])]</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                <span class="p">)</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="p">)</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="k">lambda</span><span class="p">:</span> <span class="nb">sum</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="n">start_size</span> <span class="o">=</span> <span class="n">size</span><span class="p">()</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">start_size</span> <span class="o">-</span> <span class="n">size</span><span class="p">()</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="n">dupechecker</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_duplicates">
                             <input id="get_duplicates-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -315,19 +325,23 @@
 </span><span id="get_args-80"><a href="#get_args-80"><span class="linenos">80</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
 </span><span id="get_args-81"><a href="#get_args-81"><span class="linenos">81</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="get_args-82"><a href="#get_args-82"><span class="linenos">82</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Gathering files...&quot;</span><span class="p">)</span>
 </span><span id="get_args-83"><a href="#get_args-83"><span class="linenos">83</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
 </span><span id="get_args-84"><a href="#get_args-84"><span class="linenos">84</span></a>        <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
 </span><span id="get_args-85"><a href="#get_args-85"><span class="linenos">85</span></a>            <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
 </span><span id="get_args-86"><a href="#get_args-86"><span class="linenos">86</span></a>        <span class="p">)</span>
-</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos">87</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="n">younotyou</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span><span class="p">)</span>
-</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos">88</span></a>    <span class="n">num_comparisons</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">combinations</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">,</span> <span class="mi">2</span><span class="p">)))</span>
-</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos">89</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Making </span><span class="si">{</span><span class="n">num_comparisons</span><span class="si">}</span><span class="s2"> comparisons between </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
-</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos">90</span></a>
-</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos">91</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos">87</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos">88</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos">89</span></a>        <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">younotyou</span><span class="p">(</span>
+</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos">90</span></a>            <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span>
+</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos">91</span></a>        <span class="p">)</span>
+</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos">92</span></a>    <span class="p">]</span>
+</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos">93</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Comparing </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
+</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos">94</span></a>
+</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos">95</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="delete_wizard">
@@ -337,29 +351,30 @@
         <span class="def">def</span>
         <span class="name">delete_wizard</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="delete_wizard-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_wizard"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_wizard-94"><a href="#delete_wizard-94"><span class="linenos"> 94</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="delete_wizard-95"><a href="#delete_wizard-95"><span class="linenos"> 95</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
-</span><span id="delete_wizard-96"><a href="#delete_wizard-96"><span class="linenos"> 96</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="delete_wizard-97"><a href="#delete_wizard-97"><span class="linenos"> 97</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
-</span><span id="delete_wizard-98"><a href="#delete_wizard-98"><span class="linenos"> 98</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="delete_wizard-99"><a href="#delete_wizard-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
-</span><span id="delete_wizard-100"><a href="#delete_wizard-100"><span class="linenos">100</span></a>    <span class="p">)</span>
-</span><span id="delete_wizard-101"><a href="#delete_wizard-101"><span class="linenos">101</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="delete_wizard-102"><a href="#delete_wizard-102"><span class="linenos">102</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="delete_wizard-103"><a href="#delete_wizard-103"><span class="linenos">103</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
-</span><span id="delete_wizard-104"><a href="#delete_wizard-104"><span class="linenos">104</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="delete_wizard-105"><a href="#delete_wizard-105"><span class="linenos">105</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
-</span><span id="delete_wizard-106"><a href="#delete_wizard-106"><span class="linenos">106</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
-</span><span id="delete_wizard-107"><a href="#delete_wizard-107"><span class="linenos">107</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
-</span><span id="delete_wizard-108"><a href="#delete_wizard-108"><span class="linenos">108</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_wizard-98"><a href="#delete_wizard-98"><span class="linenos"> 98</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="delete_wizard-99"><a href="#delete_wizard-99"><span class="linenos"> 99</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
+</span><span id="delete_wizard-100"><a href="#delete_wizard-100"><span class="linenos">100</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="delete_wizard-101"><a href="#delete_wizard-101"><span class="linenos">101</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
+</span><span id="delete_wizard-102"><a href="#delete_wizard-102"><span class="linenos">102</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="delete_wizard-103"><a href="#delete_wizard-103"><span class="linenos">103</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
+</span><span id="delete_wizard-104"><a href="#delete_wizard-104"><span class="linenos">104</span></a>    <span class="p">)</span>
+</span><span id="delete_wizard-105"><a href="#delete_wizard-105"><span class="linenos">105</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="delete_wizard-106"><a href="#delete_wizard-106"><span class="linenos">106</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="delete_wizard-107"><a href="#delete_wizard-107"><span class="linenos">107</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
+</span><span id="delete_wizard-108"><a href="#delete_wizard-108"><span class="linenos">108</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="delete_wizard-109"><a href="#delete_wizard-109"><span class="linenos">109</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
+</span><span id="delete_wizard-110"><a href="#delete_wizard-110"><span class="linenos">110</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
+</span><span id="delete_wizard-111"><a href="#delete_wizard-111"><span class="linenos">111</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
+</span><span id="delete_wizard-112"><a href="#delete_wizard-112"><span class="linenos">112</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+</span><span id="delete_wizard-113"><a href="#delete_wizard-113"><span class="linenos">113</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Ask which file to keep for each set.</p>
 </div>
 
 
@@ -371,19 +386,19 @@
         <span class="def">def</span>
         <span class="name">autodelete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="autodelete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#autodelete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="autodelete-111"><a href="#autodelete-111"><span class="linenos">111</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="autodelete-112"><a href="#autodelete-112"><span class="linenos">112</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
-</span><span id="autodelete-113"><a href="#autodelete-113"><span class="linenos">113</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="autodelete-114"><a href="#autodelete-114"><span class="linenos">114</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="autodelete-115"><a href="#autodelete-115"><span class="linenos">115</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="autodelete-116"><a href="#autodelete-116"><span class="linenos">116</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="autodelete-117"><a href="#autodelete-117"><span class="linenos">117</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
+</span><span id="autodelete-118"><a href="#autodelete-118"><span class="linenos">118</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="autodelete-119"><a href="#autodelete-119"><span class="linenos">119</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="autodelete-120"><a href="#autodelete-120"><span class="linenos">120</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Keep one of each set in <code>matches</code> and delete the others.</p>
 </div>
 
 
@@ -395,42 +410,47 @@
         <span class="def">def</span>
         <span class="name">dupechecker</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="dupechecker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#dupechecker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="dupechecker-118"><a href="#dupechecker-118"><span class="linenos">118</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="dupechecker-119"><a href="#dupechecker-119"><span class="linenos">119</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="dupechecker-120"><a href="#dupechecker-120"><span class="linenos">120</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="dupechecker-121"><a href="#dupechecker-121"><span class="linenos">121</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="dupechecker-122"><a href="#dupechecker-122"><span class="linenos">122</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="dupechecker-123"><a href="#dupechecker-123"><span class="linenos">123</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="dupechecker-124"><a href="#dupechecker-124"><span class="linenos">124</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
-</span><span id="dupechecker-125"><a href="#dupechecker-125"><span class="linenos">125</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
-</span><span id="dupechecker-126"><a href="#dupechecker-126"><span class="linenos">126</span></a>    <span class="p">]</span>
-</span><span id="dupechecker-127"><a href="#dupechecker-127"><span class="linenos">127</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="dupechecker-128"><a href="#dupechecker-128"><span class="linenos">128</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
-</span><span id="dupechecker-129"><a href="#dupechecker-129"><span class="linenos">129</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
-</span><span id="dupechecker-130"><a href="#dupechecker-130"><span class="linenos">130</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>
-</span><span id="dupechecker-131"><a href="#dupechecker-131"><span class="linenos">131</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
-</span><span id="dupechecker-132"><a href="#dupechecker-132"><span class="linenos">132</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
-</span><span id="dupechecker-133"><a href="#dupechecker-133"><span class="linenos">133</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
-</span><span id="dupechecker-134"><a href="#dupechecker-134"><span class="linenos">134</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
-</span><span id="dupechecker-135"><a href="#dupechecker-135"><span class="linenos">135</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="dupechecker-136"><a href="#dupechecker-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
-</span><span id="dupechecker-137"><a href="#dupechecker-137"><span class="linenos">137</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
-</span><span id="dupechecker-138"><a href="#dupechecker-138"><span class="linenos">138</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
-</span><span id="dupechecker-139"><a href="#dupechecker-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
-</span><span id="dupechecker-140"><a href="#dupechecker-140"><span class="linenos">140</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="dupechecker-141"><a href="#dupechecker-141"><span class="linenos">141</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
-</span><span id="dupechecker-142"><a href="#dupechecker-142"><span class="linenos">142</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="dupechecker-143"><a href="#dupechecker-143"><span class="linenos">143</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="dupechecker-144"><a href="#dupechecker-144"><span class="linenos">144</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="dupechecker-145"><a href="#dupechecker-145"><span class="linenos">145</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="dupechecker-123"><a href="#dupechecker-123"><span class="linenos">123</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="dupechecker-124"><a href="#dupechecker-124"><span class="linenos">124</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="dupechecker-125"><a href="#dupechecker-125"><span class="linenos">125</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="dupechecker-126"><a href="#dupechecker-126"><span class="linenos">126</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="dupechecker-127"><a href="#dupechecker-127"><span class="linenos">127</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="dupechecker-128"><a href="#dupechecker-128"><span class="linenos">128</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="dupechecker-129"><a href="#dupechecker-129"><span class="linenos">129</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
+</span><span id="dupechecker-130"><a href="#dupechecker-130"><span class="linenos">130</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
+</span><span id="dupechecker-131"><a href="#dupechecker-131"><span class="linenos">131</span></a>    <span class="p">]</span>
+</span><span id="dupechecker-132"><a href="#dupechecker-132"><span class="linenos">132</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="dupechecker-133"><a href="#dupechecker-133"><span class="linenos">133</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
+</span><span id="dupechecker-134"><a href="#dupechecker-134"><span class="linenos">134</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
+</span><span id="dupechecker-135"><a href="#dupechecker-135"><span class="linenos">135</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">deepcopy</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">))</span>
+</span><span id="dupechecker-136"><a href="#dupechecker-136"><span class="linenos">136</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
+</span><span id="dupechecker-137"><a href="#dupechecker-137"><span class="linenos">137</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</span><span id="dupechecker-138"><a href="#dupechecker-138"><span class="linenos">138</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
+</span><span id="dupechecker-139"><a href="#dupechecker-139"><span class="linenos">139</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
+</span><span id="dupechecker-140"><a href="#dupechecker-140"><span class="linenos">140</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="dupechecker-141"><a href="#dupechecker-141"><span class="linenos">141</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
+</span><span id="dupechecker-142"><a href="#dupechecker-142"><span class="linenos">142</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
+</span><span id="dupechecker-143"><a href="#dupechecker-143"><span class="linenos">143</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="dupechecker-144"><a href="#dupechecker-144"><span class="linenos">144</span></a>                <span class="n">griddy</span><span class="p">(</span>
+</span><span id="dupechecker-145"><a href="#dupechecker-145"><span class="linenos">145</span></a>                    <span class="p">[[</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">])]</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="dupechecker-146"><a href="#dupechecker-146"><span class="linenos">146</span></a>                <span class="p">)</span>
+</span><span id="dupechecker-147"><a href="#dupechecker-147"><span class="linenos">147</span></a>            <span class="p">)</span>
+</span><span id="dupechecker-148"><a href="#dupechecker-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
+</span><span id="dupechecker-149"><a href="#dupechecker-149"><span class="linenos">149</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="k">lambda</span><span class="p">:</span> <span class="nb">sum</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="dupechecker-150"><a href="#dupechecker-150"><span class="linenos">150</span></a>            <span class="n">start_size</span> <span class="o">=</span> <span class="n">size</span><span class="p">()</span>
+</span><span id="dupechecker-151"><a href="#dupechecker-151"><span class="linenos">151</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
+</span><span id="dupechecker-152"><a href="#dupechecker-152"><span class="linenos">152</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">start_size</span> <span class="o">-</span> <span class="n">size</span><span class="p">()</span>
+</span><span id="dupechecker-153"><a href="#dupechecker-153"><span class="linenos">153</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="dupechecker-154"><a href="#dupechecker-154"><span class="linenos">154</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="dupechecker-155"><a href="#dupechecker-155"><span class="linenos">155</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 
 ****** dupechecker.dupechecker ******
 ⁰ View Source
 __1import argparse
 __2import filecmp
 __3import time
 __4from concurrent.futures import ThreadPoolExecutor
-__5from itertools import combinations
+__5from copy import deepcopy
 __6
 __7from griddle import griddy
 __8from pathier import Pathier
 __9from printbuddies import Spinner
 _10from younotyou import younotyou
 _11
 _12
@@ -99,83 +99,93 @@
 _80    files = []
 _81    print("Gathering files...")
 _82    for path in args.paths:
 _83        files.extend(
 _84            list(path.rglob("*.*")) if args.recursive else list(path.glob
 ("*.*"))
 _85        )
-_86    args.paths = younotyou([str(file) for file in files],
-exclude_patterns=args.ignores)
-_87    num_comparisons = len(list(combinations(args.paths, 2)))
-_88    print(f"Making {num_comparisons} comparisons between {len(args.paths)}
-files...")
-_89
-_90    return args
-_91
-_92
-_93def delete_wizard(matches: list[list[Pathier]]):
-_94    """Ask which file to keep for each set."""
-_95    print()
-_96    print("Enter the corresponding number of the file to keep.")
-_97    print(
-_98        "Press 'Enter' without giving a number to skip deleting any files
+_86    args.paths = [
+_87        Pathier(path)
+_88        for path in younotyou(
+_89            [str(file) for file in files], exclude_patterns=args.ignores
+_90        )
+_91    ]
+_92    print(f"Comparing {len(args.paths)} files...")
+_93
+_94    return args
+_95
+_96
+_97def delete_wizard(matches: list[list[Pathier]]):
+_98    """Ask which file to keep for each set."""
+_99    print()
+100    print("Enter the corresponding number of the file to keep.")
+101    print(
+102        "Press 'Enter' without giving a number to skip deleting any files
 for the given set."
-_99    )
-100    print()
-101    for match in matches:
-102        map_ = {str(i): file for i, file in enumerate(match, 1)}
-103        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
+103    )
+104    print()
+105    for match in matches:
+106        map_ = {str(i): file for i, file in enumerate(match, 1)}
+107        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
 "\n"
-104        print(options)
-105        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
+108        print(options)
+109        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
 ())}): ")
-106        if keeper:
-107            [map_[num].delete() for num in map_ if num != keeper]
-108
-109
-110def autodelete(matches: list[list[Pathier]]):
-111    """Keep one of each set in `matches` and delete the others."""
-112    for match in matches:
-113        match.pop()
-114        [file.delete() for file in match]
-115
-116
-117def dupechecker(args: argparse.Namespace | None = None):
-118    print()
-119    if not args:
-120        args = get_args()
-121    s = [
-122        ch.rjust(i + j)
-123        for i in range(1, 25, 3)
-124        for j, ch in enumerate(["/", "-", "\\"])
-125    ]
-126    s += s[::-1]
-127    with Spinner(s) as spinner:
-128        with ThreadPoolExecutor() as exc:
-129            thread = exc.submit(get_duplicates, args.paths)
-130            while not thread.done():
-131                spinner.display()
-132                time.sleep(0.025)
-133            matches = thread.result()
-134    if matches:
-135        print(f"Found {len(matches)} duplicate sets of files.")
-136        if not args.no_show:
-137            print(griddy(matches))
-138        if args.delete_dupes or args.autodelete:
-139            size = args.path.size()
-140            delete_wizard(matches) if args.delete_dupes else autodelete
+110        if keeper:
+111            [map_[num].delete() for num in map_ if num != keeper]
+112        print()
+113
+114
+115def autodelete(matches: list[list[Pathier]]):
+116    """Keep one of each set in `matches` and delete the others."""
+117    for match in matches:
+118        match.pop()
+119        [file.delete() for file in match]
+120
+121
+122def dupechecker(args: argparse.Namespace | None = None):
+123    print()
+124    if not args:
+125        args = get_args()
+126    s = [
+127        ch.rjust(i + j)
+128        for i in range(1, 25, 3)
+129        for j, ch in enumerate(["/", "-", "\\"])
+130    ]
+131    s += s[::-1]
+132    with Spinner(s) as spinner:
+133        with ThreadPoolExecutor() as exc:
+134            thread = exc.submit(get_duplicates, deepcopy(args.paths))
+135            while not thread.done():
+136                spinner.display()
+137                time.sleep(0.025)
+138            matches = thread.result()
+139    if matches:
+140        print(f"Found {len(matches)} duplicate sets of files.")
+141        if not args.no_show:
+142            print(
+143                griddy(
+144                    [["\n".join([str(file) for file in match])] for match in
+matches]
+145                )
+146            )
+147        if args.delete_dupes or args.autodelete:
+148            size = lambda: sum(path.size() for path in args.paths)  # type:
+ignore
+149            start_size = size()
+150            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
-141            deleted_size = size - args.path.size()
-142            print(f"Deleted {Pathier.format_size(deleted_size)}.")
-143    else:
-144        print("No duplicates detected.")
-145
-146
-147if __name__ == "__main__":
-148    dupechecker(get_args())
+151            deleted_size = start_size - size()
+152            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+153    else:
+154        print("No duplicates detected.")
+155
+156
+157if __name__ == "__main__":
+158    dupechecker(get_args())
   ⁰
 def get_duplicates(
 paths: list[pathier.pathier.Pathier]) -> list[list[pathier.pathier.Pathier]]:
 View Source
 14def get_duplicates(paths: list[Pathier]) -> list[list[Pathier]]:
 15    """Return a list of lists for duplicate files in `paths`."""
 16    matching_sets = []
@@ -252,75 +262,85 @@
 81    files = []
 82    print("Gathering files...")
 83    for path in args.paths:
 84        files.extend(
 85            list(path.rglob("*.*")) if args.recursive else list(path.glob
 ("*.*"))
 86        )
-87    args.paths = younotyou([str(file) for file in files],
-exclude_patterns=args.ignores)
-88    num_comparisons = len(list(combinations(args.paths, 2)))
-89    print(f"Making {num_comparisons} comparisons between {len(args.paths)}
-files...")
-90
-91    return args
+87    args.paths = [
+88        Pathier(path)
+89        for path in younotyou(
+90            [str(file) for file in files], exclude_patterns=args.ignores
+91        )
+92    ]
+93    print(f"Comparing {len(args.paths)} files...")
+94
+95    return args
   ⁰
 def delete_wizard(matches: list[list[pathier.pathier.Pathier]]): View Source
-_94def delete_wizard(matches: list[list[Pathier]]):
-_95    """Ask which file to keep for each set."""
-_96    print()
-_97    print("Enter the corresponding number of the file to keep.")
-_98    print(
-_99        "Press 'Enter' without giving a number to skip deleting any files
+_98def delete_wizard(matches: list[list[Pathier]]):
+_99    """Ask which file to keep for each set."""
+100    print()
+101    print("Enter the corresponding number of the file to keep.")
+102    print(
+103        "Press 'Enter' without giving a number to skip deleting any files
 for the given set."
-100    )
-101    print()
-102    for match in matches:
-103        map_ = {str(i): file for i, file in enumerate(match, 1)}
-104        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
+104    )
+105    print()
+106    for match in matches:
+107        map_ = {str(i): file for i, file in enumerate(match, 1)}
+108        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
 "\n"
-105        print(options)
-106        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
+109        print(options)
+110        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
 ())}): ")
-107        if keeper:
-108            [map_[num].delete() for num in map_ if num != keeper]
+111        if keeper:
+112            [map_[num].delete() for num in map_ if num != keeper]
+113        print()
 Ask which file to keep for each set.
   ⁰
 def autodelete(matches: list[list[pathier.pathier.Pathier]]): View Source
-111def autodelete(matches: list[list[Pathier]]):
-112    """Keep one of each set in `matches` and delete the others."""
-113    for match in matches:
-114        match.pop()
-115        [file.delete() for file in match]
+116def autodelete(matches: list[list[Pathier]]):
+117    """Keep one of each set in `matches` and delete the others."""
+118    for match in matches:
+119        match.pop()
+120        [file.delete() for file in match]
 Keep one of each set in matches and delete the others.
   ⁰
 def dupechecker(args: argparse.Namespace | None = None): View Source
-118def dupechecker(args: argparse.Namespace | None = None):
-119    print()
-120    if not args:
-121        args = get_args()
-122    s = [
-123        ch.rjust(i + j)
-124        for i in range(1, 25, 3)
-125        for j, ch in enumerate(["/", "-", "\\"])
-126    ]
-127    s += s[::-1]
-128    with Spinner(s) as spinner:
-129        with ThreadPoolExecutor() as exc:
-130            thread = exc.submit(get_duplicates, args.paths)
-131            while not thread.done():
-132                spinner.display()
-133                time.sleep(0.025)
-134            matches = thread.result()
-135    if matches:
-136        print(f"Found {len(matches)} duplicate sets of files.")
-137        if not args.no_show:
-138            print(griddy(matches))
-139        if args.delete_dupes or args.autodelete:
-140            size = args.path.size()
-141            delete_wizard(matches) if args.delete_dupes else autodelete
+123def dupechecker(args: argparse.Namespace | None = None):
+124    print()
+125    if not args:
+126        args = get_args()
+127    s = [
+128        ch.rjust(i + j)
+129        for i in range(1, 25, 3)
+130        for j, ch in enumerate(["/", "-", "\\"])
+131    ]
+132    s += s[::-1]
+133    with Spinner(s) as spinner:
+134        with ThreadPoolExecutor() as exc:
+135            thread = exc.submit(get_duplicates, deepcopy(args.paths))
+136            while not thread.done():
+137                spinner.display()
+138                time.sleep(0.025)
+139            matches = thread.result()
+140    if matches:
+141        print(f"Found {len(matches)} duplicate sets of files.")
+142        if not args.no_show:
+143            print(
+144                griddy(
+145                    [["\n".join([str(file) for file in match])] for match in
+matches]
+146                )
+147            )
+148        if args.delete_dupes or args.autodelete:
+149            size = lambda: sum(path.size() for path in args.paths)  # type:
+ignore
+150            start_size = size()
+151            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
-142            deleted_size = size - args.path.size()
-143            print(f"Deleted {Pathier.format_size(deleted_size)}.")
-144    else:
-145        print("No duplicates detected.")
+152            deleted_size = start_size - size()
+153            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+154    else:
+155        print("No duplicates detected.")
```

### Comparing `dupechecker-0.2.0/src/dupechecker/dupechecker.py` & `dupechecker-0.2.1/src/dupechecker/dupechecker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import filecmp
 import time
 from concurrent.futures import ThreadPoolExecutor
-from itertools import combinations
+from copy import deepcopy
 
 from griddle import griddy
 from pathier import Pathier
 from printbuddies import Spinner
 from younotyou import younotyou
 
 
@@ -79,17 +79,21 @@
         args.paths = [Pathier(path) for path in args.paths]
     files = []
     print("Gathering files...")
     for path in args.paths:
         files.extend(
             list(path.rglob("*.*")) if args.recursive else list(path.glob("*.*"))
         )
-    args.paths = younotyou([str(file) for file in files], exclude_patterns=args.ignores)
-    num_comparisons = len(list(combinations(args.paths, 2)))
-    print(f"Making {num_comparisons} comparisons between {len(args.paths)} files...")
+    args.paths = [
+        Pathier(path)
+        for path in younotyou(
+            [str(file) for file in files], exclude_patterns=args.ignores
+        )
+    ]
+    print(f"Comparing {len(args.paths)} files...")
 
     return args
 
 
 def delete_wizard(matches: list[list[Pathier]]):
     """Ask which file to keep for each set."""
     print()
@@ -101,14 +105,15 @@
     for match in matches:
         map_ = {str(i): file for i, file in enumerate(match, 1)}
         options = "\n".join(f"({i}) {file}" for i, file in map_.items()) + "\n"
         print(options)
         keeper = input(f"Enter number of file to keep ({', '.join(map_.keys())}): ")
         if keeper:
             [map_[num].delete() for num in map_ if num != keeper]
+        print()
 
 
 def autodelete(matches: list[list[Pathier]]):
     """Keep one of each set in `matches` and delete the others."""
     for match in matches:
         match.pop()
         [file.delete() for file in match]
@@ -122,27 +127,32 @@
         ch.rjust(i + j)
         for i in range(1, 25, 3)
         for j, ch in enumerate(["/", "-", "\\"])
     ]
     s += s[::-1]
     with Spinner(s) as spinner:
         with ThreadPoolExecutor() as exc:
-            thread = exc.submit(get_duplicates, args.paths)
+            thread = exc.submit(get_duplicates, deepcopy(args.paths))
             while not thread.done():
                 spinner.display()
                 time.sleep(0.025)
             matches = thread.result()
     if matches:
         print(f"Found {len(matches)} duplicate sets of files.")
         if not args.no_show:
-            print(griddy(matches))
+            print(
+                griddy(
+                    [["\n".join([str(file) for file in match])] for match in matches]
+                )
+            )
         if args.delete_dupes or args.autodelete:
-            size = args.path.size()
+            size = lambda: sum(path.size() for path in args.paths)  # type: ignore
+            start_size = size()
             delete_wizard(matches) if args.delete_dupes else autodelete(matches)
-            deleted_size = size - args.path.size()
+            deleted_size = start_size - size()
             print(f"Deleted {Pathier.format_size(deleted_size)}.")
     else:
         print("No duplicates detected.")
 
 
 if __name__ == "__main__":
     dupechecker(get_args())
```

### Comparing `dupechecker-0.2.0/LICENSE.txt` & `dupechecker-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dupechecker-0.2.0/README.md` & `dupechecker-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dupechecker-0.2.0/pyproject.toml` & `dupechecker-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6475 7065 6368 6563 6b65 7222 0d0a   "dupechecker"..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 2243  description = "C
 00000080: 6865 636b 2066 6f72 2061 6e64 2064 656c  heck for and del
 00000090: 6574 6520 6475 706c 6963 6174 6520 6669  ete duplicate fi
 000000a0: 6c65 7320 6672 6f6d 2074 6865 2063 6f6d  les from the com
 000000b0: 6d61 6e64 206c 696e 652e 220d 0a76 6572  mand line."..ver
-000000c0: 7369 6f6e 203d 2022 302e 322e 3022 0d0a  sion = "0.2.0"..
+000000c0: 7369 6f6e 203d 2022 302e 322e 3122 0d0a  sion = "0.2.1"..
 000000d0: 7265 7175 6972 6573 2d70 7974 686f 6e20  requires-python 
 000000e0: 3d20 223e 3d33 2e31 3022 0d0a 6465 7065  = ">=3.10"..depe
 000000f0: 6e64 656e 6369 6573 203d 205b 2267 7269  ndencies = ["gri
 00000100: 6464 6c65 222c 2022 7061 7468 6965 7222  ddle", "pathier"
 00000110: 2c20 2270 7269 6e74 6275 6464 6965 7322  , "printbuddies"
 00000120: 2c20 2270 7974 6573 7422 2c20 2279 6f75  , "pytest", "you
 00000130: 6e6f 7479 6f75 225d 0d0a 7265 6164 6d65  notyou"]..readme
```

### Comparing `dupechecker-0.2.0/PKG-INFO` & `dupechecker-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dupechecker
-Version: 0.2.0
+Version: 0.2.1
 Summary: Check for and delete duplicate files from the command line.
 Project-URL: Homepage, https://github.com/matt-manes/dupechecker
 Project-URL: Documentation, https://github.com/matt-manes/dupechecker/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/dupechecker/tree/main/src/dupechecker
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,filecmp,filesystem
```

