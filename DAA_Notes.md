<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DAA_Notes</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__left">
    <div class="stackedit__toc">
      
<ul>
<li><a href="#daa-notes-for-mst">DAA Notes for MST</a></li>
<li><a href="#searching--sorting-algorithms">Searching & Sorting Algorithms</a>
<ul>
<li><a href="#unsorted-case">Unsorted Case</a>
<ul>
<li></li>
</ul>
</li>
<li><a href="#binary-search">Binary Search</a>
<ul>
<li></li>
</ul>
</li>
<li><a href="#selection-sort">Selection Sort</a>
<ul>
<li></li>
</ul>
</li>
<li><a href="#selection-sort-recursive">Selection Sort Recursive</a>
<ul>
<li></li>
</ul>
</li>
<li><a href="#insertion-sort">Insertion Sort</a>
<ul>
<li></li>
<li><a href="#python-code-3">Python Code</a></li>
</ul>
</li>
</ul>
</li>
<li><a href="#questions-for-mst">Questions for MST</a></li>
<li><a href="#introduction-ppt---shortnotes">Introduction PPT - Shortnotes</a>
<ul>
<li><a href="#basics--variables-datatypes-etc-">Basics ( Variables, Datatypes, etc )</a></li>
<li><a href="#variables">Variables</a></li>
<li><a href="#data-types">Data types</a></li>
<li><a href="#data-structure">Data Structure</a></li>
<li><a href="#abstract-data-types-adts">Abstract Data Types ADT’s</a></li>
<li><a href="#commonly-used-rate-of-growths">Commonly Used Rate of growths</a></li>
<li><a href="#asymptotic-notation">Asymptotic Notation</a></li>
<li><a href="#big-o-notation">Big-O Notation</a></li>
<li><a href="#big-ω-notation">Big-Ω Notation</a></li>
<li><a href="#theta-notation">Theta Notation</a></li>
</ul>
</li>
<li><a href="#arrays-and-linked-lists">Arrays and Linked Lists</a>
<ul>
<li><a href="#linked-list">Linked List</a></li>
<li><a href="#arrays">Arrays</a></li>
<li><a href="#difference-between-linked-lists-and-arrays">Difference between Linked Lists and Arrays</a></li>
</ul>
</li>
<li><a href="#stacks-and-queues">Stacks and Queues</a>
<ul>
<li><a href="#stacks">Stacks</a></li>
</ul>
</li>
<li><a href="#searching-and-sorting">Searching and Sorting</a></li>
</ul>

    </div>
  </div>
  <div class="stackedit__right">
    <div class="stackedit__html">
      <h1 id="daa-notes-for-mst">DAA Notes for MST</h1>
<blockquote>
<p>Author : Aaron Augustine</p>
</blockquote>
<blockquote>
<p>Star the gist so that I can get a consensus on how many people are using this resource</p>
</blockquote>
<h1 id="searching--sorting-algorithms">Searching &amp; Sorting Algorithms</h1>
<blockquote>
<p>Cheat sheet for algorithm Time Complexity</p>
</blockquote>

