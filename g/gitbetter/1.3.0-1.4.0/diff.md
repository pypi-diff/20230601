# Comparing `tmp/gitbetter-1.3.0.tar.gz` & `tmp/gitbetter-1.4.0.tar.gz`

## Comparing `gitbetter-1.3.0.tar` & `gitbetter-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 gitbetter-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 gitbetter-1.3.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-1.3.0/docs/index.html
--rw-r--r--   0        0        0    63983 2020-02-02 00:00:00.000000 gitbetter-1.3.0/docs/search.js
--rw-r--r--   0        0        0   238036 2020-02-02 00:00:00.000000 gitbetter-1.3.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   249963 2020-02-02 00:00:00.000000 gitbetter-1.3.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-1.3.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 gitbetter-1.3.0/src/gitbetter/git.py
--rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 gitbetter-1.3.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-1.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 gitbetter-1.3.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 gitbetter-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 gitbetter-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/index.html
+-rw-r--r--   0        0        0    63979 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/search.js
+-rw-r--r--   0        0        0   238036 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   250260 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-1.4.0/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 gitbetter-1.4.0/src/gitbetter/git.py
+-rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 gitbetter-1.4.0/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 gitbetter-1.4.0/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 gitbetter-1.4.0/PKG-INFO
```

### Comparing `gitbetter-1.3.0/CHANGELOG.md` & `gitbetter-1.4.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## v1.3.0 (2023-05-30)
+
+#### New Features
+
+* add current_branch property to Git class
+#### Refactorings
+
+* Git().branch() arg defaults to empty string
+
+
 ## v1.2.0 (2023-05-30)
 
 #### New Features
 
 * add context manager to turn stdout capture on then back off
 #### Docs
```

### Comparing `gitbetter-1.3.0/docs/gitbetter.html` & `gitbetter-1.4.0/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-1.3.0/docs/search.js` & `gitbetter-1.4.0/docs/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -969,17 +969,17 @@
         "modulename": "gitbetter.gitbetter",
         "qualname": "commit_files_parser",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">ArgShellParser</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.gitbetter.amend_files_parser",
+        "fullname": "gitbetter.gitbetter.add_files_parser",
         "modulename": "gitbetter.gitbetter",
-        "qualname": "amend_files_parser",
+        "qualname": "add_files_parser",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">ArgShellParser</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.delete_branch_parser",
         "modulename": "gitbetter.gitbetter",
