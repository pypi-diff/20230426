# Comparing `tmp/printbuddies-1.1.0.tar.gz` & `tmp/printbuddies-1.2.0.tar.gz`

## Comparing `printbuddies-1.1.0.tar` & `printbuddies-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 printbuddies-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 printbuddies-1.1.0/docs/index.html
--rw-r--r--   0        0        0    34260 2020-02-02 00:00:00.000000 printbuddies-1.1.0/docs/printbuddies.html
--rw-r--r--   0        0        0    28001 2020-02-02 00:00:00.000000 printbuddies-1.1.0/docs/search.js
--rw-r--r--   0        0        0   153632 2020-02-02 00:00:00.000000 printbuddies-1.1.0/docs/printbuddies/printbuddies.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 printbuddies-1.1.0/src/printbuddies/__init__.py
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 printbuddies-1.1.0/src/printbuddies/printbuddies.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 printbuddies-1.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 printbuddies-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 printbuddies-1.1.0/README.md
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 printbuddies-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 printbuddies-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 printbuddies-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 printbuddies-1.2.0/docs/index.html
+-rw-r--r--   0        0        0    34315 2020-02-02 00:00:00.000000 printbuddies-1.2.0/docs/printbuddies.html
+-rw-r--r--   0        0        0    34442 2020-02-02 00:00:00.000000 printbuddies-1.2.0/docs/search.js
+-rw-r--r--   0        0        0   200796 2020-02-02 00:00:00.000000 printbuddies-1.2.0/docs/printbuddies/printbuddies.html
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 printbuddies-1.2.0/src/printbuddies/__init__.py
+-rw-r--r--   0        0        0     9406 2020-02-02 00:00:00.000000 printbuddies-1.2.0/src/printbuddies/printbuddies.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 printbuddies-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 printbuddies-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 printbuddies-1.2.0/README.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 printbuddies-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 printbuddies-1.2.0/PKG-INFO
```

### Comparing `printbuddies-1.1.0/docs/printbuddies.html` & `printbuddies-1.2.0/docs/printbuddies.html`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 printbuddies    </h1>
 
                 
                         <input id="mod-printbuddies-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-printbuddies-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">.printbuddies</span> <span class="kn">import</span> <span class="n">ProgBar</span><span class="p">,</span> <span class="n">clear</span><span class="p">,</span> <span class="n">print_in_place</span><span class="p">,</span> <span class="n">ticker</span>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">.printbuddies</span> <span class="kn">import</span> <span class="n">ProgBar</span><span class="p">,</span> <span class="n">Spinner</span><span class="p">,</span> <span class="n">clear</span><span class="p">,</span> <span class="n">print_in_place</span><span class="p">,</span> <span class="n">ticker</span>
 </span></pre></div>
 
 
             </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -4,9 +4,9 @@
 [Unknown INPUT type]
 ***** Submodules *****
     * printbuddies
 built_with_pdoc[pdoc_logo]
 
 ****** printbuddies ******
 ⁰ View Source
-1from .printbuddies import ProgBar, clear, print_in_place, ticker
+1from .printbuddies import ProgBar, Spinner, clear, print_in_place, ticker
```

### Comparing `printbuddies-1.1.0/docs/printbuddies/printbuddies.html` & `printbuddies-1.2.0/docs/printbuddies/printbuddies.html`

 * *Files 23% similar despite different names*