<table>
<thead>
<tr>
<th>Algorithm</th>
<th>Best</th>
<th>Average</th>
<th>Worst</th>
<th>Auxillary Space</th>
</tr>
</thead>
<tbody>
<tr>
<td>Selection Sort</td>
<td>O(n<sup>2</sup>)</td>
<td>O(n<sup>2</sup>)</td>
<td>O(n<sup>2</sup>)</td>
<td>O(1)</td>
</tr>
<tr>
<td>Insertion Sort &amp; Bubble Sort</td>
<td>O(n)</td>
<td>O(n<sup>2</sup>)</td>
<td>O(n<sup>2</sup>)</td>
<td>O(1) or O(n) for worst case</td>
</tr>
<tr>
<td>Quick Sort</td>
<td>O(nlogn)</td>
<td>O(nlogn)</td>
<td>O(n<sup>2</sup>)</td>
<td>O(logn) or O(n) for worst case</td>
</tr>
<tr>
<td>Merge Sort</td>
<td>O(nlogn)</td>
<td>O(nlogn)</td>
<td>O(nlogn)</td>
<td>O(n)</td>
</tr>
<tr>
<td>Unsorted Case</td>
<td>O(1)</td>
<td>O(n)</td>
<td>O(n)</td>
<td></td>
</tr>
<tr>
<td>Binary Search</td>
<td>O(1)</td>
<td>O(logn)</td>
<td>O(logn)</td>
<td></td>
</tr>
</tbody>
</table><hr>
<blockquote>
<p><a href="https://www.geeksforgeeks.org/analysis-of-different-sorting-techniques/">Additional Reference : GFG Sorting Techniques</a></p>
</blockquote>
<p><br><br></p>
<h2 id="unsorted-case">Unsorted Case</h2>
<p><em>Best Case</em> : Here the best case would be if the element to be found is the first element [ O(1)]<br>
<em>Average Case</em> : O(n)<br>
<em>Worst Case</em> : Element to be found is the last element [ O(n) ]</p>
<h4 id="algorithm"><em>Algorithm</em></h4>
<pre><code>function search(A, K)
    i = 0;

    while i &lt; n and A[i] != K do
        i = i + 1;

    if i &lt; n
        return i;
    else
        return -1;

</code></pre>
<h4 id="python-code"><em>Python Code</em></h4>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">def</span> <span class="token function">search</span><span class="token punctuation">(</span>array<span class="token punctuation">,</span> k <span class="token punctuation">)</span><span class="token punctuation">:</span>
	i <span class="token operator">=</span> <span class="token number">0</span>
	n <span class="token operator">=</span> <span class="token builtin">len</span><span class="token punctuation">(</span>array<span class="token punctuation">)</span>
<span class="token keyword">while</span> i <span class="token operator">&lt;</span> n <span class="token operator">and</span> A<span class="token punctuation">[</span>i<span class="token punctuation">]</span> <span class="token operator">!=</span> k <span class="token punctuation">:</span> 
	i <span class="token operator">=</span> i <span class="token operator">+</span> <span class="token number">1</span>

<span class="token keyword">if</span> i <span class="token operator">&lt;</span>n <span class="token punctuation">:</span> 
	<span class="token keyword">return</span> i<span class="token punctuation">;</span>
<span class="token keyword">else</span> <span class="token punctuation">:</span> 
	<span class="token keyword">return</span> <span class="token operator">-</span><span class="token number">1</span><span class="token punctuation">;</span>

<span class="token comment">#remaining code to input the values into unsorted search</span>
</code></pre>
<blockquote>
<p>Worst case would be the need to scan the entire sequence A.</p>
<ul>
<li>Time complexity : O(n)</li>
</ul>
</blockquote>
<p><strong>Now let us look at the case where A is sorted</strong><br>
Steps to follow :</p>
<ul>
<li>Compare k with midpoint of A</li>
<li>If midpoint is K, the value is found</li>
<li>If K &lt; midpoint, search left half of the array</li>
<li>If K &gt; midpoint, search right half of the array</li>
</ul>
<p><br><br></p>
<h2 id="binary-search">Binary Search</h2>
<p><em>Best Case</em> : Here the best case would be if the element to be found is the middle element [ O(1) ]<br>
<em>Average Case</em> : O(log<sub>2</sub>n)<br>
<em>Worst Case</em> : Element to be found is on either extremes[ O(log<sub>2</sub>n) ]</p>
<blockquote>
<p>Since it is <strong>Binary</strong> search, the base of the log will be 2</p>
</blockquote>
<h4 id="algorithm-1"><em>Algorithm</em></h4>
<pre><code>bsearch(K, A, l, r) // A sorted, search for K in A[l..r-1]
    if (r - l == 0)
        return false

    mid = (l + r) div 2 // integer division

    if (K == A[mid])
        return true

    if (K &lt; A[mid])
        return bsearch(K, A, l, mid)
    else
        return bsearch(K, A, mid + 1, r)