```

### Comparing `gitbetter-1.3.0/docs/gitbetter/git.html` & `gitbetter-1.4.0/docs/gitbetter/git.html`

 * *Files identical despite different names*

### Comparing `gitbetter-1.3.0/docs/gitbetter/gitbetter.html` & `gitbetter-1.4.0/docs/gitbetter/gitbetter.html`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             <li>
                     <a class="function" href="#new_remote_parser">new_remote_parser</a>
             </li>
             <li>
                     <a class="function" href="#commit_files_parser">commit_files_parser</a>
             </li>
             <li>
-                    <a class="function" href="#amend_files_parser">amend_files_parser</a>
+                    <a class="function" href="#add_files_parser">add_files_parser</a>
             </li>
             <li>
                     <a class="function" href="#delete_branch_parser">delete_branch_parser</a>
             </li>
             <li>
                     <a class="function" href="#recurse_files">recurse_files</a>
             </li>
@@ -209,265 +209,266 @@
 </span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="s2">        search for it in subfolders. This avoids having to type paths to files in subfolders,</span>
 </span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="s2">        but if you have multiple files in different subfolders with the same name that have changes they</span>
 </span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="s2">        will all be staged and committed.&quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="p">)</span>
 </span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>
 </span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="k">def</span> <span class="nf">amend_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="k">def</span> <span class="nf">add_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
 </span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
 </span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;-f&quot;</span><span class="p">,</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;--files&quot;</span><span class="p">,</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="p">)</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; If a file name is not found in the current working directory,</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="s2">        search for it in subfolders. This avoids having to type paths to files in subfolders,</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="s2">        but if you have multiple files in different subfolders with the same name that have changes they</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="s2">        will all be staged and committed.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="p">)</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="k">return</span> <span class="n">parser</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;files&quot;</span><span class="p">,</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. </span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        If not given, all files will be added.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="p">)</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; If a file name is not found in the current working directory,</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="s2">        search for it in subfolders. This avoids having to type paths to files in subfolders,</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="s2">        but if you have multiple files in different subfolders with the same name that have changes they</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="s2">        will all be staged and committed.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="p">)</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="k">def</span> <span class="nf">delete_branch_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="s2">&quot;branch&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the branch to delete. &quot;&quot;&quot;</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="p">)</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="s2">&quot;--remote&quot;</span><span class="p">,</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="p">)</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="k">return</span> <span class="n">parser</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="k">def</span> <span class="nf">delete_branch_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;branch&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the branch to delete. &quot;&quot;&quot;</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="p">)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="s2">&quot;--remote&quot;</span><span class="p">,</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="p">)</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="k">def</span> <span class="nf">recurse_files</span><span class="p">(</span><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="k">for</span> <span class="n">filename</span> <span class="ow">in</span> <span class="n">filenames</span><span class="p">:</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">))</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">results</span><span class="p">:</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;WARNING: Could not find any files with name </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>                <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">])</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="n">files</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="k">return</span> <span class="n">files</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="k">def</span> <span class="nf">recurse_files</span><span class="p">(</span><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">for</span> <span class="n">filename</span> <span class="ow">in</span> <span class="n">filenames</span><span class="p">:</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">))</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;WARNING: Could not find any files with name </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>                <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">])</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>            <span class="n">files</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="k">return</span> <span class="n">files</span>
 </span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="k">def</span> <span class="nf">files_postparser</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">:</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="o">=</span> <span class="n">recurse_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="k">def</span> <span class="nf">files_postparser</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">:</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="o">=</span> <span class="n">recurse_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="k">class</span> <span class="nc">GitBetter</span><span class="p">(</span><span class="n">ArgShell</span><span class="p">):</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="sd">&quot;&quot;&quot;GitBetter Shell.&quot;&quot;&quot;</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting gitbetter...</span><span class="se">\n</span><span class="s2">Enter &#39;help&#39; or &#39;?&#39; for command help.&quot;</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="n">git</span> <span class="o">=</span> <span class="n">Git</span><span class="p">()</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>                <span class="p">)</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="nd">@property</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="p">)</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="k">class</span> <span class="nc">GitBetter</span><span class="p">(</span><span class="n">ArgShell</span><span class="p">):</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="sd">&quot;&quot;&quot;GitBetter Shell.&quot;&quot;&quot;</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting gitbetter...</span><span class="se">\n</span><span class="s2">Enter &#39;help&#39; or &#39;?&#39; for command help.&quot;</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="n">git</span> <span class="o">=</span> <span class="n">Git</span><span class="p">()</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>                <span class="p">)</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="nd">@property</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="p">)</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">add_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">add_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>    <span class="n">main</span><span class="p">()</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="new_remote_parser">
                             <input id="new_remote_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -528,44 +529,45 @@
 </span><span id="commit_files_parser-41"><a href="#commit_files_parser-41"><span class="linenos">41</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span></pre></div>
 
 
     
 
                 </section>
-                <section id="amend_files_parser">
-                            <input id="amend_files_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                <section id="add_files_parser">
+                            <input id="add_files_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">amend_files_parser</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShellParser</span>:</span></span>
+        <span class="name">add_files_parser</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShellParser</span>:</span></span>
 
-                <label class="view-source-button" for="amend_files_parser-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="add_files_parser-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#amend_files_parser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="amend_files_parser-44"><a href="#amend_files_parser-44"><span class="linenos">44</span></a><span class="k">def</span> <span class="nf">amend_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
-</span><span id="amend_files_parser-45"><a href="#amend_files_parser-45"><span class="linenos">45</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
-</span><span id="amend_files_parser-46"><a href="#amend_files_parser-46"><span class="linenos">46</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="amend_files_parser-47"><a href="#amend_files_parser-47"><span class="linenos">47</span></a>        <span class="s2">&quot;-f&quot;</span><span class="p">,</span>
-</span><span id="amend_files_parser-48"><a href="#amend_files_parser-48"><span class="linenos">48</span></a>        <span class="s2">&quot;--files&quot;</span><span class="p">,</span>
-</span><span id="amend_files_parser-49"><a href="#amend_files_parser-49"><span class="linenos">49</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="amend_files_parser-50"><a href="#amend_files_parser-50"><span class="linenos">50</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="amend_files_parser-51"><a href="#amend_files_parser-51"><span class="linenos">51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="amend_files_parser-52"><a href="#amend_files_parser-52"><span class="linenos">52</span></a>    <span class="p">)</span>
-</span><span id="amend_files_parser-53"><a href="#amend_files_parser-53"><span class="linenos">53</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="amend_files_parser-54"><a href="#amend_files_parser-54"><span class="linenos">54</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="amend_files_parser-55"><a href="#amend_files_parser-55"><span class="linenos">55</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
-</span><span id="amend_files_parser-56"><a href="#amend_files_parser-56"><span class="linenos">56</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="amend_files_parser-57"><a href="#amend_files_parser-57"><span class="linenos">57</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; If a file name is not found in the current working directory,</span>
-</span><span id="amend_files_parser-58"><a href="#amend_files_parser-58"><span class="linenos">58</span></a><span class="s2">        search for it in subfolders. This avoids having to type paths to files in subfolders,</span>
-</span><span id="amend_files_parser-59"><a href="#amend_files_parser-59"><span class="linenos">59</span></a><span class="s2">        but if you have multiple files in different subfolders with the same name that have changes they</span>
-</span><span id="amend_files_parser-60"><a href="#amend_files_parser-60"><span class="linenos">60</span></a><span class="s2">        will all be staged and committed.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="amend_files_parser-61"><a href="#amend_files_parser-61"><span class="linenos">61</span></a>    <span class="p">)</span>
-</span><span id="amend_files_parser-62"><a href="#amend_files_parser-62"><span class="linenos">62</span></a>    <span class="k">return</span> <span class="n">parser</span>
+    <a class="headerlink" href="#add_files_parser"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="add_files_parser-44"><a href="#add_files_parser-44"><span class="linenos">44</span></a><span class="k">def</span> <span class="nf">add_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
+</span><span id="add_files_parser-45"><a href="#add_files_parser-45"><span class="linenos">45</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
+</span><span id="add_files_parser-46"><a href="#add_files_parser-46"><span class="linenos">46</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="add_files_parser-47"><a href="#add_files_parser-47"><span class="linenos">47</span></a>        <span class="s2">&quot;files&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-48"><a href="#add_files_parser-48"><span class="linenos">48</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="add_files_parser-49"><a href="#add_files_parser-49"><span class="linenos">49</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-50"><a href="#add_files_parser-50"><span class="linenos">50</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="add_files_parser-51"><a href="#add_files_parser-51"><span class="linenos">51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. </span>
+</span><span id="add_files_parser-52"><a href="#add_files_parser-52"><span class="linenos">52</span></a><span class="s2">        If not given, all files will be added.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-53"><a href="#add_files_parser-53"><span class="linenos">53</span></a>    <span class="p">)</span>
+</span><span id="add_files_parser-54"><a href="#add_files_parser-54"><span class="linenos">54</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="add_files_parser-55"><a href="#add_files_parser-55"><span class="linenos">55</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-56"><a href="#add_files_parser-56"><span class="linenos">56</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-57"><a href="#add_files_parser-57"><span class="linenos">57</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-58"><a href="#add_files_parser-58"><span class="linenos">58</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; If a file name is not found in the current working directory,</span>
+</span><span id="add_files_parser-59"><a href="#add_files_parser-59"><span class="linenos">59</span></a><span class="s2">        search for it in subfolders. This avoids having to type paths to files in subfolders,</span>
+</span><span id="add_files_parser-60"><a href="#add_files_parser-60"><span class="linenos">60</span></a><span class="s2">        but if you have multiple files in different subfolders with the same name that have changes they</span>
+</span><span id="add_files_parser-61"><a href="#add_files_parser-61"><span class="linenos">61</span></a><span class="s2">        will all be staged and committed.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-62"><a href="#add_files_parser-62"><span class="linenos">62</span></a>    <span class="p">)</span>
+</span><span id="add_files_parser-63"><a href="#add_files_parser-63"><span class="linenos">63</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="delete_branch_parser">
@@ -575,27 +577,27 @@
         <span class="def">def</span>
         <span class="name">delete_branch_parser</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShellParser</span>:</span></span>
 
                 <label class="view-source-button" for="delete_branch_parser-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_branch_parser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_branch_parser-65"><a href="#delete_branch_parser-65"><span class="linenos">65</span></a><span class="k">def</span> <span class="nf">delete_branch_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
-</span><span id="delete_branch_parser-66"><a href="#delete_branch_parser-66"><span class="linenos">66</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
-</span><span id="delete_branch_parser-67"><a href="#delete_branch_parser-67"><span class="linenos">67</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="delete_branch_parser-68"><a href="#delete_branch_parser-68"><span class="linenos">68</span></a>        <span class="s2">&quot;branch&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the branch to delete. &quot;&quot;&quot;</span>
-</span><span id="delete_branch_parser-69"><a href="#delete_branch_parser-69"><span class="linenos">69</span></a>    <span class="p">)</span>
-</span><span id="delete_branch_parser-70"><a href="#delete_branch_parser-70"><span class="linenos">70</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="delete_branch_parser-71"><a href="#delete_branch_parser-71"><span class="linenos">71</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="delete_branch_parser-72"><a href="#delete_branch_parser-72"><span class="linenos">72</span></a>        <span class="s2">&quot;--remote&quot;</span><span class="p">,</span>
-</span><span id="delete_branch_parser-73"><a href="#delete_branch_parser-73"><span class="linenos">73</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="delete_branch_parser-74"><a href="#delete_branch_parser-74"><span class="linenos">74</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
-</span><span id="delete_branch_parser-75"><a href="#delete_branch_parser-75"><span class="linenos">75</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="delete_branch_parser-76"><a href="#delete_branch_parser-76"><span class="linenos">76</span></a>    <span class="p">)</span>
-</span><span id="delete_branch_parser-77"><a href="#delete_branch_parser-77"><span class="linenos">77</span></a>    <span class="k">return</span> <span class="n">parser</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_branch_parser-66"><a href="#delete_branch_parser-66"><span class="linenos">66</span></a><span class="k">def</span> <span class="nf">delete_branch_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
+</span><span id="delete_branch_parser-67"><a href="#delete_branch_parser-67"><span class="linenos">67</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
+</span><span id="delete_branch_parser-68"><a href="#delete_branch_parser-68"><span class="linenos">68</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="delete_branch_parser-69"><a href="#delete_branch_parser-69"><span class="linenos">69</span></a>        <span class="s2">&quot;branch&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the branch to delete. &quot;&quot;&quot;</span>
+</span><span id="delete_branch_parser-70"><a href="#delete_branch_parser-70"><span class="linenos">70</span></a>    <span class="p">)</span>
+</span><span id="delete_branch_parser-71"><a href="#delete_branch_parser-71"><span class="linenos">71</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="delete_branch_parser-72"><a href="#delete_branch_parser-72"><span class="linenos">72</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="delete_branch_parser-73"><a href="#delete_branch_parser-73"><span class="linenos">73</span></a>        <span class="s2">&quot;--remote&quot;</span><span class="p">,</span>
+</span><span id="delete_branch_parser-74"><a href="#delete_branch_parser-74"><span class="linenos">74</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="delete_branch_parser-75"><a href="#delete_branch_parser-75"><span class="linenos">75</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
+</span><span id="delete_branch_parser-76"><a href="#delete_branch_parser-76"><span class="linenos">76</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="delete_branch_parser-77"><a href="#delete_branch_parser-77"><span class="linenos">77</span></a>    <span class="p">)</span>
+</span><span id="delete_branch_parser-78"><a href="#delete_branch_parser-78"><span class="linenos">78</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="recurse_files">
@@ -605,26 +607,26 @@
         <span class="def">def</span>
         <span class="name">recurse_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="recurse_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#recurse_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="recurse_files-80"><a href="#recurse_files-80"><span class="linenos">80</span></a><span class="k">def</span> <span class="nf">recurse_files</span><span class="p">(</span><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="recurse_files-81"><a href="#recurse_files-81"><span class="linenos">81</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="recurse_files-82"><a href="#recurse_files-82"><span class="linenos">82</span></a>    <span class="k">for</span> <span class="n">filename</span> <span class="ow">in</span> <span class="n">filenames</span><span class="p">:</span>
-</span><span id="recurse_files-83"><a href="#recurse_files-83"><span class="linenos">83</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="recurse_files-84"><a href="#recurse_files-84"><span class="linenos">84</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">))</span>
-</span><span id="recurse_files-85"><a href="#recurse_files-85"><span class="linenos">85</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">results</span><span class="p">:</span>
-</span><span id="recurse_files-86"><a href="#recurse_files-86"><span class="linenos">86</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;WARNING: Could not find any files with name </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="recurse_files-87"><a href="#recurse_files-87"><span class="linenos">87</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="recurse_files-88"><a href="#recurse_files-88"><span class="linenos">88</span></a>                <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">])</span>
-</span><span id="recurse_files-89"><a href="#recurse_files-89"><span class="linenos">89</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="recurse_files-90"><a href="#recurse_files-90"><span class="linenos">90</span></a>            <span class="n">files</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span>
-</span><span id="recurse_files-91"><a href="#recurse_files-91"><span class="linenos">91</span></a>    <span class="k">return</span> <span class="n">files</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="recurse_files-81"><a href="#recurse_files-81"><span class="linenos">81</span></a><span class="k">def</span> <span class="nf">recurse_files</span><span class="p">(</span><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="recurse_files-82"><a href="#recurse_files-82"><span class="linenos">82</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="recurse_files-83"><a href="#recurse_files-83"><span class="linenos">83</span></a>    <span class="k">for</span> <span class="n">filename</span> <span class="ow">in</span> <span class="n">filenames</span><span class="p">:</span>
+</span><span id="recurse_files-84"><a href="#recurse_files-84"><span class="linenos">84</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="recurse_files-85"><a href="#recurse_files-85"><span class="linenos">85</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">))</span>
+</span><span id="recurse_files-86"><a href="#recurse_files-86"><span class="linenos">86</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="recurse_files-87"><a href="#recurse_files-87"><span class="linenos">87</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;WARNING: Could not find any files with name </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="recurse_files-88"><a href="#recurse_files-88"><span class="linenos">88</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="recurse_files-89"><a href="#recurse_files-89"><span class="linenos">89</span></a>                <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">])</span>
+</span><span id="recurse_files-90"><a href="#recurse_files-90"><span class="linenos">90</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="recurse_files-91"><a href="#recurse_files-91"><span class="linenos">91</span></a>            <span class="n">files</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span>
+</span><span id="recurse_files-92"><a href="#recurse_files-92"><span class="linenos">92</span></a>    <span class="k">return</span> <span class="n">files</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="files_postparser">
@@ -634,18 +636,18 @@
         <span class="def">def</span>
         <span class="name">files_postparser</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">) -> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="files_postparser-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#files_postparser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="files_postparser-94"><a href="#files_postparser-94"><span class="linenos">94</span></a><span class="k">def</span> <span class="nf">files_postparser</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
-</span><span id="files_postparser-95"><a href="#files_postparser-95"><span class="linenos">95</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">:</span>
-</span><span id="files_postparser-96"><a href="#files_postparser-96"><span class="linenos">96</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="o">=</span> <span class="n">recurse_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="files_postparser-97"><a href="#files_postparser-97"><span class="linenos">97</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="files_postparser-95"><a href="#files_postparser-95"><span class="linenos">95</span></a><span class="k">def</span> <span class="nf">files_postparser</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
+</span><span id="files_postparser-96"><a href="#files_postparser-96"><span class="linenos">96</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">:</span>
+</span><span id="files_postparser-97"><a href="#files_postparser-97"><span class="linenos">97</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="o">=</span> <span class="n">recurse_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="files_postparser-98"><a href="#files_postparser-98"><span class="linenos">98</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="GitBetter">
@@ -655,201 +657,201 @@
     <span class="def">class</span>
     <span class="name">GitBetter</span><wbr>(<span class="base">argshell.argshell.ArgShell</span>):
 
                 <label class="view-source-button" for="GitBetter-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter-100"><a href="#GitBetter-100"><span class="linenos">100</span></a><span class="k">class</span> <span class="nc">GitBetter</span><span class="p">(</span><span class="n">ArgShell</span><span class="p">):</span>
-</span><span id="GitBetter-101"><a href="#GitBetter-101"><span class="linenos">101</span></a>    <span class="sd">&quot;&quot;&quot;GitBetter Shell.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-102"><a href="#GitBetter-102"><span class="linenos">102</span></a>
-</span><span id="GitBetter-103"><a href="#GitBetter-103"><span class="linenos">103</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting gitbetter...</span><span class="se">\n</span><span class="s2">Enter &#39;help&#39; or &#39;?&#39; for command help.&quot;</span>
-</span><span id="GitBetter-104"><a href="#GitBetter-104"><span class="linenos">104</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
-</span><span id="GitBetter-105"><a href="#GitBetter-105"><span class="linenos">105</span></a>    <span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="GitBetter-106"><a href="#GitBetter-106"><span class="linenos">106</span></a>    <span class="n">git</span> <span class="o">=</span> <span class="n">Git</span><span class="p">()</span>
-</span><span id="GitBetter-107"><a href="#GitBetter-107"><span class="linenos">107</span></a>
-</span><span id="GitBetter-108"><a href="#GitBetter-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-109"><a href="#GitBetter-109"><span class="linenos">109</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="GitBetter-110"><a href="#GitBetter-110"><span class="linenos">110</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="GitBetter-111"><a href="#GitBetter-111"><span class="linenos">111</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="GitBetter-112"><a href="#GitBetter-112"><span class="linenos">112</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="GitBetter-113"><a href="#GitBetter-113"><span class="linenos">113</span></a>
-</span><span id="GitBetter-114"><a href="#GitBetter-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-115"><a href="#GitBetter-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-116"><a href="#GitBetter-116"><span class="linenos">116</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="GitBetter-117"><a href="#GitBetter-117"><span class="linenos">117</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="GitBetter-118"><a href="#GitBetter-118"><span class="linenos">118</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="GitBetter-119"><a href="#GitBetter-119"><span class="linenos">119</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="GitBetter-120"><a href="#GitBetter-120"><span class="linenos">120</span></a>                <span class="nb">print</span><span class="p">(</span>
-</span><span id="GitBetter-121"><a href="#GitBetter-121"><span class="linenos">121</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
-</span><span id="GitBetter-122"><a href="#GitBetter-122"><span class="linenos">122</span></a>                <span class="p">)</span>
-</span><span id="GitBetter-123"><a href="#GitBetter-123"><span class="linenos">123</span></a>        <span class="nb">print</span><span class="p">()</span>
-</span><span id="GitBetter-124"><a href="#GitBetter-124"><span class="linenos">124</span></a>
-</span><span id="GitBetter-125"><a href="#GitBetter-125"><span class="linenos">125</span></a>    <span class="nd">@property</span>
-</span><span id="GitBetter-126"><a href="#GitBetter-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter-127"><a href="#GitBetter-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="GitBetter-128"><a href="#GitBetter-128"><span class="linenos">128</span></a>
-</span><span id="GitBetter-129"><a href="#GitBetter-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-130"><a href="#GitBetter-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
-</span><span id="GitBetter-131"><a href="#GitBetter-131"><span class="linenos">131</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
-</span><span id="GitBetter-132"><a href="#GitBetter-132"><span class="linenos">132</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-133"><a href="#GitBetter-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
-</span><span id="GitBetter-134"><a href="#GitBetter-134"><span class="linenos">134</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
-</span><span id="GitBetter-135"><a href="#GitBetter-135"><span class="linenos">135</span></a>        <span class="p">)</span>
-</span><span id="GitBetter-136"><a href="#GitBetter-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="GitBetter-137"><a href="#GitBetter-137"><span class="linenos">137</span></a>
-</span><span id="GitBetter-138"><a href="#GitBetter-138"><span class="linenos">138</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-139"><a href="#GitBetter-139"><span class="linenos">139</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-140"><a href="#GitBetter-140"><span class="linenos">140</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="GitBetter-141"><a href="#GitBetter-141"><span class="linenos">141</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
-</span><span id="GitBetter-142"><a href="#GitBetter-142"><span class="linenos">142</span></a>
-</span><span id="GitBetter-143"><a href="#GitBetter-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-144"><a href="#GitBetter-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="GitBetter-145"><a href="#GitBetter-145"><span class="linenos">145</span></a>
-</span><span id="GitBetter-146"><a href="#GitBetter-146"><span class="linenos">146</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-147"><a href="#GitBetter-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="GitBetter-148"><a href="#GitBetter-148"><span class="linenos">148</span></a>
-</span><span id="GitBetter-149"><a href="#GitBetter-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-150"><a href="#GitBetter-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-151"><a href="#GitBetter-151"><span class="linenos">151</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
-</span><span id="GitBetter-152"><a href="#GitBetter-152"><span class="linenos">152</span></a>
-</span><span id="GitBetter-153"><a href="#GitBetter-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-154"><a href="#GitBetter-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-155"><a href="#GitBetter-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
-</span><span id="GitBetter-156"><a href="#GitBetter-156"><span class="linenos">156</span></a>
-</span><span id="GitBetter-157"><a href="#GitBetter-157"><span class="linenos">157</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="GitBetter-158"><a href="#GitBetter-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-159"><a href="#GitBetter-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="GitBetter-160"><a href="#GitBetter-160"><span class="linenos">160</span></a>
-</span><span id="GitBetter-161"><a href="#GitBetter-161"><span class="linenos">161</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-162"><a href="#GitBetter-162"><span class="linenos">162</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="GitBetter-163"><a href="#GitBetter-163"><span class="linenos">163</span></a>
-</span><span id="GitBetter-164"><a href="#GitBetter-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-165"><a href="#GitBetter-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-166"><a href="#GitBetter-166"><span class="linenos">166</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
-</span><span id="GitBetter-167"><a href="#GitBetter-167"><span class="linenos">167</span></a>
-</span><span id="GitBetter-168"><a href="#GitBetter-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-169"><a href="#GitBetter-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-170"><a href="#GitBetter-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
-</span><span id="GitBetter-171"><a href="#GitBetter-171"><span class="linenos">171</span></a>
-</span><span id="GitBetter-172"><a href="#GitBetter-172"><span class="linenos">172</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-173"><a href="#GitBetter-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-174"><a href="#GitBetter-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="GitBetter-175"><a href="#GitBetter-175"><span class="linenos">175</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-176"><a href="#GitBetter-176"><span class="linenos">176</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-177"><a href="#GitBetter-177"><span class="linenos">177</span></a>
-</span><span id="GitBetter-178"><a href="#GitBetter-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-179"><a href="#GitBetter-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-180"><a href="#GitBetter-180"><span class="linenos">180</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="GitBetter-181"><a href="#GitBetter-181"><span class="linenos">181</span></a>
-</span><span id="GitBetter-182"><a href="#GitBetter-182"><span class="linenos">182</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-183"><a href="#GitBetter-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-184"><a href="#GitBetter-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-185"><a href="#GitBetter-185"><span class="linenos">185</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span><span id="GitBetter-186"><a href="#GitBetter-186"><span class="linenos">186</span></a>
-</span><span id="GitBetter-187"><a href="#GitBetter-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-188"><a href="#GitBetter-188"><span class="linenos">188</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-189"><a href="#GitBetter-189"><span class="linenos">189</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-190"><a href="#GitBetter-190"><span class="linenos">190</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter-191"><a href="#GitBetter-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-192"><a href="#GitBetter-192"><span class="linenos">192</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter-193"><a href="#GitBetter-193"><span class="linenos">193</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="GitBetter-194"><a href="#GitBetter-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-195"><a href="#GitBetter-195"><span class="linenos">195</span></a>
-</span><span id="GitBetter-196"><a href="#GitBetter-196"><span class="linenos">196</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-197"><a href="#GitBetter-197"><span class="linenos">197</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-198"><a href="#GitBetter-198"><span class="linenos">198</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-199"><a href="#GitBetter-199"><span class="linenos">199</span></a>
-</span><span id="GitBetter-200"><a href="#GitBetter-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-201"><a href="#GitBetter-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-202"><a href="#GitBetter-202"><span class="linenos">202</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="GitBetter-203"><a href="#GitBetter-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-204"><a href="#GitBetter-204"><span class="linenos">204</span></a>
-</span><span id="GitBetter-205"><a href="#GitBetter-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-206"><a href="#GitBetter-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-207"><a href="#GitBetter-207"><span class="linenos">207</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-208"><a href="#GitBetter-208"><span class="linenos">208</span></a>
-</span><span id="GitBetter-209"><a href="#GitBetter-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-210"><a href="#GitBetter-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="GitBetter-211"><a href="#GitBetter-211"><span class="linenos">211</span></a>
-</span><span id="GitBetter-212"><a href="#GitBetter-212"><span class="linenos">212</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-213"><a href="#GitBetter-213"><span class="linenos">213</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="GitBetter-214"><a href="#GitBetter-214"><span class="linenos">214</span></a>
-</span><span id="GitBetter-215"><a href="#GitBetter-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-216"><a href="#GitBetter-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="GitBetter-217"><a href="#GitBetter-217"><span class="linenos">217</span></a>
-</span><span id="GitBetter-218"><a href="#GitBetter-218"><span class="linenos">218</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-219"><a href="#GitBetter-219"><span class="linenos">219</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="GitBetter-220"><a href="#GitBetter-220"><span class="linenos">220</span></a>
-</span><span id="GitBetter-221"><a href="#GitBetter-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-222"><a href="#GitBetter-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-223"><a href="#GitBetter-223"><span class="linenos">223</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
-</span><span id="GitBetter-224"><a href="#GitBetter-224"><span class="linenos">224</span></a>
-</span><span id="GitBetter-225"><a href="#GitBetter-225"><span class="linenos">225</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>
-</span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
-</span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>
-</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>
-</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
-</span><span id="GitBetter-240"><a href="#GitBetter-240"><span class="linenos">240</span></a>
-</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>
-</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>
-</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
-</span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>
-</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>
-</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter-264"><a href="#GitBetter-264"><span class="linenos">264</span></a>
-</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a>
-</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="GitBetter-269"><a href="#GitBetter-269"><span class="linenos">269</span></a>
-</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter-272"><a href="#GitBetter-272"><span class="linenos">272</span></a>
-</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a>
-</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="GitBetter-277"><a href="#GitBetter-277"><span class="linenos">277</span></a>
-</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter-280"><a href="#GitBetter-280"><span class="linenos">280</span></a>
-</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a>
-</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter-284"><a href="#GitBetter-284"><span class="linenos">284</span></a>
-</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter-101"><a href="#GitBetter-101"><span class="linenos">101</span></a><span class="k">class</span> <span class="nc">GitBetter</span><span class="p">(</span><span class="n">ArgShell</span><span class="p">):</span>
+</span><span id="GitBetter-102"><a href="#GitBetter-102"><span class="linenos">102</span></a>    <span class="sd">&quot;&quot;&quot;GitBetter Shell.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-103"><a href="#GitBetter-103"><span class="linenos">103</span></a>
+</span><span id="GitBetter-104"><a href="#GitBetter-104"><span class="linenos">104</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting gitbetter...</span><span class="se">\n</span><span class="s2">Enter &#39;help&#39; or &#39;?&#39; for command help.&quot;</span>
+</span><span id="GitBetter-105"><a href="#GitBetter-105"><span class="linenos">105</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="GitBetter-106"><a href="#GitBetter-106"><span class="linenos">106</span></a>    <span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="GitBetter-107"><a href="#GitBetter-107"><span class="linenos">107</span></a>    <span class="n">git</span> <span class="o">=</span> <span class="n">Git</span><span class="p">()</span>
+</span><span id="GitBetter-108"><a href="#GitBetter-108"><span class="linenos">108</span></a>
+</span><span id="GitBetter-109"><a href="#GitBetter-109"><span class="linenos">109</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-110"><a href="#GitBetter-110"><span class="linenos">110</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter-111"><a href="#GitBetter-111"><span class="linenos">111</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter-112"><a href="#GitBetter-112"><span class="linenos">112</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="GitBetter-113"><a href="#GitBetter-113"><span class="linenos">113</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter-114"><a href="#GitBetter-114"><span class="linenos">114</span></a>
+</span><span id="GitBetter-115"><a href="#GitBetter-115"><span class="linenos">115</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-116"><a href="#GitBetter-116"><span class="linenos">116</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-117"><a href="#GitBetter-117"><span class="linenos">117</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter-118"><a href="#GitBetter-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="GitBetter-119"><a href="#GitBetter-119"><span class="linenos">119</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter-120"><a href="#GitBetter-120"><span class="linenos">120</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter-121"><a href="#GitBetter-121"><span class="linenos">121</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="GitBetter-122"><a href="#GitBetter-122"><span class="linenos">122</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="GitBetter-123"><a href="#GitBetter-123"><span class="linenos">123</span></a>                <span class="p">)</span>
+</span><span id="GitBetter-124"><a href="#GitBetter-124"><span class="linenos">124</span></a>        <span class="nb">print</span><span class="p">()</span>
+</span><span id="GitBetter-125"><a href="#GitBetter-125"><span class="linenos">125</span></a>
+</span><span id="GitBetter-126"><a href="#GitBetter-126"><span class="linenos">126</span></a>    <span class="nd">@property</span>
+</span><span id="GitBetter-127"><a href="#GitBetter-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter-128"><a href="#GitBetter-128"><span class="linenos">128</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="GitBetter-129"><a href="#GitBetter-129"><span class="linenos">129</span></a>
+</span><span id="GitBetter-130"><a href="#GitBetter-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-131"><a href="#GitBetter-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="GitBetter-132"><a href="#GitBetter-132"><span class="linenos">132</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="GitBetter-133"><a href="#GitBetter-133"><span class="linenos">133</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-134"><a href="#GitBetter-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="GitBetter-135"><a href="#GitBetter-135"><span class="linenos">135</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="GitBetter-136"><a href="#GitBetter-136"><span class="linenos">136</span></a>        <span class="p">)</span>
+</span><span id="GitBetter-137"><a href="#GitBetter-137"><span class="linenos">137</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter-138"><a href="#GitBetter-138"><span class="linenos">138</span></a>
+</span><span id="GitBetter-139"><a href="#GitBetter-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-140"><a href="#GitBetter-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-141"><a href="#GitBetter-141"><span class="linenos">141</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="GitBetter-142"><a href="#GitBetter-142"><span class="linenos">142</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="GitBetter-143"><a href="#GitBetter-143"><span class="linenos">143</span></a>
+</span><span id="GitBetter-144"><a href="#GitBetter-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-145"><a href="#GitBetter-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="GitBetter-146"><a href="#GitBetter-146"><span class="linenos">146</span></a>
+</span><span id="GitBetter-147"><a href="#GitBetter-147"><span class="linenos">147</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-148"><a href="#GitBetter-148"><span class="linenos">148</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter-149"><a href="#GitBetter-149"><span class="linenos">149</span></a>
+</span><span id="GitBetter-150"><a href="#GitBetter-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-151"><a href="#GitBetter-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-152"><a href="#GitBetter-152"><span class="linenos">152</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="GitBetter-153"><a href="#GitBetter-153"><span class="linenos">153</span></a>
+</span><span id="GitBetter-154"><a href="#GitBetter-154"><span class="linenos">154</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-155"><a href="#GitBetter-155"><span class="linenos">155</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-156"><a href="#GitBetter-156"><span class="linenos">156</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+</span><span id="GitBetter-157"><a href="#GitBetter-157"><span class="linenos">157</span></a>
+</span><span id="GitBetter-158"><a href="#GitBetter-158"><span class="linenos">158</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="GitBetter-159"><a href="#GitBetter-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-160"><a href="#GitBetter-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="GitBetter-161"><a href="#GitBetter-161"><span class="linenos">161</span></a>
+</span><span id="GitBetter-162"><a href="#GitBetter-162"><span class="linenos">162</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-163"><a href="#GitBetter-163"><span class="linenos">163</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="GitBetter-164"><a href="#GitBetter-164"><span class="linenos">164</span></a>
+</span><span id="GitBetter-165"><a href="#GitBetter-165"><span class="linenos">165</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-166"><a href="#GitBetter-166"><span class="linenos">166</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-167"><a href="#GitBetter-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+</span><span id="GitBetter-168"><a href="#GitBetter-168"><span class="linenos">168</span></a>
+</span><span id="GitBetter-169"><a href="#GitBetter-169"><span class="linenos">169</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-170"><a href="#GitBetter-170"><span class="linenos">170</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-171"><a href="#GitBetter-171"><span class="linenos">171</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+</span><span id="GitBetter-172"><a href="#GitBetter-172"><span class="linenos">172</span></a>
+</span><span id="GitBetter-173"><a href="#GitBetter-173"><span class="linenos">173</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">add_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-174"><a href="#GitBetter-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-175"><a href="#GitBetter-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="GitBetter-176"><a href="#GitBetter-176"><span class="linenos">176</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-177"><a href="#GitBetter-177"><span class="linenos">177</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-178"><a href="#GitBetter-178"><span class="linenos">178</span></a>
+</span><span id="GitBetter-179"><a href="#GitBetter-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-180"><a href="#GitBetter-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-181"><a href="#GitBetter-181"><span class="linenos">181</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-182"><a href="#GitBetter-182"><span class="linenos">182</span></a>
+</span><span id="GitBetter-183"><a href="#GitBetter-183"><span class="linenos">183</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-184"><a href="#GitBetter-184"><span class="linenos">184</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-185"><a href="#GitBetter-185"><span class="linenos">185</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-186"><a href="#GitBetter-186"><span class="linenos">186</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+</span><span id="GitBetter-187"><a href="#GitBetter-187"><span class="linenos">187</span></a>
+</span><span id="GitBetter-188"><a href="#GitBetter-188"><span class="linenos">188</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-189"><a href="#GitBetter-189"><span class="linenos">189</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-190"><a href="#GitBetter-190"><span class="linenos">190</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-191"><a href="#GitBetter-191"><span class="linenos">191</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter-192"><a href="#GitBetter-192"><span class="linenos">192</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-193"><a href="#GitBetter-193"><span class="linenos">193</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter-194"><a href="#GitBetter-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="GitBetter-195"><a href="#GitBetter-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-196"><a href="#GitBetter-196"><span class="linenos">196</span></a>
+</span><span id="GitBetter-197"><a href="#GitBetter-197"><span class="linenos">197</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-198"><a href="#GitBetter-198"><span class="linenos">198</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-199"><a href="#GitBetter-199"><span class="linenos">199</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-200"><a href="#GitBetter-200"><span class="linenos">200</span></a>
+</span><span id="GitBetter-201"><a href="#GitBetter-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-202"><a href="#GitBetter-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-203"><a href="#GitBetter-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="GitBetter-204"><a href="#GitBetter-204"><span class="linenos">204</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-205"><a href="#GitBetter-205"><span class="linenos">205</span></a>
+</span><span id="GitBetter-206"><a href="#GitBetter-206"><span class="linenos">206</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-207"><a href="#GitBetter-207"><span class="linenos">207</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-208"><a href="#GitBetter-208"><span class="linenos">208</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-209"><a href="#GitBetter-209"><span class="linenos">209</span></a>
+</span><span id="GitBetter-210"><a href="#GitBetter-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-211"><a href="#GitBetter-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="GitBetter-212"><a href="#GitBetter-212"><span class="linenos">212</span></a>
+</span><span id="GitBetter-213"><a href="#GitBetter-213"><span class="linenos">213</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-214"><a href="#GitBetter-214"><span class="linenos">214</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-215"><a href="#GitBetter-215"><span class="linenos">215</span></a>
+</span><span id="GitBetter-216"><a href="#GitBetter-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-217"><a href="#GitBetter-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="GitBetter-218"><a href="#GitBetter-218"><span class="linenos">218</span></a>
+</span><span id="GitBetter-219"><a href="#GitBetter-219"><span class="linenos">219</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-220"><a href="#GitBetter-220"><span class="linenos">220</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-221"><a href="#GitBetter-221"><span class="linenos">221</span></a>
+</span><span id="GitBetter-222"><a href="#GitBetter-222"><span class="linenos">222</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-223"><a href="#GitBetter-223"><span class="linenos">223</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-224"><a href="#GitBetter-224"><span class="linenos">224</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+</span><span id="GitBetter-225"><a href="#GitBetter-225"><span class="linenos">225</span></a>
+</span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>
+</span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>
+</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>
+</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-240"><a href="#GitBetter-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>
+</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">add_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>
+</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>
+</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>
+</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>
+</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-264"><a href="#GitBetter-264"><span class="linenos">264</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a>
+</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a>
+</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-269"><a href="#GitBetter-269"><span class="linenos">269</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a>
+</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-272"><a href="#GitBetter-272"><span class="linenos">272</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a>
+</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a>
+</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-277"><a href="#GitBetter-277"><span class="linenos">277</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a>
+</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-280"><a href="#GitBetter-280"><span class="linenos">280</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a>
+</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a>
+</span><span id="GitBetter-284"><a href="#GitBetter-284"><span class="linenos">284</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a>
+</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-287"><a href="#GitBetter-287"><span class="linenos">287</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>GitBetter Shell.</p>
 </div>
 
 
@@ -860,19 +862,19 @@
         <span class="def">def</span>
         <span class="name">default</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">line</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.default-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.default"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.default-108"><a href="#GitBetter.default-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.default-109"><a href="#GitBetter.default-109"><span class="linenos">109</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="GitBetter.default-110"><a href="#GitBetter.default-110"><span class="linenos">110</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="GitBetter.default-111"><a href="#GitBetter.default-111"><span class="linenos">111</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="GitBetter.default-112"><a href="#GitBetter.default-112"><span class="linenos">112</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.default-109"><a href="#GitBetter.default-109"><span class="linenos">109</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.default-110"><a href="#GitBetter.default-110"><span class="linenos">110</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter.default-111"><a href="#GitBetter.default-111"><span class="linenos">111</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter.default-112"><a href="#GitBetter.default-112"><span class="linenos">112</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="GitBetter.default-113"><a href="#GitBetter.default-113"><span class="linenos">113</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Called on an input line when the command prefix is not recognized.</p>
 
 <p>If this method is not overridden, it prints an error message and
 returns.</p>
@@ -887,24 +889,24 @@
         <span class="def">def</span>
         <span class="name">do_help</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_help-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_help"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_help-114"><a href="#GitBetter.do_help-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_help-115"><a href="#GitBetter.do_help-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_help-116"><a href="#GitBetter.do_help-116"><span class="linenos">116</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="GitBetter.do_help-117"><a href="#GitBetter.do_help-117"><span class="linenos">117</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="GitBetter.do_help-118"><a href="#GitBetter.do_help-118"><span class="linenos">118</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="GitBetter.do_help-119"><a href="#GitBetter.do_help-119"><span class="linenos">119</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="GitBetter.do_help-120"><a href="#GitBetter.do_help-120"><span class="linenos">120</span></a>                <span class="nb">print</span><span class="p">(</span>
-</span><span id="GitBetter.do_help-121"><a href="#GitBetter.do_help-121"><span class="linenos">121</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
-</span><span id="GitBetter.do_help-122"><a href="#GitBetter.do_help-122"><span class="linenos">122</span></a>                <span class="p">)</span>
-</span><span id="GitBetter.do_help-123"><a href="#GitBetter.do_help-123"><span class="linenos">123</span></a>        <span class="nb">print</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_help-115"><a href="#GitBetter.do_help-115"><span class="linenos">115</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_help-116"><a href="#GitBetter.do_help-116"><span class="linenos">116</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_help-117"><a href="#GitBetter.do_help-117"><span class="linenos">117</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter.do_help-118"><a href="#GitBetter.do_help-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="GitBetter.do_help-119"><a href="#GitBetter.do_help-119"><span class="linenos">119</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter.do_help-120"><a href="#GitBetter.do_help-120"><span class="linenos">120</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter.do_help-121"><a href="#GitBetter.do_help-121"><span class="linenos">121</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="GitBetter.do_help-122"><a href="#GitBetter.do_help-122"><span class="linenos">122</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="GitBetter.do_help-123"><a href="#GitBetter.do_help-123"><span class="linenos">123</span></a>                <span class="p">)</span>
+</span><span id="GitBetter.do_help-124"><a href="#GitBetter.do_help-124"><span class="linenos">124</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>List available commands with "help" or detailed help with "help cmd".</p>
 </div>
 
 
@@ -916,22 +918,22 @@
         <span class="def">def</span>
         <span class="name">do_toggle_unrecognized_command_behavior</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_toggle_unrecognized_command_behavior-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_toggle_unrecognized_command_behavior"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_toggle_unrecognized_command_behavior-129"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-130"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-131"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-131"><span class="linenos">131</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-132"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-132"><span class="linenos">132</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-133"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-134"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-134"><span class="linenos">134</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-135"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-135"><span class="linenos">135</span></a>        <span class="p">)</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-136"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_toggle_unrecognized_command_behavior-130"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-131"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-132"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-132"><span class="linenos">132</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-133"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-133"><span class="linenos">133</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-134"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-135"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-135"><span class="linenos">135</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-136"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-136"><span class="linenos">136</span></a>        <span class="p">)</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-137"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-137"><span class="linenos">137</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.
 When on (the default), <code><a href="#GitBetter">GitBetter</a></code> will treat unrecognized commands as if you added the <code>sys</code> command in front of the input, i.e. <code>os.system(your_input)</code>.
 When off, an <code>unknown syntax</code> message will be printed and no commands will be executed.</p>
 </div>
@@ -945,18 +947,18 @@
         <span class="def">def</span>
         <span class="name">do_cd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_cd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_cd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cd-138"><a href="#GitBetter.do_cd-138"><span class="linenos">138</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_cd-139"><a href="#GitBetter.do_cd-139"><span class="linenos">139</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_cd-140"><a href="#GitBetter.do_cd-140"><span class="linenos">140</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="GitBetter.do_cd-141"><a href="#GitBetter.do_cd-141"><span class="linenos">141</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cd-139"><a href="#GitBetter.do_cd-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_cd-140"><a href="#GitBetter.do_cd-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_cd-141"><a href="#GitBetter.do_cd-141"><span class="linenos">141</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="GitBetter.do_cd-142"><a href="#GitBetter.do_cd-142"><span class="linenos">142</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Change current working directory to <code>path</code>.</p>
 </div>
 
 
@@ -968,19 +970,19 @@
         <span class="def">def</span>
         <span class="name">do_git</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_git-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_git"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_git-143"><a href="#GitBetter.do_git-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_git-144"><a href="#GitBetter.do_git-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="GitBetter.do_git-145"><a href="#GitBetter.do_git-145"><span class="linenos">145</span></a>
-</span><span id="GitBetter.do_git-146"><a href="#GitBetter.do_git-146"><span class="linenos">146</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_git-147"><a href="#GitBetter.do_git-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_git-144"><a href="#GitBetter.do_git-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_git-145"><a href="#GitBetter.do_git-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="GitBetter.do_git-146"><a href="#GitBetter.do_git-146"><span class="linenos">146</span></a>
+</span><span id="GitBetter.do_git-147"><a href="#GitBetter.do_git-147"><span class="linenos">147</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_git-148"><a href="#GitBetter.do_git-148"><span class="linenos">148</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Directly execute <code>git {arg}</code>.</p>
 
 <p>i.e. You can still do everything directly invoking git can do.</p>
 </div>
@@ -994,17 +996,17 @@
         <span class="def">def</span>
         <span class="name">do_new_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_repo-149"><a href="#GitBetter.do_new_repo-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_repo-150"><a href="#GitBetter.do_new_repo-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_repo-151"><a href="#GitBetter.do_new_repo-151"><span class="linenos">151</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_repo-150"><a href="#GitBetter.do_new_repo-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_repo-151"><a href="#GitBetter.do_new_repo-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_repo-152"><a href="#GitBetter.do_new_repo-152"><span class="linenos">152</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a new git repo in this directory.</p>
 </div>
 
 
@@ -1016,17 +1018,17 @@
         <span class="def">def</span>
         <span class="name">do_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_branch-153"><a href="#GitBetter.do_new_branch-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_branch-154"><a href="#GitBetter.do_new_branch-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_branch-155"><a href="#GitBetter.do_new_branch-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_branch-154"><a href="#GitBetter.do_new_branch-154"><span class="linenos">154</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_branch-155"><a href="#GitBetter.do_new_branch-155"><span class="linenos">155</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_branch-156"><a href="#GitBetter.do_new_branch-156"><span class="linenos">156</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create and switch to a new branch named after the supplied arg.</p>
 </div>
 
 
@@ -1039,20 +1041,20 @@
         <span class="def">def</span>
         <span class="name">do_new_gh_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_gh_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_gh_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-157"><a href="#GitBetter.do_new_gh_remote-157"><span class="linenos">157</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_new_gh_remote-158"><a href="#GitBetter.do_new_gh_remote-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_gh_remote-159"><a href="#GitBetter.do_new_gh_remote-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="GitBetter.do_new_gh_remote-160"><a href="#GitBetter.do_new_gh_remote-160"><span class="linenos">160</span></a>
-</span><span id="GitBetter.do_new_gh_remote-161"><a href="#GitBetter.do_new_gh_remote-161"><span class="linenos">161</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_gh_remote-162"><a href="#GitBetter.do_new_gh_remote-162"><span class="linenos">162</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-158"><a href="#GitBetter.do_new_gh_remote-158"><span class="linenos">158</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_new_gh_remote-159"><a href="#GitBetter.do_new_gh_remote-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_gh_remote-160"><a href="#GitBetter.do_new_gh_remote-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="GitBetter.do_new_gh_remote-161"><a href="#GitBetter.do_new_gh_remote-161"><span class="linenos">161</span></a>
+</span><span id="GitBetter.do_new_gh_remote-162"><a href="#GitBetter.do_new_gh_remote-162"><span class="linenos">162</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_gh_remote-163"><a href="#GitBetter.do_new_gh_remote-163"><span class="linenos">163</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a remote GitHub repository for this repo.</p>
 
 <p>GitHub CLI must be installed and configured for this to work.</p>
 </div>
@@ -1066,17 +1068,17 @@
         <span class="def">def</span>
         <span class="name">do_initcommit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_initcommit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_initcommit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-164"><a href="#GitBetter.do_initcommit-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_initcommit-165"><a href="#GitBetter.do_initcommit-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_initcommit-166"><a href="#GitBetter.do_initcommit-166"><span class="linenos">166</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-165"><a href="#GitBetter.do_initcommit-165"><span class="linenos">165</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_initcommit-166"><a href="#GitBetter.do_initcommit-166"><span class="linenos">166</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_initcommit-167"><a href="#GitBetter.do_initcommit-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with message "Initial Commit".</p>
 </div>
 
 
@@ -1088,42 +1090,42 @@
         <span class="def">def</span>
         <span class="name">do_undo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-168"><a href="#GitBetter.do_undo-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_undo-169"><a href="#GitBetter.do_undo-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_undo-170"><a href="#GitBetter.do_undo-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-169"><a href="#GitBetter.do_undo-169"><span class="linenos">169</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_undo-170"><a href="#GitBetter.do_undo-170"><span class="linenos">170</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_undo-171"><a href="#GitBetter.do_undo-171"><span class="linenos">171</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo all uncommitted changes.</p>
 </div>
 
 
                             </div>
                             <div id="GitBetter.do_add" class="classattr">
                                         <input id="GitBetter.do_add-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
-                    <div class="decorator">@with_parser(amend_files_parser, [files_postparser])</div>
+                    <div class="decorator">@with_parser(add_files_parser, [files_postparser])</div>
 
         <span class="def">def</span>
         <span class="name">do_add</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_add-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_add"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add-172"><a href="#GitBetter.do_add-172"><span class="linenos">172</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_add-173"><a href="#GitBetter.do_add-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_add-174"><a href="#GitBetter.do_add-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="GitBetter.do_add-175"><a href="#GitBetter.do_add-175"><span class="linenos">175</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_add-176"><a href="#GitBetter.do_add-176"><span class="linenos">176</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add-173"><a href="#GitBetter.do_add-173"><span class="linenos">173</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">add_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_add-174"><a href="#GitBetter.do_add-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_add-175"><a href="#GitBetter.do_add-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="GitBetter.do_add-176"><a href="#GitBetter.do_add-176"><span class="linenos">176</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_add-177"><a href="#GitBetter.do_add-177"><span class="linenos">177</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage a list of files.
 If no files are given, all files will be added.</p>
 </div>
 
@@ -1136,17 +1138,17 @@
         <span class="def">def</span>
         <span class="name">do_commit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commit-178"><a href="#GitBetter.do_commit-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-179"><a href="#GitBetter.do_commit-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commit-180"><a href="#GitBetter.do_commit-180"><span class="linenos">180</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commit-179"><a href="#GitBetter.do_commit-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_commit-180"><a href="#GitBetter.do_commit-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commit-181"><a href="#GitBetter.do_commit-181"><span class="linenos">181</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Commit staged files with provided <code>args</code> string.</p>
 </div>
 
 
@@ -1159,18 +1161,18 @@
         <span class="def">def</span>
         <span class="name">do_commitf</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commitf-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commitf"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-182"><a href="#GitBetter.do_commitf-182"><span class="linenos">182</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_commitf-183"><a href="#GitBetter.do_commitf-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitf-184"><a href="#GitBetter.do_commitf-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitf-185"><a href="#GitBetter.do_commitf-185"><span class="linenos">185</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-183"><a href="#GitBetter.do_commitf-183"><span class="linenos">183</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_commitf-184"><a href="#GitBetter.do_commitf-184"><span class="linenos">184</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitf-185"><a href="#GitBetter.do_commitf-185"><span class="linenos">185</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commitf-186"><a href="#GitBetter.do_commitf-186"><span class="linenos">186</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit a list of files.</p>
 </div>
 
 
@@ -1182,22 +1184,22 @@
         <span class="def">def</span>
         <span class="name">do_commitall</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commitall-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commitall"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitall-187"><a href="#GitBetter.do_commitall-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-188"><a href="#GitBetter.do_commitall-188"><span class="linenos">188</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitall-189"><a href="#GitBetter.do_commitall-189"><span class="linenos">189</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-190"><a href="#GitBetter.do_commitall-190"><span class="linenos">190</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter.do_commitall-191"><a href="#GitBetter.do_commitall-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-192"><a href="#GitBetter.do_commitall-192"><span class="linenos">192</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter.do_commitall-193"><a href="#GitBetter.do_commitall-193"><span class="linenos">193</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="GitBetter.do_commitall-194"><a href="#GitBetter.do_commitall-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitall-188"><a href="#GitBetter.do_commitall-188"><span class="linenos">188</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-189"><a href="#GitBetter.do_commitall-189"><span class="linenos">189</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commitall-190"><a href="#GitBetter.do_commitall-190"><span class="linenos">190</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-191"><a href="#GitBetter.do_commitall-191"><span class="linenos">191</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter.do_commitall-192"><a href="#GitBetter.do_commitall-192"><span class="linenos">192</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-193"><a href="#GitBetter.do_commitall-193"><span class="linenos">193</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter.do_commitall-194"><a href="#GitBetter.do_commitall-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="GitBetter.do_commitall-195"><a href="#GitBetter.do_commitall-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with this message.</p>
 </div>
 
 
@@ -1209,17 +1211,17 @@
         <span class="def">def</span>
         <span class="name">do_switch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_switch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_switch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_switch-196"><a href="#GitBetter.do_switch-196"><span class="linenos">196</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_switch-197"><a href="#GitBetter.do_switch-197"><span class="linenos">197</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_switch-198"><a href="#GitBetter.do_switch-198"><span class="linenos">198</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_switch-197"><a href="#GitBetter.do_switch-197"><span class="linenos">197</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_switch-198"><a href="#GitBetter.do_switch-198"><span class="linenos">198</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_switch-199"><a href="#GitBetter.do_switch-199"><span class="linenos">199</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Switch to this branch.</p>
 </div>
 
 
@@ -1231,18 +1233,18 @@
         <span class="def">def</span>
         <span class="name">do_add_url</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_add_url-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_add_url"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add_url-200"><a href="#GitBetter.do_add_url-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_add_url-201"><a href="#GitBetter.do_add_url-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_add_url-202"><a href="#GitBetter.do_add_url-202"><span class="linenos">202</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="GitBetter.do_add_url-203"><a href="#GitBetter.do_add_url-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add_url-201"><a href="#GitBetter.do_add_url-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_add_url-202"><a href="#GitBetter.do_add_url-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_add_url-203"><a href="#GitBetter.do_add_url-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="GitBetter.do_add_url-204"><a href="#GitBetter.do_add_url-204"><span class="linenos">204</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add remote origin url for repo and push repo.</p>
 </div>
 
 
@@ -1254,17 +1256,17 @@
         <span class="def">def</span>
         <span class="name">do_push_new</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push_new-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push_new"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-205"><a href="#GitBetter.do_push_new-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push_new-206"><a href="#GitBetter.do_push_new-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push_new-207"><a href="#GitBetter.do_push_new-207"><span class="linenos">207</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-206"><a href="#GitBetter.do_push_new-206"><span class="linenos">206</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push_new-207"><a href="#GitBetter.do_push_new-207"><span class="linenos">207</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push_new-208"><a href="#GitBetter.do_push_new-208"><span class="linenos">208</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push this new branch to origin with -u flag.</p>
 </div>
 
 
@@ -1276,19 +1278,19 @@
         <span class="def">def</span>
         <span class="name">do_push</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push-209"><a href="#GitBetter.do_push-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push-210"><a href="#GitBetter.do_push-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="GitBetter.do_push-211"><a href="#GitBetter.do_push-211"><span class="linenos">211</span></a>
-</span><span id="GitBetter.do_push-212"><a href="#GitBetter.do_push-212"><span class="linenos">212</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push-213"><a href="#GitBetter.do_push-213"><span class="linenos">213</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push-210"><a href="#GitBetter.do_push-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push-211"><a href="#GitBetter.do_push-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="GitBetter.do_push-212"><a href="#GitBetter.do_push-212"><span class="linenos">212</span></a>
+</span><span id="GitBetter.do_push-213"><a href="#GitBetter.do_push-213"><span class="linenos">213</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push-214"><a href="#GitBetter.do_push-214"><span class="linenos">214</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git push</code>.</p>
 
 <p><code>args</code> can be any additional args that <code>git push</code> accepts.</p>
 </div>
@@ -1302,19 +1304,19 @@
         <span class="def">def</span>
         <span class="name">do_pull</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull-215"><a href="#GitBetter.do_pull-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull-216"><a href="#GitBetter.do_pull-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="GitBetter.do_pull-217"><a href="#GitBetter.do_pull-217"><span class="linenos">217</span></a>
-</span><span id="GitBetter.do_pull-218"><a href="#GitBetter.do_pull-218"><span class="linenos">218</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull-219"><a href="#GitBetter.do_pull-219"><span class="linenos">219</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull-216"><a href="#GitBetter.do_pull-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull-217"><a href="#GitBetter.do_pull-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="GitBetter.do_pull-218"><a href="#GitBetter.do_pull-218"><span class="linenos">218</span></a>
+</span><span id="GitBetter.do_pull-219"><a href="#GitBetter.do_pull-219"><span class="linenos">219</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull-220"><a href="#GitBetter.do_pull-220"><span class="linenos">220</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git pull</code>.</p>
 
 <p><code>args</code> can be any additional args that <code>git pull</code> accepts.</p>
 </div>
@@ -1328,17 +1330,17 @@
         <span class="def">def</span>
         <span class="name">do_branches</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_branches-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_branches"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_branches-221"><a href="#GitBetter.do_branches-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_branches-222"><a href="#GitBetter.do_branches-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_branches-223"><a href="#GitBetter.do_branches-223"><span class="linenos">223</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_branches-222"><a href="#GitBetter.do_branches-222"><span class="linenos">222</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_branches-223"><a href="#GitBetter.do_branches-223"><span class="linenos">223</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_branches-224"><a href="#GitBetter.do_branches-224"><span class="linenos">224</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Show local and remote branches.</p>
 </div>
 
 
@@ -1350,17 +1352,17 @@
         <span class="def">def</span>
         <span class="name">do_loggy</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_loggy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_loggy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-225"><a href="#GitBetter.do_loggy-225"><span class="linenos">225</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_loggy-226"><a href="#GitBetter.do_loggy-226"><span class="linenos">226</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_loggy-227"><a href="#GitBetter.do_loggy-227"><span class="linenos">227</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-226"><a href="#GitBetter.do_loggy-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_loggy-227"><a href="#GitBetter.do_loggy-227"><span class="linenos">227</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_loggy-228"><a href="#GitBetter.do_loggy-228"><span class="linenos">228</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git --oneline --name-only --abbrev-commit --graph</code>.</p>
 </div>
 
 
@@ -1372,17 +1374,17 @@
         <span class="def">def</span>
         <span class="name">do_status</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_status-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_status"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_status-229"><a href="#GitBetter.do_status-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_status-230"><a href="#GitBetter.do_status-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_status-231"><a href="#GitBetter.do_status-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_status-230"><a href="#GitBetter.do_status-230"><span class="linenos">230</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_status-231"><a href="#GitBetter.do_status-231"><span class="linenos">231</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_status-232"><a href="#GitBetter.do_status-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git status</code>.</p>
 </div>
 
 
@@ -1394,17 +1396,17 @@
         <span class="def">def</span>
         <span class="name">do_merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-233"><a href="#GitBetter.do_merge-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_merge-234"><a href="#GitBetter.do_merge-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_merge-235"><a href="#GitBetter.do_merge-235"><span class="linenos">235</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-234"><a href="#GitBetter.do_merge-234"><span class="linenos">234</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_merge-235"><a href="#GitBetter.do_merge-235"><span class="linenos">235</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_merge-236"><a href="#GitBetter.do_merge-236"><span class="linenos">236</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge supplied <code>branch_name</code> with the currently active branch.</p>
 </div>
 
 
@@ -1416,41 +1418,41 @@
         <span class="def">def</span>
         <span class="name">do_tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-237"><a href="#GitBetter.do_tag-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_tag-238"><a href="#GitBetter.do_tag-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_tag-239"><a href="#GitBetter.do_tag-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-238"><a href="#GitBetter.do_tag-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_tag-239"><a href="#GitBetter.do_tag-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_tag-240"><a href="#GitBetter.do_tag-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Tag current commit with <code>tag_id</code>.</p>
 </div>
 
 
                             </div>
                             <div id="GitBetter.do_amend" class="classattr">
                                         <input id="GitBetter.do_amend-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
-                    <div class="decorator">@with_parser(amend_files_parser, [files_postparser])</div>
+                    <div class="decorator">@with_parser(add_files_parser, [files_postparser])</div>
 
         <span class="def">def</span>
         <span class="name">do_amend</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_amend-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_amend"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-241"><a href="#GitBetter.do_amend-241"><span class="linenos">241</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_amend-242"><a href="#GitBetter.do_amend-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_amend-243"><a href="#GitBetter.do_amend-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_amend-244"><a href="#GitBetter.do_amend-244"><span class="linenos">244</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-242"><a href="#GitBetter.do_amend-242"><span class="linenos">242</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">add_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_amend-243"><a href="#GitBetter.do_amend-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_amend-244"><a href="#GitBetter.do_amend-244"><span class="linenos">244</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_amend-245"><a href="#GitBetter.do_amend-245"><span class="linenos">245</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage files and add to previous commit.</p>
 </div>
 
 
@@ -1463,18 +1465,18 @@
         <span class="def">def</span>
         <span class="name">do_delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-246"><a href="#GitBetter.do_delete_branch-246"><span class="linenos">246</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_delete_branch-247"><a href="#GitBetter.do_delete_branch-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_branch-248"><a href="#GitBetter.do_delete_branch-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_branch-249"><a href="#GitBetter.do_delete_branch-249"><span class="linenos">249</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-247"><a href="#GitBetter.do_delete_branch-247"><span class="linenos">247</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_delete_branch-248"><a href="#GitBetter.do_delete_branch-248"><span class="linenos">248</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_branch-249"><a href="#GitBetter.do_delete_branch-249"><span class="linenos">249</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_branch-250"><a href="#GitBetter.do_delete_branch-250"><span class="linenos">250</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete branch.</p>
 </div>
 
 
@@ -1486,17 +1488,17 @@
         <span class="def">def</span>
         <span class="name">do_pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-251"><a href="#GitBetter.do_pull_branch-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull_branch-252"><a href="#GitBetter.do_pull_branch-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull_branch-253"><a href="#GitBetter.do_pull_branch-253"><span class="linenos">253</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-252"><a href="#GitBetter.do_pull_branch-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull_branch-253"><a href="#GitBetter.do_pull_branch-253"><span class="linenos">253</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull_branch-254"><a href="#GitBetter.do_pull_branch-254"><span class="linenos">254</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull this branch from the origin.</p>
 </div>
 
 
@@ -1508,20 +1510,20 @@
         <span class="def">def</span>
         <span class="name">do_ignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_ignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_ignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-255"><a href="#GitBetter.do_ignore-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_ignore-256"><a href="#GitBetter.do_ignore-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_ignore-257"><a href="#GitBetter.do_ignore-257"><span class="linenos">257</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter.do_ignore-258"><a href="#GitBetter.do_ignore-258"><span class="linenos">258</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-256"><a href="#GitBetter.do_ignore-256"><span class="linenos">256</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_ignore-257"><a href="#GitBetter.do_ignore-257"><span class="linenos">257</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_ignore-258"><a href="#GitBetter.do_ignore-258"><span class="linenos">258</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-261"><a href="#GitBetter.do_ignore-261"><span class="linenos">261</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add the list of patterns to <code>.gitignore</code>.</p>
 </div>
 
 
@@ -1533,21 +1535,21 @@
         <span class="def">def</span>
         <span class="name">do_make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-262"><a href="#GitBetter.do_make_private-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_private-263"><a href="#GitBetter.do_make_private-263"><span class="linenos">263</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter.do_make_private-264"><a href="#GitBetter.do_make_private-264"><span class="linenos">264</span></a>
-</span><span id="GitBetter.do_make_private-265"><a href="#GitBetter.do_make_private-265"><span class="linenos">265</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a>
-</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-263"><a href="#GitBetter.do_make_private-263"><span class="linenos">263</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_private-264"><a href="#GitBetter.do_make_private-264"><span class="linenos">264</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter.do_make_private-265"><a href="#GitBetter.do_make_private-265"><span class="linenos">265</span></a>
+</span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a>
+</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_private-269"><a href="#GitBetter.do_make_private-269"><span class="linenos">269</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo private.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1563,21 +1565,21 @@
         <span class="def">def</span>
         <span class="name">do_make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-270"><a href="#GitBetter.do_make_public-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_public-271"><a href="#GitBetter.do_make_public-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter.do_make_public-272"><a href="#GitBetter.do_make_public-272"><span class="linenos">272</span></a>
-</span><span id="GitBetter.do_make_public-273"><a href="#GitBetter.do_make_public-273"><span class="linenos">273</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a>
-</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-271"><a href="#GitBetter.do_make_public-271"><span class="linenos">271</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_public-272"><a href="#GitBetter.do_make_public-272"><span class="linenos">272</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter.do_make_public-273"><a href="#GitBetter.do_make_public-273"><span class="linenos">273</span></a>
+</span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a>
+</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_public-277"><a href="#GitBetter.do_make_public-277"><span class="linenos">277</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo public.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1593,23 +1595,23 @@
         <span class="def">def</span>
         <span class="name">do_delete_gh_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_gh_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_gh_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-278"><a href="#GitBetter.do_delete_gh_repo-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_gh_repo-279"><a href="#GitBetter.do_delete_gh_repo-279"><span class="linenos">279</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter.do_delete_gh_repo-280"><a href="#GitBetter.do_delete_gh_repo-280"><span class="linenos">280</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-281"><a href="#GitBetter.do_delete_gh_repo-281"><span class="linenos">281</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter.do_delete_gh_repo-284"><a href="#GitBetter.do_delete_gh_repo-284"><span class="linenos">284</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-279"><a href="#GitBetter.do_delete_gh_repo-279"><span class="linenos">279</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_gh_repo-280"><a href="#GitBetter.do_delete_gh_repo-280"><span class="linenos">280</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter.do_delete_gh_repo-281"><a href="#GitBetter.do_delete_gh_repo-281"><span class="linenos">281</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-284"><a href="#GitBetter.do_delete_gh_repo-284"><span class="linenos">284</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_gh_repo-287"><a href="#GitBetter.do_delete_gh_repo-287"><span class="linenos">287</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete this repo from GitHub.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1657,16 +1659,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-289"><a href="#main-289"><span class="linenos">289</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-290"><a href="#main-290"><span class="linenos">290</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-290"><a href="#main-290"><span class="linenos">290</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-291"><a href="#main-291"><span class="linenos">291</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 
 
   ⁰
 ____ gitbetter [Unknown INPUT type]
 ***** API Documentation *****
     * new_remote_parser
     * commit_files_parser
-    * amend_files_parser
+    * add_files_parser
     * delete_branch_parser
     * recurse_files
     * files_postparser
     * GitBetter
           o default
           o do_help
           o do_toggle_unrecognized_command_behavior
@@ -89,387 +89,76 @@
 _37        but if you have multiple files in different subfolders with the same
 name that have changes they
 _38        will all be staged and committed.""",
 _39    )
 _40    return parser
 _41
 _42
-_43def amend_files_parser() -> ArgShellParser:
+_43def add_files_parser() -> ArgShellParser:
 _44    parser = ArgShellParser()
 _45    parser.add_argument(
-_46        "-f",
-_47        "--files",
-_48        type=str,
-_49        nargs="*",
-_50        help=""" List of files to stage and commit. """,
-_51    )
-_52    parser.add_argument(
-_53        "-r",
-_54        "--recursive",
-_55        action="store_true",
-_56        help=""" If a file name is not found in the current working
+_46        "files",
+_47        type=str,
+_48        nargs="*",
+_49        default=None,
+_50        help=""" List of files to stage and commit.
+_51        If not given, all files will be added.""",
+_52    )
+_53    parser.add_argument(
+_54        "-r",
+_55        "--recursive",
+_56        action="store_true",
+_57        help=""" If a file name is not found in the current working
 directory,
-_57        search for it in subfolders. This avoids having to type paths to
+_58        search for it in subfolders. This avoids having to type paths to
 files in subfolders,
-_58        but if you have multiple files in different subfolders with the same
+_59        but if you have multiple files in different subfolders with the same
 name that have changes they
-_59        will all be staged and committed.""",
-_60    )
-_61    return parser
-_62
+_60        will all be staged and committed.""",
+_61    )
+_62    return parser
 _63
-_64def delete_branch_parser() -> ArgShellParser:
-_65    parser = ArgShellParser()
-_66    parser.add_argument(
-_67        "branch", type=str, help=""" The name of the branch to delete. """
-_68    )
-_69    parser.add_argument(
-_70        "-r",
-_71        "--remote",
-_72        action="store_true",
-_73        help=""" Delete the remote and remote-tracking branches along with
+_64
+_65def delete_branch_parser() -> ArgShellParser:
+_66    parser = ArgShellParser()
+_67    parser.add_argument(
+_68        "branch", type=str, help=""" The name of the branch to delete. """
+_69    )
+_70    parser.add_argument(
+_71        "-r",
+_72        "--remote",
+_73        action="store_true",
+_74        help=""" Delete the remote and remote-tracking branches along with
 the local branch.
-_74        By default only the local branch is deleted.""",
-_75    )
-_76    return parser
-_77
+_75        By default only the local branch is deleted.""",
+_76    )
+_77    return parser
 _78
-_79def recurse_files(filenames: list[str]) -> list[str]:
-_80    files = []
-_81    for filename in filenames:
-_82        if not Pathier(filename).exists():
-_83            results = list(Pathier.cwd().rglob(f"{filename}"))
-_84            if not results:
-_85                print(f"WARNING: Could not find any files with name
+_79
+_80def recurse_files(filenames: list[str]) -> list[str]:
+_81    files = []
+_82    for filename in filenames:
+_83        if not Pathier(filename).exists():
+_84            results = list(Pathier.cwd().rglob(f"{filename}"))
+_85            if not results:
+_86                print(f"WARNING: Could not find any files with name
 {filename}")
-_86            else:
-_87                files.extend([str(result) for result in results])
-_88        else:
-_89            files.append(filename)
-_90    return files
-_91
+_87            else:
+_88                files.extend([str(result) for result in results])
+_89        else:
+_90            files.append(filename)
+_91    return files
 _92
-_93def files_postparser(args: Namespace) -> Namespace:
-_94    if args.recursive:
-_95        args.files = recurse_files(args.files)
-_96    return args
-_97
+_93
+_94def files_postparser(args: Namespace) -> Namespace:
+_95    if args.recursive:
+_96        args.files = recurse_files(args.files)
+_97    return args
 _98
-_99class GitBetter(ArgShell):
-100    """GitBetter Shell."""
-101
-102    intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
-103    prompt = f"gitbetter::{Pathier.cwd()}>"
-104    execute_in_terminal_if_unrecognized = True
-105    git = Git()
-106
-107    def default(self, line: str):
-108        if self.execute_in_terminal_if_unrecognized:
-109            os.system(line)
-110        else:
-111            super().default(line)
-112
-113    def do_help(self, arg: str):
-114        """List available commands with "help" or detailed help with "help
-cmd"."""
-115        super().do_help(arg)
-116        if not arg:
-117            print(self.unrecognized_command_behavior_status)
-118            if self.execute_in_terminal_if_unrecognized:
-119                print(
-120                    "^Essentially makes this shell function as a super-shell
-of whatever shell you launched gitbetter from.^"
-121                )
-122        print()
-123
-124    @property
-125    def unrecognized_command_behavior_status(self):
-126        return f"Unrecognized command behavior: {'Execute in shell with
-os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown
-syntax error'}"
-127
-128    def do_toggle_unrecognized_command_behavior(self, arg: str):
-129        """Toggle whether the shell will attempt to execute unrecognized
-commands as system commands in the terminal.
-130        When on (the default), `GitBetter` will treat unrecognized commands
-as if you added the `sys` command in front of the input, i.e. `os.system
-(your_input)`.
-131        When off, an `unknown syntax` message will be printed and no
-commands will be executed."""
-132        self.execute_in_terminal_if_unrecognized = (
-133            not self.execute_in_terminal_if_unrecognized
-134        )
-135        print(self.unrecognized_command_behavior_status)
-136
-137    def do_cd(self, path: str):
-138        """Change current working directory to `path`."""
-139        os.chdir(path)
-140        self.prompt = f"gitbetter::{Pathier.cwd()}>"
-141
-142    def do_git(self, arg: str):
-143        """Directly execute `git {arg}`.
-144
-145        i.e. You can still do everything directly invoking git can do."""
-146        self.git.execute(arg)
-147
-148    def do_new_repo(self, _: str):
-149        """Create a new git repo in this directory."""
-150        self.git.new_repo()
-151
-152    def do_new_branch(self, name: str):
-153        """Create and switch to a new branch named after the supplied
-arg."""
-154        self.git.create_new_branch(name)
-155
-156    @with_parser(new_remote_parser)
-157    def do_new_gh_remote(self, args: Namespace):
-158        """Create a remote GitHub repository for this repo.
-159
-160        GitHub CLI must be installed and configured for this to work."""
-161        self.git.create_remote_from_cwd(args.public)
-162
-163    def do_initcommit(self, _: str):
-164        """Stage and commit all files with message "Initial Commit"."""
-165        self.git.initcommit()
-166
-167    def do_undo(self, _: str):
-168        """Undo all uncommitted changes."""
-169        self.git.undo()
-170
-171    @with_parser(amend_files_parser, [files_postparser])
-172    def do_add(self, args: Namespace):
-173        """Stage a list of files.
-174        If no files are given, all files will be added."""
-175        self.git.add(None if not args.files else args.files)
-176
-177    def do_commit(self, args: str):
-178        """Commit staged files with provided `args` string."""
-179        self.git.commit(args)
-180
-181    @with_parser(commit_files_parser, [files_postparser])
-182    def do_commitf(self, args: Namespace):
-183        """Stage and commit a list of files."""
-184        self.git.commit_files(args.files, args.message)
-185
-186    def do_commitall(self, message: str):
-187        """Stage and commit all files with this message."""
-188        if not message.startswith('"'):
-189            message = '"' + message
-190        if not message.endswith('"'):
-191            message += '"'
-192        self.git.add()
-193        self.git.commit(f"-m {message}")
-194
-195    def do_switch(self, branch_name: str):
-196        """Switch to this branch."""
-197        self.git.switch_branch(branch_name)
-198
-199    def do_add_url(self, url: str):
-200        """Add remote origin url for repo and push repo."""
-201        self.git.add_remote_url(url)
-202        self.git.push("-u origin main")
-203
-204    def do_push_new(self, branch_name: str):
-205        """Push this new branch to origin with -u flag."""
-206        self.git.push_new_branch(branch_name)
-207
-208    def do_push(self, args: str):
-209        """Execute `git push`.
-210
-211        `args` can be any additional args that `git push` accepts."""
-212        self.git.push(args)
-213
-214    def do_pull(self, args: str):
-215        """Execute `git pull`.
-216
-217        `args` can be any additional args that `git pull` accepts."""
-218        self.git.pull(args)
-219
-220    def do_branches(self, _: str):
-221        """Show local and remote branches."""
-222        self.git.list_branches()
-223
-224    def do_loggy(self, _: str):
-225        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-226        self.git.loggy()
-227
-228    def do_status(self, _: str):
-229        """Execute `git status`."""
-230        self.git.status()
-231
-232    def do_merge(self, branch_name: str):
-233        """Merge supplied `branch_name` with the currently active branch."""
-234        self.git.merge(branch_name)
-235
-236    def do_tag(self, tag_id: str):
-237        """Tag current commit with `tag_id`."""
-238        self.git.tag(tag_id)
-239
-240    @with_parser(amend_files_parser, [files_postparser])
-241    def do_amend(self, args: Namespace):
-242        """Stage files and add to previous commit."""
-243        self.git.amend(args.files)
-244
-245    @with_parser(delete_branch_parser)
-246    def do_delete_branch(self, args: Namespace):
-247        """Delete branch."""
-248        self.git.delete_branch(args.branch, not args.remote)
-249
-250    def do_pull_branch(self, branch: str):
-251        """Pull this branch from the origin."""
-252        self.git.pull_branch(branch)
-253
-254    def do_ignore(self, patterns: str):
-255        """Add the list of patterns to `.gitignore`."""
-256        patterns = "\n".join(patterns.split())
-257        path = Pathier(".gitignore")
-258        path.append("\n")
-259        path.append(patterns, False)
-260
-261    def do_make_private(self, owner: str):
-262        """Make the GitHub remote for this repo private.
-263
-264        Expects an argument for the repo owner, i.e. the `OWNER` in
-`github.com/{OWNER}/{repo-name}`
-265
-266        This repo must exist and GitHub CLI must be installed and
-configured."""
-267        self.git.make_private(owner, Pathier.cwd().stem)
-268
-269    def do_make_public(self, owner: str):
-270        """Make the GitHub remote for this repo public.
-271
-272        Expects an argument for the repo owner, i.e. the `OWNER` in
-`github.com/{OWNER}/{repo-name}`
-273
-274        This repo must exist and GitHub CLI must be installed and
-configured."""
-275        self.git.make_public(owner, Pathier.cwd().stem)
-276
-277    def do_delete_gh_repo(self, owner: str):
-278        """Delete this repo from GitHub.
-279
-280        Expects an argument for the repo owner, i.e. the `OWNER` in
-`github.com/{OWNER}/{repo-name}`
-281
-282        GitHub CLI must be installed and configured.
-283
-284        May require you to reauthorize and rerun command."""
-285        self.git.delete_remote(owner, Pathier.cwd().stem)
-286
-287
-288def main():
-289    GitBetter().cmdloop()
-290
-291
-292if __name__ == "__main__":
-293    main()
-  ⁰
-def new_remote_parser() -> argshell.argshell.ArgShellParser: View Source
-10def new_remote_parser() -> ArgShellParser:
-11    parser = ArgShellParser()
-12    parser.add_argument(
-13        "--public",
-14        action="store_true",
-15        help=""" Set the new remote visibility as public. Defaults to
-private. """,
-16    )
-17    return parser
-  ⁰
-def commit_files_parser() -> argshell.argshell.ArgShellParser: View Source
-20def commit_files_parser() -> ArgShellParser:
-21    parser = ArgShellParser()
-22    parser.add_argument(
-23        "files", type=str, nargs="*", help=""" List of files to stage and
-commit. """
-24    )
-25    parser.add_argument(
-26        "-m",
-27        "--message",
-28        type=str,
-29        required=True,
-30        help=""" The commit message to use. """,
-31    )
-32    parser.add_argument(
-33        "-r",
-34        "--recursive",
-35        action="store_true",
-36        help=""" If a file name is not found in the current working
-directory,
-37        search for it in subfolders. This avoids having to type paths to
-files in subfolders,
-38        but if you have multiple files in different subfolders with the same
-name that have changes they
-39        will all be staged and committed.""",
-40    )
-41    return parser
-  ⁰
-def amend_files_parser() -> argshell.argshell.ArgShellParser: View Source
-44def amend_files_parser() -> ArgShellParser:
-45    parser = ArgShellParser()
-46    parser.add_argument(
-47        "-f",
-48        "--files",
-49        type=str,
-50        nargs="*",
-51        help=""" List of files to stage and commit. """,
-52    )
-53    parser.add_argument(
-54        "-r",
-55        "--recursive",
-56        action="store_true",
-57        help=""" If a file name is not found in the current working
-directory,
-58        search for it in subfolders. This avoids having to type paths to
-files in subfolders,
-59        but if you have multiple files in different subfolders with the same
-name that have changes they
-60        will all be staged and committed.""",
-61    )
-62    return parser
-  ⁰
-def delete_branch_parser() -> argshell.argshell.ArgShellParser: View Source
-65def delete_branch_parser() -> ArgShellParser:
-66    parser = ArgShellParser()
-67    parser.add_argument(
-68        "branch", type=str, help=""" The name of the branch to delete. """
-69    )
-70    parser.add_argument(
-71        "-r",
-72        "--remote",
-73        action="store_true",
-74        help=""" Delete the remote and remote-tracking branches along with
-the local branch.
-75        By default only the local branch is deleted.""",
-76    )
-77    return parser
-  ⁰
-def recurse_files(filenames: list[str]) -> list[str]: View Source
-80def recurse_files(filenames: list[str]) -> list[str]:
-81    files = []
-82    for filename in filenames:
-83        if not Pathier(filename).exists():
-84            results = list(Pathier.cwd().rglob(f"{filename}"))
-85            if not results:
-86                print(f"WARNING: Could not find any files with name
-{filename}")
-87            else:
-88                files.extend([str(result) for result in results])
-89        else:
-90            files.append(filename)
-91    return files
-  ⁰
-def files_postparser(args: argshell.argshell.Namespace) -
-> argshell.argshell.Namespace: View Source
-94def files_postparser(args: Namespace) -> Namespace:
-95    if args.recursive:
-96        args.files = recurse_files(args.files)
-97    return args
-  ⁰
-class GitBetter(argshell.argshell.ArgShell): View Source
+_99
 100class GitBetter(ArgShell):
 101    """GitBetter Shell."""
 102
 103    intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
 104    prompt = f"gitbetter::{Pathier.cwd()}>"
 105    execute_in_terminal_if_unrecognized = True
 106    git = Git()
@@ -543,15 +232,15 @@
 165        """Stage and commit all files with message "Initial Commit"."""
 166        self.git.initcommit()
 167
 168    def do_undo(self, _: str):
 169        """Undo all uncommitted changes."""
 170        self.git.undo()
 171
-172    @with_parser(amend_files_parser, [files_postparser])
+172    @with_parser(add_files_parser, [files_postparser])
 173    def do_add(self, args: Namespace):
 174        """Stage a list of files.
 175        If no files are given, all files will be added."""
 176        self.git.add(None if not args.files else args.files)
 177
 178    def do_commit(self, args: str):
 179        """Commit staged files with provided `args` string."""
@@ -612,15 +301,15 @@
 234        """Merge supplied `branch_name` with the currently active branch."""
 235        self.git.merge(branch_name)
 236
 237    def do_tag(self, tag_id: str):
 238        """Tag current commit with `tag_id`."""
 239        self.git.tag(tag_id)
 240
-241    @with_parser(amend_files_parser, [files_postparser])
+241    @with_parser(add_files_parser, [files_postparser])
 242    def do_amend(self, args: Namespace):
 243        """Stage files and add to previous commit."""
 244        self.git.amend(args.files)
 245
 246    @with_parser(delete_branch_parser)
 247    def do_delete_branch(self, args: Namespace):
 248        """Delete branch."""
@@ -663,288 +352,601 @@
 281        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
 282
 283        GitHub CLI must be installed and configured.
 284
 285        May require you to reauthorize and rerun command."""
 286        self.git.delete_remote(owner, Pathier.cwd().stem)
+287
+288
+289def main():
+290    GitBetter().cmdloop()
+291
+292
+293if __name__ == "__main__":
+294    main()
+  ⁰
+def new_remote_parser() -> argshell.argshell.ArgShellParser: View Source
+10def new_remote_parser() -> ArgShellParser:
+11    parser = ArgShellParser()
+12    parser.add_argument(
+13        "--public",
+14        action="store_true",
+15        help=""" Set the new remote visibility as public. Defaults to
+private. """,
+16    )
+17    return parser
+  ⁰
+def commit_files_parser() -> argshell.argshell.ArgShellParser: View Source
+20def commit_files_parser() -> ArgShellParser:
+21    parser = ArgShellParser()
+22    parser.add_argument(
+23        "files", type=str, nargs="*", help=""" List of files to stage and
+commit. """
+24    )
+25    parser.add_argument(
+26        "-m",
+27        "--message",
+28        type=str,
+29        required=True,
+30        help=""" The commit message to use. """,
+31    )
+32    parser.add_argument(
+33        "-r",
+34        "--recursive",
+35        action="store_true",
+36        help=""" If a file name is not found in the current working
+directory,
+37        search for it in subfolders. This avoids having to type paths to
+files in subfolders,
+38        but if you have multiple files in different subfolders with the same
+name that have changes they
+39        will all be staged and committed.""",
+40    )
+41    return parser
+  ⁰
+def add_files_parser() -> argshell.argshell.ArgShellParser: View Source
+44def add_files_parser() -> ArgShellParser:
+45    parser = ArgShellParser()
+46    parser.add_argument(
+47        "files",
+48        type=str,
+49        nargs="*",
+50        default=None,
+51        help=""" List of files to stage and commit.
+52        If not given, all files will be added.""",
+53    )
+54    parser.add_argument(
+55        "-r",
+56        "--recursive",
+57        action="store_true",
+58        help=""" If a file name is not found in the current working
+directory,
+59        search for it in subfolders. This avoids having to type paths to
+files in subfolders,
+60        but if you have multiple files in different subfolders with the same
+name that have changes they
+61        will all be staged and committed.""",
+62    )
+63    return parser
+  ⁰
+def delete_branch_parser() -> argshell.argshell.ArgShellParser: View Source
+66def delete_branch_parser() -> ArgShellParser:
+67    parser = ArgShellParser()
+68    parser.add_argument(
+69        "branch", type=str, help=""" The name of the branch to delete. """
+70    )
+71    parser.add_argument(
+72        "-r",
+73        "--remote",
+74        action="store_true",
+75        help=""" Delete the remote and remote-tracking branches along with
+the local branch.
+76        By default only the local branch is deleted.""",
+77    )
+78    return parser
+  ⁰
+def recurse_files(filenames: list[str]) -> list[str]: View Source
+81def recurse_files(filenames: list[str]) -> list[str]:
+82    files = []
+83    for filename in filenames:
+84        if not Pathier(filename).exists():
+85            results = list(Pathier.cwd().rglob(f"{filename}"))
+86            if not results:
+87                print(f"WARNING: Could not find any files with name
+{filename}")
+88            else:
+89                files.extend([str(result) for result in results])
+90        else:
+91            files.append(filename)
+92    return files
+  ⁰
+def files_postparser(args: argshell.argshell.Namespace) -
+> argshell.argshell.Namespace: View Source
+95def files_postparser(args: Namespace) -> Namespace:
+96    if args.recursive:
+97        args.files = recurse_files(args.files)
+98    return args
+  ⁰
+class GitBetter(argshell.argshell.ArgShell): View Source
+101class GitBetter(ArgShell):
+102    """GitBetter Shell."""
+103
+104    intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
+105    prompt = f"gitbetter::{Pathier.cwd()}>"
+106    execute_in_terminal_if_unrecognized = True
+107    git = Git()
+108
+109    def default(self, line: str):
+110        if self.execute_in_terminal_if_unrecognized:
+111            os.system(line)
+112        else:
+113            super().default(line)
+114
+115    def do_help(self, arg: str):
+116        """List available commands with "help" or detailed help with "help
+cmd"."""
+117        super().do_help(arg)
+118        if not arg:
+119            print(self.unrecognized_command_behavior_status)
+120            if self.execute_in_terminal_if_unrecognized:
+121                print(
+122                    "^Essentially makes this shell function as a super-shell
+of whatever shell you launched gitbetter from.^"
+123                )
+124        print()
+125
+126    @property
+127    def unrecognized_command_behavior_status(self):
+128        return f"Unrecognized command behavior: {'Execute in shell with
+os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown
+syntax error'}"
+129
+130    def do_toggle_unrecognized_command_behavior(self, arg: str):
+131        """Toggle whether the shell will attempt to execute unrecognized
+commands as system commands in the terminal.
+132        When on (the default), `GitBetter` will treat unrecognized commands
+as if you added the `sys` command in front of the input, i.e. `os.system
+(your_input)`.
+133        When off, an `unknown syntax` message will be printed and no
+commands will be executed."""
+134        self.execute_in_terminal_if_unrecognized = (
+135            not self.execute_in_terminal_if_unrecognized
+136        )
+137        print(self.unrecognized_command_behavior_status)
+138
+139    def do_cd(self, path: str):
+140        """Change current working directory to `path`."""
+141        os.chdir(path)
+142        self.prompt = f"gitbetter::{Pathier.cwd()}>"
+143
+144    def do_git(self, arg: str):
+145        """Directly execute `git {arg}`.
+146
+147        i.e. You can still do everything directly invoking git can do."""
+148        self.git.execute(arg)
+149
+150    def do_new_repo(self, _: str):
+151        """Create a new git repo in this directory."""
+152        self.git.new_repo()
+153
+154    def do_new_branch(self, name: str):
+155        """Create and switch to a new branch named after the supplied
+arg."""
+156        self.git.create_new_branch(name)
+157
+158    @with_parser(new_remote_parser)
+159    def do_new_gh_remote(self, args: Namespace):
+160        """Create a remote GitHub repository for this repo.
+161
+162        GitHub CLI must be installed and configured for this to work."""
+163        self.git.create_remote_from_cwd(args.public)
+164
+165    def do_initcommit(self, _: str):
+166        """Stage and commit all files with message "Initial Commit"."""
+167        self.git.initcommit()
+168
+169    def do_undo(self, _: str):
+170        """Undo all uncommitted changes."""
+171        self.git.undo()
+172
+173    @with_parser(add_files_parser, [files_postparser])
+174    def do_add(self, args: Namespace):
+175        """Stage a list of files.
+176        If no files are given, all files will be added."""
+177        self.git.add(None if not args.files else args.files)
+178
+179    def do_commit(self, args: str):
+180        """Commit staged files with provided `args` string."""
+181        self.git.commit(args)
+182
+183    @with_parser(commit_files_parser, [files_postparser])
+184    def do_commitf(self, args: Namespace):
+185        """Stage and commit a list of files."""
+186        self.git.commit_files(args.files, args.message)
+187
+188    def do_commitall(self, message: str):
+189        """Stage and commit all files with this message."""
+190        if not message.startswith('"'):
+191            message = '"' + message
+192        if not message.endswith('"'):
+193            message += '"'
+194        self.git.add()
+195        self.git.commit(f"-m {message}")
+196
+197    def do_switch(self, branch_name: str):
+198        """Switch to this branch."""
+199        self.git.switch_branch(branch_name)
+200
+201    def do_add_url(self, url: str):
+202        """Add remote origin url for repo and push repo."""
+203        self.git.add_remote_url(url)
+204        self.git.push("-u origin main")
+205
+206    def do_push_new(self, branch_name: str):
+207        """Push this new branch to origin with -u flag."""
+208        self.git.push_new_branch(branch_name)
+209
+210    def do_push(self, args: str):
+211        """Execute `git push`.
+212
+213        `args` can be any additional args that `git push` accepts."""
+214        self.git.push(args)
+215
+216    def do_pull(self, args: str):
+217        """Execute `git pull`.
+218
+219        `args` can be any additional args that `git pull` accepts."""
+220        self.git.pull(args)
+221
+222    def do_branches(self, _: str):
+223        """Show local and remote branches."""
+224        self.git.list_branches()
+225
+226    def do_loggy(self, _: str):
+227        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+228        self.git.loggy()
+229
+230    def do_status(self, _: str):
+231        """Execute `git status`."""
+232        self.git.status()
+233
+234    def do_merge(self, branch_name: str):
+235        """Merge supplied `branch_name` with the currently active branch."""
+236        self.git.merge(branch_name)
+237
+238    def do_tag(self, tag_id: str):
+239        """Tag current commit with `tag_id`."""
+240        self.git.tag(tag_id)
+241
+242    @with_parser(add_files_parser, [files_postparser])
+243    def do_amend(self, args: Namespace):
+244        """Stage files and add to previous commit."""
+245        self.git.amend(args.files)
+246
+247    @with_parser(delete_branch_parser)
+248    def do_delete_branch(self, args: Namespace):
+249        """Delete branch."""
+250        self.git.delete_branch(args.branch, not args.remote)
+251
+252    def do_pull_branch(self, branch: str):
+253        """Pull this branch from the origin."""
+254        self.git.pull_branch(branch)
+255
+256    def do_ignore(self, patterns: str):
+257        """Add the list of patterns to `.gitignore`."""
+258        patterns = "\n".join(patterns.split())
+259        path = Pathier(".gitignore")
+260        path.append("\n")
+261        path.append(patterns, False)
+262
+263    def do_make_private(self, owner: str):
+264        """Make the GitHub remote for this repo private.
+265
+266        Expects an argument for the repo owner, i.e. the `OWNER` in
+`github.com/{OWNER}/{repo-name}`
+267
+268        This repo must exist and GitHub CLI must be installed and
+configured."""
+269        self.git.make_private(owner, Pathier.cwd().stem)
+270
+271    def do_make_public(self, owner: str):
+272        """Make the GitHub remote for this repo public.
+273
+274        Expects an argument for the repo owner, i.e. the `OWNER` in
+`github.com/{OWNER}/{repo-name}`
+275
+276        This repo must exist and GitHub CLI must be installed and
+configured."""
+277        self.git.make_public(owner, Pathier.cwd().stem)
+278
+279    def do_delete_gh_repo(self, owner: str):
+280        """Delete this repo from GitHub.
+281
+282        Expects an argument for the repo owner, i.e. the `OWNER` in
+`github.com/{OWNER}/{repo-name}`
+283
+284        GitHub CLI must be installed and configured.
+285
+286        May require you to reauthorize and rerun command."""
+287        self.git.delete_remote(owner, Pathier.cwd().stem)
 GitBetter Shell.
 ⁰
 def default(self, line: str): View Source
-108    def default(self, line: str):
-109        if self.execute_in_terminal_if_unrecognized:
-110            os.system(line)
-111        else:
-112            super().default(line)
+109    def default(self, line: str):
+110        if self.execute_in_terminal_if_unrecognized:
+111            os.system(line)
+112        else:
+113            super().default(line)
 Called on an input line when the command prefix is not recognized.
 If this method is not overridden, it prints an error message and returns.
 ⁰
 def do_help(self, arg: str): View Source
-114    def do_help(self, arg: str):
-115        """List available commands with "help" or detailed help with "help
+115    def do_help(self, arg: str):
+116        """List available commands with "help" or detailed help with "help
 cmd"."""
-116        super().do_help(arg)
-117        if not arg:
-118            print(self.unrecognized_command_behavior_status)
-119            if self.execute_in_terminal_if_unrecognized:
-120                print(
-121                    "^Essentially makes this shell function as a super-shell
+117        super().do_help(arg)
+118        if not arg:
+119            print(self.unrecognized_command_behavior_status)
+120            if self.execute_in_terminal_if_unrecognized:
+121                print(
+122                    "^Essentially makes this shell function as a super-shell
 of whatever shell you launched gitbetter from.^"
-122                )
-123        print()
+123                )
+124        print()
 List available commands with "help" or detailed help with "help cmd".
 ⁰
 def do_toggle_unrecognized_command_behavior(self, arg: str): View Source
-129    def do_toggle_unrecognized_command_behavior(self, arg: str):
-130        """Toggle whether the shell will attempt to execute unrecognized
+130    def do_toggle_unrecognized_command_behavior(self, arg: str):
+131        """Toggle whether the shell will attempt to execute unrecognized
 commands as system commands in the terminal.
-131        When on (the default), `GitBetter` will treat unrecognized commands
+132        When on (the default), `GitBetter` will treat unrecognized commands
 as if you added the `sys` command in front of the input, i.e. `os.system
 (your_input)`.
-132        When off, an `unknown syntax` message will be printed and no
+133        When off, an `unknown syntax` message will be printed and no
 commands will be executed."""
-133        self.execute_in_terminal_if_unrecognized = (
-134            not self.execute_in_terminal_if_unrecognized
-135        )
-136        print(self.unrecognized_command_behavior_status)
+134        self.execute_in_terminal_if_unrecognized = (
+135            not self.execute_in_terminal_if_unrecognized
+136        )
+137        print(self.unrecognized_command_behavior_status)
 Toggle whether the shell will attempt to execute unrecognized commands as
 system commands in the terminal. When on (the default), GitBetter will treat
 unrecognized commands as if you added the sys command in front of the input,
 i.e. os.system(your_input). When off, an unknown syntax message will be printed
 and no commands will be executed.
 ⁰
 def do_cd(self, path: str): View Source
-138    def do_cd(self, path: str):
-139        """Change current working directory to `path`."""
-140        os.chdir(path)
-141        self.prompt = f"gitbetter::{Pathier.cwd()}>"
+139    def do_cd(self, path: str):
+140        """Change current working directory to `path`."""
+141        os.chdir(path)
+142        self.prompt = f"gitbetter::{Pathier.cwd()}>"
 Change current working directory to path.
 ⁰
 def do_git(self, arg: str): View Source
-143    def do_git(self, arg: str):
-144        """Directly execute `git {arg}`.
-145
-146        i.e. You can still do everything directly invoking git can do."""
-147        self.git.execute(arg)
+144    def do_git(self, arg: str):
+145        """Directly execute `git {arg}`.
+146
+147        i.e. You can still do everything directly invoking git can do."""
+148        self.git.execute(arg)
 Directly execute git {arg}.
 i.e. You can still do everything directly invoking git can do.
 ⁰
 def do_new_repo(self, _: str): View Source
-149    def do_new_repo(self, _: str):
-150        """Create a new git repo in this directory."""
-151        self.git.new_repo()
+150    def do_new_repo(self, _: str):
+151        """Create a new git repo in this directory."""
+152        self.git.new_repo()
 Create a new git repo in this directory.
 ⁰
 def do_new_branch(self, name: str): View Source
-153    def do_new_branch(self, name: str):
-154        """Create and switch to a new branch named after the supplied
+154    def do_new_branch(self, name: str):
+155        """Create and switch to a new branch named after the supplied
 arg."""
-155        self.git.create_new_branch(name)
+156        self.git.create_new_branch(name)
 Create and switch to a new branch named after the supplied arg.
 ⁰
 @with_parser(new_remote_parser)
 def do_new_gh_remote(self, args: argshell.argshell.Namespace): View Source
-157    @with_parser(new_remote_parser)
-158    def do_new_gh_remote(self, args: Namespace):
-159        """Create a remote GitHub repository for this repo.
-160
-161        GitHub CLI must be installed and configured for this to work."""
-162        self.git.create_remote_from_cwd(args.public)
+158    @with_parser(new_remote_parser)
+159    def do_new_gh_remote(self, args: Namespace):
+160        """Create a remote GitHub repository for this repo.
+161
+162        GitHub CLI must be installed and configured for this to work."""
+163        self.git.create_remote_from_cwd(args.public)
 Create a remote GitHub repository for this repo.
 GitHub CLI must be installed and configured for this to work.
 ⁰
 def do_initcommit(self, _: str): View Source
-164    def do_initcommit(self, _: str):
-165        """Stage and commit all files with message "Initial Commit"."""
-166        self.git.initcommit()
+165    def do_initcommit(self, _: str):
+166        """Stage and commit all files with message "Initial Commit"."""
+167        self.git.initcommit()
 Stage and commit all files with message "Initial Commit".
 ⁰
 def do_undo(self, _: str): View Source
-168    def do_undo(self, _: str):
-169        """Undo all uncommitted changes."""
-170        self.git.undo()
+169    def do_undo(self, _: str):
+170        """Undo all uncommitted changes."""
+171        self.git.undo()
 Undo all uncommitted changes.
 ⁰
-@with_parser(amend_files_parser, [files_postparser])
+@with_parser(add_files_parser, [files_postparser])
 def do_add(self, args: argshell.argshell.Namespace): View Source
-172    @with_parser(amend_files_parser, [files_postparser])
-173    def do_add(self, args: Namespace):
-174        """Stage a list of files.
-175        If no files are given, all files will be added."""
-176        self.git.add(None if not args.files else args.files)
+173    @with_parser(add_files_parser, [files_postparser])
+174    def do_add(self, args: Namespace):
+175        """Stage a list of files.
+176        If no files are given, all files will be added."""
+177        self.git.add(None if not args.files else args.files)
 Stage a list of files. If no files are given, all files will be added.
 ⁰
 def do_commit(self, args: str): View Source
-178    def do_commit(self, args: str):
-179        """Commit staged files with provided `args` string."""
-180        self.git.commit(args)
+179    def do_commit(self, args: str):
+180        """Commit staged files with provided `args` string."""
+181        self.git.commit(args)
 Commit staged files with provided args string.
 ⁰
 @with_parser(commit_files_parser, [files_postparser])
 def do_commitf(self, args: argshell.argshell.Namespace): View Source
-182    @with_parser(commit_files_parser, [files_postparser])
-183    def do_commitf(self, args: Namespace):
-184        """Stage and commit a list of files."""
-185        self.git.commit_files(args.files, args.message)
+183    @with_parser(commit_files_parser, [files_postparser])
+184    def do_commitf(self, args: Namespace):
+185        """Stage and commit a list of files."""
+186        self.git.commit_files(args.files, args.message)
 Stage and commit a list of files.
 ⁰
 def do_commitall(self, message: str): View Source
-187    def do_commitall(self, message: str):
-188        """Stage and commit all files with this message."""
-189        if not message.startswith('"'):
-190            message = '"' + message
-191        if not message.endswith('"'):
-192            message += '"'
-193        self.git.add()
-194        self.git.commit(f"-m {message}")
+188    def do_commitall(self, message: str):
+189        """Stage and commit all files with this message."""
+190        if not message.startswith('"'):
+191            message = '"' + message
+192        if not message.endswith('"'):
+193            message += '"'
+194        self.git.add()
+195        self.git.commit(f"-m {message}")
 Stage and commit all files with this message.
 ⁰
 def do_switch(self, branch_name: str): View Source
-196    def do_switch(self, branch_name: str):
-197        """Switch to this branch."""
-198        self.git.switch_branch(branch_name)
+197    def do_switch(self, branch_name: str):
+198        """Switch to this branch."""
+199        self.git.switch_branch(branch_name)
 Switch to this branch.
 ⁰
 def do_add_url(self, url: str): View Source
-200    def do_add_url(self, url: str):
-201        """Add remote origin url for repo and push repo."""
-202        self.git.add_remote_url(url)
-203        self.git.push("-u origin main")
+201    def do_add_url(self, url: str):
+202        """Add remote origin url for repo and push repo."""
+203        self.git.add_remote_url(url)
+204        self.git.push("-u origin main")
 Add remote origin url for repo and push repo.
 ⁰
 def do_push_new(self, branch_name: str): View Source
-205    def do_push_new(self, branch_name: str):
-206        """Push this new branch to origin with -u flag."""
-207        self.git.push_new_branch(branch_name)
+206    def do_push_new(self, branch_name: str):
+207        """Push this new branch to origin with -u flag."""
+208        self.git.push_new_branch(branch_name)
 Push this new branch to origin with -u flag.
 ⁰
 def do_push(self, args: str): View Source
-209    def do_push(self, args: str):
-210        """Execute `git push`.
-211
-212        `args` can be any additional args that `git push` accepts."""
-213        self.git.push(args)
+210    def do_push(self, args: str):
+211        """Execute `git push`.
+212
+213        `args` can be any additional args that `git push` accepts."""
+214        self.git.push(args)
 Execute git push.
 args can be any additional args that git push accepts.
 ⁰
 def do_pull(self, args: str): View Source
-215    def do_pull(self, args: str):
-216        """Execute `git pull`.
-217
-218        `args` can be any additional args that `git pull` accepts."""
-219        self.git.pull(args)
+216    def do_pull(self, args: str):
+217        """Execute `git pull`.
+218
+219        `args` can be any additional args that `git pull` accepts."""
+220        self.git.pull(args)
 Execute git pull.
 args can be any additional args that git pull accepts.
 ⁰
 def do_branches(self, _: str): View Source
-221    def do_branches(self, _: str):
-222        """Show local and remote branches."""
-223        self.git.list_branches()
+222    def do_branches(self, _: str):
+223        """Show local and remote branches."""
+224        self.git.list_branches()
 Show local and remote branches.
 ⁰
 def do_loggy(self, _: str): View Source
-225    def do_loggy(self, _: str):
-226        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-227        self.git.loggy()
+226    def do_loggy(self, _: str):
+227        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+228        self.git.loggy()
 Execute git --oneline --name-only --abbrev-commit --graph.
 ⁰
 def do_status(self, _: str): View Source
-229    def do_status(self, _: str):
-230        """Execute `git status`."""
-231        self.git.status()
+230    def do_status(self, _: str):
+231        """Execute `git status`."""
+232        self.git.status()
 Execute git status.
 ⁰
 def do_merge(self, branch_name: str): View Source
-233    def do_merge(self, branch_name: str):
-234        """Merge supplied `branch_name` with the currently active branch."""
-235        self.git.merge(branch_name)
+234    def do_merge(self, branch_name: str):
+235        """Merge supplied `branch_name` with the currently active branch."""
+236        self.git.merge(branch_name)
 Merge supplied branch_name with the currently active branch.
 ⁰
 def do_tag(self, tag_id: str): View Source
-237    def do_tag(self, tag_id: str):
-238        """Tag current commit with `tag_id`."""
-239        self.git.tag(tag_id)
+238    def do_tag(self, tag_id: str):
+239        """Tag current commit with `tag_id`."""
+240        self.git.tag(tag_id)
 Tag current commit with tag_id.
 ⁰
-@with_parser(amend_files_parser, [files_postparser])
+@with_parser(add_files_parser, [files_postparser])
 def do_amend(self, args: argshell.argshell.Namespace): View Source
-241    @with_parser(amend_files_parser, [files_postparser])
-242    def do_amend(self, args: Namespace):
-243        """Stage files and add to previous commit."""
-244        self.git.amend(args.files)
+242    @with_parser(add_files_parser, [files_postparser])
+243    def do_amend(self, args: Namespace):
+244        """Stage files and add to previous commit."""
+245        self.git.amend(args.files)
 Stage files and add to previous commit.
 ⁰
 @with_parser(delete_branch_parser)
 def do_delete_branch(self, args: argshell.argshell.Namespace): View Source
-246    @with_parser(delete_branch_parser)
-247    def do_delete_branch(self, args: Namespace):
-248        """Delete branch."""
-249        self.git.delete_branch(args.branch, not args.remote)
+247    @with_parser(delete_branch_parser)
+248    def do_delete_branch(self, args: Namespace):
+249        """Delete branch."""
+250        self.git.delete_branch(args.branch, not args.remote)
 Delete branch.
 ⁰
 def do_pull_branch(self, branch: str): View Source
-251    def do_pull_branch(self, branch: str):
-252        """Pull this branch from the origin."""
-253        self.git.pull_branch(branch)
+252    def do_pull_branch(self, branch: str):
+253        """Pull this branch from the origin."""
+254        self.git.pull_branch(branch)
 Pull this branch from the origin.
 ⁰
 def do_ignore(self, patterns: str): View Source
-255    def do_ignore(self, patterns: str):
-256        """Add the list of patterns to `.gitignore`."""
-257        patterns = "\n".join(patterns.split())
-258        path = Pathier(".gitignore")
-259        path.append("\n")
-260        path.append(patterns, False)
+256    def do_ignore(self, patterns: str):
+257        """Add the list of patterns to `.gitignore`."""
+258        patterns = "\n".join(patterns.split())
+259        path = Pathier(".gitignore")
+260        path.append("\n")
+261        path.append(patterns, False)
 Add the list of patterns to .gitignore.
 ⁰
 def do_make_private(self, owner: str): View Source
-262    def do_make_private(self, owner: str):
-263        """Make the GitHub remote for this repo private.
-264
-265        Expects an argument for the repo owner, i.e. the `OWNER` in
+263    def do_make_private(self, owner: str):
+264        """Make the GitHub remote for this repo private.
+265
+266        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-266
-267        This repo must exist and GitHub CLI must be installed and
+267
+268        This repo must exist and GitHub CLI must be installed and
 configured."""
-268        self.git.make_private(owner, Pathier.cwd().stem)
+269        self.git.make_private(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo private.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_make_public(self, owner: str): View Source
-270    def do_make_public(self, owner: str):
-271        """Make the GitHub remote for this repo public.
-272
-273        Expects an argument for the repo owner, i.e. the `OWNER` in
+271    def do_make_public(self, owner: str):
+272        """Make the GitHub remote for this repo public.
+273
+274        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-274
-275        This repo must exist and GitHub CLI must be installed and
+275
+276        This repo must exist and GitHub CLI must be installed and
 configured."""
-276        self.git.make_public(owner, Pathier.cwd().stem)
+277        self.git.make_public(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo public.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_delete_gh_repo(self, owner: str): View Source
-278    def do_delete_gh_repo(self, owner: str):
-279        """Delete this repo from GitHub.
-280
-281        Expects an argument for the repo owner, i.e. the `OWNER` in
+279    def do_delete_gh_repo(self, owner: str):
+280        """Delete this repo from GitHub.
+281
+282        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-282
-283        GitHub CLI must be installed and configured.
-284
-285        May require you to reauthorize and rerun command."""
-286        self.git.delete_remote(owner, Pathier.cwd().stem)
+283
+284        GitHub CLI must be installed and configured.
+285
+286        May require you to reauthorize and rerun command."""
+287        self.git.delete_remote(owner, Pathier.cwd().stem)
 Delete this repo from GitHub.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 GitHub CLI must be installed and configured.
 May require you to reauthorize and rerun command.
 ** Inherited Members **
   ⁰
 def main(): View Source
-289def main():
-290    GitBetter().cmdloop()
+290def main():
+291    GitBetter().cmdloop()
```