```diff
@@ -56,14 +56,26 @@
                         </li>
                         <li>
                                 <a class="function" href="#ProgBar.display">display</a>
                         </li>
                 </ul>
 
             </li>
+            <li>
+                    <a class="class" href="#Spinner">Spinner</a>
+                            <ul class="memberlist">
+                        <li>
+                                <a class="function" href="#Spinner.__init__">Spinner</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#Spinner.display">display</a>
+                        </li>
+                </ul>
+
+            </li>
     </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
@@ -132,145 +144,219 @@
 </span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">info</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
 </span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="nb">int</span><span class="p">((</span><span class="n">height</span><span class="p">)</span> <span class="o">/</span> <span class="mi">2</span><span class="p">)),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
 </span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
 </span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
 </span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="k">class</span> <span class="nc">ProgBar</span><span class="p">:</span>
 </span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="sd">&quot;&quot;&quot;Self incrementing, dynamically sized progress bar.</span>
 </span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">    Includes a Timer object from noiftimer that starts timing</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">    on the first call to display and stops timing once</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">    self.counter &gt;= self.total.</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="sd">    It can be easily added to the progress bar display by calling</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">    Timer&#39;s checkTime function and passing the value to the &#39;prefix&#39; or &#39;suffix&#39;</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">    param of self.display():</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">    bar = ProgBar(total=someTotal)</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">    bar.display(prefix=f&quot;Run time: {bar.timer.checkTime()}&quot;)&quot;&quot;&quot;</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">    Includes an internal timer that starts when this object is created.</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">    It can be easily added to the progress bar display by adding</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">    the &#39;runtime&#39; property to display&#39;s prefix or suffix param:</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">    &gt;&gt;&gt; bar = ProgBar(total=100)</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">    &gt;&gt;&gt; time.sleep(30)</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">    &gt;&gt;&gt; bar.display(prefix=bar.runtime)</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">    &gt;&gt;&gt; &quot;runtime: 30s [_///////////////////]1.00%&quot; &quot;&quot;&quot;</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
 </span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
 </span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
 </span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span><span class="p">,</span>
 </span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
 </span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
 </span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="p">):</span>
 </span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="sd">&quot;&quot;&quot;:param total: The number of calls to reach 100% completion.</span>
 </span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">        :param update_frequency: The progress bar will only update once every this number of calls to display().</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">        The larger the value, the less performance impact ProgBar has on the loop in which it is called.</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        e.g.</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        Note: If &#39;total&#39; is not a multiple of &#39;update_frequency&#39;, the display will not show 100% completion when the loop finishes.</span>
 </span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">()</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="k">return</span> <span class="n">percent</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">_prepare_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="n">bar_length</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="n">progress</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">bar_length</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">)</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">*</span> <span class="n">progress</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">*</span> <span class="p">(</span><span class="n">bar_length</span> <span class="o">-</span> <span class="n">progress</span><span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_percent</span><span class="p">()</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_bar</span><span class="p">()</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">_trim_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="n">original_width</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">)</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">-=</span> <span class="mf">0.01</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">original_width</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>            <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="nd">@property</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">runtime</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;runtime:</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}</span><span class="s2"> [</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">return</span> <span class="n">percent</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">_prepare_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="n">bar_length</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="n">progress</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">bar_length</span> <span class="o">*</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">))</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">*</span> <span class="n">progress</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">*</span> <span class="p">(</span><span class="n">bar_length</span> <span class="o">-</span> <span class="n">progress</span><span class="p">)</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_percent</span><span class="p">()</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_bar</span><span class="p">()</span>
 </span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">        e.g.</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">        bar = ProgBar(9)</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">_trim_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="n">original_width</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">)</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">-=</span> <span class="mf">0.01</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">original_width</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        myList = [bar.display(return_object=i) for i in range(10)]&quot;&quot;&quot;</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>                <span class="n">clear</span><span class="p">()</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>                <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="k">return</span> <span class="n">return_object</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="sd">        e.g.</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>            <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>            <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>                    <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>                    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="k">return</span> <span class="n">return_object</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="k">class</span> <span class="nc">Spinner</span><span class="p">:</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="sd">&quot;&quot;&quot;Prints one of a sequence of characters in order everytime display() is called.</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">    The display function writes the new character to the same line, overwriting the previous character.</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.&quot;&quot;&quot;</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">        :param sequence: Override the built in spin sequence.&quot;&quot;&quot;</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="k">if</span> <span class="n">sequence</span><span class="p">:</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">]</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="nd">@property</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="c1"># Buffer each element with a leading space</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="c1"># so that the character isn&#39;t obscured by the cursor</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot; &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span> <span class="k">for</span> <span class="n">ch</span> <span class="ow">in</span> <span class="n">character_list</span><span class="p">]</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of self._sequence,</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">        append it to the end, and return the element.&quot;&quot;&quot;</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="k">return</span> <span class="n">ch</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="clear">
                             <input id="clear-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -396,210 +482,272 @@
                 <label class="view-source-button" for="ProgBar-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar-54"><a href="#ProgBar-54"><span class="linenos"> 54</span></a><span class="k">class</span> <span class="nc">ProgBar</span><span class="p">:</span>
 </span><span id="ProgBar-55"><a href="#ProgBar-55"><span class="linenos"> 55</span></a>    <span class="sd">&quot;&quot;&quot;Self incrementing, dynamically sized progress bar.</span>
 </span><span id="ProgBar-56"><a href="#ProgBar-56"><span class="linenos"> 56</span></a>
-</span><span id="ProgBar-57"><a href="#ProgBar-57"><span class="linenos"> 57</span></a><span class="sd">    Includes a Timer object from noiftimer that starts timing</span>
-</span><span id="ProgBar-58"><a href="#ProgBar-58"><span class="linenos"> 58</span></a><span class="sd">    on the first call to display and stops timing once</span>
-</span><span id="ProgBar-59"><a href="#ProgBar-59"><span class="linenos"> 59</span></a><span class="sd">    self.counter &gt;= self.total.</span>
-</span><span id="ProgBar-60"><a href="#ProgBar-60"><span class="linenos"> 60</span></a><span class="sd">    It can be easily added to the progress bar display by calling</span>
-</span><span id="ProgBar-61"><a href="#ProgBar-61"><span class="linenos"> 61</span></a><span class="sd">    Timer&#39;s checkTime function and passing the value to the &#39;prefix&#39; or &#39;suffix&#39;</span>
-</span><span id="ProgBar-62"><a href="#ProgBar-62"><span class="linenos"> 62</span></a><span class="sd">    param of self.display():</span>
-</span><span id="ProgBar-63"><a href="#ProgBar-63"><span class="linenos"> 63</span></a>
-</span><span id="ProgBar-64"><a href="#ProgBar-64"><span class="linenos"> 64</span></a><span class="sd">    bar = ProgBar(total=someTotal)</span>
-</span><span id="ProgBar-65"><a href="#ProgBar-65"><span class="linenos"> 65</span></a><span class="sd">    bar.display(prefix=f&quot;Run time: {bar.timer.checkTime()}&quot;)&quot;&quot;&quot;</span>
-</span><span id="ProgBar-66"><a href="#ProgBar-66"><span class="linenos"> 66</span></a>
-</span><span id="ProgBar-67"><a href="#ProgBar-67"><span class="linenos"> 67</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="ProgBar-68"><a href="#ProgBar-68"><span class="linenos"> 68</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="ProgBar-69"><a href="#ProgBar-69"><span class="linenos"> 69</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
+</span><span id="ProgBar-57"><a href="#ProgBar-57"><span class="linenos"> 57</span></a><span class="sd">    Includes an internal timer that starts when this object is created.</span>
+</span><span id="ProgBar-58"><a href="#ProgBar-58"><span class="linenos"> 58</span></a><span class="sd">    It can be easily added to the progress bar display by adding</span>
+</span><span id="ProgBar-59"><a href="#ProgBar-59"><span class="linenos"> 59</span></a><span class="sd">    the &#39;runtime&#39; property to display&#39;s prefix or suffix param:</span>
+</span><span id="ProgBar-60"><a href="#ProgBar-60"><span class="linenos"> 60</span></a>
+</span><span id="ProgBar-61"><a href="#ProgBar-61"><span class="linenos"> 61</span></a><span class="sd">    &gt;&gt;&gt; bar = ProgBar(total=100)</span>
+</span><span id="ProgBar-62"><a href="#ProgBar-62"><span class="linenos"> 62</span></a><span class="sd">    &gt;&gt;&gt; time.sleep(30)</span>
+</span><span id="ProgBar-63"><a href="#ProgBar-63"><span class="linenos"> 63</span></a><span class="sd">    &gt;&gt;&gt; bar.display(prefix=bar.runtime)</span>
+</span><span id="ProgBar-64"><a href="#ProgBar-64"><span class="linenos"> 64</span></a><span class="sd">    &gt;&gt;&gt; &quot;runtime: 30s [_///////////////////]1.00%&quot; &quot;&quot;&quot;</span>
+</span><span id="ProgBar-65"><a href="#ProgBar-65"><span class="linenos"> 65</span></a>
+</span><span id="ProgBar-66"><a href="#ProgBar-66"><span class="linenos"> 66</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="ProgBar-67"><a href="#ProgBar-67"><span class="linenos"> 67</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="ProgBar-68"><a href="#ProgBar-68"><span class="linenos"> 68</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
+</span><span id="ProgBar-69"><a href="#ProgBar-69"><span class="linenos"> 69</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
 </span><span id="ProgBar-70"><a href="#ProgBar-70"><span class="linenos"> 70</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
 </span><span id="ProgBar-71"><a href="#ProgBar-71"><span class="linenos"> 71</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
 </span><span id="ProgBar-72"><a href="#ProgBar-72"><span class="linenos"> 72</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span><span class="p">,</span>
 </span><span id="ProgBar-73"><a href="#ProgBar-73"><span class="linenos"> 73</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
 </span><span id="ProgBar-74"><a href="#ProgBar-74"><span class="linenos"> 74</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
 </span><span id="ProgBar-75"><a href="#ProgBar-75"><span class="linenos"> 75</span></a>    <span class="p">):</span>
 </span><span id="ProgBar-76"><a href="#ProgBar-76"><span class="linenos"> 76</span></a>        <span class="sd">&quot;&quot;&quot;:param total: The number of calls to reach 100% completion.</span>
 </span><span id="ProgBar-77"><a href="#ProgBar-77"><span class="linenos"> 77</span></a>
-</span><span id="ProgBar-78"><a href="#ProgBar-78"><span class="linenos"> 78</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
-</span><span id="ProgBar-79"><a href="#ProgBar-79"><span class="linenos"> 79</span></a>
-</span><span id="ProgBar-80"><a href="#ProgBar-80"><span class="linenos"> 80</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
-</span><span id="ProgBar-81"><a href="#ProgBar-81"><span class="linenos"> 81</span></a>
-</span><span id="ProgBar-82"><a href="#ProgBar-82"><span class="linenos"> 82</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
-</span><span id="ProgBar-83"><a href="#ProgBar-83"><span class="linenos"> 83</span></a>
-</span><span id="ProgBar-84"><a href="#ProgBar-84"><span class="linenos"> 84</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
-</span><span id="ProgBar-85"><a href="#ProgBar-85"><span class="linenos"> 85</span></a>
-</span><span id="ProgBar-86"><a href="#ProgBar-86"><span class="linenos"> 86</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
+</span><span id="ProgBar-78"><a href="#ProgBar-78"><span class="linenos"> 78</span></a><span class="sd">        :param update_frequency: The progress bar will only update once every this number of calls to display().</span>
+</span><span id="ProgBar-79"><a href="#ProgBar-79"><span class="linenos"> 79</span></a><span class="sd">        The larger the value, the less performance impact ProgBar has on the loop in which it is called.</span>
+</span><span id="ProgBar-80"><a href="#ProgBar-80"><span class="linenos"> 80</span></a><span class="sd">        e.g.</span>
+</span><span id="ProgBar-81"><a href="#ProgBar-81"><span class="linenos"> 81</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
+</span><span id="ProgBar-82"><a href="#ProgBar-82"><span class="linenos"> 82</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
+</span><span id="ProgBar-83"><a href="#ProgBar-83"><span class="linenos"> 83</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
+</span><span id="ProgBar-84"><a href="#ProgBar-84"><span class="linenos"> 84</span></a>
+</span><span id="ProgBar-85"><a href="#ProgBar-85"><span class="linenos"> 85</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
+</span><span id="ProgBar-86"><a href="#ProgBar-86"><span class="linenos"> 86</span></a><span class="sd">        Note: If &#39;total&#39; is not a multiple of &#39;update_frequency&#39;, the display will not show 100% completion when the loop finishes.</span>
 </span><span id="ProgBar-87"><a href="#ProgBar-87"><span class="linenos"> 87</span></a>
-</span><span id="ProgBar-88"><a href="#ProgBar-88"><span class="linenos"> 88</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
-</span><span id="ProgBar-89"><a href="#ProgBar-89"><span class="linenos"> 89</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
-</span><span id="ProgBar-90"><a href="#ProgBar-90"><span class="linenos"> 90</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
-</span><span id="ProgBar-91"><a href="#ProgBar-91"><span class="linenos"> 91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="ProgBar-92"><a href="#ProgBar-92"><span class="linenos"> 92</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="ProgBar-93"><a href="#ProgBar-93"><span class="linenos"> 93</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="ProgBar-94"><a href="#ProgBar-94"><span class="linenos"> 94</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
-</span><span id="ProgBar-95"><a href="#ProgBar-95"><span class="linenos"> 95</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
-</span><span id="ProgBar-96"><a href="#ProgBar-96"><span class="linenos"> 96</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">()</span>
-</span><span id="ProgBar-97"><a href="#ProgBar-97"><span class="linenos"> 97</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
-</span><span id="ProgBar-98"><a href="#ProgBar-98"><span class="linenos"> 98</span></a>
-</span><span id="ProgBar-99"><a href="#ProgBar-99"><span class="linenos"> 99</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-100"><a href="#ProgBar-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="ProgBar-101"><a href="#ProgBar-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-102"><a href="#ProgBar-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-103"><a href="#ProgBar-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-104"><a href="#ProgBar-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-105"><a href="#ProgBar-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-106"><a href="#ProgBar-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-107"><a href="#ProgBar-107"><span class="linenos">107</span></a>
-</span><span id="ProgBar-108"><a href="#ProgBar-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="ProgBar-109"><a href="#ProgBar-109"><span class="linenos">109</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
-</span><span id="ProgBar-110"><a href="#ProgBar-110"><span class="linenos">110</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
-</span><span id="ProgBar-111"><a href="#ProgBar-111"><span class="linenos">111</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
-</span><span id="ProgBar-112"><a href="#ProgBar-112"><span class="linenos">112</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="ProgBar-113"><a href="#ProgBar-113"><span class="linenos">113</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
-</span><span id="ProgBar-114"><a href="#ProgBar-114"><span class="linenos">114</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="ProgBar-115"><a href="#ProgBar-115"><span class="linenos">115</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
-</span><span id="ProgBar-116"><a href="#ProgBar-116"><span class="linenos">116</span></a>        <span class="k">return</span> <span class="n">percent</span>
-</span><span id="ProgBar-117"><a href="#ProgBar-117"><span class="linenos">117</span></a>
-</span><span id="ProgBar-118"><a href="#ProgBar-118"><span class="linenos">118</span></a>    <span class="k">def</span> <span class="nf">_prepare_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-119"><a href="#ProgBar-119"><span class="linenos">119</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span>
-</span><span id="ProgBar-120"><a href="#ProgBar-120"><span class="linenos">120</span></a>        <span class="n">bar_length</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
-</span><span id="ProgBar-121"><a href="#ProgBar-121"><span class="linenos">121</span></a>        <span class="n">progress</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">bar_length</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">)</span>
-</span><span id="ProgBar-122"><a href="#ProgBar-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">*</span> <span class="n">progress</span>
-</span><span id="ProgBar-123"><a href="#ProgBar-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">*</span> <span class="p">(</span><span class="n">bar_length</span> <span class="o">-</span> <span class="n">progress</span><span class="p">)</span>
-</span><span id="ProgBar-124"><a href="#ProgBar-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_percent</span><span class="p">()</span>
-</span><span id="ProgBar-125"><a href="#ProgBar-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_bar</span><span class="p">()</span>
-</span><span id="ProgBar-126"><a href="#ProgBar-126"><span class="linenos">126</span></a>
-</span><span id="ProgBar-127"><a href="#ProgBar-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">_trim_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-128"><a href="#ProgBar-128"><span class="linenos">128</span></a>        <span class="n">original_width</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span>
-</span><span id="ProgBar-129"><a href="#ProgBar-129"><span class="linenos">129</span></a>        <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">)</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="ProgBar-130"><a href="#ProgBar-130"><span class="linenos">130</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">-=</span> <span class="mf">0.01</span>
-</span><span id="ProgBar-131"><a href="#ProgBar-131"><span class="linenos">131</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="ProgBar-132"><a href="#ProgBar-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">original_width</span>
+</span><span id="ProgBar-88"><a href="#ProgBar-88"><span class="linenos"> 88</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
+</span><span id="ProgBar-89"><a href="#ProgBar-89"><span class="linenos"> 89</span></a>
+</span><span id="ProgBar-90"><a href="#ProgBar-90"><span class="linenos"> 90</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
+</span><span id="ProgBar-91"><a href="#ProgBar-91"><span class="linenos"> 91</span></a>
+</span><span id="ProgBar-92"><a href="#ProgBar-92"><span class="linenos"> 92</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
+</span><span id="ProgBar-93"><a href="#ProgBar-93"><span class="linenos"> 93</span></a>
+</span><span id="ProgBar-94"><a href="#ProgBar-94"><span class="linenos"> 94</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
+</span><span id="ProgBar-95"><a href="#ProgBar-95"><span class="linenos"> 95</span></a>
+</span><span id="ProgBar-96"><a href="#ProgBar-96"><span class="linenos"> 96</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
+</span><span id="ProgBar-97"><a href="#ProgBar-97"><span class="linenos"> 97</span></a>
+</span><span id="ProgBar-98"><a href="#ProgBar-98"><span class="linenos"> 98</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
+</span><span id="ProgBar-99"><a href="#ProgBar-99"><span class="linenos"> 99</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
+</span><span id="ProgBar-100"><a href="#ProgBar-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
+</span><span id="ProgBar-101"><a href="#ProgBar-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
+</span><span id="ProgBar-102"><a href="#ProgBar-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="ProgBar-103"><a href="#ProgBar-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="ProgBar-104"><a href="#ProgBar-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="ProgBar-105"><a href="#ProgBar-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
+</span><span id="ProgBar-106"><a href="#ProgBar-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
+</span><span id="ProgBar-107"><a href="#ProgBar-107"><span class="linenos">107</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="ProgBar-108"><a href="#ProgBar-108"><span class="linenos">108</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="ProgBar-109"><a href="#ProgBar-109"><span class="linenos">109</span></a>
+</span><span id="ProgBar-110"><a href="#ProgBar-110"><span class="linenos">110</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-111"><a href="#ProgBar-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="ProgBar-112"><a href="#ProgBar-112"><span class="linenos">112</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="ProgBar-113"><a href="#ProgBar-113"><span class="linenos">113</span></a>
+</span><span id="ProgBar-114"><a href="#ProgBar-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="ProgBar-115"><a href="#ProgBar-115"><span class="linenos">115</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar-116"><a href="#ProgBar-116"><span class="linenos">116</span></a>            <span class="n">clear</span><span class="p">()</span>
+</span><span id="ProgBar-117"><a href="#ProgBar-117"><span class="linenos">117</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="ProgBar-118"><a href="#ProgBar-118"><span class="linenos">118</span></a>            <span class="nb">print</span><span class="p">()</span>
+</span><span id="ProgBar-119"><a href="#ProgBar-119"><span class="linenos">119</span></a>
+</span><span id="ProgBar-120"><a href="#ProgBar-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-121"><a href="#ProgBar-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="ProgBar-122"><a href="#ProgBar-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-123"><a href="#ProgBar-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-124"><a href="#ProgBar-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-125"><a href="#ProgBar-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-126"><a href="#ProgBar-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-127"><a href="#ProgBar-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-128"><a href="#ProgBar-128"><span class="linenos">128</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="ProgBar-129"><a href="#ProgBar-129"><span class="linenos">129</span></a>
+</span><span id="ProgBar-130"><a href="#ProgBar-130"><span class="linenos">130</span></a>    <span class="nd">@property</span>
+</span><span id="ProgBar-131"><a href="#ProgBar-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">runtime</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="ProgBar-132"><a href="#ProgBar-132"><span class="linenos">132</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;runtime:</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="ProgBar-133"><a href="#ProgBar-133"><span class="linenos">133</span></a>
-</span><span id="ProgBar-134"><a href="#ProgBar-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-135"><a href="#ProgBar-135"><span class="linenos">135</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}</span><span class="s2"> [</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="ProgBar-136"><a href="#ProgBar-136"><span class="linenos">136</span></a>
-</span><span id="ProgBar-137"><a href="#ProgBar-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
-</span><span id="ProgBar-138"><a href="#ProgBar-138"><span class="linenos">138</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="ProgBar-139"><a href="#ProgBar-139"><span class="linenos">139</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="ProgBar-140"><a href="#ProgBar-140"><span class="linenos">140</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="ProgBar-141"><a href="#ProgBar-141"><span class="linenos">141</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar-142"><a href="#ProgBar-142"><span class="linenos">142</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar-143"><a href="#ProgBar-143"><span class="linenos">143</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar-144"><a href="#ProgBar-144"><span class="linenos">144</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="ProgBar-145"><a href="#ProgBar-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
-</span><span id="ProgBar-146"><a href="#ProgBar-146"><span class="linenos">146</span></a>
-</span><span id="ProgBar-147"><a href="#ProgBar-147"><span class="linenos">147</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
-</span><span id="ProgBar-148"><a href="#ProgBar-148"><span class="linenos">148</span></a>
-</span><span id="ProgBar-149"><a href="#ProgBar-149"><span class="linenos">149</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
-</span><span id="ProgBar-150"><a href="#ProgBar-150"><span class="linenos">150</span></a>
-</span><span id="ProgBar-151"><a href="#ProgBar-151"><span class="linenos">151</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
+</span><span id="ProgBar-134"><a href="#ProgBar-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="ProgBar-135"><a href="#ProgBar-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
+</span><span id="ProgBar-136"><a href="#ProgBar-136"><span class="linenos">136</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
+</span><span id="ProgBar-137"><a href="#ProgBar-137"><span class="linenos">137</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
+</span><span id="ProgBar-138"><a href="#ProgBar-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="ProgBar-139"><a href="#ProgBar-139"><span class="linenos">139</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
+</span><span id="ProgBar-140"><a href="#ProgBar-140"><span class="linenos">140</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="ProgBar-141"><a href="#ProgBar-141"><span class="linenos">141</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
+</span><span id="ProgBar-142"><a href="#ProgBar-142"><span class="linenos">142</span></a>        <span class="k">return</span> <span class="n">percent</span>
+</span><span id="ProgBar-143"><a href="#ProgBar-143"><span class="linenos">143</span></a>
+</span><span id="ProgBar-144"><a href="#ProgBar-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">_prepare_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-145"><a href="#ProgBar-145"><span class="linenos">145</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span>
+</span><span id="ProgBar-146"><a href="#ProgBar-146"><span class="linenos">146</span></a>        <span class="n">bar_length</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
+</span><span id="ProgBar-147"><a href="#ProgBar-147"><span class="linenos">147</span></a>        <span class="n">progress</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">bar_length</span> <span class="o">*</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">))</span>
+</span><span id="ProgBar-148"><a href="#ProgBar-148"><span class="linenos">148</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">*</span> <span class="n">progress</span>
+</span><span id="ProgBar-149"><a href="#ProgBar-149"><span class="linenos">149</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">*</span> <span class="p">(</span><span class="n">bar_length</span> <span class="o">-</span> <span class="n">progress</span><span class="p">)</span>
+</span><span id="ProgBar-150"><a href="#ProgBar-150"><span class="linenos">150</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_percent</span><span class="p">()</span>
+</span><span id="ProgBar-151"><a href="#ProgBar-151"><span class="linenos">151</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_bar</span><span class="p">()</span>
 </span><span id="ProgBar-152"><a href="#ProgBar-152"><span class="linenos">152</span></a>
-</span><span id="ProgBar-153"><a href="#ProgBar-153"><span class="linenos">153</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
-</span><span id="ProgBar-154"><a href="#ProgBar-154"><span class="linenos">154</span></a>
-</span><span id="ProgBar-155"><a href="#ProgBar-155"><span class="linenos">155</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
-</span><span id="ProgBar-156"><a href="#ProgBar-156"><span class="linenos">156</span></a>
-</span><span id="ProgBar-157"><a href="#ProgBar-157"><span class="linenos">157</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
-</span><span id="ProgBar-158"><a href="#ProgBar-158"><span class="linenos">158</span></a>
-</span><span id="ProgBar-159"><a href="#ProgBar-159"><span class="linenos">159</span></a><span class="sd">        e.g.</span>
-</span><span id="ProgBar-160"><a href="#ProgBar-160"><span class="linenos">160</span></a>
-</span><span id="ProgBar-161"><a href="#ProgBar-161"><span class="linenos">161</span></a><span class="sd">        bar = ProgBar(9)</span>
+</span><span id="ProgBar-153"><a href="#ProgBar-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">_trim_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-154"><a href="#ProgBar-154"><span class="linenos">154</span></a>        <span class="n">original_width</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span>
+</span><span id="ProgBar-155"><a href="#ProgBar-155"><span class="linenos">155</span></a>        <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">)</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar-156"><a href="#ProgBar-156"><span class="linenos">156</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">-=</span> <span class="mf">0.01</span>
+</span><span id="ProgBar-157"><a href="#ProgBar-157"><span class="linenos">157</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="ProgBar-158"><a href="#ProgBar-158"><span class="linenos">158</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">original_width</span>
+</span><span id="ProgBar-159"><a href="#ProgBar-159"><span class="linenos">159</span></a>
+</span><span id="ProgBar-160"><a href="#ProgBar-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-161"><a href="#ProgBar-161"><span class="linenos">161</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="ProgBar-162"><a href="#ProgBar-162"><span class="linenos">162</span></a>
-</span><span id="ProgBar-163"><a href="#ProgBar-163"><span class="linenos">163</span></a><span class="sd">        myList = [bar.display(return_object=i) for i in range(10)]&quot;&quot;&quot;</span>
-</span><span id="ProgBar-164"><a href="#ProgBar-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
-</span><span id="ProgBar-165"><a href="#ProgBar-165"><span class="linenos">165</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="ProgBar-166"><a href="#ProgBar-166"><span class="linenos">166</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="ProgBar-167"><a href="#ProgBar-167"><span class="linenos">167</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
-</span><span id="ProgBar-168"><a href="#ProgBar-168"><span class="linenos">168</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
-</span><span id="ProgBar-169"><a href="#ProgBar-169"><span class="linenos">169</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
-</span><span id="ProgBar-170"><a href="#ProgBar-170"><span class="linenos">170</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
-</span><span id="ProgBar-171"><a href="#ProgBar-171"><span class="linenos">171</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="ProgBar-172"><a href="#ProgBar-172"><span class="linenos">172</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="ProgBar-173"><a href="#ProgBar-173"><span class="linenos">173</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
-</span><span id="ProgBar-174"><a href="#ProgBar-174"><span class="linenos">174</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
-</span><span id="ProgBar-175"><a href="#ProgBar-175"><span class="linenos">175</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="ProgBar-176"><a href="#ProgBar-176"><span class="linenos">176</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
-</span><span id="ProgBar-177"><a href="#ProgBar-177"><span class="linenos">177</span></a>        <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
-</span><span id="ProgBar-178"><a href="#ProgBar-178"><span class="linenos">178</span></a>        <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="ProgBar-179"><a href="#ProgBar-179"><span class="linenos">179</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ProgBar-180"><a href="#ProgBar-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
-</span><span id="ProgBar-181"><a href="#ProgBar-181"><span class="linenos">181</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="ProgBar-182"><a href="#ProgBar-182"><span class="linenos">182</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar-183"><a href="#ProgBar-183"><span class="linenos">183</span></a>                <span class="n">clear</span><span class="p">()</span>
-</span><span id="ProgBar-184"><a href="#ProgBar-184"><span class="linenos">184</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar-185"><a href="#ProgBar-185"><span class="linenos">185</span></a>                <span class="nb">print</span><span class="p">()</span>
-</span><span id="ProgBar-186"><a href="#ProgBar-186"><span class="linenos">186</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="ProgBar-187"><a href="#ProgBar-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="n">return_object</span>
+</span><span id="ProgBar-163"><a href="#ProgBar-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
+</span><span id="ProgBar-164"><a href="#ProgBar-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="ProgBar-165"><a href="#ProgBar-165"><span class="linenos">165</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="ProgBar-166"><a href="#ProgBar-166"><span class="linenos">166</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="ProgBar-167"><a href="#ProgBar-167"><span class="linenos">167</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar-168"><a href="#ProgBar-168"><span class="linenos">168</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar-169"><a href="#ProgBar-169"><span class="linenos">169</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar-170"><a href="#ProgBar-170"><span class="linenos">170</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="ProgBar-171"><a href="#ProgBar-171"><span class="linenos">171</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
+</span><span id="ProgBar-172"><a href="#ProgBar-172"><span class="linenos">172</span></a>
+</span><span id="ProgBar-173"><a href="#ProgBar-173"><span class="linenos">173</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
+</span><span id="ProgBar-174"><a href="#ProgBar-174"><span class="linenos">174</span></a>
+</span><span id="ProgBar-175"><a href="#ProgBar-175"><span class="linenos">175</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
+</span><span id="ProgBar-176"><a href="#ProgBar-176"><span class="linenos">176</span></a>
+</span><span id="ProgBar-177"><a href="#ProgBar-177"><span class="linenos">177</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
+</span><span id="ProgBar-178"><a href="#ProgBar-178"><span class="linenos">178</span></a>
+</span><span id="ProgBar-179"><a href="#ProgBar-179"><span class="linenos">179</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
+</span><span id="ProgBar-180"><a href="#ProgBar-180"><span class="linenos">180</span></a>
+</span><span id="ProgBar-181"><a href="#ProgBar-181"><span class="linenos">181</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
+</span><span id="ProgBar-182"><a href="#ProgBar-182"><span class="linenos">182</span></a>
+</span><span id="ProgBar-183"><a href="#ProgBar-183"><span class="linenos">183</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
+</span><span id="ProgBar-184"><a href="#ProgBar-184"><span class="linenos">184</span></a>
+</span><span id="ProgBar-185"><a href="#ProgBar-185"><span class="linenos">185</span></a><span class="sd">        e.g.</span>
+</span><span id="ProgBar-186"><a href="#ProgBar-186"><span class="linenos">186</span></a>
+</span><span id="ProgBar-187"><a href="#ProgBar-187"><span class="linenos">187</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
+</span><span id="ProgBar-188"><a href="#ProgBar-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
+</span><span id="ProgBar-189"><a href="#ProgBar-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
+</span><span id="ProgBar-190"><a href="#ProgBar-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
+</span><span id="ProgBar-191"><a href="#ProgBar-191"><span class="linenos">191</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
+</span><span id="ProgBar-192"><a href="#ProgBar-192"><span class="linenos">192</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
+</span><span id="ProgBar-193"><a href="#ProgBar-193"><span class="linenos">193</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
+</span><span id="ProgBar-194"><a href="#ProgBar-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="ProgBar-195"><a href="#ProgBar-195"><span class="linenos">195</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="ProgBar-196"><a href="#ProgBar-196"><span class="linenos">196</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="ProgBar-197"><a href="#ProgBar-197"><span class="linenos">197</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
+</span><span id="ProgBar-198"><a href="#ProgBar-198"><span class="linenos">198</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
+</span><span id="ProgBar-199"><a href="#ProgBar-199"><span class="linenos">199</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
+</span><span id="ProgBar-200"><a href="#ProgBar-200"><span class="linenos">200</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
+</span><span id="ProgBar-201"><a href="#ProgBar-201"><span class="linenos">201</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar-202"><a href="#ProgBar-202"><span class="linenos">202</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="ProgBar-203"><a href="#ProgBar-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar-204"><a href="#ProgBar-204"><span class="linenos">204</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
+</span><span id="ProgBar-205"><a href="#ProgBar-205"><span class="linenos">205</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
+</span><span id="ProgBar-206"><a href="#ProgBar-206"><span class="linenos">206</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="ProgBar-207"><a href="#ProgBar-207"><span class="linenos">207</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
+</span><span id="ProgBar-208"><a href="#ProgBar-208"><span class="linenos">208</span></a>            <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
+</span><span id="ProgBar-209"><a href="#ProgBar-209"><span class="linenos">209</span></a>            <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="ProgBar-210"><a href="#ProgBar-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ProgBar-211"><a href="#ProgBar-211"><span class="linenos">211</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
+</span><span id="ProgBar-212"><a href="#ProgBar-212"><span class="linenos">212</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="ProgBar-213"><a href="#ProgBar-213"><span class="linenos">213</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
+</span><span id="ProgBar-214"><a href="#ProgBar-214"><span class="linenos">214</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar-215"><a href="#ProgBar-215"><span class="linenos">215</span></a>                    <span class="n">clear</span><span class="p">()</span>
+</span><span id="ProgBar-216"><a href="#ProgBar-216"><span class="linenos">216</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar-217"><a href="#ProgBar-217"><span class="linenos">217</span></a>                    <span class="nb">print</span><span class="p">()</span>
+</span><span id="ProgBar-218"><a href="#ProgBar-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="ProgBar-219"><a href="#ProgBar-219"><span class="linenos">219</span></a>        <span class="k">return</span> <span class="n">return_object</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Self incrementing, dynamically sized progress bar.</p>
 
-<p>Includes a Timer object from noiftimer that starts timing
-on the first call to display and stops timing once
-self.counter &gt;= self.total.
-It can be easily added to the progress bar display by calling
-Timer's checkTime function and passing the value to the 'prefix' or 'suffix'
-param of self.display():</p>
-
-<p>bar = ProgBar(total=someTotal)
-bar.display(prefix=f"Run time: {bar.timer.checkTime()}")</p>
+<p>Includes an internal timer that starts when this object is created.
+It can be easily added to the progress bar display by adding
+the 'runtime' property to display's prefix or suffix param:</p>
+
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="n">total</span><span class="o">=</span><span class="mi">100</span><span class="p">)</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mi">30</span><span class="p">)</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">prefix</span><span class="o">=</span><span class="n">bar</span><span class="o">.</span><span class="n">runtime</span><span class="p">)</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="s2">&quot;runtime: 30s [_///////////////////]1.00%&quot;</span>
+</code></pre>
+</div>
 </div>
 
 
                             <div id="ProgBar.__init__" class="classattr">
                                         <input id="ProgBar.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
-        <span class="name">ProgBar</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">total</span><span class="p">:</span> <span class="nb">float</span>,</span><span class="param">	<span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;_&#39;</span>,</span><span class="param">	<span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;/&#39;</span>,</span><span class="param">	<span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span>,</span><span class="param">	<span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
+        <span class="name">ProgBar</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">total</span><span class="p">:</span> <span class="nb">float</span>,</span><span class="param">	<span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span>,</span><span class="param">	<span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;_&#39;</span>,</span><span class="param">	<span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;/&#39;</span>,</span><span class="param">	<span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span>,</span><span class="param">	<span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
 
                 <label class="view-source-button" for="ProgBar.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.__init__-67"><a href="#ProgBar.__init__-67"><span class="linenos">67</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="ProgBar.__init__-68"><a href="#ProgBar.__init__-68"><span class="linenos">68</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-69"><a href="#ProgBar.__init__-69"><span class="linenos">69</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-70"><a href="#ProgBar.__init__-70"><span class="linenos">70</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-71"><a href="#ProgBar.__init__-71"><span class="linenos">71</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-72"><a href="#ProgBar.__init__-72"><span class="linenos">72</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-73"><a href="#ProgBar.__init__-73"><span class="linenos">73</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-74"><a href="#ProgBar.__init__-74"><span class="linenos">74</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-75"><a href="#ProgBar.__init__-75"><span class="linenos">75</span></a>    <span class="p">):</span>
-</span><span id="ProgBar.__init__-76"><a href="#ProgBar.__init__-76"><span class="linenos">76</span></a>        <span class="sd">&quot;&quot;&quot;:param total: The number of calls to reach 100% completion.</span>
-</span><span id="ProgBar.__init__-77"><a href="#ProgBar.__init__-77"><span class="linenos">77</span></a>
-</span><span id="ProgBar.__init__-78"><a href="#ProgBar.__init__-78"><span class="linenos">78</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
-</span><span id="ProgBar.__init__-79"><a href="#ProgBar.__init__-79"><span class="linenos">79</span></a>
-</span><span id="ProgBar.__init__-80"><a href="#ProgBar.__init__-80"><span class="linenos">80</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
-</span><span id="ProgBar.__init__-81"><a href="#ProgBar.__init__-81"><span class="linenos">81</span></a>
-</span><span id="ProgBar.__init__-82"><a href="#ProgBar.__init__-82"><span class="linenos">82</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
-</span><span id="ProgBar.__init__-83"><a href="#ProgBar.__init__-83"><span class="linenos">83</span></a>
-</span><span id="ProgBar.__init__-84"><a href="#ProgBar.__init__-84"><span class="linenos">84</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
-</span><span id="ProgBar.__init__-85"><a href="#ProgBar.__init__-85"><span class="linenos">85</span></a>
-</span><span id="ProgBar.__init__-86"><a href="#ProgBar.__init__-86"><span class="linenos">86</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
-</span><span id="ProgBar.__init__-87"><a href="#ProgBar.__init__-87"><span class="linenos">87</span></a>
-</span><span id="ProgBar.__init__-88"><a href="#ProgBar.__init__-88"><span class="linenos">88</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
-</span><span id="ProgBar.__init__-89"><a href="#ProgBar.__init__-89"><span class="linenos">89</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
-</span><span id="ProgBar.__init__-90"><a href="#ProgBar.__init__-90"><span class="linenos">90</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
-</span><span id="ProgBar.__init__-91"><a href="#ProgBar.__init__-91"><span class="linenos">91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="ProgBar.__init__-92"><a href="#ProgBar.__init__-92"><span class="linenos">92</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="ProgBar.__init__-93"><a href="#ProgBar.__init__-93"><span class="linenos">93</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="ProgBar.__init__-94"><a href="#ProgBar.__init__-94"><span class="linenos">94</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
-</span><span id="ProgBar.__init__-95"><a href="#ProgBar.__init__-95"><span class="linenos">95</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
-</span><span id="ProgBar.__init__-96"><a href="#ProgBar.__init__-96"><span class="linenos">96</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">()</span>
-</span><span id="ProgBar.__init__-97"><a href="#ProgBar.__init__-97"><span class="linenos">97</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.__init__-66"><a href="#ProgBar.__init__-66"><span class="linenos"> 66</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="ProgBar.__init__-67"><a href="#ProgBar.__init__-67"><span class="linenos"> 67</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-68"><a href="#ProgBar.__init__-68"><span class="linenos"> 68</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-69"><a href="#ProgBar.__init__-69"><span class="linenos"> 69</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-70"><a href="#ProgBar.__init__-70"><span class="linenos"> 70</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-71"><a href="#ProgBar.__init__-71"><span class="linenos"> 71</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-72"><a href="#ProgBar.__init__-72"><span class="linenos"> 72</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-73"><a href="#ProgBar.__init__-73"><span class="linenos"> 73</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-74"><a href="#ProgBar.__init__-74"><span class="linenos"> 74</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-75"><a href="#ProgBar.__init__-75"><span class="linenos"> 75</span></a>    <span class="p">):</span>
+</span><span id="ProgBar.__init__-76"><a href="#ProgBar.__init__-76"><span class="linenos"> 76</span></a>        <span class="sd">&quot;&quot;&quot;:param total: The number of calls to reach 100% completion.</span>
+</span><span id="ProgBar.__init__-77"><a href="#ProgBar.__init__-77"><span class="linenos"> 77</span></a>
+</span><span id="ProgBar.__init__-78"><a href="#ProgBar.__init__-78"><span class="linenos"> 78</span></a><span class="sd">        :param update_frequency: The progress bar will only update once every this number of calls to display().</span>
+</span><span id="ProgBar.__init__-79"><a href="#ProgBar.__init__-79"><span class="linenos"> 79</span></a><span class="sd">        The larger the value, the less performance impact ProgBar has on the loop in which it is called.</span>
+</span><span id="ProgBar.__init__-80"><a href="#ProgBar.__init__-80"><span class="linenos"> 80</span></a><span class="sd">        e.g.</span>
+</span><span id="ProgBar.__init__-81"><a href="#ProgBar.__init__-81"><span class="linenos"> 81</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
+</span><span id="ProgBar.__init__-82"><a href="#ProgBar.__init__-82"><span class="linenos"> 82</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
+</span><span id="ProgBar.__init__-83"><a href="#ProgBar.__init__-83"><span class="linenos"> 83</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
+</span><span id="ProgBar.__init__-84"><a href="#ProgBar.__init__-84"><span class="linenos"> 84</span></a>
+</span><span id="ProgBar.__init__-85"><a href="#ProgBar.__init__-85"><span class="linenos"> 85</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
+</span><span id="ProgBar.__init__-86"><a href="#ProgBar.__init__-86"><span class="linenos"> 86</span></a><span class="sd">        Note: If &#39;total&#39; is not a multiple of &#39;update_frequency&#39;, the display will not show 100% completion when the loop finishes.</span>
+</span><span id="ProgBar.__init__-87"><a href="#ProgBar.__init__-87"><span class="linenos"> 87</span></a>
+</span><span id="ProgBar.__init__-88"><a href="#ProgBar.__init__-88"><span class="linenos"> 88</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
+</span><span id="ProgBar.__init__-89"><a href="#ProgBar.__init__-89"><span class="linenos"> 89</span></a>
+</span><span id="ProgBar.__init__-90"><a href="#ProgBar.__init__-90"><span class="linenos"> 90</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
+</span><span id="ProgBar.__init__-91"><a href="#ProgBar.__init__-91"><span class="linenos"> 91</span></a>
+</span><span id="ProgBar.__init__-92"><a href="#ProgBar.__init__-92"><span class="linenos"> 92</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
+</span><span id="ProgBar.__init__-93"><a href="#ProgBar.__init__-93"><span class="linenos"> 93</span></a>
+</span><span id="ProgBar.__init__-94"><a href="#ProgBar.__init__-94"><span class="linenos"> 94</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
+</span><span id="ProgBar.__init__-95"><a href="#ProgBar.__init__-95"><span class="linenos"> 95</span></a>
+</span><span id="ProgBar.__init__-96"><a href="#ProgBar.__init__-96"><span class="linenos"> 96</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
+</span><span id="ProgBar.__init__-97"><a href="#ProgBar.__init__-97"><span class="linenos"> 97</span></a>
+</span><span id="ProgBar.__init__-98"><a href="#ProgBar.__init__-98"><span class="linenos"> 98</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
+</span><span id="ProgBar.__init__-99"><a href="#ProgBar.__init__-99"><span class="linenos"> 99</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
+</span><span id="ProgBar.__init__-100"><a href="#ProgBar.__init__-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
+</span><span id="ProgBar.__init__-101"><a href="#ProgBar.__init__-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
+</span><span id="ProgBar.__init__-102"><a href="#ProgBar.__init__-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="ProgBar.__init__-103"><a href="#ProgBar.__init__-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="ProgBar.__init__-104"><a href="#ProgBar.__init__-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="ProgBar.__init__-105"><a href="#ProgBar.__init__-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
+</span><span id="ProgBar.__init__-106"><a href="#ProgBar.__init__-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
+</span><span id="ProgBar.__init__-107"><a href="#ProgBar.__init__-107"><span class="linenos">107</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="ProgBar.__init__-108"><a href="#ProgBar.__init__-108"><span class="linenos">108</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><h6 id="parameters">Parameters</h6>
 
 <ul>
 <li><p><strong>total</strong>:  The number of calls to reach 100% completion.</p></li>
+<li><p><strong>update_frequency</strong>:  The progress bar will only update once every this number of calls to display().
+The larger the value, the less performance impact ProgBar has on the loop in which it is called.
+e.g.</p>
+
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="mi">100</span><span class="p">,</span> <span class="n">update_frequency</span><span class="o">=</span><span class="mi">10</span><span class="p">)</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">100</span><span class="p">):</span>
+<span class="gp">&gt;&gt;&gt; </span>    <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</code></pre>
+</div></li>
+</ul>
+
+<p>^The progress bar in the terminal will only update once every ten calls, going from 0%->100% in 10% increments.
+Note: If 'total' is not a multiple of 'update_frequency', the display will not show 100% completion when the loop finishes.</p>
+
+<ul>
 <li><p><strong>fill_ch</strong>:  The character used to represent the completed part of the bar.</p></li>
 <li><p><strong>unfill_ch</strong>:  The character used to represent the uncompleted part of the bar.</p></li>
 <li><p><strong>width_ratio</strong>:  The width of the progress bar relative to the width of the terminal window.</p></li>
 <li><p><strong>new_line_after_completion</strong>:  Make a call to print() once self.counter &gt;= self.total.</p></li>
 <li><p><strong>clear_after_completion</strong>:  Make a call to printbuddies.clear() once self.counter &gt;= self.total.</p></li>
 </ul>
 
@@ -616,22 +764,23 @@
         <span class="def">def</span>
         <span class="name">reset</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ProgBar.reset-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.reset"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.reset-99"><a href="#ProgBar.reset-99"><span class="linenos"> 99</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar.reset-100"><a href="#ProgBar.reset-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="ProgBar.reset-101"><a href="#ProgBar.reset-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-102"><a href="#ProgBar.reset-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-103"><a href="#ProgBar.reset-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-104"><a href="#ProgBar.reset-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-105"><a href="#ProgBar.reset-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-106"><a href="#ProgBar.reset-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.reset-120"><a href="#ProgBar.reset-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar.reset-121"><a href="#ProgBar.reset-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="ProgBar.reset-122"><a href="#ProgBar.reset-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-123"><a href="#ProgBar.reset-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-124"><a href="#ProgBar.reset-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-125"><a href="#ProgBar.reset-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-126"><a href="#ProgBar.reset-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-127"><a href="#ProgBar.reset-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-128"><a href="#ProgBar.reset-128"><span class="linenos">128</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="ProgBar.get_percent" class="classattr">
@@ -641,23 +790,23 @@
         <span class="def">def</span>
         <span class="name">get_percent</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="ProgBar.get_percent-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.get_percent"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.get_percent-108"><a href="#ProgBar.get_percent-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="ProgBar.get_percent-109"><a href="#ProgBar.get_percent-109"><span class="linenos">109</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
-</span><span id="ProgBar.get_percent-110"><a href="#ProgBar.get_percent-110"><span class="linenos">110</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
-</span><span id="ProgBar.get_percent-111"><a href="#ProgBar.get_percent-111"><span class="linenos">111</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
-</span><span id="ProgBar.get_percent-112"><a href="#ProgBar.get_percent-112"><span class="linenos">112</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="ProgBar.get_percent-113"><a href="#ProgBar.get_percent-113"><span class="linenos">113</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
-</span><span id="ProgBar.get_percent-114"><a href="#ProgBar.get_percent-114"><span class="linenos">114</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="ProgBar.get_percent-115"><a href="#ProgBar.get_percent-115"><span class="linenos">115</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
-</span><span id="ProgBar.get_percent-116"><a href="#ProgBar.get_percent-116"><span class="linenos">116</span></a>        <span class="k">return</span> <span class="n">percent</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.get_percent-134"><a href="#ProgBar.get_percent-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="ProgBar.get_percent-135"><a href="#ProgBar.get_percent-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
+</span><span id="ProgBar.get_percent-136"><a href="#ProgBar.get_percent-136"><span class="linenos">136</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
+</span><span id="ProgBar.get_percent-137"><a href="#ProgBar.get_percent-137"><span class="linenos">137</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
+</span><span id="ProgBar.get_percent-138"><a href="#ProgBar.get_percent-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="ProgBar.get_percent-139"><a href="#ProgBar.get_percent-139"><span class="linenos">139</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
+</span><span id="ProgBar.get_percent-140"><a href="#ProgBar.get_percent-140"><span class="linenos">140</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="ProgBar.get_percent-141"><a href="#ProgBar.get_percent-141"><span class="linenos">141</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
+</span><span id="ProgBar.get_percent-142"><a href="#ProgBar.get_percent-142"><span class="linenos">142</span></a>        <span class="k">return</span> <span class="n">percent</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns the percentage complete to two decimal places
 as a string without the %.</p>
 </div>
 
@@ -670,84 +819,90 @@
         <span class="def">def</span>
         <span class="name">get_bar</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ProgBar.get_bar-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.get_bar"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.get_bar-134"><a href="#ProgBar.get_bar-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar.get_bar-135"><a href="#ProgBar.get_bar-135"><span class="linenos">135</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}</span><span class="s2"> [</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.get_bar-160"><a href="#ProgBar.get_bar-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar.get_bar-161"><a href="#ProgBar.get_bar-161"><span class="linenos">161</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="ProgBar.display" class="classattr">
                                         <input id="ProgBar.display-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">display</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>,</span><span class="param">	<span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>,</span><span class="param">	<span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
+        <span class="name">display</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>,</span><span class="param">	<span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>,</span><span class="param">	<span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">return_object</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="ProgBar.display-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.display"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.display-137"><a href="#ProgBar.display-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
-</span><span id="ProgBar.display-138"><a href="#ProgBar.display-138"><span class="linenos">138</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="ProgBar.display-139"><a href="#ProgBar.display-139"><span class="linenos">139</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="ProgBar.display-140"><a href="#ProgBar.display-140"><span class="linenos">140</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="ProgBar.display-141"><a href="#ProgBar.display-141"><span class="linenos">141</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar.display-142"><a href="#ProgBar.display-142"><span class="linenos">142</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar.display-143"><a href="#ProgBar.display-143"><span class="linenos">143</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar.display-144"><a href="#ProgBar.display-144"><span class="linenos">144</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="ProgBar.display-145"><a href="#ProgBar.display-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
-</span><span id="ProgBar.display-146"><a href="#ProgBar.display-146"><span class="linenos">146</span></a>
-</span><span id="ProgBar.display-147"><a href="#ProgBar.display-147"><span class="linenos">147</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
-</span><span id="ProgBar.display-148"><a href="#ProgBar.display-148"><span class="linenos">148</span></a>
-</span><span id="ProgBar.display-149"><a href="#ProgBar.display-149"><span class="linenos">149</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
-</span><span id="ProgBar.display-150"><a href="#ProgBar.display-150"><span class="linenos">150</span></a>
-</span><span id="ProgBar.display-151"><a href="#ProgBar.display-151"><span class="linenos">151</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
-</span><span id="ProgBar.display-152"><a href="#ProgBar.display-152"><span class="linenos">152</span></a>
-</span><span id="ProgBar.display-153"><a href="#ProgBar.display-153"><span class="linenos">153</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
-</span><span id="ProgBar.display-154"><a href="#ProgBar.display-154"><span class="linenos">154</span></a>
-</span><span id="ProgBar.display-155"><a href="#ProgBar.display-155"><span class="linenos">155</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
-</span><span id="ProgBar.display-156"><a href="#ProgBar.display-156"><span class="linenos">156</span></a>
-</span><span id="ProgBar.display-157"><a href="#ProgBar.display-157"><span class="linenos">157</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
-</span><span id="ProgBar.display-158"><a href="#ProgBar.display-158"><span class="linenos">158</span></a>
-</span><span id="ProgBar.display-159"><a href="#ProgBar.display-159"><span class="linenos">159</span></a><span class="sd">        e.g.</span>
-</span><span id="ProgBar.display-160"><a href="#ProgBar.display-160"><span class="linenos">160</span></a>
-</span><span id="ProgBar.display-161"><a href="#ProgBar.display-161"><span class="linenos">161</span></a><span class="sd">        bar = ProgBar(9)</span>
-</span><span id="ProgBar.display-162"><a href="#ProgBar.display-162"><span class="linenos">162</span></a>
-</span><span id="ProgBar.display-163"><a href="#ProgBar.display-163"><span class="linenos">163</span></a><span class="sd">        myList = [bar.display(return_object=i) for i in range(10)]&quot;&quot;&quot;</span>
-</span><span id="ProgBar.display-164"><a href="#ProgBar.display-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
-</span><span id="ProgBar.display-165"><a href="#ProgBar.display-165"><span class="linenos">165</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="ProgBar.display-166"><a href="#ProgBar.display-166"><span class="linenos">166</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="ProgBar.display-167"><a href="#ProgBar.display-167"><span class="linenos">167</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
-</span><span id="ProgBar.display-168"><a href="#ProgBar.display-168"><span class="linenos">168</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
-</span><span id="ProgBar.display-169"><a href="#ProgBar.display-169"><span class="linenos">169</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
-</span><span id="ProgBar.display-170"><a href="#ProgBar.display-170"><span class="linenos">170</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
-</span><span id="ProgBar.display-171"><a href="#ProgBar.display-171"><span class="linenos">171</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="ProgBar.display-172"><a href="#ProgBar.display-172"><span class="linenos">172</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="ProgBar.display-173"><a href="#ProgBar.display-173"><span class="linenos">173</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
-</span><span id="ProgBar.display-174"><a href="#ProgBar.display-174"><span class="linenos">174</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
-</span><span id="ProgBar.display-175"><a href="#ProgBar.display-175"><span class="linenos">175</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="ProgBar.display-176"><a href="#ProgBar.display-176"><span class="linenos">176</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
-</span><span id="ProgBar.display-177"><a href="#ProgBar.display-177"><span class="linenos">177</span></a>        <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
-</span><span id="ProgBar.display-178"><a href="#ProgBar.display-178"><span class="linenos">178</span></a>        <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="ProgBar.display-179"><a href="#ProgBar.display-179"><span class="linenos">179</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ProgBar.display-180"><a href="#ProgBar.display-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
-</span><span id="ProgBar.display-181"><a href="#ProgBar.display-181"><span class="linenos">181</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="ProgBar.display-182"><a href="#ProgBar.display-182"><span class="linenos">182</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar.display-183"><a href="#ProgBar.display-183"><span class="linenos">183</span></a>                <span class="n">clear</span><span class="p">()</span>
-</span><span id="ProgBar.display-184"><a href="#ProgBar.display-184"><span class="linenos">184</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar.display-185"><a href="#ProgBar.display-185"><span class="linenos">185</span></a>                <span class="nb">print</span><span class="p">()</span>
-</span><span id="ProgBar.display-186"><a href="#ProgBar.display-186"><span class="linenos">186</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="ProgBar.display-187"><a href="#ProgBar.display-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="n">return_object</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.display-163"><a href="#ProgBar.display-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
+</span><span id="ProgBar.display-164"><a href="#ProgBar.display-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="ProgBar.display-165"><a href="#ProgBar.display-165"><span class="linenos">165</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="ProgBar.display-166"><a href="#ProgBar.display-166"><span class="linenos">166</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="ProgBar.display-167"><a href="#ProgBar.display-167"><span class="linenos">167</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar.display-168"><a href="#ProgBar.display-168"><span class="linenos">168</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar.display-169"><a href="#ProgBar.display-169"><span class="linenos">169</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar.display-170"><a href="#ProgBar.display-170"><span class="linenos">170</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="ProgBar.display-171"><a href="#ProgBar.display-171"><span class="linenos">171</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
+</span><span id="ProgBar.display-172"><a href="#ProgBar.display-172"><span class="linenos">172</span></a>
+</span><span id="ProgBar.display-173"><a href="#ProgBar.display-173"><span class="linenos">173</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
+</span><span id="ProgBar.display-174"><a href="#ProgBar.display-174"><span class="linenos">174</span></a>
+</span><span id="ProgBar.display-175"><a href="#ProgBar.display-175"><span class="linenos">175</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
+</span><span id="ProgBar.display-176"><a href="#ProgBar.display-176"><span class="linenos">176</span></a>
+</span><span id="ProgBar.display-177"><a href="#ProgBar.display-177"><span class="linenos">177</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
+</span><span id="ProgBar.display-178"><a href="#ProgBar.display-178"><span class="linenos">178</span></a>
+</span><span id="ProgBar.display-179"><a href="#ProgBar.display-179"><span class="linenos">179</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
+</span><span id="ProgBar.display-180"><a href="#ProgBar.display-180"><span class="linenos">180</span></a>
+</span><span id="ProgBar.display-181"><a href="#ProgBar.display-181"><span class="linenos">181</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
+</span><span id="ProgBar.display-182"><a href="#ProgBar.display-182"><span class="linenos">182</span></a>
+</span><span id="ProgBar.display-183"><a href="#ProgBar.display-183"><span class="linenos">183</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
+</span><span id="ProgBar.display-184"><a href="#ProgBar.display-184"><span class="linenos">184</span></a>
+</span><span id="ProgBar.display-185"><a href="#ProgBar.display-185"><span class="linenos">185</span></a><span class="sd">        e.g.</span>
+</span><span id="ProgBar.display-186"><a href="#ProgBar.display-186"><span class="linenos">186</span></a>
+</span><span id="ProgBar.display-187"><a href="#ProgBar.display-187"><span class="linenos">187</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
+</span><span id="ProgBar.display-188"><a href="#ProgBar.display-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
+</span><span id="ProgBar.display-189"><a href="#ProgBar.display-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
+</span><span id="ProgBar.display-190"><a href="#ProgBar.display-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
+</span><span id="ProgBar.display-191"><a href="#ProgBar.display-191"><span class="linenos">191</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
+</span><span id="ProgBar.display-192"><a href="#ProgBar.display-192"><span class="linenos">192</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
+</span><span id="ProgBar.display-193"><a href="#ProgBar.display-193"><span class="linenos">193</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
+</span><span id="ProgBar.display-194"><a href="#ProgBar.display-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="ProgBar.display-195"><a href="#ProgBar.display-195"><span class="linenos">195</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="ProgBar.display-196"><a href="#ProgBar.display-196"><span class="linenos">196</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="ProgBar.display-197"><a href="#ProgBar.display-197"><span class="linenos">197</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
+</span><span id="ProgBar.display-198"><a href="#ProgBar.display-198"><span class="linenos">198</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
+</span><span id="ProgBar.display-199"><a href="#ProgBar.display-199"><span class="linenos">199</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
+</span><span id="ProgBar.display-200"><a href="#ProgBar.display-200"><span class="linenos">200</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
+</span><span id="ProgBar.display-201"><a href="#ProgBar.display-201"><span class="linenos">201</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar.display-202"><a href="#ProgBar.display-202"><span class="linenos">202</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="ProgBar.display-203"><a href="#ProgBar.display-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar.display-204"><a href="#ProgBar.display-204"><span class="linenos">204</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
+</span><span id="ProgBar.display-205"><a href="#ProgBar.display-205"><span class="linenos">205</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
+</span><span id="ProgBar.display-206"><a href="#ProgBar.display-206"><span class="linenos">206</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="ProgBar.display-207"><a href="#ProgBar.display-207"><span class="linenos">207</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
+</span><span id="ProgBar.display-208"><a href="#ProgBar.display-208"><span class="linenos">208</span></a>            <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
+</span><span id="ProgBar.display-209"><a href="#ProgBar.display-209"><span class="linenos">209</span></a>            <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="ProgBar.display-210"><a href="#ProgBar.display-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ProgBar.display-211"><a href="#ProgBar.display-211"><span class="linenos">211</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
+</span><span id="ProgBar.display-212"><a href="#ProgBar.display-212"><span class="linenos">212</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="ProgBar.display-213"><a href="#ProgBar.display-213"><span class="linenos">213</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
+</span><span id="ProgBar.display-214"><a href="#ProgBar.display-214"><span class="linenos">214</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar.display-215"><a href="#ProgBar.display-215"><span class="linenos">215</span></a>                    <span class="n">clear</span><span class="p">()</span>
+</span><span id="ProgBar.display-216"><a href="#ProgBar.display-216"><span class="linenos">216</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar.display-217"><a href="#ProgBar.display-217"><span class="linenos">217</span></a>                    <span class="nb">print</span><span class="p">()</span>
+</span><span id="ProgBar.display-218"><a href="#ProgBar.display-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="ProgBar.display-219"><a href="#ProgBar.display-219"><span class="linenos">219</span></a>        <span class="k">return</span> <span class="n">return_object</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Writes the progress bar to the terminal.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -759,17 +914,137 @@
 <li><p><strong>return_object</strong>:  An object to be returned by display().</p></li>
 </ul>
 
 <p>Allows display() to be called within a comprehension:</p>
 
 <p>e.g.</p>
 
-<p>bar = ProgBar(9)</p>
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="k">def</span> <span class="nf">square</span><span class="p">(</span><span class="n">x</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="nb">float</span><span class="p">)</span><span class="o">-&gt;</span><span class="nb">int</span><span class="o">|</span><span class="nb">float</span><span class="p">:</span>
+<span class="gp">&gt;&gt;&gt; </span>    <span class="k">return</span> <span class="n">x</span> <span class="o">*</span> <span class="n">x</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">myList</span> <span class="o">=</span> <span class="p">[</span><span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">return_object</span><span class="o">=</span><span class="n">square</span><span class="p">(</span><span class="n">i</span><span class="p">))</span> <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">10</span><span class="p">)]</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="o">&lt;</span><span class="n">progress</span> <span class="n">bar</span> <span class="n">gets</span> <span class="n">displayed</span><span class="o">&gt;</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">myList</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">16</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">36</span><span class="p">,</span> <span class="mi">49</span><span class="p">,</span> <span class="mi">64</span><span class="p">,</span> <span class="mi">81</span><span class="p">]</span>
+</code></pre>
+</div>
+</div>
+
+
+                            </div>
+                </section>
+                <section id="Spinner">
+                            <input id="Spinner-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr class">
+            
+    <span class="def">class</span>
+    <span class="name">Spinner</span>:
+
+                <label class="view-source-button" for="Spinner-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Spinner"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner-222"><a href="#Spinner-222"><span class="linenos">222</span></a><span class="k">class</span> <span class="nc">Spinner</span><span class="p">:</span>
+</span><span id="Spinner-223"><a href="#Spinner-223"><span class="linenos">223</span></a>    <span class="sd">&quot;&quot;&quot;Prints one of a sequence of characters in order everytime display() is called.</span>
+</span><span id="Spinner-224"><a href="#Spinner-224"><span class="linenos">224</span></a><span class="sd">    The display function writes the new character to the same line, overwriting the previous character.</span>
+</span><span id="Spinner-225"><a href="#Spinner-225"><span class="linenos">225</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
+</span><span id="Spinner-226"><a href="#Spinner-226"><span class="linenos">226</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.&quot;&quot;&quot;</span>
+</span><span id="Spinner-227"><a href="#Spinner-227"><span class="linenos">227</span></a>
+</span><span id="Spinner-228"><a href="#Spinner-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="Spinner-229"><a href="#Spinner-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Spinner-230"><a href="#Spinner-230"><span class="linenos">230</span></a><span class="sd">        :param sequence: Override the built in spin sequence.&quot;&quot;&quot;</span>
+</span><span id="Spinner-231"><a href="#Spinner-231"><span class="linenos">231</span></a>        <span class="k">if</span> <span class="n">sequence</span><span class="p">:</span>
+</span><span id="Spinner-232"><a href="#Spinner-232"><span class="linenos">232</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="Spinner-233"><a href="#Spinner-233"><span class="linenos">233</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Spinner-234"><a href="#Spinner-234"><span class="linenos">234</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">]</span>
+</span><span id="Spinner-235"><a href="#Spinner-235"><span class="linenos">235</span></a>
+</span><span id="Spinner-236"><a href="#Spinner-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner-237"><a href="#Spinner-237"><span class="linenos">237</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="Spinner-238"><a href="#Spinner-238"><span class="linenos">238</span></a>
+</span><span id="Spinner-239"><a href="#Spinner-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="Spinner-240"><a href="#Spinner-240"><span class="linenos">240</span></a>        <span class="n">clear</span><span class="p">()</span>
+</span><span id="Spinner-241"><a href="#Spinner-241"><span class="linenos">241</span></a>
+</span><span id="Spinner-242"><a href="#Spinner-242"><span class="linenos">242</span></a>    <span class="nd">@property</span>
+</span><span id="Spinner-243"><a href="#Spinner-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="Spinner-244"><a href="#Spinner-244"><span class="linenos">244</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
+</span><span id="Spinner-245"><a href="#Spinner-245"><span class="linenos">245</span></a>
+</span><span id="Spinner-246"><a href="#Spinner-246"><span class="linenos">246</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="Spinner-247"><a href="#Spinner-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
+</span><span id="Spinner-248"><a href="#Spinner-248"><span class="linenos">248</span></a>        <span class="c1"># Buffer each element with a leading space</span>
+</span><span id="Spinner-249"><a href="#Spinner-249"><span class="linenos">249</span></a>        <span class="c1"># so that the character isn&#39;t obscured by the cursor</span>
+</span><span id="Spinner-250"><a href="#Spinner-250"><span class="linenos">250</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot; &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span> <span class="k">for</span> <span class="n">ch</span> <span class="ow">in</span> <span class="n">character_list</span><span class="p">]</span>
+</span><span id="Spinner-251"><a href="#Spinner-251"><span class="linenos">251</span></a>
+</span><span id="Spinner-252"><a href="#Spinner-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Spinner-253"><a href="#Spinner-253"><span class="linenos">253</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of self._sequence,</span>
+</span><span id="Spinner-254"><a href="#Spinner-254"><span class="linenos">254</span></a><span class="sd">        append it to the end, and return the element.&quot;&quot;&quot;</span>
+</span><span id="Spinner-255"><a href="#Spinner-255"><span class="linenos">255</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="Spinner-256"><a href="#Spinner-256"><span class="linenos">256</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
+</span><span id="Spinner-257"><a href="#Spinner-257"><span class="linenos">257</span></a>        <span class="k">return</span> <span class="n">ch</span>
+</span><span id="Spinner-258"><a href="#Spinner-258"><span class="linenos">258</span></a>
+</span><span id="Spinner-259"><a href="#Spinner-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner-260"><a href="#Spinner-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="Spinner-261"><a href="#Spinner-261"><span class="linenos">261</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Prints one of a sequence of characters in order everytime display() is called.
+The display function writes the new character to the same line, overwriting the previous character.
+The sequence will be cycled through indefinitely.
+If used as a context manager, the last printed character will be cleared upon exiting.</p>
+</div>
+
+
+                            <div id="Spinner.__init__" class="classattr">
+                                        <input id="Spinner.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="name">Spinner</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span>)</span>
+
+                <label class="view-source-button" for="Spinner.__init__-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Spinner.__init__"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.__init__-228"><a href="#Spinner.__init__-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="Spinner.__init__-229"><a href="#Spinner.__init__-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Spinner.__init__-230"><a href="#Spinner.__init__-230"><span class="linenos">230</span></a><span class="sd">        :param sequence: Override the built in spin sequence.&quot;&quot;&quot;</span>
+</span><span id="Spinner.__init__-231"><a href="#Spinner.__init__-231"><span class="linenos">231</span></a>        <span class="k">if</span> <span class="n">sequence</span><span class="p">:</span>
+</span><span id="Spinner.__init__-232"><a href="#Spinner.__init__-232"><span class="linenos">232</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="Spinner.__init__-233"><a href="#Spinner.__init__-233"><span class="linenos">233</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Spinner.__init__-234"><a href="#Spinner.__init__-234"><span class="linenos">234</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">]</span>
+</span></pre></div>
+
+
+            <div class="docstring"><h6 id="parameters">Parameters</h6>
+
+<ul>
+<li><strong>sequence</strong>:  Override the built in spin sequence.</li>
+</ul>
+</div>
+
+
+                            </div>
+                            <div id="Spinner.display" class="classattr">
+                                        <input id="Spinner.display-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">display</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="Spinner.display-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Spinner.display"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.display-259"><a href="#Spinner.display-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner.display-260"><a href="#Spinner.display-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="Spinner.display-261"><a href="#Spinner.display-261"><span class="linenos">261</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span></pre></div>
+
 
-<p>myList = [bar.display(return_object=i) for i in range(10)]</p>
+            <div class="docstring"><p>Print the next character in the sequence.</p>
 </div>
 
 
                             </div>
                 </section>
     </main>
 <script>
```

