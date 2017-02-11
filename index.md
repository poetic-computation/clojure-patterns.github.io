<html>
<body>

<h1>Clojure Function Patterns</h1>

<h2><code>(butlast col)</code></h2>

<pre><code>Return a seq of all but the last item in coll, in linear time
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>butlast <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24butlast_arg0.png"> <span style="font-size: 2em;">)</span></code></span>
</div>

<div><code>;;=></code></div>

<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24butlast_post.png"></span>
</div>

<h2><code>(concat x y)</code></h2>

<pre><code>Returns a lazy seq representing the concatenation of the elements
in the supplied colls.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>concat <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24concat_arg0.png"> <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24concat_arg1.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24concat_post.png"></span>
</div>


<h2><code>(conj coll x) (conj coll x &amp; xs)</code></h2>

<pre><code>conj[oin]. Returns a new collection with the xs
'added'. (conj nil item) returns (item).  The 'addition' may
happen at different 'places' depending on the concrete type.
</code></pre>

<h5><code>conj vector</code></h5>

<div>
<span><span style="font-size: 2em;">(</span><code>conj <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24conj_arg0_vec.png"> <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24conj_arg1_vec.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24conj_post_vec.png"></span>
</div>


<h5><code>conj list</code></h5>

<div>
<span><span style="font-size: 2em;">(</span><code>conj <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24conj_arg0_list.png"> <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24conj_arg1_list.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24conj_post_list.png"></span>
</div>


<h2><code>(cons x seq)</code></h2>

<pre><code>Returns a new seq where x is the first element and seq is
the rest.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>cons <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24cons_arg0.png"> <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24cons_arg1.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24cons_post.png"></span>
</div>


<h2><code>(dedupe col)</code></h2>

<pre><code>Returns a lazy sequence removing consecutive duplicates in coll. 
Returns a transducer when no collection is provided.</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>dedupe <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24dedupe_arg0.png"> <span style="font-size: 2em;">)</span></code></span>
</div>

<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24dedupe_post.png"></span>
</div>


<h2><code>(distinct col)</code></h2>

<pre><code>Returns a lazy sequence of the elements of coll with duplicates removed.
Returns a stateful transducer when no collection is provided.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>distinct <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24distinct_arg0.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24distinct_post.png"></span>
</div>


<h2><code>(drop-last n col)</code></h2>

<pre><code>Return a lazy sequence of all but the last n (default 1) items in coll
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>drop-last 2 <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24drop_last_arg1.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24drop_last_post.png"></span>
</div>


<h2><code>(flatten col)</code></h2>

<pre><code>Takes any nested combination of sequential things (lists, vectors,
etc.) and returns their contents as a single, flat foldable
collection.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>flatten <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24flatten_arg0.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24flatten_post.png"></span>
</div>


<h2><code>(interpose sep col)</code></h2>

<pre><code>Returns a lazy seq of the elements of coll separated by sep.
Returns a stateful transducer when no collection is provided.
</code></pre>

<div style="padding-bottom: 10px;">
<span><span style="font-size: 2em;">(</span><code>interpose <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24interpose_arg0.png"> <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24interpose_arg1.png"><span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24interpose_post.png"></span>
</div>


<h2><code>(interleave col col)</code></h2>

<pre><code>Returns a lazy seq of the first item in each coll, then the second etc.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>interleave <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24interleave_arg0.png"> <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24interleave_arg1.png"><span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24interleave_post.png"></span>
</div>


<h2><code>(nthnext col n)</code></h2>

<pre><code>Returns the nth next of coll, (seq coll) when n is 0.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>nthnext <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24nthnext_arg0.png"> 2<span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24nthnext_post.png"></span>
</div>


<h2><code>(nthrest n col)</code></h2>

<pre><code>Returns the nth rest of coll, coll when n is 0.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>nthrest 2 <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24nthrest_arg0.png"><span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24nthrest_post.png"></span>
</div>


<h2><code>(partition n col)</code></h2>

<pre><code>Returns a lazy sequence of lists of n items each, at offsets step apart.
If step is not supplied, defaults to n, i.e. the partitions do not overlap.
If a pad collection is supplied, use its elements as necessary to complete
last partition upto n items. In case there are not enough padding elements,
return a partition with less than n items.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>partition 3 <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24partition_arg1.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24partition_post.png"></span>
</div>


<h2><code>(partition-all n col)</code></h2>

<pre><code>Returns a lazy sequence of lists like partition, but may include
partitions with fewer than n items at the end.  Returns a stateful
transducer when no collection is provided.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>partition-all 3 <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24partition_all_arg1.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24partition_all_post.png"></span>
</div>


<h2><code>(replace smap col)</code></h2>

<pre><code>Given a map of replacement pairs and a vector/collection, returns a vector/seq
with any elements = a key in smap replaced with the corresponding val in smap.  
Returns a transducer when no collection is provided.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>replace <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24replace_arg0.png"> [0 3 4] <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24replace_post.png"></span>
</div>


<h2><code>(rest col)</code></h2>

<pre><code>Returns a possibly empty seq of the items after the first. Calls seq on its
argument.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>rest <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24rest_arg0.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24rest_post.png"></span>
</div>


<h2><code>(reverse col)</code></h2>

<pre><code>Returns a seq of the items in coll in reverse order. Not lazy.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>reverse <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24reverse_arg0.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24reverse_post.png"></span>
</div>


<h2><code>(shuffle coll)</code></h2>

<pre><code>Return a random permutation of coll.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>shuffle <img style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24shuffle_arg0.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24shuffle_post.png"></span>
</div>


<h2><code>(sort coll)</code></h2>

<pre><code>Returns a sorted sequence of the items in coll. If no comparator is
supplied, uses compare.  comparator must implement
java.util.Comparator.  Guaranteed to be stable: equal elements will
not be reordered.  If coll is a Java array, it will be modified.  To
avoid this, sort a copy of the array.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>sort <img style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24sort_arg0.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24sort_post.png"></span>
</div>


<h2><code>(take-nth n coll)</code></h2>

<pre><code>Returns a lazy seq of every nth item in coll.
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>take-nth 3 <img style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24take_nth_arg1.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24take_nth_post.png"></span>
</div>


<h2><code>(split-at n col)</code></h2>

<pre><code>Returns a vector of [(take n coll) (drop n coll)]
</code></pre>

<div>
<span><span style="font-size: 2em;">(</span><code>split-at 2 <img  style="vertical-align:middle" src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24split_at_arg1.png"> <span style="font-size: 2em;">)</span></code></span>
</div>


<div><code>;;=></code></div>


<div style="padding-bottom: 40px;">
<span><img src="https://raw.githubusercontent.com/josephwilk/functions-as-patterns/master/doc/clojure.core%24split_at_post.png"></span>
</div>
</body>
</html>