### Comparing `gitbetter-1.3.0/src/gitbetter/git.py` & `gitbetter-1.4.0/src/gitbetter/git.py`

 * *Files identical despite different names*

### Comparing `gitbetter-1.3.0/src/gitbetter/gitbetter.py` & `gitbetter-1.4.0/src/gitbetter/gitbetter.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,22 +36,23 @@
         search for it in subfolders. This avoids having to type paths to files in subfolders,
         but if you have multiple files in different subfolders with the same name that have changes they
         will all be staged and committed.""",
     )
     return parser
 
 
-def amend_files_parser() -> ArgShellParser:
+def add_files_parser() -> ArgShellParser:
     parser = ArgShellParser()
     parser.add_argument(
-        "-f",
-        "--files",
+        "files",
         type=str,
         nargs="*",
-        help=""" List of files to stage and commit. """,
+        default=None,
+        help=""" List of files to stage and commit. 
+        If not given, all files will be added.""",
     )
     parser.add_argument(
         "-r",
         "--recursive",
         action="store_true",
         help=""" If a file name is not found in the current working directory,
         search for it in subfolders. This avoids having to type paths to files in subfolders,
@@ -164,15 +165,15 @@
         """Stage and commit all files with message "Initial Commit"."""
         self.git.initcommit()
 
     def do_undo(self, _: str):
         """Undo all uncommitted changes."""
         self.git.undo()
 