#### html2text {}

```diff
@@ -8,14 +8,17 @@
     * ticker
     * ProgBar
           o ProgBar
           o reset
           o get_percent
           o get_bar
           o display
+    * Spinner
+          o Spinner
+          o display
 built_with_pdoc[pdoc_logo]
 
 ****** printbuddies.printbuddies ******
 ⁰ View Source
 __1from os import get_terminal_size
 __2from time import sleep
 __3from typing import Any
@@ -68,155 +71,236 @@
 _49    print(*info, sep="\n", end="")
 _50    print("\n" * (int((height) / 2)), end="")
 _51
 _52
 _53class ProgBar:
 _54    """Self incrementing, dynamically sized progress bar.
 _55
-_56    Includes a Timer object from noiftimer that starts timing
-_57    on the first call to display and stops timing once
-_58    self.counter >= self.total.
-_59    It can be easily added to the progress bar display by calling
-_60    Timer's checkTime function and passing the value to the 'prefix' or
-'suffix'
-_61    param of self.display():
-_62
-_63    bar = ProgBar(total=someTotal)
-_64    bar.display(prefix=f"Run time: {bar.timer.checkTime()}")"""
-_65
-_66    def __init__(
-_67        self,
-_68        total: float,
+_56    Includes an internal timer that starts when this object is created.
+_57    It can be easily added to the progress bar display by adding
+_58    the 'runtime' property to display's prefix or suffix param:
+_59
+_60    >>> bar = ProgBar(total=100)
+_61    >>> time.sleep(30)
+_62    >>> bar.display(prefix=bar.runtime)
+_63    >>> "runtime: 30s [_///////////////////]1.00%" """
+_64
+_65    def __init__(
+_66        self,
+_67        total: float,
+_68        update_frequency: int = 1,
 _69        fill_ch: str = "_",
 _70        unfill_ch: str = "/",
 _71        width_ratio: float = 0.75,
 _72        new_line_after_completion: bool = True,
 _73        clear_after_completion: bool = False,
 _74    ):
 _75        """:param total: The number of calls to reach 100% completion.
 _76
-_77        :param fill_ch: The character used to represent the completed part
+_77        :param update_frequency: The progress bar will only update once
+every this number of calls to display().
+_78        The larger the value, the less performance impact ProgBar has on the
+loop in which it is called.
+_79        e.g.
+_80        >>> bar = ProgBar(100, update_frequency=10)
+_81        >>> for _ in range(100):
+_82        >>>     bar.display()
+_83
+_84        ^The progress bar in the terminal will only update once every ten
+calls, going from 0%->100% in 10% increments.
+_85        Note: If 'total' is not a multiple of 'update_frequency', the
+display will not show 100% completion when the loop finishes.
+_86
+_87        :param fill_ch: The character used to represent the completed part
 of the bar.
-_78
-_79        :param unfill_ch: The character used to represent the uncompleted
+_88
+_89        :param unfill_ch: The character used to represent the uncompleted
 part of the bar.
-_80
-_81        :param width_ratio: The width of the progress bar relative to the
+_90
+_91        :param width_ratio: The width of the progress bar relative to the
 width of the terminal window.
-_82
-_83        :param new_line_after_completion: Make a call to print() once
+_92
+_93        :param new_line_after_completion: Make a call to print() once
 self.counter >= self.total.
-_84
-_85        :param clear_after_completion: Make a call to printbuddies.clear()
+_94
+_95        :param clear_after_completion: Make a call to printbuddies.clear()
 once self.counter >= self.total.
-_86
-_87        Note: if new_line_after_completion and clear_after_completion are
+_96
+_97        Note: if new_line_after_completion and clear_after_completion are
 both True, the line will be cleared
-_88        then a call to print() will be made."""
-_89        self.total = total
-_90        self.fill_ch = fill_ch[0]
-_91        self.unfill_ch = unfill_ch[0]
-_92        self.width_ratio = width_ratio
-_93        self.new_line_after_completion = new_line_after_completion
-_94        self.clear_after_completion = clear_after_completion
-_95        self.timer = Timer()
-_96        self.reset()
-_97
-_98    def reset(self):
-_99        self.counter = 0
-100        self.percent = ""
-101        self.prefix = ""
-102        self.suffix = ""
-103        self.filled = ""
-104        self.unfilled = ""
-105        self.bar = ""
-106
-107    def get_percent(self) -> str:
-108        """Returns the percentage complete to two decimal places
-109        as a string without the %."""
-110        percent = str(round(100.0 * self.counter / self.total, 2))
-111        if len(percent.split(".")[1]) == 1:
-112            percent = percent + "0"
-113        if len(percent.split(".")[0]) == 1:
-114            percent = "0" + percent
-115        return percent
-116
-117    def _prepare_bar(self):
-118        self.terminal_width = get_terminal_size().columns - 1
-119        bar_length = int(self.terminal_width * self.width_ratio)
-120        progress = int(bar_length * self.counter / self.total)
-121        self.filled = self.fill_ch * progress
-122        self.unfilled = self.unfill_ch * (bar_length - progress)
-123        self.percent = self.get_percent()
-124        self.bar = self.get_bar()
-125
-126    def _trim_bar(self):
-127        original_width = self.width_ratio
-128        while len(self.bar) > self.terminal_width and self.width_ratio > 0:
-129            self.width_ratio -= 0.01
-130            self._prepare_bar()
-131        self.width_ratio = original_width
+_98        then a call to print() will be made."""
+_99        self.total = total
+100        self.update_frequency = update_frequency
+101        self.fill_ch = fill_ch[0]
+102        self.unfill_ch = unfill_ch[0]
+103        self.width_ratio = width_ratio
+104        self.new_line_after_completion = new_line_after_completion
+105        self.clear_after_completion = clear_after_completion
+106        self.reset()
+107        self.with_context = False
+108
+109    def __enter__(self):
+110        self.with_context = True
+111        return self
+112
+113    def __exit__(self, *args, **kwargs):
+114        if self.clear_after_completion:
+115            clear()
+116        else:
+117            print()
+118
+119    def reset(self):
+120        self.counter = 1
+121        self.percent = ""
+122        self.prefix = ""
+123        self.suffix = ""
+124        self.filled = ""
+125        self.unfilled = ""
+126        self.bar = ""
+127        self.timer = Timer(subsecond_resolution=False).start()
+128
+129    @property
+130    def runtime(self) -> str:
+131        return f"runtime:{self.timer.elapsed_str}"
 132
-133    def get_bar(self):
-134        return f"{self.prefix} [{self.filled}{self.unfilled}]-
-{self.percent}% {self.suffix}"
-135
-136    def display(
-137        self,
-138        prefix: str = "",
-139        suffix: str = "",
-140        counter_override: float = None,
-141        total_override: float = None,
-142        return_object: Any = None,
-143    ) -> Any:
-144        """Writes the progress bar to the terminal.
-145
-146        :param prefix: String affixed to the front of the progress bar.
-147
-148        :param suffix: String appended to the end of the progress bar.
-149
-150        :param counter_override: When an externally incremented completion
-counter is needed.
+133    def get_percent(self) -> str:
+134        """Returns the percentage complete to two decimal places
+135        as a string without the %."""
+136        percent = str(round(100.0 * self.counter / self.total, 2))
+137        if len(percent.split(".")[1]) == 1:
+138            percent = percent + "0"
+139        if len(percent.split(".")[0]) == 1:
+140            percent = "0" + percent
+141        return percent
+142
+143    def _prepare_bar(self):
+144        self.terminal_width = get_terminal_size().columns - 1
+145        bar_length = int(self.terminal_width * self.width_ratio)
+146        progress = int(bar_length * min(self.counter / self.total, 1.0))
+147        self.filled = self.fill_ch * progress
+148        self.unfilled = self.unfill_ch * (bar_length - progress)
+149        self.percent = self.get_percent()
+150        self.bar = self.get_bar()
 151
-152        :param total_override: When an externally controlled bar total is
-needed.
-153
-154        :param return_object: An object to be returned by display().
-155
-156        Allows display() to be called within a comprehension:
-157
-158        e.g.
-159
-160        bar = ProgBar(9)
+152    def _trim_bar(self):
+153        original_width = self.width_ratio
+154        while len(self.bar) > self.terminal_width and self.width_ratio > 0:
+155            self.width_ratio -= 0.01
+156            self._prepare_bar()
+157        self.width_ratio = original_width
+158
+159    def get_bar(self):
+160        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
+{self.unfilled}]-{self.percent}% {self.suffix}"
 161
-162        myList = [bar.display(return_object=i) for i in range(10)]"""
-163        if not self.timer.started:
-164            self.timer.start()
-165        if counter_override is not None:
-166            self.counter = counter_override
-167        if total_override:
-168            self.total = total_override
-169        # Don't wanna divide by 0 there, pal
-170        while self.total <= 0:
-171            self.total += 1
-172        self.prefix = prefix
-173        self.suffix = suffix
-174        self._prepare_bar()
-175        self._trim_bar()
-176        pad = " " * (self.terminal_width - len(self.bar))
-177        width = get_terminal_size().columns
-178        print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
-179        if self.counter >= self.total:
-180            self.timer.stop()
-181            if self.clear_after_completion:
-182                clear()
-183            if self.new_line_after_completion:
-184                print()
-185        self.counter += 1
-186        return return_object
+162    def display(
+163        self,
+164        prefix: str = "",
+165        suffix: str = "",
+166        counter_override: float | None = None,
+167        total_override: float | None = None,
+168        return_object: Any | None = None,
+169    ) -> Any:
+170        """Writes the progress bar to the terminal.
+171
+172        :param prefix: String affixed to the front of the progress bar.
+173
+174        :param suffix: String appended to the end of the progress bar.
+175
+176        :param counter_override: When an externally incremented completion
+counter is needed.
+177
+178        :param total_override: When an externally controlled bar total is
+needed.
+179
+180        :param return_object: An object to be returned by display().
+181
+182        Allows display() to be called within a comprehension:
+183
+184        e.g.
+185
+186        >>> bar = ProgBar(10)
+187        >>> def square(x: int | float)->int|float:
+188        >>>     return x * x
+189        >>> myList = [bar.display(return_object=square(i)) for i in range
+(10)]
+190        >>> <progress bar gets displayed>
+191        >>> myList
+192        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
+193        if not self.timer.started:
+194            self.timer.start()
+195        if counter_override is not None:
+196            self.counter = counter_override
+197        if total_override:
+198            self.total = total_override
+199        # Don't wanna divide by 0 there, pal
+200        while self.total <= 0:
+201            self.total += 1
+202        if self.counter % self.update_frequency == 0:
+203            self.prefix = prefix
+204            self.suffix = suffix
+205            self._prepare_bar()
+206            self._trim_bar()
+207            pad = " " * (self.terminal_width - len(self.bar))
+208            width = get_terminal_size().columns
+209            print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
+210        if self.counter >= self.total:
+211            self.timer.stop()
+212            if not self.with_context:
+213                if self.clear_after_completion:
+214                    clear()
+215                if self.new_line_after_completion:
+216                    print()
+217        self.counter += 1
+218        return return_object
+219
+220
+221class Spinner:
+222    """Prints one of a sequence of characters in order everytime display()
+is called.
+223    The display function writes the new character to the same line,
+overwriting the previous character.
+224    The sequence will be cycled through indefinitely.
+225    If used as a context manager, the last printed character will be cleared
+upon exiting."""
+226
+227    def __init__(self, sequence: list[Any] | None = None):
+228        """
+229        :param sequence: Override the built in spin sequence."""
+230        if sequence:
+231            self.sequence = sequence
+232        else:
+233            self.sequence = ["/", "-", "\\"]
+234
+235    def __enter__(self):
+236        return self
+237
+238    def __exit__(self, *args, **kwargs):
+239        clear()
+240
+241    @property
+242    def sequence(self) -> list[Any]:
+243        return self._sequence
+244
+245    @sequence.setter
+246    def sequence(self, character_list: list[Any]):
+247        # Buffer each element with a leading space
+248        # so that the character isn't obscured by the cursor
+249        self._sequence = [" " + str(ch) for ch in character_list]
+250
+251    def _get_next(self) -> str:
+252        """Pop the first element of self._sequence,
+253        append it to the end, and return the element."""
+254        ch = self.sequence.pop(0)
+255        self.sequence.append(ch)
+256        return ch
+257
+258    def display(self):
+259        """Print the next character in the sequence."""
+260        print_in_place(self._get_next())
   ⁰
 def clear(): View Source
 _9def clear():
 10    """Erase the current line from the terminal."""
 11    print(" " * (get_terminal_size().columns - 1), flush=True, end="\r")
 Erase the current line from the terminal.
   ⁰
@@ -272,315 +356,458 @@
 print info without showing previous outputs from ticker calls.
 Similar visually to print_in_place, but for multiple lines.
   ⁰
 class ProgBar: View Source
 _54class ProgBar:
 _55    """Self incrementing, dynamically sized progress bar.
 _56
-_57    Includes a Timer object from noiftimer that starts timing
-_58    on the first call to display and stops timing once
-_59    self.counter >= self.total.
-_60    It can be easily added to the progress bar display by calling
-_61    Timer's checkTime function and passing the value to the 'prefix' or
-'suffix'
-_62    param of self.display():
-_63
-_64    bar = ProgBar(total=someTotal)
-_65    bar.display(prefix=f"Run time: {bar.timer.checkTime()}")"""
-_66
-_67    def __init__(
-_68        self,
-_69        total: float,
+_57    Includes an internal timer that starts when this object is created.
+_58    It can be easily added to the progress bar display by adding
+_59    the 'runtime' property to display's prefix or suffix param:
+_60
+_61    >>> bar = ProgBar(total=100)
+_62    >>> time.sleep(30)
+_63    >>> bar.display(prefix=bar.runtime)
+_64    >>> "runtime: 30s [_///////////////////]1.00%" """
+_65
+_66    def __init__(
+_67        self,
+_68        total: float,
+_69        update_frequency: int = 1,
 _70        fill_ch: str = "_",
 _71        unfill_ch: str = "/",
 _72        width_ratio: float = 0.75,
 _73        new_line_after_completion: bool = True,
 _74        clear_after_completion: bool = False,
 _75    ):
 _76        """:param total: The number of calls to reach 100% completion.
 _77
-_78        :param fill_ch: The character used to represent the completed part
+_78        :param update_frequency: The progress bar will only update once
+every this number of calls to display().
+_79        The larger the value, the less performance impact ProgBar has on the
+loop in which it is called.
+_80        e.g.
+_81        >>> bar = ProgBar(100, update_frequency=10)
+_82        >>> for _ in range(100):
+_83        >>>     bar.display()
+_84
+_85        ^The progress bar in the terminal will only update once every ten
+calls, going from 0%->100% in 10% increments.
+_86        Note: If 'total' is not a multiple of 'update_frequency', the
+display will not show 100% completion when the loop finishes.
+_87
+_88        :param fill_ch: The character used to represent the completed part
 of the bar.
-_79
-_80        :param unfill_ch: The character used to represent the uncompleted
+_89
+_90        :param unfill_ch: The character used to represent the uncompleted
 part of the bar.
-_81
-_82        :param width_ratio: The width of the progress bar relative to the
+_91
+_92        :param width_ratio: The width of the progress bar relative to the
 width of the terminal window.
-_83
-_84        :param new_line_after_completion: Make a call to print() once
+_93
+_94        :param new_line_after_completion: Make a call to print() once
 self.counter >= self.total.
-_85
-_86        :param clear_after_completion: Make a call to printbuddies.clear()
+_95
+_96        :param clear_after_completion: Make a call to printbuddies.clear()
 once self.counter >= self.total.
-_87
-_88        Note: if new_line_after_completion and clear_after_completion are
+_97
+_98        Note: if new_line_after_completion and clear_after_completion are
 both True, the line will be cleared
-_89        then a call to print() will be made."""
-_90        self.total = total
-_91        self.fill_ch = fill_ch[0]
-_92        self.unfill_ch = unfill_ch[0]
-_93        self.width_ratio = width_ratio
-_94        self.new_line_after_completion = new_line_after_completion
-_95        self.clear_after_completion = clear_after_completion
-_96        self.timer = Timer()
-_97        self.reset()
-_98
-_99    def reset(self):
-100        self.counter = 0
-101        self.percent = ""
-102        self.prefix = ""
-103        self.suffix = ""
-104        self.filled = ""
-105        self.unfilled = ""
-106        self.bar = ""
-107
-108    def get_percent(self) -> str:
-109        """Returns the percentage complete to two decimal places
-110        as a string without the %."""
-111        percent = str(round(100.0 * self.counter / self.total, 2))
-112        if len(percent.split(".")[1]) == 1:
-113            percent = percent + "0"
-114        if len(percent.split(".")[0]) == 1:
-115            percent = "0" + percent
-116        return percent
-117
-118    def _prepare_bar(self):
-119        self.terminal_width = get_terminal_size().columns - 1
-120        bar_length = int(self.terminal_width * self.width_ratio)
-121        progress = int(bar_length * self.counter / self.total)
-122        self.filled = self.fill_ch * progress
-123        self.unfilled = self.unfill_ch * (bar_length - progress)
-124        self.percent = self.get_percent()
-125        self.bar = self.get_bar()
-126
-127    def _trim_bar(self):
-128        original_width = self.width_ratio
-129        while len(self.bar) > self.terminal_width and self.width_ratio > 0:
-130            self.width_ratio -= 0.01
-131            self._prepare_bar()
-132        self.width_ratio = original_width
+_99        then a call to print() will be made."""
+100        self.total = total
+101        self.update_frequency = update_frequency
+102        self.fill_ch = fill_ch[0]
+103        self.unfill_ch = unfill_ch[0]
+104        self.width_ratio = width_ratio
+105        self.new_line_after_completion = new_line_after_completion
+106        self.clear_after_completion = clear_after_completion
+107        self.reset()
+108        self.with_context = False
+109
+110    def __enter__(self):
+111        self.with_context = True
+112        return self
+113
+114    def __exit__(self, *args, **kwargs):
+115        if self.clear_after_completion:
+116            clear()
+117        else:
+118            print()
+119
+120    def reset(self):
+121        self.counter = 1
+122        self.percent = ""
+123        self.prefix = ""
+124        self.suffix = ""
+125        self.filled = ""
+126        self.unfilled = ""
+127        self.bar = ""
+128        self.timer = Timer(subsecond_resolution=False).start()
+129
+130    @property
+131    def runtime(self) -> str:
+132        return f"runtime:{self.timer.elapsed_str}"
 133
-134    def get_bar(self):
-135        return f"{self.prefix} [{self.filled}{self.unfilled}]-
-{self.percent}% {self.suffix}"
-136
-137    def display(
-138        self,
-139        prefix: str = "",
-140        suffix: str = "",
-141        counter_override: float = None,
-142        total_override: float = None,
-143        return_object: Any = None,
-144    ) -> Any:
-145        """Writes the progress bar to the terminal.
-146
-147        :param prefix: String affixed to the front of the progress bar.
-148
-149        :param suffix: String appended to the end of the progress bar.
-150
-151        :param counter_override: When an externally incremented completion
-counter is needed.
+134    def get_percent(self) -> str:
+135        """Returns the percentage complete to two decimal places
+136        as a string without the %."""
+137        percent = str(round(100.0 * self.counter / self.total, 2))
+138        if len(percent.split(".")[1]) == 1:
+139            percent = percent + "0"
+140        if len(percent.split(".")[0]) == 1:
+141            percent = "0" + percent
+142        return percent
+143
+144    def _prepare_bar(self):
+145        self.terminal_width = get_terminal_size().columns - 1
+146        bar_length = int(self.terminal_width * self.width_ratio)
+147        progress = int(bar_length * min(self.counter / self.total, 1.0))
+148        self.filled = self.fill_ch * progress
+149        self.unfilled = self.unfill_ch * (bar_length - progress)
+150        self.percent = self.get_percent()
+151        self.bar = self.get_bar()
 152
-153        :param total_override: When an externally controlled bar total is
-needed.
-154
-155        :param return_object: An object to be returned by display().
-156
-157        Allows display() to be called within a comprehension:
-158
-159        e.g.
-160
-161        bar = ProgBar(9)
+153    def _trim_bar(self):
+154        original_width = self.width_ratio
+155        while len(self.bar) > self.terminal_width and self.width_ratio > 0:
+156            self.width_ratio -= 0.01
+157            self._prepare_bar()
+158        self.width_ratio = original_width
+159
+160    def get_bar(self):
+161        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
+{self.unfilled}]-{self.percent}% {self.suffix}"
 162
-163        myList = [bar.display(return_object=i) for i in range(10)]"""
-164        if not self.timer.started:
-165            self.timer.start()
-166        if counter_override is not None:
-167            self.counter = counter_override
-168        if total_override:
-169            self.total = total_override
-170        # Don't wanna divide by 0 there, pal
-171        while self.total <= 0:
-172            self.total += 1
-173        self.prefix = prefix
-174        self.suffix = suffix
-175        self._prepare_bar()
-176        self._trim_bar()
-177        pad = " " * (self.terminal_width - len(self.bar))
-178        width = get_terminal_size().columns
-179        print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
-180        if self.counter >= self.total:
-181            self.timer.stop()
-182            if self.clear_after_completion:
-183                clear()
-184            if self.new_line_after_completion:
-185                print()
-186        self.counter += 1
-187        return return_object
+163    def display(
+164        self,
+165        prefix: str = "",
+166        suffix: str = "",
+167        counter_override: float | None = None,
+168        total_override: float | None = None,
+169        return_object: Any | None = None,
+170    ) -> Any:
+171        """Writes the progress bar to the terminal.
+172
+173        :param prefix: String affixed to the front of the progress bar.
+174
+175        :param suffix: String appended to the end of the progress bar.
+176
+177        :param counter_override: When an externally incremented completion
+counter is needed.
+178
+179        :param total_override: When an externally controlled bar total is
+needed.
+180
+181        :param return_object: An object to be returned by display().
+182
+183        Allows display() to be called within a comprehension:
+184
+185        e.g.
+186
+187        >>> bar = ProgBar(10)
+188        >>> def square(x: int | float)->int|float:
+189        >>>     return x * x
+190        >>> myList = [bar.display(return_object=square(i)) for i in range
+(10)]
+191        >>> <progress bar gets displayed>
+192        >>> myList
+193        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
+194        if not self.timer.started:
+195            self.timer.start()
+196        if counter_override is not None:
+197            self.counter = counter_override
+198        if total_override:
+199            self.total = total_override
+200        # Don't wanna divide by 0 there, pal
+201        while self.total <= 0:
+202            self.total += 1
+203        if self.counter % self.update_frequency == 0:
+204            self.prefix = prefix
+205            self.suffix = suffix
+206            self._prepare_bar()
+207            self._trim_bar()
+208            pad = " " * (self.terminal_width - len(self.bar))
+209            width = get_terminal_size().columns
+210            print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
+211        if self.counter >= self.total:
+212            self.timer.stop()
+213            if not self.with_context:
+214                if self.clear_after_completion:
+215                    clear()
+216                if self.new_line_after_completion:
+217                    print()
+218        self.counter += 1
+219        return return_object
 Self incrementing, dynamically sized progress bar.
-Includes a Timer object from noiftimer that starts timing on the first call to
-display and stops timing once self.counter >= self.total. It can be easily
-added to the progress bar display by calling Timer's checkTime function and
-passing the value to the 'prefix' or 'suffix' param of self.display():
-bar = ProgBar(total=someTotal) bar.display(prefix=f"Run time:
-{bar.timer.checkTime()}")
+Includes an internal timer that starts when this object is created. It can be
+easily added to the progress bar display by adding the 'runtime' property to
+display's prefix or suffix param:
+>>> bar = ProgBar(total=100)
+>>> time.sleep(30)
+>>> bar.display(prefix=bar.runtime)
+>>> "runtime: 30s [_///////////////////]1.00%"
 ⁰
 ProgBar(
 total: float,
+update_frequency: int = 1,
 fill_ch: str = '_',
 unfill_ch: str = '/',
 width_ratio: float = 0.75,
 new_line_after_completion: bool = True,
 clear_after_completion: bool = False) View Source
-67    def __init__(
-68        self,
-69        total: float,
-70        fill_ch: str = "_",
-71        unfill_ch: str = "/",
-72        width_ratio: float = 0.75,
-73        new_line_after_completion: bool = True,
-74        clear_after_completion: bool = False,
-75    ):
-76        """:param total: The number of calls to reach 100% completion.
-77
-78        :param fill_ch: The character used to represent the completed part of
-the bar.
-79
-80        :param unfill_ch: The character used to represent the uncompleted
+_66    def __init__(
+_67        self,
+_68        total: float,
+_69        update_frequency: int = 1,
+_70        fill_ch: str = "_",
+_71        unfill_ch: str = "/",
+_72        width_ratio: float = 0.75,
+_73        new_line_after_completion: bool = True,
+_74        clear_after_completion: bool = False,
+_75    ):
+_76        """:param total: The number of calls to reach 100% completion.
+_77
+_78        :param update_frequency: The progress bar will only update once
+every this number of calls to display().
+_79        The larger the value, the less performance impact ProgBar has on the
+loop in which it is called.
+_80        e.g.
+_81        >>> bar = ProgBar(100, update_frequency=10)
+_82        >>> for _ in range(100):
+_83        >>>     bar.display()
+_84
+_85        ^The progress bar in the terminal will only update once every ten
+calls, going from 0%->100% in 10% increments.
+_86        Note: If 'total' is not a multiple of 'update_frequency', the
+display will not show 100% completion when the loop finishes.
+_87
+_88        :param fill_ch: The character used to represent the completed part
+of the bar.
+_89
+_90        :param unfill_ch: The character used to represent the uncompleted
 part of the bar.
-81
-82        :param width_ratio: The width of the progress bar relative to the
+_91
+_92        :param width_ratio: The width of the progress bar relative to the
 width of the terminal window.
-83
-84        :param new_line_after_completion: Make a call to print() once
+_93
+_94        :param new_line_after_completion: Make a call to print() once
 self.counter >= self.total.
-85
-86        :param clear_after_completion: Make a call to printbuddies.clear()
+_95
+_96        :param clear_after_completion: Make a call to printbuddies.clear()
 once self.counter >= self.total.
-87
-88        Note: if new_line_after_completion and clear_after_completion are
+_97
+_98        Note: if new_line_after_completion and clear_after_completion are
 both True, the line will be cleared
-89        then a call to print() will be made."""
-90        self.total = total
-91        self.fill_ch = fill_ch[0]
-92        self.unfill_ch = unfill_ch[0]
-93        self.width_ratio = width_ratio
-94        self.new_line_after_completion = new_line_after_completion
-95        self.clear_after_completion = clear_after_completion
-96        self.timer = Timer()
-97        self.reset()
+_99        then a call to print() will be made."""
+100        self.total = total
+101        self.update_frequency = update_frequency
+102        self.fill_ch = fill_ch[0]
+103        self.unfill_ch = unfill_ch[0]
+104        self.width_ratio = width_ratio
+105        self.new_line_after_completion = new_line_after_completion
+106        self.clear_after_completion = clear_after_completion
+107        self.reset()
+108        self.with_context = False
 * Parameters *
     * total: The number of calls to reach 100% completion.
+    * update_frequency: The progress bar will only update once every this
+      number of calls to display(). The larger the value, the less performance
+      impact ProgBar has on the loop in which it is called. e.g.
+      >>> bar = ProgBar(100, update_frequency=10)
+      >>> for _ in range(100):
+      >>>     bar.display()
+^The progress bar in the terminal will only update once every ten calls, going
+from 0%->100% in 10% increments. Note: If 'total' is not a multiple of
+'update_frequency', the display will not show 100% completion when the loop
+finishes.
     * fill_ch: The character used to represent the completed part of the bar.
     * unfill_ch: The character used to represent the uncompleted part of the
       bar.
     * width_ratio: The width of the progress bar relative to the width of the
       terminal window.
     * new_line_after_completion: Make a call to print() once self.counter >=
       self.total.
     * clear_after_completion: Make a call to printbuddies.clear() once
       self.counter >= self.total.
 Note: if new_line_after_completion and clear_after_completion are both True,
 the line will be cleared then a call to print() will be made.
 ⁰
 def reset(self): View Source
-_99    def reset(self):
-100        self.counter = 0
-101        self.percent = ""
-102        self.prefix = ""
-103        self.suffix = ""
-104        self.filled = ""
-105        self.unfilled = ""
-106        self.bar = ""
+120    def reset(self):
+121        self.counter = 1
+122        self.percent = ""
+123        self.prefix = ""
+124        self.suffix = ""
+125        self.filled = ""
+126        self.unfilled = ""
+127        self.bar = ""
+128        self.timer = Timer(subsecond_resolution=False).start()
 ⁰
 def get_percent(self) -> str: View Source
-108    def get_percent(self) -> str:
-109        """Returns the percentage complete to two decimal places
-110        as a string without the %."""
-111        percent = str(round(100.0 * self.counter / self.total, 2))
-112        if len(percent.split(".")[1]) == 1:
-113            percent = percent + "0"
-114        if len(percent.split(".")[0]) == 1:
-115            percent = "0" + percent
-116        return percent
+134    def get_percent(self) -> str:
+135        """Returns the percentage complete to two decimal places
+136        as a string without the %."""
+137        percent = str(round(100.0 * self.counter / self.total, 2))
+138        if len(percent.split(".")[1]) == 1:
+139            percent = percent + "0"
+140        if len(percent.split(".")[0]) == 1:
+141            percent = "0" + percent
+142        return percent
 Returns the percentage complete to two decimal places as a string without the
 %.
 ⁰
 def get_bar(self): View Source
-134    def get_bar(self):
-135        return f"{self.prefix} [{self.filled}{self.unfilled}]-
-{self.percent}% {self.suffix}"
+160    def get_bar(self):
+161        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
+{self.unfilled}]-{self.percent}% {self.suffix}"
 ⁰
 def display(
 self,
 prefix: str = '',
 suffix: str = '',
-counter_override: float = None,
-total_override: float = None,
-return_object: Any = None) -> Any: View Source
-137    def display(
-138        self,
-139        prefix: str = "",
-140        suffix: str = "",
-141        counter_override: float = None,
-142        total_override: float = None,
-143        return_object: Any = None,
-144    ) -> Any:
-145        """Writes the progress bar to the terminal.
-146
-147        :param prefix: String affixed to the front of the progress bar.
-148
-149        :param suffix: String appended to the end of the progress bar.
-150
-151        :param counter_override: When an externally incremented completion
+counter_override: float | None = None,
+total_override: float | None = None,
+return_object: typing.Any | None = None) -> Any: View Source
+163    def display(
+164        self,
+165        prefix: str = "",
+166        suffix: str = "",
+167        counter_override: float | None = None,
+168        total_override: float | None = None,
+169        return_object: Any | None = None,
+170    ) -> Any:
+171        """Writes the progress bar to the terminal.
+172
+173        :param prefix: String affixed to the front of the progress bar.
+174
+175        :param suffix: String appended to the end of the progress bar.
+176
+177        :param counter_override: When an externally incremented completion
 counter is needed.
-152
-153        :param total_override: When an externally controlled bar total is
+178
+179        :param total_override: When an externally controlled bar total is
 needed.
-154
-155        :param return_object: An object to be returned by display().
-156
-157        Allows display() to be called within a comprehension:
-158
-159        e.g.
-160
-161        bar = ProgBar(9)
-162
-163        myList = [bar.display(return_object=i) for i in range(10)]"""
-164        if not self.timer.started:
-165            self.timer.start()
-166        if counter_override is not None:
-167            self.counter = counter_override
-168        if total_override:
-169            self.total = total_override
-170        # Don't wanna divide by 0 there, pal
-171        while self.total <= 0:
-172            self.total += 1
-173        self.prefix = prefix
-174        self.suffix = suffix
-175        self._prepare_bar()
-176        self._trim_bar()
-177        pad = " " * (self.terminal_width - len(self.bar))
-178        width = get_terminal_size().columns
-179        print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
-180        if self.counter >= self.total:
-181            self.timer.stop()
-182            if self.clear_after_completion:
-183                clear()
-184            if self.new_line_after_completion:
-185                print()
-186        self.counter += 1
-187        return return_object
+180
+181        :param return_object: An object to be returned by display().
+182
+183        Allows display() to be called within a comprehension:
+184
+185        e.g.
+186
+187        >>> bar = ProgBar(10)
+188        >>> def square(x: int | float)->int|float:
+189        >>>     return x * x
+190        >>> myList = [bar.display(return_object=square(i)) for i in range
+(10)]
+191        >>> <progress bar gets displayed>
+192        >>> myList
+193        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
+194        if not self.timer.started:
+195            self.timer.start()
+196        if counter_override is not None:
+197            self.counter = counter_override
+198        if total_override:
+199            self.total = total_override
+200        # Don't wanna divide by 0 there, pal
+201        while self.total <= 0:
+202            self.total += 1
+203        if self.counter % self.update_frequency == 0:
+204            self.prefix = prefix
+205            self.suffix = suffix
+206            self._prepare_bar()
+207            self._trim_bar()
+208            pad = " " * (self.terminal_width - len(self.bar))
+209            width = get_terminal_size().columns
+210            print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
+211        if self.counter >= self.total:
+212            self.timer.stop()
+213            if not self.with_context:
+214                if self.clear_after_completion:
+215                    clear()
+216                if self.new_line_after_completion:
+217                    print()
+218        self.counter += 1
+219        return return_object
 Writes the progress bar to the terminal.
 * Parameters *
     * prefix: String affixed to the front of the progress bar.
     * suffix: String appended to the end of the progress bar.
     * counter_override: When an externally incremented completion counter is
       needed.
     * total_override: When an externally controlled bar total is needed.
     * return_object: An object to be returned by display().
 Allows display() to be called within a comprehension:
 e.g.
-bar = ProgBar(9)
-myList = [bar.display(return_object=i) for i in range(10)]
+>>> bar = ProgBar(10)
+>>> def square(x: int | float)->int|float:
+>>>     return x * x
+>>> myList = [bar.display(return_object=square(i)) for i in range(10)]
+>>> <progress bar gets displayed>
+>>> myList
+>>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
+  ⁰
+class Spinner: View Source
+222class Spinner:
+223    """Prints one of a sequence of characters in order everytime display()
+is called.
+224    The display function writes the new character to the same line,
+overwriting the previous character.
+225    The sequence will be cycled through indefinitely.
+226    If used as a context manager, the last printed character will be cleared
+upon exiting."""
+227
+228    def __init__(self, sequence: list[Any] | None = None):
+229        """
+230        :param sequence: Override the built in spin sequence."""
+231        if sequence:
+232            self.sequence = sequence
+233        else:
+234            self.sequence = ["/", "-", "\\"]
+235
+236    def __enter__(self):
+237        return self
+238
+239    def __exit__(self, *args, **kwargs):
+240        clear()
+241
+242    @property
+243    def sequence(self) -> list[Any]:
+244        return self._sequence
+245
+246    @sequence.setter
+247    def sequence(self, character_list: list[Any]):
+248        # Buffer each element with a leading space
+249        # so that the character isn't obscured by the cursor
+250        self._sequence = [" " + str(ch) for ch in character_list]
+251
+252    def _get_next(self) -> str:
+253        """Pop the first element of self._sequence,
+254        append it to the end, and return the element."""
+255        ch = self.sequence.pop(0)
+256        self.sequence.append(ch)
+257        return ch
+258
+259    def display(self):
+260        """Print the next character in the sequence."""
+261        print_in_place(self._get_next())
+Prints one of a sequence of characters in order everytime display() is called.
+The display function writes the new character to the same line, overwriting the
+previous character. The sequence will be cycled through indefinitely. If used
+as a context manager, the last printed character will be cleared upon exiting.
+⁰
+Spinner(sequence: list[typing.Any] | None = None) View Source
+228    def __init__(self, sequence: list[Any] | None = None):
+229        """
+230        :param sequence: Override the built in spin sequence."""
+231        if sequence:
+232            self.sequence = sequence
+233        else:
+234            self.sequence = ["/", "-", "\\"]
+* Parameters *
+    * sequence: Override the built in spin sequence.
+⁰
+def display(self): View Source
+259    def display(self):
+260        """Print the next character in the sequence."""
+261        print_in_place(self._get_next())
+Print the next character in the sequence.
```