</code></pre>
<h4 id="python-code-1"><em>Python Code</em></h4>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">def</span> <span class="token function">bsearch</span><span class="token punctuation">(</span>k<span class="token punctuation">,</span> array<span class="token punctuation">,</span> l<span class="token punctuation">,</span> r<span class="token punctuation">)</span> <span class="token punctuation">:</span>
	<span class="token keyword">if</span> <span class="token punctuation">(</span> r <span class="token operator">-</span> l <span class="token operator">==</span> <span class="token number">0</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
		<span class="token keyword">return</span> false
	
	mid <span class="token operator">=</span> <span class="token punctuation">(</span> l <span class="token operator">+</span> r <span class="token punctuation">)</span><span class="token operator">/</span><span class="token number">2</span>
	<span class="token keyword">if</span> <span class="token punctuation">(</span> k <span class="token operator">==</span> arra<span class="token punctuation">[</span>mid<span class="token punctuation">]</span><span class="token punctuation">)</span> <span class="token punctuation">:</span> 
		<span class="token keyword">return</span> true
	<span class="token keyword">if</span> <span class="token punctuation">(</span> k <span class="token operator">&lt;</span> array<span class="token punctuation">[</span>mid<span class="token punctuation">]</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
		<span class="token keyword">return</span> <span class="token punctuation">(</span>bsearch<span class="token punctuation">(</span>k<span class="token punctuation">,</span> array<span class="token punctuation">,</span> l<span class="token punctuation">,</span> mid<span class="token punctuation">)</span><span class="token punctuation">)</span>
	<span class="token keyword">else</span><span class="token punctuation">:</span>
		<span class="token keyword">return</span> <span class="token punctuation">(</span>bsearch<span class="token punctuation">(</span>k<span class="token punctuation">,</span> array<span class="token punctuation">,</span> mid<span class="token operator">+</span><span class="token number">1</span><span class="token punctuation">,</span> r<span class="token punctuation">)</span><span class="token punctuation">)</span>

<span class="token comment">#remaining code to input the values into bsearch</span>
</code></pre>
<blockquote>
<p>T(n) : time to search an array of size n :<br>
T(0) = 1<br>
T(n) = 1 + T(n/2)</p>
</blockquote>
<p>Therefore if we unwind the recurrence</p>
<blockquote>
<p>T(n) = 1 + 1 + T(n/2<sup>2</sup>) = …<br>
T(n) = 1 + 1 + … + T(n/2<sup>k</sup>)<br>
T(n) = 1 + 1 + … + 1 + T(n/2<sup>logn</sup>) = O(logn)</p>
</blockquote>
<p><strong>Binary search works only for arrays</strong></p>
<p><br><br></p>
<h2 id="selection-sort">Selection Sort</h2>
<p><em>Best Case</em> : O(n<sup>2</sup>)<br>
<em>Average Case</em> : O(n<sup>2</sup>)<br>
<em>Worst Case</em> : O(n<sup>2</sup>)</p>
<blockquote>
<p>The idea here is to move the item into it’s correct place in the final sorted list ( Not to use another extra array ).</p>
<ul>
<li>It basically iterates through the array.</li>
<li>Compares each element to the current element.</li>
<li>Looks to swap if the compared element is smaller.</li>
</ul>
</blockquote>
<h4 id="algorithm-2"><em>Algorithm</em></h4>
<pre><code>SelectionSort(A, n) // Sort A of size n
    for (startpos = 0; startpos &lt; n; startpos++)
        // Scan segments A[0]..A[n-1], A[1]..A[n-1], ...
        
        minpos = startpos;
        for (i = minpos + 1; i &lt; n; i++)
            if (A[i] &lt; A[minpos])
                minpos = i;

        swap(A, startpos, minpos)

</code></pre>
<h4 id="java-code"><em>Java Code</em></h4>
<pre class=" language-java"><code class="prism  language-java"><span class="token keyword">import</span> java<span class="token punctuation">.</span>io<span class="token punctuation">.</span>*<span class="token punctuation">;</span>
<span class="token keyword">import</span> java<span class="token punctuation">.</span>util<span class="token punctuation">.</span>Scanner<span class="token punctuation">;</span>

<span class="token keyword">public</span> <span class="token keyword">class</span> <span class="token class-name">selection_sort</span> <span class="token punctuation">{</span>
    
    <span class="token keyword">void</span> <span class="token function">sort</span><span class="token punctuation">(</span><span class="token keyword">int</span> arr<span class="token punctuation">[</span><span class="token punctuation">]</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
        <span class="token keyword">int</span> n <span class="token operator">=</span> arr<span class="token punctuation">.</span>length<span class="token punctuation">;</span>

        <span class="token comment">// Traversing the array</span>
        <span class="token keyword">for</span><span class="token punctuation">(</span><span class="token keyword">int</span> i <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">;</span> i <span class="token operator">&lt;</span> n<span class="token punctuation">;</span> i<span class="token operator">++</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
            <span class="token keyword">int</span> min_idx <span class="token operator">=</span> i<span class="token punctuation">;</span>
            <span class="token keyword">for</span><span class="token punctuation">(</span><span class="token keyword">int</span> j <span class="token operator">=</span> i <span class="token operator">+</span> <span class="token number">1</span><span class="token punctuation">;</span> j <span class="token operator">&lt;</span> n<span class="token punctuation">;</span> j<span class="token operator">++</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
                <span class="token keyword">if</span><span class="token punctuation">(</span>arr<span class="token punctuation">[</span>j<span class="token punctuation">]</span> <span class="token operator">&lt;</span> arr<span class="token punctuation">[</span>min_idx<span class="token punctuation">]</span><span class="token punctuation">)</span>
                    min_idx <span class="token operator">=</span> j<span class="token punctuation">;</span>
            <span class="token punctuation">}</span>

            <span class="token comment">// Time to swap them</span>
            <span class="token keyword">int</span> temp <span class="token operator">=</span> arr<span class="token punctuation">[</span>min_idx<span class="token punctuation">]</span><span class="token punctuation">;</span>
            arr<span class="token punctuation">[</span>min_idx<span class="token punctuation">]</span> <span class="token operator">=</span> arr<span class="token punctuation">[</span>i<span class="token punctuation">]</span><span class="token punctuation">;</span>
            arr<span class="token punctuation">[</span>i<span class="token punctuation">]</span> <span class="token operator">=</span> temp<span class="token punctuation">;</span>
        <span class="token punctuation">}</span>
    <span class="token punctuation">}</span>

    <span class="token keyword">public</span> <span class="token keyword">static</span> <span class="token keyword">void</span> <span class="token function">main</span><span class="token punctuation">(</span>String<span class="token punctuation">[</span><span class="token punctuation">]</span> args<span class="token punctuation">)</span> <span class="token punctuation">{</span>
        Scanner scanner <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">Scanner</span><span class="token punctuation">(</span>System<span class="token punctuation">.</span>in<span class="token punctuation">)</span><span class="token punctuation">;</span>
        selection_sort ob <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">selection_sort</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

        <span class="token comment">// int arr[] = {24, 70, 22, 4, 65, 7, 21};</span>
        System<span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">print</span><span class="token punctuation">(</span><span class="token string">"Input the size of the array to be sorted : "</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
        <span class="token keyword">int</span> size <span class="token operator">=</span> scanner<span class="token punctuation">.</span><span class="token function">nextInt</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

        <span class="token keyword">int</span> arr<span class="token punctuation">[</span><span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">int</span><span class="token punctuation">[</span>size<span class="token punctuation">]</span><span class="token punctuation">;</span>

        System<span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">print</span><span class="token punctuation">(</span><span class="token string">"Input the elements of the array : "</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
        <span class="token keyword">for</span><span class="token punctuation">(</span><span class="token keyword">int</span> i <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">;</span> i <span class="token operator">&lt;</span> size<span class="token punctuation">;</span> i<span class="token operator">++</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
            arr<span class="token punctuation">[</span>i<span class="token punctuation">]</span> <span class="token operator">=</span> scanner<span class="token punctuation">.</span><span class="token function">nextInt</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
        <span class="token punctuation">}</span>

        scanner<span class="token punctuation">.</span><span class="token function">close</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

        ob<span class="token punctuation">.</span><span class="token function">sort</span><span class="token punctuation">(</span>arr<span class="token punctuation">)</span><span class="token punctuation">;</span>
        System<span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">println</span><span class="token punctuation">(</span><span class="token string">"Sorted Array"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
        <span class="token keyword">int</span> n <span class="token operator">=</span> arr<span class="token punctuation">.</span>length<span class="token punctuation">;</span>
        <span class="token keyword">for</span><span class="token punctuation">(</span><span class="token keyword">int</span> i <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">;</span> i <span class="token operator">&lt;</span> n<span class="token punctuation">;</span> i<span class="token operator">++</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
            System<span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">print</span><span class="token punctuation">(</span>arr<span class="token punctuation">[</span>i<span class="token punctuation">]</span> <span class="token operator">+</span> <span class="token string">" "</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
            System<span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">println</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
        <span class="token punctuation">}</span>
    <span class="token punctuation">}</span>
<span class="token punctuation">}</span>
</code></pre>
<blockquote>
<p>Time complexity : O(n<sup>2</sup>)<br>
Finding minimum in unsorted segment of length k requires one scan, k steps<br>
T(n) = n + (n-1) + (n-2) + … + 1 = n(n+1)/2 = O(n<sup>2</sup>)</p>
</blockquote>
<p><br><br></p>
<h2 id="selection-sort-recursive">Selection Sort <sub>Recursive</sub></h2>
<p><em>Best Case</em> : O(n<sup>2</sup>)<br>
<em>Average Case</em> : O(n<sup>2</sup>)<br>
<em>Worst Case</em> : O(n<sup>2</sup>)</p>
<h4 id="algorithm-3"><em>Algorithm</em></h4>
<pre><code>SelectionSort(A, start, n) // Sort A from start to n-1
    if (start &gt;= n - 1)
        return;

    // Locate minimum element and move to start of segment
    minpos = start;
    for (i = start + 1; i &lt; n; i++)
        if (A[i] &lt; A[minpos])
            minpos = i;

    swap(A, start, minpos)

    // Recursively sort the rest
    SelectionSort(A, start + 1, n)

</code></pre>
<h4 id="python-code-2"><em>Python Code</em></h4>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">def</span> <span class="token function">selection_sort_recursive</span><span class="token punctuation">(</span>A<span class="token punctuation">,</span> start<span class="token punctuation">,</span> n<span class="token punctuation">)</span><span class="token punctuation">:</span>
    <span class="token keyword">if</span> start <span class="token operator">&gt;=</span> n <span class="token operator">-</span> <span class="token number">1</span><span class="token punctuation">:</span>
        <span class="token keyword">return</span>
    
    <span class="token comment"># Locate minimum element and move to start of segment</span>
    minpos <span class="token operator">=</span> start
    <span class="token keyword">for</span> i <span class="token keyword">in</span> <span class="token builtin">range</span><span class="token punctuation">(</span>start <span class="token operator">+</span> <span class="token number">1</span><span class="token punctuation">,</span> n<span class="token punctuation">)</span><span class="token punctuation">:</span>
        <span class="token keyword">if</span> A<span class="token punctuation">[</span>i<span class="token punctuation">]</span> <span class="token operator">&lt;</span> A<span class="token punctuation">[</span>minpos<span class="token punctuation">]</span><span class="token punctuation">:</span>
            minpos <span class="token operator">=</span> i
    
    <span class="token comment"># Swap elements</span>
    A<span class="token punctuation">[</span>start<span class="token punctuation">]</span><span class="token punctuation">,</span> A<span class="token punctuation">[</span>minpos<span class="token punctuation">]</span> <span class="token operator">=</span> A<span class="token punctuation">[</span>minpos<span class="token punctuation">]</span><span class="token punctuation">,</span> A<span class="token punctuation">[</span>start<span class="token punctuation">]</span>
    
    <span class="token comment"># Recursively sort the rest</span>
    selection_sort_recursive<span class="token punctuation">(</span>A<span class="token punctuation">,</span> start <span class="token operator">+</span> <span class="token number">1</span><span class="token punctuation">,</span> n<span class="token punctuation">)</span>

<span class="token comment"># Example usage:</span>
array <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">64</span><span class="token punctuation">,</span> <span class="token number">25</span><span class="token punctuation">,</span> <span class="token number">12</span><span class="token punctuation">,</span> <span class="token number">22</span><span class="token punctuation">,</span> <span class="token number">11</span><span class="token punctuation">]</span>
selection_sort_recursive<span class="token punctuation">(</span>array<span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token builtin">len</span><span class="token punctuation">(</span>array<span class="token punctuation">)</span><span class="token punctuation">)</span>

<span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Sorted array:"</span><span class="token punctuation">,</span> array<span class="token punctuation">)</span>

</code></pre>
<p><br><br></p>
<h2 id="insertion-sort">Insertion Sort</h2>
<p><em>Best Case</em> : O(n<sup>2</sup>)<br>
<em>Average Case</em> : O(n<sup>2</sup>)<br>
<em>Worst Case</em> : O(n<sup>2</sup>)</p>
<blockquote>
<p>We start by building a sorted sequence with one element<br>
Then we pick up the next unsorted element and insert it into it’s correct place in the already sorted sequence</p>
</blockquote>
<h4 id="algorithm-4"><em>Algorithm</em></h4>
<pre><code>
</code></pre>
<h3 id="python-code-3"><em>Python Code</em></h3>
<pre class=" language-python"><code class="prism  language-python">
</code></pre>
<h1 id="questions-for-mst">Questions for MST</h1>
<blockquote>
<p>Q1. What is an Algorithm ? Why do we analyse algorithms?</p>
</blockquote>
<p><strong>Ans</strong>. <em>An Algorithm is the step-by-step instruction given to sove a certain problem</em><br>
Just how there are many ways to travel from a given ‘City A’ to ‘City B’, there can be multiple algorithms for a given question.<br>
Analysing them helps us figure out which algorithm is the most suitable and the most effective.</p>
<hr>
<blockquote>
<p>Q2. What is running time anaylsis ?</p>
</blockquote>
<p><strong>Ans</strong>. It is the process of determining how processing time increases as the size of the problem ( input size ) increases.<br>
The following are the different types of inputs we encounter :</p>
<ul>
<li>Size of an array</li>
<li>Polynomial Degree</li>
<li>Number of elements in a  matrix</li>
<li>Number of bits in binary representation of the input</li>
<li>Vertices and edges of a  graph</li>
</ul>
<hr>
<blockquote>
<p>Q3.</p>
</blockquote>
<p><br><br></p>
<h1 id="introduction-ppt---shortnotes">Introduction PPT - Shortnotes</h1>
<h2 id="basics--variables-datatypes-etc-">Basics ( Variables, Datatypes, etc )</h2>
<blockquote>
<p>Ref : <a href="https://classroom.google.com/c/NjU3MzUwMzg0NDgy/m/NjU4Mjc0MDkzNDYx/details">Chap_1_pdf</a></p>
</blockquote>
<h2 id="variables">Variables</h2>
<p>X, y, z or any other alphabets that are used as “<em>placeholders</em>” to store values ( data ) are known as variables.</p>
<h2 id="data-types">Data types</h2>
<p>The variables defined form equations when used. To solve the equations we need them to hold specific types of values and ‘data type’ is the name being use to define those specific values.<br>
<em>In Programming language it is a set of data with values having predefined characteristics</em></p>
<blockquote>
<p>Ex. : char, integer, boolean, long int, short int, etc</p>
</blockquote>
<p>There are two types of Data Types :</p>
<ul>
<li>System defined data types / Primitive Data types ( <em>int, float, char, double, bool, etc …</em> )</li>
<li>User Defined Data types :<br>
<img src="https://lh7-us.googleusercontent.com/rylKh1jPp5tTkKNDRyDw4jy8VJTXGnKO9BAdBF_AhoevlPpGEkTV8AYI693xJW3NIaByvFifQNjldUqIYLJWQmN6AXWRIQGK0S_UqY3n9AW3zUthqG20MaaMf1m636t69-LZNgKVz1k4tg9Q758DkZ4" alt=""></li>
</ul>
<h2 id="data-structure">Data Structure</h2>
<blockquote>
<p><a href="https://www.sanfoundry.com/sorting-multiple-choice-questions-mcq/">Reference : Data structure based mcqs</a></p>
</blockquote>
<p><em>Data Structure is a particular way of storinga nd organizing data on a computer so that it can be used efficiently</em><br>
There are two types of Data Structures :</p>
<ul>
<li>Linear Data Structures ( <em>elements are accessed in a sequential order</em>)</li>
<li>Non-Linear Data Structures (<em>elements are stored/accessed in a non-linear order</em>)</li>
</ul>
<h2 id="abstract-data-types-adts">Abstract Data Types <sub>ADT’s</sub></h2>
<p>When we combine the user defined data structures with their operations they are known as ‘Abstract Data Types’, and they consist of two parts :</p>
<ul>
<li>Declaration of Data</li>
<li>Declaration of Operations</li>
</ul>
<p>Ex : Linked Lists, Stacks, Queues, Priority Queues, Binary Trees, Dictionaries, Disjoint Sets, Hash Tables, Graphs, etc</p>
<h2 id="commonly-used-rate-of-growths">Commonly Used Rate of growths</h2>
<p><strong><img src="https://lh7-us.googleusercontent.com/2xn1LSkl1ln_fqdyGy_zTpqf4RTOVa0sWsjRShl66SWilHgt-vIoXbMa7UWKujaJloy0GvPnxFczfhL_LzM2rTnV5uwGmueezRQlzw6egAeUFlsz7K2MmsSkXXMkPC1OOPp3U79SFFbfby5Xk-5EACE" alt=""></strong><br>
The table above shows the relation between different rates of growth and examples</p>
<p><strong><img src="https://lh7-us.googleusercontent.com/7lwSiL-rvYP66ye8VnLkpxkWpex5wZjH1UExrhnFXop-0t5aBDcRVLWNGWT67t9ni1An9V5__tkyLXh9RAvEKdYRlhukY0dGOtvuFlcPv2fKdPjQgDFsFCPE7DXg1l_OH6tlPA9Q5LzrCEJZHEpM4Hg" alt=""></strong><br>
The flowchart above describes the decrease in time complexity, of the rate of growth.</p>
<blockquote>
<p>There are 3 types of analyis :</p>
<ul>
<li>Worst Case</li>
<li>Best Case</li>
<li>Averge Case</li>
</ul>
</blockquote>
<h2 id="asymptotic-notation">Asymptotic Notation</h2>
<p><a href="https://www.youtube.com/watch?v=A03oI0znAoc">Reference : Aysmptotic notations - Big-O,Ω and theta</a></p>
<h2 id="big-o-notation">Big-O Notation</h2>
<p>*This shows upper bound of a function<br>
*Represented as f(n) = O(g(n)), i.e. for larger values of n, f(n) = g(n)</p>
<h2 id="big-ω-notation">Big-Ω Notation</h2>
<ul>
<li>This shows lower bound of a function</li>
</ul>
<h2 id="theta-notation">Theta Notation</h2>
<ul>
<li>This shows the average bound of afunction</li>
</ul>
<hr>
<h1 id="arrays-and-linked-lists">Arrays and Linked Lists</h1>
<blockquote>
<p><a href="https://www.sanfoundry.com/data-structure-questions-answers-array-array-operations/">Reference : Array and Array ops mcqs</a></p>
</blockquote>
<h2 id="linked-list">Linked List</h2>
<p>It is a DS used to store collections of data, and it has the following properties</p>
<ul>
<li>Successive elements are connected by pointers.</li>
<li>Last elements points to NULL</li>
<li>Can grow or shrink in size during execution of a program</li>
<li>Can be made just as long as required</li>
<li>Does not waste memory space</li>
</ul>
<h3 id="main-linked-list-operations-">Main linked list operations :</h3>
<ul>
<li><strong>Insert</strong> : Inserts an element into the list</li>
<li><strong>Delete</strong> : Deletes an element from the list :</li>
</ul>
<h3 id="auxillary-linked-list-operations">Auxillary linked list operations</h3>
<ul>
<li><strong>Delete List</strong> : Removes all the elements of the list / disposes of the list</li>
<li><strong>Count</strong> : Returns the number of elements in the list</li>
<li>Find n<sup>th</sup> node from the end of the list</li>
</ul>
<hr>
<h2 id="arrays">Arrays</h2>
<p><strong><img src="https://lh7-us.googleusercontent.com/u1tT-MC3ilPz4B14Z2NyewoKneBuAs41xufwguVhYx6IxN7KlHDKjs_dQOzdfMnpiQOQxgySPUvwLUH8dH_z7XApN1KkeJRDNGB37wRtLl1jQvv9FY3TBTzKOYWC3wO4wQSt5FNPDuPy1asdyXZj5_4" alt=""></strong></p>
<h3 id="advantages-of-arrays-">Advantages of Arrays :</h3>
<ol>
<li>Simple and easy to use</li>
<li>Faster access to the elements</li>
</ol>
<h3 id="disadvantages-of-arrays-">Disadvantages of Arrays :</h3>
<ol>
<li><strong>Fixed Size</strong> : The size of the array is static ( specify the array size before using it )<br>
2.<strong>One block allocation</strong> : To allocate the array at the beginning itself, sometimes it may not be possible to get the memory for the complete array.</li>
<li><strong>Complex position-based insertion</strong> : TO insert an element at a given position we may need to shift the elements. This will create a position for us to insert the new element at the desired position.</li>
</ol>
<p><strong>The main disadvantage of linked lists is the long access time for any element in a linked list</strong></p>
<h2 id="difference-between-linked-lists-and-arrays">Difference between Linked Lists and Arrays</h2>
<p><strong><img src="https://lh7-us.googleusercontent.com/NAA1UFQ0FDQeuqWy0qmLmAL3aa8nVEAc7xyeI33P_7z_wl6LB-HX0YPwEFI0Ul3mlQscFeqcspIVXxbLGESJcB6eb4I3dLwD8-16mUQPMTdd8XUI9H8NBzPXFhLimice1EWISd3OotRYumeAUyyi28g" alt=""></strong></p>
<h1 id="stacks-and-queues">Stacks and Queues</h1>
<h2 id="stacks">Stacks</h2>
<p>A stack is a simple data structure used for storing data. In this the order that they arrive in is important, just like a stack of plates, the first one stacked is the last to be used.</p>
<blockquote>
<p>Two operations that can be done on astack are “Push” (insert data ) and “Pop” ( remove data )</p>
</blockquote>
<p><strong><img src="https://lh7-us.googleusercontent.com/eB8AtQSRUY1d89s7QtMfoSSsiVcKzPgAbnwL6hhH5-EJyjPV77aE7FMjnH1QGBbiJluc-malu0khGY975dkPQyWkYZgZTEJwpv1m9Yk_DB32auUOUPxUCTVRtz38hemQMRklcb4frrTUsXEKywRM89Q" alt=""></strong></p>
<h1 id="searching-and-sorting">Searching and Sorting</h1>
<blockquote>
<p><a href="https://www.sanfoundry.com/sorting-multiple-choice-questions-mcq/">Reference : Sorting based mcqs</a></p>
</blockquote>

    </div>
  </div>
</body>

</html>