-    @with_parser(amend_files_parser, [files_postparser])
+    @with_parser(add_files_parser, [files_postparser])
     def do_add(self, args: Namespace):
         """Stage a list of files.
         If no files are given, all files will be added."""
         self.git.add(None if not args.files else args.files)
 
     def do_commit(self, args: str):
         """Commit staged files with provided `args` string."""
@@ -233,15 +234,15 @@
         """Merge supplied `branch_name` with the currently active branch."""
         self.git.merge(branch_name)
 
     def do_tag(self, tag_id: str):
         """Tag current commit with `tag_id`."""
         self.git.tag(tag_id)
 
-    @with_parser(amend_files_parser, [files_postparser])
+    @with_parser(add_files_parser, [files_postparser])
     def do_amend(self, args: Namespace):
         """Stage files and add to previous commit."""
         self.git.amend(args.files)
 
     @with_parser(delete_branch_parser)
     def do_delete_branch(self, args: Namespace):
         """Delete branch."""
```

### Comparing `gitbetter-1.3.0/LICENSE.txt` & `gitbetter-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-1.3.0/README.md` & `gitbetter-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gitbetter-1.3.0/pyproject.toml` & `gitbetter-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2231 2e33 2e30 220d  rsion = "1.3.0".
+000000b0: 7273 696f 6e20 3d20 2231 2e34 2e30 220d  rsion = "1.4.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-1.3.0/PKG-INFO` & `gitbetter-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 1.3.0
+Version: 1.4.0
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
```