### Comparing `printbuddies-1.1.0/src/printbuddies/printbuddies.py` & `printbuddies-1.2.0/src/printbuddies/printbuddies.py`

 * *Files 22% similar despite different names*

```diff
@@ -49,101 +49,127 @@
     print(*info, sep="\n", end="")
     print("\n" * (int((height) / 2)), end="")
 
 
 class ProgBar:
     """Self incrementing, dynamically sized progress bar.
 
-    Includes a Timer object from noiftimer that starts timing
-    on the first call to display and stops timing once
-    self.counter >= self.total.
-    It can be easily added to the progress bar display by calling
-    Timer's checkTime function and passing the value to the 'prefix' or 'suffix'
-    param of self.display():
-
-    bar = ProgBar(total=someTotal)
-    bar.display(prefix=f"Run time: {bar.timer.checkTime()}")"""
+    Includes an internal timer that starts when this object is created.
+    It can be easily added to the progress bar display by adding
+    the 'runtime' property to display's prefix or suffix param:
+
+    >>> bar = ProgBar(total=100)
+    >>> time.sleep(30)
+    >>> bar.display(prefix=bar.runtime)
+    >>> "runtime: 30s [_///////////////////]1.00%" """
 
     def __init__(
         self,
         total: float,
+        update_frequency: int = 1,
         fill_ch: str = "_",
         unfill_ch: str = "/",
         width_ratio: float = 0.75,
         new_line_after_completion: bool = True,
         clear_after_completion: bool = False,
     ):
         """:param total: The number of calls to reach 100% completion.
 
+        :param update_frequency: The progress bar will only update once every this number of calls to display().
+        The larger the value, the less performance impact ProgBar has on the loop in which it is called.
+        e.g.
+        >>> bar = ProgBar(100, update_frequency=10)
+        >>> for _ in range(100):
+        >>>     bar.display()
+
+        ^The progress bar in the terminal will only update once every ten calls, going from 0%->100% in 10% increments.
+        Note: If 'total' is not a multiple of 'update_frequency', the display will not show 100% completion when the loop finishes.
+
         :param fill_ch: The character used to represent the completed part of the bar.
 
         :param unfill_ch: The character used to represent the uncompleted part of the bar.
 
         :param width_ratio: The width of the progress bar relative to the width of the terminal window.
 
         :param new_line_after_completion: Make a call to print() once self.counter >= self.total.
 
         :param clear_after_completion: Make a call to printbuddies.clear() once self.counter >= self.total.
 
         Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared
         then a call to print() will be made."""
         self.total = total
+        self.update_frequency = update_frequency
         self.fill_ch = fill_ch[0]
         self.unfill_ch = unfill_ch[0]
         self.width_ratio = width_ratio
         self.new_line_after_completion = new_line_after_completion
         self.clear_after_completion = clear_after_completion
-        self.timer = Timer()
         self.reset()
+        self.with_context = False
+
+    def __enter__(self):
+        self.with_context = True
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        if self.clear_after_completion:
+            clear()
+        else:
+            print()
 
     def reset(self):
-        self.counter = 0
+        self.counter = 1
         self.percent = ""
         self.prefix = ""
         self.suffix = ""
         self.filled = ""
         self.unfilled = ""
         self.bar = ""
+        self.timer = Timer(subsecond_resolution=False).start()
+
+    @property
+    def runtime(self) -> str:
+        return f"runtime:{self.timer.elapsed_str}"
 
     def get_percent(self) -> str:
         """Returns the percentage complete to two decimal places
         as a string without the %."""
         percent = str(round(100.0 * self.counter / self.total, 2))
         if len(percent.split(".")[1]) == 1:
             percent = percent + "0"
         if len(percent.split(".")[0]) == 1:
             percent = "0" + percent
         return percent
 
     def _prepare_bar(self):
         self.terminal_width = get_terminal_size().columns - 1
         bar_length = int(self.terminal_width * self.width_ratio)
-        progress = int(bar_length * self.counter / self.total)
+        progress = int(bar_length * min(self.counter / self.total, 1.0))
         self.filled = self.fill_ch * progress
         self.unfilled = self.unfill_ch * (bar_length - progress)
         self.percent = self.get_percent()
         self.bar = self.get_bar()
 
     def _trim_bar(self):
         original_width = self.width_ratio
         while len(self.bar) > self.terminal_width and self.width_ratio > 0:
             self.width_ratio -= 0.01
             self._prepare_bar()
         self.width_ratio = original_width
 
     def get_bar(self):
-        return f"{self.prefix} [{self.filled}{self.unfilled}]-{self.percent}% {self.suffix}"
+        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}{self.unfilled}]-{self.percent}% {self.suffix}"
 
     def display(
         self,
         prefix: str = "",
         suffix: str = "",
-        counter_override: float = None,
-        total_override: float = None,
-        return_object: Any = None,
+        counter_override: float | None = None,
+        total_override: float | None = None,
+        return_object: Any | None = None,
     ) -> Any:
         """Writes the progress bar to the terminal.
 
         :param prefix: String affixed to the front of the progress bar.
 
         :param suffix: String appended to the end of the progress bar.
 
@@ -153,34 +179,82 @@
 
         :param return_object: An object to be returned by display().
 
         Allows display() to be called within a comprehension:
 
         e.g.
 
-        bar = ProgBar(9)
-
-        myList = [bar.display(return_object=i) for i in range(10)]"""
+        >>> bar = ProgBar(10)
+        >>> def square(x: int | float)->int|float:
+        >>>     return x * x
+        >>> myList = [bar.display(return_object=square(i)) for i in range(10)]
+        >>> <progress bar gets displayed>
+        >>> myList
+        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
         if not self.timer.started:
             self.timer.start()
         if counter_override is not None:
             self.counter = counter_override
         if total_override:
             self.total = total_override
         # Don't wanna divide by 0 there, pal
         while self.total <= 0:
             self.total += 1
-        self.prefix = prefix
-        self.suffix = suffix
-        self._prepare_bar()
-        self._trim_bar()
-        pad = " " * (self.terminal_width - len(self.bar))
-        width = get_terminal_size().columns
-        print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
+        if self.counter % self.update_frequency == 0:
+            self.prefix = prefix
+            self.suffix = suffix
+            self._prepare_bar()
+            self._trim_bar()
+            pad = " " * (self.terminal_width - len(self.bar))
+            width = get_terminal_size().columns
+            print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
         if self.counter >= self.total:
             self.timer.stop()
-            if self.clear_after_completion:
-                clear()
-            if self.new_line_after_completion:
-                print()
+            if not self.with_context:
+                if self.clear_after_completion:
+                    clear()
+                if self.new_line_after_completion:
+                    print()
         self.counter += 1
         return return_object
+
+
+class Spinner:
+    """Prints one of a sequence of characters in order everytime display() is called.
+    The display function writes the new character to the same line, overwriting the previous character.
+    The sequence will be cycled through indefinitely.
+    If used as a context manager, the last printed character will be cleared upon exiting."""
+
+    def __init__(self, sequence: list[Any] | None = None):
+        """
+        :param sequence: Override the built in spin sequence."""
+        if sequence:
+            self.sequence = sequence
+        else:
+            self.sequence = ["/", "-", "\\"]
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        clear()
+
+    @property
+    def sequence(self) -> list[Any]:
+        return self._sequence
+
+    @sequence.setter
+    def sequence(self, character_list: list[Any]):
+        # Buffer each element with a leading space
+        # so that the character isn't obscured by the cursor
+        self._sequence = [" " + str(ch) for ch in character_list]
+
+    def _get_next(self) -> str:
+        """Pop the first element of self._sequence,
+        append it to the end, and return the element."""
+        ch = self.sequence.pop(0)
+        self.sequence.append(ch)
+        return ch
+
+    def display(self):
+        """Print the next character in the sequence."""
+        print_in_place(self._get_next())
```

### Comparing `printbuddies-1.1.0/LICENSE.txt` & `printbuddies-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `printbuddies-1.1.0/README.md` & `printbuddies-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,26 +8,57 @@
 
 ### ProgBar
 
 ProgBar is a self-incrementing, dynamically sized progress bar.<br>
 The progress counter and completion values can be manually overriden if desired.<br>
 The width of the progress bar is set according to a ratio of the terminal width
 so it will be resized automatically if the terminal width is changed.<br>
-The display function has a 'return_object' parameter, allowing ProgBar to be used in comprehensions.<br>
 
 <pre>
 from printbuddies import ProgBar
 total = 100
-bar = ProgBar(total=total-1)
+bar = ProgBar(total=total)
 for _ in range(total):
     bar.display()
 bar.reset()
 my_list = [bar.display(return_object=i) for i in range(total)]
 </pre>
 
+The display function has a 'return_object' parameter, allowing ProgBar to be used in comprehensions.
+<pre>
+bar = ProgBar(10)
+def square(x: int | float)->int|float:
+    return x * x
+myList = [bar.display(return_object=square(i)) for i in range(10)]
+{progress bar gets displayed}
+print(myList)
+[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
+</pre>
+
+ProgBar also supports being used with a context manager.
+
+### Spinner
+
+This class will print the next character from a sequence every time it's `display` method is called, clearing whatever is currently on the line.<br>
+The characters will be cycled through indefinitely.<br>
+<pre>
+from printbuddies import Spinner
+spinner = Spinner()
+for _ in range(10):
+    spinner.display()
+</pre>
+
+The default character sequence can be overridden:
+<pre>
+spinner = Spinner(sequence=["~_~_~_~_~_~_", "_~_~_~_~_~_~"])
+for _ in range(10):
+    spinner.display()
+</pre>
+
+When used with a context manager, the last character printed will be cleared from the terminal upon exiting.
 
 ### print_in_place
 
 'print_in_place' erases the current line in the terminal and then writes the value of 
 the 'string' param to the terminal.<br>
 <pre>
 from printbuddies import print_in_place
```

### Comparing `printbuddies-1.1.0/pyproject.toml` & `printbuddies-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "printbuddies"
 authors = [{name="Matt Manes"}]
 description = "Handful of utilities to do printing tricks to the terminal."
-version = "1.1.0"
-requires-python = ">=3.9"
+version = "1.2.0"
+requires-python = ">=3.10"
 dependencies = ["noiftimer", "pytest"]
 readme = "README.md"
 keywords = [
     "terminal",
     "print",
     "printing",
     "progressbar"
```

### Comparing `printbuddies-1.1.0/PKG-INFO` & `printbuddies-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: printbuddies
-Version: 1.1.0
+Version: 1.2.0
 Summary: Handful of utilities to do printing tricks to the terminal.
 Project-URL: Homepage, https://github.com/matt-manes/printbuddies
 Project-URL: Documentation, https://github.com/matt-manes/printbuddies/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/printbuddies/tree/main/src/printbuddies
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: print,printing,progressbar,terminal
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Requires-Dist: noiftimer
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # printbuddies
 
 A few utilities to do terminal printing tricks. <br>
@@ -26,26 +26,57 @@
 
 ### ProgBar
 
 ProgBar is a self-incrementing, dynamically sized progress bar.<br>
 The progress counter and completion values can be manually overriden if desired.<br>
 The width of the progress bar is set according to a ratio of the terminal width
 so it will be resized automatically if the terminal width is changed.<br>
-The display function has a 'return_object' parameter, allowing ProgBar to be used in comprehensions.<br>
 
 <pre>
 from printbuddies import ProgBar
 total = 100
-bar = ProgBar(total=total-1)
+bar = ProgBar(total=total)
 for _ in range(total):
     bar.display()
 bar.reset()
 my_list = [bar.display(return_object=i) for i in range(total)]
 </pre>
 
+The display function has a 'return_object' parameter, allowing ProgBar to be used in comprehensions.
+<pre>
+bar = ProgBar(10)
+def square(x: int | float)->int|float:
+    return x * x
+myList = [bar.display(return_object=square(i)) for i in range(10)]
+{progress bar gets displayed}
+print(myList)
+[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
+</pre>
+
+ProgBar also supports being used with a context manager.
+
+### Spinner
+
+This class will print the next character from a sequence every time it's `display` method is called, clearing whatever is currently on the line.<br>
+The characters will be cycled through indefinitely.<br>
+<pre>
+from printbuddies import Spinner
+spinner = Spinner()
+for _ in range(10):
+    spinner.display()
+</pre>
+
+The default character sequence can be overridden:
+<pre>
+spinner = Spinner(sequence=["~_~_~_~_~_~_", "_~_~_~_~_~_~"])
+for _ in range(10):
+    spinner.display()
+</pre>
+
+When used with a context manager, the last character printed will be cleared from the terminal upon exiting.
 
 ### print_in_place
 
 'print_in_place' erases the current line in the terminal and then writes the value of 
 the 'string' param to the terminal.<br>
 <pre>
 from printbuddies import print_in_place
```

