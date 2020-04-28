<p>The&nbsp;<a title="Syntax (programming languages)" href="https://en.wikipedia.org/wiki/Syntax_(programming_languages)">syntax</a>&nbsp;of the&nbsp;<a title="Python (programming language)" href="https://en.wikipedia.org/wiki/Python_(programming_language)">Python programming language</a>&nbsp;is the set of rules that defines how a Python program will be written and interpreted (by both the&nbsp;<a title="Runtime system" href="https://en.wikipedia.org/wiki/Runtime_system">runtime system</a>&nbsp;and by human readers). The Python language has many similarities to&nbsp;<a class="mw-redirect" title="Perl (programming language)" href="https://en.wikipedia.org/wiki/Perl_(programming_language)">Perl</a>,&nbsp;<a title="C (programming language)" href="https://en.wikipedia.org/wiki/C_(programming_language)">C</a>, and&nbsp;<a title="Java (programming language)" href="https://en.wikipedia.org/wiki/Java_(programming_language)">Java</a>. However, there are some definite differences between the languages.</p>
</br>

<div class="toctitle" dir="ltr" lang="en">
<h2 id="mw-toc-heading">Contents</h2>
<label class="toctogglelabel" for="toctogglecheckbox"></label></div>
<ul>
<li class="toclevel-1 tocsection-1"><a href="#Design_philosophy"><span class="toctext">Design philosophy</span></a></li>
<li class="toclevel-1 tocsection-2"><a href="#Keywords"><span class="toctext">Keywords</span></a></li>
<li class="toclevel-1 tocsection-3"><a href="#Indentation"><span class="toctext">Indentation</span></a></li>
<li class="toclevel-1 tocsection-4"><a href="#Data_structures"><span class="toctext">Data structures</span></a>
<ul>
<li class="toclevel-2 tocsection-5"><a href="#Base_types"><span class="toctext">Base types</span></a></li>
<li class="toclevel-2 tocsection-6"><a href="#Collection_types"><span class="toctext">Collection types</span></a></li>
<li class="toclevel-2 tocsection-7"><a href="#Object_system"><span class="toctext">Object system</span></a></li>
</ul>
</li>
<li class="toclevel-1 tocsection-8"><a href="#Literals"><span class="toctext">Literals</span></a>
<ul>
<li class="toclevel-2 tocsection-9"><a href="#Strings"><span class="toctext">Strings</span></a>
<ul>
<li class="toclevel-3 tocsection-10"><a href="#Normal_string_literals"><span class="toctext">Normal string literals</span></a></li>
<li class="toclevel-3 tocsection-11"><a href="#Multi-line_string_literals"><span class="toctext">Multi-line string literals</span></a></li>
<li class="toclevel-3 tocsection-12"><a href="#Raw_strings"><span class="toctext">Raw strings</span></a></li>
<li class="toclevel-3 tocsection-13"><a href="#Concatenation_of_adjacent_string_literals"><span class="toctext">Concatenation of adjacent string literals</span></a></li>
</ul>
</li>
<li class="toclevel-2 tocsection-14"><a href="#Numbers"><span class="toctext">Numbers</span></a></li>
<li class="toclevel-2 tocsection-15"><a href="#Lists,_tuples,_sets,_dictionaries"><span class="toctext">Lists, tuples, sets, dictionaries</span></a></li>
</ul>
</li>
<li class="toclevel-1 tocsection-16"><a href="#Operators"><span class="toctext">Operators</span></a>
<ul>
<li class="toclevel-2 tocsection-17"><a href="#Arithmetic"><span class="toctext">Arithmetic</span></a></li>
<li class="toclevel-2 tocsection-18"><a href="#Comparison_operators"><span class="toctext">Comparison operators</span></a></li>
<li class="toclevel-2 tocsection-19"><a href="#Logical_operators"><span class="toctext">Logical operators</span></a></li>
</ul>
</li>
<li class="toclevel-1 tocsection-20"><a href="#Functional_programming"><span class="toctext">Functional programming</span></a>
<ul>
<li class="toclevel-2 tocsection-21"><a href="#Comprehensions"><span class="toctext">Comprehensions</span></a></li>
<li class="toclevel-2 tocsection-22"><a href="#First-class_functions"><span class="toctext">First-class functions</span></a></li>
<li class="toclevel-2 tocsection-23"><a href="#Closures"><span class="toctext">Closures</span></a></li>
<li class="toclevel-2 tocsection-24"><a href="#Generators"><span class="toctext">Generators</span></a></li>
<li class="toclevel-2 tocsection-25"><a href="#Generator_expressions"><span class="toctext">Generator expressions</span></a></li>
<li class="toclevel-2 tocsection-26"><a href="#Dictionary_and_set_comprehensions"><span class="toctext">Dictionary and set comprehensions</span></a></li>
</ul>
</li>
<li class="toclevel-1 tocsection-27"><a href="#Objects"><span class="toctext">Objects</span></a>
<ul>
<li class="toclevel-2 tocsection-28"><a href="#With_statements"><span class="toctext">With statements</span></a></li>
<li class="toclevel-2 tocsection-29"><a href="#Properties"><span class="toctext">Properties</span></a></li>
<li class="toclevel-2 tocsection-30"><a href="#Descriptors"><span class="toctext">Descriptors</span></a></li>
<li class="toclevel-2 tocsection-31"><a href="#Class_and_static_methods"><span class="toctext">Class and static methods</span></a></li>
</ul>
</li>
<li class="toclevel-1 tocsection-32"><a href="#Exceptions"><span class="toctext">Exceptions</span></a></li>
<li class="toclevel-1 tocsection-33"><a href="#Comments_and_docstrings"><span class="toctext">Comments and docstrings</span></a></li>
<li class="toclevel-1 tocsection-34"><a href="#Function_annotations"><span class="toctext">Function annotations</span></a></li>
<li class="toclevel-1 tocsection-35"><a href="#Decorators"><span class="toctext">Decorators</span></a></li>
<li class="toclevel-1 tocsection-36"><a href="#Easter_eggs"><span class="toctext">Easter eggs</span></a></li>
</ul>

<p>&nbsp;</p>

<h2><span id="Design_philosophy" class="mw-headline">Design philosophy</span></h2>
<p>Python was designed to be a highly readable language.&nbsp;It has a relatively uncluttered visual layout and uses English keywords frequently where other languages use punctuation. Python aims to be simple and consistent in the design of its syntax, encapsulated in the mantra "There should be one&mdash;and preferably only one&mdash;obvious way to do it", from "<a class="mw-redirect" title="The Zen of Python" href="https://en.wikipedia.org/wiki/The_Zen_of_Python">The Zen of Python</a>".</p>
<p>This mantra is deliberately opposed to the&nbsp;<a title="Perl" href="https://en.wikipedia.org/wiki/Perl">Perl</a>&nbsp;and&nbsp;<a title="Ruby (programming language)" href="https://en.wikipedia.org/wiki/Ruby_(programming_language)">Ruby</a>&nbsp;mantra, "<a title="There's more than one way to do it" href="https://en.wikipedia.org/wiki/There%27s_more_than_one_way_to_do_it">there's more than one way to do it</a>".</p>
<h2><span id="Keywords" class="mw-headline">Keywords</span></h2>
<p>Python has the following keywords or&nbsp;<em>reserved words</em>; they cannot be used as identifiers.</p>
<div class="div-col columns column-width">
<ul>
<li><code>and</code></li>
<li><code>as</code></li>
<li><code>assert</code></li>
<li><code>async</code></li>
<li><code>await</code></li>
<li><code>break</code></li>
<li><code>class</code></li>
<li><code>continue</code></li>
<li><code>def</code></li>
<li><code>del</code></li>
<li><code>elif</code></li>
<li><code>else</code></li>
<li><code>except</code></li>
<li><code>False</code></li>
<li><code>finally</code></li>
<li><code>for</code></li>
<li><code>from</code></li>
<li><code>global</code></li>
<li><code>if</code></li>
<li><code>import</code></li>
<li><code>in</code></li>
<li><code>is</code></li>
<li><code>lambda</code></li>
<li><code>None</code></li>
<li><code>nonlocal</code></li>
<li><code>not</code></li>
<li><code>or</code></li>
<li><code>pass</code></li>
<li><code>raise</code></li>
<li><code>return</code></li>
<li><code>True</code></li>
<li><code>try</code></li>
<li><code>while</code></li>
<li><code>with</code></li>
<li><code>yield</code></li>
</ul>
</div>
<dl>
<dt>Notes</dt>
</dl>
<div class="reflist">
<div class="mw-references-wrap">
<ol class="references">
<li id="cite_note-keywordIn35-6"><span class="reference-text">Starting from Python 3.5,&nbsp;<code>async</code>&nbsp;and&nbsp;<code>await</code>&nbsp;were introduced.</span></li>
<li id="cite_note-keywordIn3-7"><span class="reference-text">Starting from Python 3, keywords&nbsp;<code>True</code>,&nbsp;<code>False</code>&nbsp;and&nbsp;<code>nonlocal</code>&nbsp;were introduced.</span></li>
</ol>
</div>
</div>
<h2><span id="Indentation" class="mw-headline">Indentation</span></h2>
<p>Python uses&nbsp;<a title="Whitespace character" href="https://en.wikipedia.org/wiki/Whitespace_character">whitespace</a>&nbsp;to delimit&nbsp;<a title="Control flow" href="https://en.wikipedia.org/wiki/Control_flow">control flow</a>&nbsp;blocks (following the&nbsp;<a title="Off-side rule" href="https://en.wikipedia.org/wiki/Off-side_rule">off-side rule</a>). Python borrows this feature from its predecessor&nbsp;<a title="ABC (programming language)" href="https://en.wikipedia.org/wiki/ABC_(programming_language)">ABC</a>: instead of punctuation or keywords, it uses indentation to indicate the run of a block.</p>
<p>In so-called "free-format" languages &mdash; that use the block structure derived from&nbsp;<a title="ALGOL" href="https://en.wikipedia.org/wiki/ALGOL">ALGOL</a>&nbsp;&mdash; blocks of code are set off with braces (<code>{ }</code>) or keywords. In most coding conventions for these languages, programmers conventionally indent the code within a block, to visually set it apart from the surrounding code (<a title="Prettyprint" href="https://en.wikipedia.org/wiki/Prettyprint">prettyprinting</a>).</p>
<p>Consider a function,&nbsp;<code>foo</code>, which is passed a single&nbsp;<a title="Parameter (computer programming)" href="https://en.wikipedia.org/wiki/Parameter_(computer_programming)">parameter</a>,&nbsp;<code>x</code>, and if the parameter is 0 will call&nbsp;<code>bar</code>&nbsp;and&nbsp;<code>baz</code>, otherwise it will call&nbsp;<code>qux</code>, passing&nbsp;<code>x</code>, and also call itself recursively, passing&nbsp;<code>x-1</code>&nbsp;as the parameter. Here are implementations of this function in both C and Python:</p>
<p><code>foo</code>&nbsp;function in&nbsp;<a title="C (programming language)" href="https://en.wikipedia.org/wiki/C_(programming_language)">C</a>&nbsp;with&nbsp;<a class="mw-redirect" title="Indent style" href="https://en.wikipedia.org/wiki/Indent_style#K&amp;R">K&amp;R indent style</a>:</p>
<div class="mw-highlight mw-highlight-lang-c mw-content-ltr" dir="ltr">
<pre><span class="kt">void</span> <span class="nf">foo</span><span class="p">(</span><span class="kt">int</span> <span class="n">x</span><span class="p">)</span>
<span class="p">{</span>
    <span class="k">if</span> <span class="p">(</span><span class="n">x</span> <span class="o">==</span> <span class="mi">0</span><span class="p">)</span> <span class="p">{</span>
        <span class="n">bar</span><span class="p">();</span>
        <span class="n">baz</span><span class="p">();</span>
    <span class="p">}</span> <span class="k">else</span> <span class="p">{</span>
        <span class="n">qux</span><span class="p">(</span><span class="n">x</span><span class="p">);</span>
        <span class="n">foo</span><span class="p">(</span><span class="n">x</span> <span class="o">-</span> <span class="mi">1</span><span class="p">);</span>
    <span class="p">}</span>
<span class="p">}</span>
</pre>
</div>
<p><code>foo</code>&nbsp;function in Python:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">foo</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">x</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
        <span class="n">bar</span><span class="p">()</span>
        <span class="n">baz</span><span class="p">()</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="n">qux</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
        <span class="n">foo</span><span class="p">(</span><span class="n">x</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span>
</pre>
</div>
<p>Python mandates a convention that programmers in&nbsp;<a title="ALGOL" href="https://en.wikipedia.org/wiki/ALGOL">ALGOL</a>-style languages often follow. Incorrectly indented code can be understood by human reader differently than does a compiler or interpreter.</p>
<p>This example illustrates an error introduced by incorrect indentation:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">foo</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">x</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
        <span class="n">bar</span><span class="p">()</span>
        <span class="n">baz</span><span class="p">()</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="n">qux</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
    <span class="n">foo</span><span class="p">(</span><span class="n">x</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span>
</pre>
</div>
<p>Here, in contrast to the above Python&nbsp;<code>foo</code>&nbsp;example, the function call&nbsp;<code>foo(x - 1)</code>&nbsp;always gets executed, resulting in an endless recursion. Such an indentation error (like the accidental removal of the indentation in the last line) is only possible in programming languages that do not mark blocks with distinct markers, like curly brackets in C. In this particular case, not even an editor with automatic indentation could prevent the erroneous behaviour of this Python code. This unintended error can easily pass into the code base without prior noticing by the programmer. In most other programming languages, this would not be possible (deleting a block-end marker in C would lead to a compiler error), and this makes the Python syntax less robust than most other languages.</p>
<p>Both&nbsp;<a title="Space (punctuation)" href="https://en.wikipedia.org/wiki/Space_(punctuation)">space</a>&nbsp;characters and&nbsp;<a title="Tab key" href="https://en.wikipedia.org/wiki/Tab_key">tab</a>&nbsp;characters are currently accepted as forms of indentation in Python. Since many tools do not visually distinguish them, mixing spaces and tabs can create bugs that take specific efforts to find (a perennial suggestion among Python users has been removing tabs as block markers; other Python users propound removing spaces instead). Moreover, formatting routines which remove whitespace&mdash;for instance, many&nbsp;<a title="Internet forum" href="https://en.wikipedia.org/wiki/Internet_forum">Internet forums</a>&mdash;can destroy the syntax of a Python program, whereas a program in a bracketed language would merely become more difficult to read.</p>
<p>Many popular code editors handle Python's indentation conventions seamlessly, sometimes after a configuration option is enabled.</p>
<h2><span id="Data_structures" class="mw-headline">Data structures</span></h2>
<p>Since Python is a&nbsp;<a class="mw-redirect" title="Dynamic typing" href="https://en.wikipedia.org/wiki/Dynamic_typing">dynamically typed</a>&nbsp;language, Python&nbsp;<em>values,</em>&nbsp;not variables, carry type. This has implications for many aspects of the way the language functions.</p>
<p>All variables in Python hold references to objects, and these references are passed to functions; a function cannot change the value of variable references in its calling function (but see below for exceptions). Some people (including&nbsp;<a title="Guido van Rossum" href="https://en.wikipedia.org/wiki/Guido_van_Rossum">Guido van Rossum</a>&nbsp;himself) have called this parameter-passing scheme "Call by object reference." An object reference means a name, and the passed reference is an "alias", i.e. a copy of the reference to the same object, just as in C/C++. The object's value may be changed in the called function with the "alias", for example:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="o">&gt;&gt;&gt;</span> <span class="n">alist</span> <span class="o">=</span> <span class="p">[</span><span class="s1">'a'</span><span class="p">,</span> <span class="s1">'b'</span><span class="p">,</span> <span class="s1">'c'</span><span class="p">]</span>
<span class="o">&gt;&gt;&gt;</span> <span class="k">def</span> <span class="nf">my_func</span><span class="p">(</span><span class="n">al</span><span class="p">):</span>
<span class="o">...</span>     <span class="n">al</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">'x'</span><span class="p">)</span>
<span class="o">...</span>     <span class="nb">print</span><span class="p">(</span><span class="n">al</span><span class="p">)</span>
<span class="o">...</span>
<span class="o">&gt;&gt;&gt;</span> <span class="n">my_func</span><span class="p">(</span><span class="n">alist</span><span class="p">)</span>
<span class="p">[</span><span class="s1">'a'</span><span class="p">,</span> <span class="s1">'b'</span><span class="p">,</span> <span class="s1">'c'</span><span class="p">,</span> <span class="s1">'x'</span><span class="p">]</span>
<span class="o">&gt;&gt;&gt;</span> <span class="n">alist</span>
<span class="p">[</span><span class="s1">'a'</span><span class="p">,</span> <span class="s1">'b'</span><span class="p">,</span> <span class="s1">'c'</span><span class="p">,</span> <span class="s1">'x'</span><span class="p">]</span>
</pre>
</div>
<p>Function&nbsp;<code>my_func</code>&nbsp;changed the value of&nbsp;<code>alist</code>&nbsp;with the formal argument&nbsp;<code>al</code>, which is an alias of&nbsp;<code>alist</code>. However, any attempt to operate on the alias itself will have no effect on the original object. In Python, non-innermost-local and not-declared-global accessible names are all aliases.</p>
<p>Among dynamically typed languages, Python is moderately type-checked. Implicit&nbsp;<a title="Type conversion" href="https://en.wikipedia.org/wiki/Type_conversion">conversion</a>&nbsp;is defined for numeric types (as well as booleans), so one may validly multiply a complex number by an integer (for instance) without explicit casting. However, there is no implicit conversion between, for example, numbers and strings; a string is an invalid argument to a mathematical function expecting a number.</p>
<h3><span id="Base_types" class="mw-headline">Base types</span></h3>
<p>Python has a broad range of basic data types. Alongside conventional integer and&nbsp;<a class="mw-redirect" title="Floating-point" href="https://en.wikipedia.org/wiki/Floating-point">floating-point</a>&nbsp;arithmetic, it transparently supports&nbsp;<a title="Arbitrary-precision arithmetic" href="https://en.wikipedia.org/wiki/Arbitrary-precision_arithmetic">arbitrary-precision arithmetic</a>,&nbsp;<a title="Complex number" href="https://en.wikipedia.org/wiki/Complex_number">complex numbers</a>, and&nbsp;<a title="Decimal floating point" href="https://en.wikipedia.org/wiki/Decimal_floating_point">decimal floating point numbers</a>.</p>
<p>Python supports a wide variety of string operations. Strings in Python are&nbsp;<a title="Immutable object" href="https://en.wikipedia.org/wiki/Immutable_object">immutable</a>, so a string operation such as a substitution of characters, that in other programming languages might alter a string in place, returns a new string in Python. Performance considerations sometimes push for using special techniques in programs that modify strings intensively, such as joining character arrays into strings only as needed.</p>
<h3><span id="Collection_types" class="mw-headline">Collection types</span></h3>
<p>One of the very useful aspects of Python is the concept of&nbsp;<a title="Collection (abstract data type)" href="https://en.wikipedia.org/wiki/Collection_(abstract_data_type)"><em>collection</em>&nbsp;(or&nbsp;<em>container</em>) types</a>. In general a collection is an object that contains other objects in a way that is easily referenced or&nbsp;<em>indexed</em>. Collections come in two basic forms:&nbsp;<em>sequences</em>&nbsp;and&nbsp;<em>mappings</em>.</p>
<p>The ordered sequential types are lists (dynamic&nbsp;<a title="Array data type" href="https://en.wikipedia.org/wiki/Array_data_type">arrays</a>),&nbsp;<a title="Tuple" href="https://en.wikipedia.org/wiki/Tuple">tuples</a>, and strings. All sequences are indexed positionally (0 through&nbsp;<em>length</em>&nbsp;&minus; 1) and all but strings can contain any type of object, including multiple types in the same sequence. Both strings and tuples are immutable, making them perfect candidates for dictionary keys (see below). Lists, on the other hand, are mutable; elements can be inserted, deleted, modified, appended, or sorted&nbsp;<a title="In-place algorithm" href="https://en.wikipedia.org/wiki/In-place_algorithm">in-place</a>.</p>
<p>Mappings, on the other hand, are unordered types implemented in the form of&nbsp;<em>dictionaries</em>&nbsp;which "map" a set of&nbsp;<a title="Immutable object" href="https://en.wikipedia.org/wiki/Immutable_object">immutable</a>&nbsp;keys to corresponding elements (much like a mathematical function). For example, one could define a dictionary having a string&nbsp;<code>"toast"</code>&nbsp;mapped to the integer 42 or vice versa. The keys in a dictionary must be of an immutable Python type, such as an integer or a string, because under the hood they are implemented via a&nbsp;<a title="Hash function" href="https://en.wikipedia.org/wiki/Hash_function">hash function</a>. This makes for much faster lookup times, but requires keys not change (and also results in a dictionary's lack of order).</p>
<p>Dictionaries are also central to the internals of the language as they reside at the core of all Python objects and classes: the mappings between variable names (strings) and the values which the names reference are stored as dictionaries (see&nbsp;<a title="Python syntax and semantics" href="https://en.wikipedia.org/wiki/Python_syntax_and_semantics#Object_system">Object system</a>). Since these dictionaries are directly accessible (via an object's&nbsp;<code>__dict__</code>&nbsp;attribute),&nbsp;<a title="Metaprogramming" href="https://en.wikipedia.org/wiki/Metaprogramming">metaprogramming</a>&nbsp;is a straightforward and natural process in Python.</p>
<p>A&nbsp;<a class="mw-redirect" title="Set (computer science)" href="https://en.wikipedia.org/wiki/Set_(computer_science)">set</a>&nbsp;collection type was added to the core language in version 2.4. A set is an unindexed, unordered collection that contains no duplicates, and implements&nbsp;<a title="Naive set theory" href="https://en.wikipedia.org/wiki/Naive_set_theory">set theoretic</a>&nbsp;operations such as&nbsp;<a title="Union (set theory)" href="https://en.wikipedia.org/wiki/Union_(set_theory)">union</a>,&nbsp;<a title="Intersection (set theory)" href="https://en.wikipedia.org/wiki/Intersection_(set_theory)">intersection</a>,&nbsp;<a class="mw-redirect" title="Relative complement" href="https://en.wikipedia.org/wiki/Relative_complement">difference</a>,&nbsp;<a title="Symmetric difference" href="https://en.wikipedia.org/wiki/Symmetric_difference">symmetric difference</a>, and&nbsp;<a title="Subset" href="https://en.wikipedia.org/wiki/Subset">subset</a>&nbsp;testing. There are two types of sets:&nbsp;<code>set</code>&nbsp;and&nbsp;<code>frozenset</code>, the only difference being that&nbsp;<code>set</code>&nbsp;is mutable and&nbsp;<code>frozenset</code>&nbsp;is immutable. Elements in a set must be hashable. Thus, for example, a&nbsp;<code>frozenset</code>&nbsp;can be an element of a regular&nbsp;<code>set</code>&nbsp;whereas the opposite is not true.</p>
<p>Python also provides extensive collection manipulating abilities such as built in containment checking and a generic iteration protocol.</p>
<h3><span id="Object_system" class="mw-headline">Object system</span></h3>
<p>In Python, everything is an object, even classes. Classes, as objects, have a class, which is known as their&nbsp;<a title="Metaclass" href="https://en.wikipedia.org/wiki/Metaclass">metaclass</a>. Python also supports&nbsp;<a title="Multiple inheritance" href="https://en.wikipedia.org/wiki/Multiple_inheritance">multiple inheritance</a>&nbsp;and&nbsp;<a title="Mixin" href="https://en.wikipedia.org/wiki/Mixin">mixins</a>.</p>
<p>The language supports extensive&nbsp;<a class="mw-redirect" title="Introspection (computer science)" href="https://en.wikipedia.org/wiki/Introspection_(computer_science)">introspection</a>&nbsp;of types and classes. Types can be read and compared&mdash;types are instances of&nbsp;<code>type</code>. The attributes of an object can be extracted as a dictionary.</p>
<p>Operators can be overloaded in Python by defining special member functions - for instance, defining&nbsp;<code>__add__</code>&nbsp;on a class permits one to use the&nbsp;<code>+</code>&nbsp;operator on members of that class.</p>
<h2><span id="Literals" class="mw-headline">Literals</span></h2>
<h3><span id="Strings" class="mw-headline">Strings</span></h3>
<p>Python has various kinds of&nbsp;<a title="String literal" href="https://en.wikipedia.org/wiki/String_literal">string literals</a>.</p>
<h4><span id="Normal_string_literals" class="mw-headline">Normal string literals</span></h4>
<p>Either single or double quotes can be used to quote strings. Unlike in Unix shell languages,&nbsp;<a title="Perl" href="https://en.wikipedia.org/wiki/Perl">Perl</a>&nbsp;or Perl-influenced languages such as&nbsp;<a title="Ruby (programming language)" href="https://en.wikipedia.org/wiki/Ruby_(programming_language)">Ruby</a>&nbsp;or&nbsp;<a class="mw-redirect" title="Groovy (programming language)" href="https://en.wikipedia.org/wiki/Groovy_(programming_language)">Groovy</a>, single quotes and double quotes function identically, i.e. there is no string interpolation of&nbsp;<em>$foo</em>&nbsp;expressions. However, interpolation can be done in various ways: with "f-strings" (since Python 3.6), using the&nbsp;<code>format</code>&nbsp;method or the old&nbsp;<em>%</em>&nbsp;string-format operator.</p>
<p>For instance, the Perl statement:</p>
<div class="mw-highlight mw-highlight-lang-perl mw-content-ltr" dir="ltr">
<pre><span class="k">print</span> <span class="s">"I just printed $num pages to the printer $printer\n"</span>
</pre>
</div>
<p>is equivalent to any of these Python statements:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">"I just printed </span><span class="si">{num}</span><span class="s2"> pages to the printer </span><span class="si">{printer}</span><span class="s2">"</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">"I just printed </span><span class="si">{}</span><span class="s2"> pages to the printer </span><span class="si">{}</span><span class="s2">"</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">num</span><span class="p">,</span> <span class="n">printer</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"I just printed </span><span class="si">{0}</span><span class="s2"> pages to the printer </span><span class="si">{1}</span><span class="s2">"</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">num</span><span class="p">,</span> <span class="n">printer</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"I just printed </span><span class="si">{num}</span><span class="s2"> pages to the printer </span><span class="si">{printer}</span><span class="s2">"</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">num</span><span class="o">=</span><span class="n">num</span><span class="p">,</span> <span class="n">printer</span><span class="o">=</span><span class="n">printer</span><span class="p">))</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">"I just printed </span><span class="si">%s</span><span class="s2"> pages to the printer </span><span class="si">%s</span><span class="s2">"</span> <span class="o">%</span> <span class="p">(</span><span class="n">num</span><span class="p">,</span> <span class="n">printer</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"I just printed </span><span class="si">%(num)s</span><span class="s2"> pages to the printer </span><span class="si">%(printer)s</span><span class="s2">"</span> <span class="o">%</span> <span class="p">{</span><span class="s2">"num"</span><span class="p">:</span> <span class="n">num</span><span class="p">,</span> <span class="s2">"printer"</span><span class="p">:</span> <span class="n">printer</span><span class="p">})</span>
</pre>
</div>
<h4><span id="Multi-line_string_literals" class="mw-headline">Multi-line string literals</span></h4>
<p>There are also multi-line strings, which begin and end with a series of three single or double quotes and function like&nbsp;<a title="Here document" href="https://en.wikipedia.org/wiki/Here_document">here documents</a>&nbsp;in&nbsp;<a title="Perl" href="https://en.wikipedia.org/wiki/Perl">Perl</a>&nbsp;and&nbsp;<a title="Ruby (programming language)" href="https://en.wikipedia.org/wiki/Ruby_(programming_language)">Ruby</a>.</p>
<p>A simple example with&nbsp;<a title="String interpolation" href="https://en.wikipedia.org/wiki/String_interpolation">variable interpolation</a>&nbsp;(using the&nbsp;<code>format</code>&nbsp;method) is:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="nb">print</span><span class="p">(</span><span class="s2">"""Dear </span><span class="si">{recipient}</span><span class="s2">,</span>

<span class="s2">I wish you to leave Sunnydale and never return.</span>

<span class="s2">Not Quite Love,</span>
<span class="si">{sender}</span>
<span class="s2">"""</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">sender</span><span class="o">=</span><span class="s2">"Buffy the Vampire Slayer"</span><span class="p">,</span> <span class="n">recipient</span><span class="o">=</span><span class="s2">"Spike"</span><span class="p">))</span>
</pre>
</div>
<h4><span id="Raw_strings" class="mw-headline">Raw strings</span></h4>
<p>Finally, all of the previously mentioned string types come in "<a class="mw-redirect" title="Raw string" href="https://en.wikipedia.org/wiki/Raw_string">raw</a>" varieties (denoted by placing a literal&nbsp;<em>r</em>&nbsp;before the opening quote), which do no backslash-interpolation and hence are very useful for&nbsp;<a title="Regular expression" href="https://en.wikipedia.org/wiki/Regular_expression">regular expressions</a>; compare&nbsp;<a title="C Sharp syntax" href="https://en.wikipedia.org/wiki/C_Sharp_syntax#Literals">"@-quoting"</a>&nbsp;in&nbsp;<a title="C Sharp (programming language)" href="https://en.wikipedia.org/wiki/C_Sharp_(programming_language)">C#</a>. Raw strings were originally included specifically for regular expressions. Due to limitations of the tokenizer, raw strings may not have a trailing backslash.&nbsp;Creating a raw string holding a&nbsp;<a class="mw-redirect" title="Windows" href="https://en.wikipedia.org/wiki/Windows">Windows</a>&nbsp;path ending with a backslash requires some variety of workaround (commonly, using forward slashes instead of backslashes, since Windows accepts both).</p>
<p>Examples include:</p>
<div class="mw-highlight mw-highlight-lang-pycon mw-content-ltr" dir="ltr">
<pre><span class="gp">&gt;&gt;&gt; </span><span class="c1"># A Windows path, even raw strings cannot end in a backslash</span>
<span class="gp">&gt;&gt;&gt; </span><span class="sa">r</span><span class="s2">"C:\Foo\Bar\Baz</span><span class="se">\"</span>
  File <span class="nb">"&lt;stdin&gt;"</span>, line <span class="m">1</span>
    <span class="sa">r</span><span class="s2">"C:\Foo\Bar\Baz</span><span class="se">\"</span>
                     <span class="o">^</span>
<span class="gr">SyntaxError</span>: <span class="n">EOL while scanning string literal</span>

<span class="gp">&gt;&gt;&gt; </span><span class="n">dos_path</span> <span class="o">=</span> <span class="sa">r</span><span class="s2">"C:\Foo\Bar\Baz\ "</span> <span class="c1"># avoids the error by adding</span>
<span class="gp">&gt;&gt;&gt; </span><span class="n">dos_path</span><span class="o">.</span><span class="n">rstrip</span><span class="p">()</span>              <span class="c1"># and removing trailing space</span>
<span class="go">'C:\\Foo\\Bar\\Baz\\'</span>

<span class="gp">&gt;&gt;&gt; </span><span class="n">quoted_dos_path</span> <span class="o">=</span> <span class="sa">r</span><span class="s1">'"</span><span class="si">{}</span><span class="s1">"'</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">dos_path</span><span class="p">)</span>
<span class="gp">&gt;&gt;&gt; </span><span class="n">quoted_dos_path</span>
<span class="go">'"C:\\Foo\\Bar\\Baz\\ "'</span>

<span class="gp">&gt;&gt;&gt; </span><span class="c1"># A regular expression matching a quoted string with possible backslash quoting</span>
<span class="gp">&gt;&gt;&gt; </span><span class="n">re</span><span class="o">.</span><span class="n">match</span><span class="p">(</span><span class="sa">r</span><span class="s1">'"(([^"</span><span class="se">\\</span><span class="s1">]|</span><span class="se">\\</span><span class="s1">.)*)"'</span><span class="p">,</span> <span class="n">quoted_dos_path</span><span class="p">)</span><span class="o">.</span><span class="n">group</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span><span class="o">.</span><span class="n">rstrip</span><span class="p">()</span>
<span class="go">'C:\\Foo\\Bar\\Baz\\'</span>

<span class="gp">&gt;&gt;&gt; </span><span class="n">code</span> <span class="o">=</span> <span class="s1">'foo(2, bar)'</span>
<span class="gp">&gt;&gt;&gt; </span><span class="c1"># Reverse the arguments in a two-arg function call</span>
<span class="gp">&gt;&gt;&gt; </span><span class="n">re</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="sa">r</span><span class="s1">'\(([^,]*?),([^ ,]*?)\)'</span><span class="p">,</span> <span class="sa">r</span><span class="s1">'(\2, \1)'</span><span class="p">,</span> <span class="n">code</span><span class="p">)</span>
<span class="go">'foo(2, bar)'</span>
<span class="gp">&gt;&gt;&gt; </span><span class="c1"># Note that this won't work if either argument has parens or commas in it.</span>
</pre>
</div>
<h4><span id="Concatenation_of_adjacent_string_literals" class="mw-headline">Concatenation of adjacent string literals</span></h4>
<p>String literals (using possibly different quote conventions) appearing contiguously and only separated by whitespace (including new lines), are allowed and are aggregated into a single longer string.&nbsp;Thus</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">title</span> <span class="o">=</span> <span class="s2">"One Good Turn: "</span> \
        <span class="s1">'A Natural History of the Screwdriver and the Screw'</span>
</pre>
</div>
<p>is equivalent to</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">title</span> <span class="o">=</span> <span class="s2">"One Good Turn: A Natural History of the Screwdriver and the Screw"</span>
</pre>
</div>
<h3><span id="Numbers" class="mw-headline">Numbers</span></h3>
<p>Numeric literals in Python are of the normal sort, e.g.&nbsp;<code>0</code>,&nbsp;<code>-1</code>,&nbsp;<code>3.4</code>,&nbsp;<code>3.5e-8</code>.</p>
<p>Python has arbitrary-length integers and automatically increases the storage size as necessary. Prior to Python version 3, there were two kinds of integral numbers: traditional fixed size integers and "long" integers of arbitrary range. The conversion to "long" integers was performed automatically when required, and thus the programmer usually didn't have to be aware of the two integral types. In newer language versions the fixed-size integers are completely gone.</p>
<p>Python supports normal&nbsp;<a class="mw-redirect" title="IEEE 754-2008" href="https://en.wikipedia.org/wiki/IEEE_754-2008">floating point</a>&nbsp;numbers, which are created when a dot is used in a literal (e.g.&nbsp;<code>1.1</code>), when an integer and a floating point number are used in an expression, or as a result of some mathematical operations ("true division" via the&nbsp;<code>/</code>&nbsp;operator, or exponentiation with a negative exponent).</p>
<p>Python also supports&nbsp;<a title="Complex number" href="https://en.wikipedia.org/wiki/Complex_number">complex numbers</a>&nbsp;natively. Complex numbers are indicated with the&nbsp;<code>J</code>&nbsp;or&nbsp;<code>j</code>&nbsp;suffix, e.g.&nbsp;<code>3 + 4j</code>.</p>
<h3><span id="Lists.2C_tuples.2C_sets.2C_dictionaries"></span><span id="Lists,_tuples,_sets,_dictionaries" class="mw-headline">Lists, tuples, sets, dictionaries</span></h3>
<p>Python has syntactic support for the creation of container types.</p>
<p><strong>Lists</strong>&nbsp;(class&nbsp;<code>list</code>) are mutable sequences of items of arbitrary types, and can be created either with the special syntax</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">a_list</span> <span class="o">=</span> <span class="p">[</span><span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="s2">"a dog"</span><span class="p">]</span>
</pre>
</div>
<p>or using normal object creation</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">a_second_list</span> <span class="o">=</span> <span class="nb">list</span><span class="p">()</span>
<span class="n">a_second_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="mi">4</span><span class="p">)</span>
<span class="n">a_second_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="mi">5</span><span class="p">)</span>
</pre>
</div>
<p><strong>Tuples</strong>&nbsp;(class&nbsp;<code>tuple</code>) are immutable sequences of items of arbitrary types. There is also a special syntax to create tuples</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">a_tuple</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="s2">"four"</span>
</pre>
</div>
<p>Although tuples are created by separating items with commas, the whole construct is usually wrapped in parentheses to increase readability. An empty tuple is denoted by&nbsp;<code>()</code>.</p>
<p><strong>Sets</strong>&nbsp;(class&nbsp;<code>set</code>) are mutable containers of hashable items&nbsp;of arbitrary types, with no duplicates. The items are not ordered, but sets support iteration over the items. A syntax for set creation appeared in Python 2.7/3.0</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">some_set</span> <span class="o">=</span> <span class="p">{</span><span class="mi">0</span><span class="p">,</span> <span class="p">(),</span> <span class="kc">False</span><span class="p">}</span>
</pre>
</div>
<p>In earlier Python versions, sets would be created by initializing the set class with a list argument. Python sets are very much like&nbsp;<a title="Set (mathematics)" href="https://en.wikipedia.org/wiki/Set_(mathematics)">mathematical sets</a>, and support operations like set&nbsp;<a title="Set (mathematics)" href="https://en.wikipedia.org/wiki/Set_(mathematics)#Intersections">intersection</a>&nbsp;and&nbsp;<a title="Set (mathematics)" href="https://en.wikipedia.org/wiki/Set_(mathematics)#Unions">union</a>.</p>
<p>Python also features a&nbsp;<code>frozenset</code>&nbsp;class for immutable sets.</p>
<p><strong>Dictionaries</strong>&nbsp;(class&nbsp;<code>dict</code>) are mutable mappings tying keys and corresponding values. Python has special syntax to create dictionaries (<code>{key: value}</code>)</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">a_dictionary</span> <span class="o">=</span> <span class="p">{</span><span class="s2">"key 1"</span><span class="p">:</span> <span class="s2">"value 1"</span><span class="p">,</span> <span class="mi">2</span><span class="p">:</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">4</span><span class="p">:</span> <span class="p">[]}</span>
</pre>
</div>
<p>The dictionary syntax is similar to the set syntax, the difference is the presence of colons. The empty literal&nbsp;<code>{}</code>&nbsp;results in an empty dictionary rather than an empty set, which is instead created using the non-literal constructor:&nbsp;<code>set()</code>.</p>
<h2><span id="Operators" class="mw-headline">Operators</span></h2>
<h3><span id="Arithmetic" class="mw-headline">Arithmetic</span></h3>
<p>Python includes the&nbsp;<code>+</code>,&nbsp;<code>-</code>,&nbsp;<code>*</code>,&nbsp;<code>/</code>,&nbsp;<code>%</code>&nbsp;(<a class="mw-redirect" title="Modulo operator" href="https://en.wikipedia.org/wiki/Modulo_operator">modulus</a>), and&nbsp;<code>**</code>&nbsp;(<a title="Exponentiation" href="https://en.wikipedia.org/wiki/Exponentiation">exponentiation</a>) operators, with their usual&nbsp;<a title="Order of operations" href="https://en.wikipedia.org/wiki/Order_of_operations">mathematical precedence</a>.</p>
<p>Traditionally,&nbsp;<code>x / y</code>&nbsp;performed&nbsp;<a class="mw-redirect" title="Integer division" href="https://en.wikipedia.org/wiki/Integer_division">integer division</a>&nbsp;if both&nbsp;<code>x</code>&nbsp;and&nbsp;<code>y</code>&nbsp;were integers (returning the floor of the quotient), and returned a float if either was a float. However, because Python is a dynamically typed language, it was not always possible to tell which operation was being performed, which often led to subtle bugs. For example, with</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">mean</span><span class="p">(</span><span class="n">seq</span><span class="p">):</span>
    <span class="k">return</span> <span class="nb">sum</span><span class="p">(</span><span class="n">seq</span><span class="p">)</span> <span class="o">/</span> <span class="nb">len</span><span class="p">(</span><span class="n">seq</span><span class="p">)</span>
</pre>
</div>
<p>A call to&nbsp;<code>mean([3.0, 4.0])</code>&nbsp;would return 3.5, but&nbsp;<code>mean([3, 4])</code>&nbsp;would return 3. If this was not the intended behavior, it was necessary to use a workaround such as</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">mean</span><span class="p">(</span><span class="n">seq</span><span class="p">):</span>
    <span class="k">return</span> <span class="nb">float</span><span class="p">(</span><span class="nb">sum</span><span class="p">(</span><span class="n">seq</span><span class="p">))</span> <span class="o">/</span> <span class="nb">len</span><span class="p">(</span><span class="n">seq</span><span class="p">)</span>
</pre>
</div>
<p>To avoid this issue,&nbsp;<a class="external text" href="https://www.python.org/dev/peps/pep-0238/" rel="nofollow">a proposal</a>&nbsp;was made to change the behavior of the Python division operator. In Python 2.2, a new operator&nbsp;<code>//</code>&nbsp;was introduced for floor division, both for integer and floating-point arguments. The&nbsp;<code>/</code>&nbsp;operator was changed so that the quotient of two integers returned a float, but for backwards compatibility, this behavior had to be explicitly requested until Python 3.0.</p>
<h3><span id="Comparison_operators" class="mw-headline">Comparison operators</span></h3>
<p>The basic comparison operators such as&nbsp;<code>==</code>,&nbsp;<code>&lt;</code>,&nbsp;<code>&gt;=</code>, and so forth are used on all manner of values. Numbers, strings, sequences, and mappings can all be compared. Although disparate types (such as a&nbsp;<code>str</code>&nbsp;and an&nbsp;<code>int</code>) are defined to have a consistent relative ordering, this is considered a historical design quirk and will no longer be allowed in Python 3.0.</p>
<p>Chained comparison expressions such as&nbsp;<code>a &lt; b &lt; c</code>&nbsp;have roughly the meaning that they have in mathematics, rather than the unusual meaning found in&nbsp;<a title="C (programming language)" href="https://en.wikipedia.org/wiki/C_(programming_language)">C</a>&nbsp;and similar languages. The terms are evaluated and compared in order. The operation has&nbsp;<a class="mw-redirect" title="Minimal evaluation" href="https://en.wikipedia.org/wiki/Minimal_evaluation">short-circuit semantics</a>, meaning that evaluation is guaranteed to stop as soon as a verdict is clear: if&nbsp;<code>a &lt; b</code>&nbsp;is false,&nbsp;<code>c</code>&nbsp;is never evaluated as the expression cannot possibly be true anymore.</p>
<p>For expressions without side effects,&nbsp;<code>a &lt; b &lt; c</code>&nbsp;is equivalent to&nbsp;<code>a &lt; b and b &lt; c</code>. However, there is a substantial difference when the expressions have side effects.&nbsp;<code>a &lt; f(x) &lt; b</code>&nbsp;will evaluate&nbsp;<code>f(x)</code>&nbsp;exactly once, whereas&nbsp;<code>a &lt; f(x) and f(x) &lt; b</code>&nbsp;will evaluate it twice if the value of&nbsp;<code>a</code>&nbsp;is less than&nbsp;<code>f(x)</code>&nbsp;and once otherwise.</p>
<h3><span id="Logical_operators" class="mw-headline">Logical operators</span></h3>
<p>Python 2.2 and earlier does not have an explicit boolean type. In all versions of Python, boolean operators treat zero values or empty values such as&nbsp;<code>""</code>,&nbsp;<code>0</code>,&nbsp;<code>None</code>,&nbsp;<code>0.0</code>,&nbsp;<code>[]</code>, and&nbsp;<code>{}</code>&nbsp;as false, while in general treating non-empty, non-zero values as true. In Python 2.2.1 the boolean constants&nbsp;<code>True</code>&nbsp;and&nbsp;<code>False</code>&nbsp;were added to the language (subclassed from 1 and 0). The binary comparison operators such as&nbsp;<code>==</code>&nbsp;and&nbsp;<code>&gt;</code>&nbsp;return either&nbsp;<code>True</code>&nbsp;or&nbsp;<code>False</code>.</p>
<p>The boolean operators&nbsp;<code>and</code>&nbsp;and&nbsp;<code>or</code>&nbsp;use&nbsp;<a class="mw-redirect" title="Minimal evaluation" href="https://en.wikipedia.org/wiki/Minimal_evaluation">minimal evaluation</a>. For example,&nbsp;<code>y == 0 or x/y &gt; 100</code>&nbsp;will never raise a divide-by-zero exception. These operators return the value of the last operand evaluated, rather than&nbsp;<code>True</code>&nbsp;or&nbsp;<code>False</code>. Thus the expression&nbsp;<code>(4 and 5)</code>&nbsp;evaluates to&nbsp;<code>5</code>, and&nbsp;<code>(4 or 5)</code>&nbsp;evaluates to&nbsp;<code>4</code>.</p>
<h2><span id="Functional_programming" class="mw-headline">Functional programming</span></h2>
<p>As mentioned above, another strength of Python is the availability of a&nbsp;<a title="Functional programming" href="https://en.wikipedia.org/wiki/Functional_programming">functional programming</a>&nbsp;style. As may be expected, this makes working with lists and other collections much more straightforward.</p>
<h3><span id="Comprehensions" class="mw-headline">Comprehensions</span></h3>
<div class="hatnote navigation-not-searchable">Main article:&nbsp;<a title="List comprehension" href="https://en.wikipedia.org/wiki/List_comprehension">List comprehension</a></div>
<p>One such construction is the&nbsp;<a title="List comprehension" href="https://en.wikipedia.org/wiki/List_comprehension">list comprehension</a>, which can be expressed with the following format:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">L</span> <span class="o">=</span> <span class="p">[</span><span class="n">mapping_expression</span> <span class="k">for</span> <span class="n">element</span> <span class="ow">in</span> <span class="n">source_list</span> <span class="k">if</span> <span class="n">filter_expression</span><span class="p">]</span>
</pre>
</div>
<p>Using list comprehension to calculate the first five powers of two:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">powers_of_two</span> <span class="o">=</span> <span class="p">[</span><span class="mi">2</span><span class="o">**</span><span class="n">n</span> <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">6</span><span class="p">)]</span>
</pre>
</div>
<p>The&nbsp;<a title="Quicksort" href="https://en.wikipedia.org/wiki/Quicksort">Quicksort</a>&nbsp;algorithm can be expressed elegantly (albeit inefficiently) using list comprehensions:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">qsort</span><span class="p">(</span><span class="n">L</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">L</span> <span class="o">==</span> <span class="p">[]:</span>
        <span class="k">return</span> <span class="p">[]</span>
    <span class="n">pivot</span> <span class="o">=</span> <span class="n">L</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
    <span class="k">return</span> <span class="p">(</span><span class="n">qsort</span><span class="p">([</span><span class="n">x</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">L</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">x</span> <span class="o">&lt;</span> <span class="n">pivot</span><span class="p">])</span> <span class="o">+</span>
            <span class="p">[</span><span class="n">pivot</span><span class="p">]</span> <span class="o">+</span>
            <span class="n">qsort</span><span class="p">([</span><span class="n">x</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">L</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">x</span> <span class="o">&gt;=</span> <span class="n">pivot</span><span class="p">]))</span>
</pre>
</div>
<p>Python 2.7+<sup id="cite_ref-12" class="reference"><a href="https://en.wikipedia.org/wiki/Python_syntax_and_semantics#cite_note-12">[10]</a></sup>&nbsp;also supports set comprehensions&nbsp;and dictionary comprehensions.</p>
<h3><span id="First-class_functions" class="mw-headline">First-class functions</span></h3>
<p>In Python, functions are&nbsp;<a title="First-class function" href="https://en.wikipedia.org/wiki/First-class_function">first-class</a>&nbsp;objects that can be created and passed around dynamically.</p>
<p>Python's limited support for&nbsp;<a title="Anonymous function" href="https://en.wikipedia.org/wiki/Anonymous_function">anonymous functions</a>&nbsp;is the&nbsp;<code>lambda</code>&nbsp;construct. An example is the anonymous function which squares its input, called with the argument of 5:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">f</span> <span class="o">=</span> <span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="o">**</span><span class="mi">2</span>
<span class="n">f</span><span class="p">(</span><span class="mi">5</span><span class="p">)</span>
</pre>
</div>
<p>Lambdas are limited to containing an&nbsp;<a class="mw-redirect" title="Expression (programming)" href="https://en.wikipedia.org/wiki/Expression_(programming)">expression</a>&nbsp;rather than&nbsp;<a class="mw-redirect" title="Statement (programming)" href="https://en.wikipedia.org/wiki/Statement_(programming)">statements</a>, although control flow can still be implemented less elegantly within lambda by using short-circuiting,&nbsp;and more idiomatically with conditional expressions.</p>
<h3><span id="Closures" class="mw-headline">Closures</span></h3>
<p>Python has had support for&nbsp;<a class="mw-redirect" title="Closure (computer science)" href="https://en.wikipedia.org/wiki/Closure_(computer_science)">lexical closures</a>&nbsp;since version 2.2. Here's an example:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">derivative</span><span class="p">(</span><span class="n">f</span><span class="p">,</span> <span class="n">dx</span><span class="p">):</span>
    <span class="sd">"""Return a function that approximates the derivative of f</span>
<span class="sd">    using an interval of dx, which should be appropriately small.</span>
<span class="sd">    """</span>
    <span class="k">def</span> <span class="nf">function</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
        <span class="k">return</span> <span class="p">(</span><span class="n">f</span><span class="p">(</span><span class="n">x</span> <span class="o">+</span> <span class="n">dx</span><span class="p">)</span> <span class="o">-</span> <span class="n">f</span><span class="p">(</span><span class="n">x</span><span class="p">))</span> <span class="o">/</span> <span class="n">dx</span>
    <span class="k">return</span> <span class="n">function</span>
</pre>
</div>
<p>Python's syntax, though, sometimes leads programmers of other languages to think that closures are not supported. Variable scope in Python is implicitly determined by the scope in which one assigns a value to the variable, unless scope is explicitly declared with&nbsp;<code>global</code>&nbsp;or&nbsp;<code>nonlocal</code>.</p>
<p>Note that the closure's binding of a name to some value is not mutable from within the function. Given:</p>
<div class="mw-highlight mw-highlight-lang-pycon mw-content-ltr" dir="ltr">
<pre><span class="gp">&gt;&gt;&gt; </span><span class="k">def</span> <span class="nf">foo</span><span class="p">(</span><span class="n">a</span><span class="p">,</span> <span class="n">b</span><span class="p">):</span>
<span class="gp">... </span>    <span class="nb">print</span><span class="p">(</span><span class="s1">'a: </span><span class="si">%r</span><span class="s1">'</span> <span class="o">%</span> <span class="n">a</span><span class="p">)</span>
<span class="gp">... </span>    <span class="nb">print</span><span class="p">(</span><span class="s1">'b: </span><span class="si">%r</span><span class="s1">'</span> <span class="o">%</span> <span class="n">b</span><span class="p">)</span>
<span class="gp">... </span>    <span class="k">def</span> <span class="nf">bar</span><span class="p">(</span><span class="n">c</span><span class="p">):</span>
<span class="gp">... </span>        <span class="n">b</span> <span class="o">=</span> <span class="n">c</span>
<span class="gp">... </span>        <span class="nb">print</span><span class="p">(</span><span class="s1">'b*: </span><span class="si">%r</span><span class="s1">'</span> <span class="o">%</span> <span class="n">b</span><span class="p">)</span>
<span class="gp">... </span>    <span class="n">bar</span><span class="p">(</span><span class="n">a</span><span class="p">)</span>
<span class="gp">... </span>    <span class="nb">print</span><span class="p">(</span><span class="s1">'b: </span><span class="si">%r</span><span class="s1">'</span> <span class="o">%</span> <span class="n">b</span><span class="p">)</span>

<span class="gp">&gt;&gt;&gt; </span><span class="n">foo</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">)</span>
<span class="go">a: 1</span>
<span class="go">b: 2</span>
<span class="go">b*: 1</span>
<span class="go">b: 2</span>
</pre>
</div>
<p>and you can see that&nbsp;<code>b</code>, as visible from the closure's scope, retains the value it had; the changed binding of&nbsp;<code>b</code>&nbsp;inside the inner function did not propagate out. The way around this is to use a&nbsp;<code>nonlocal b</code>&nbsp;statement in&nbsp;<code>bar</code>. In Python 2 (which lacks&nbsp;<code>nonlocal</code>), the usual workaround is to use mutable value and change that value, not the binding. E.g., a list with one element.</p>
<h3><span id="Generators" class="mw-headline">Generators</span></h3>
<p>Introduced in Python 2.2 as an optional feature and finalized in version 2.3,&nbsp;<a class="mw-redirect" title="Generator (computer science)" href="https://en.wikipedia.org/wiki/Generator_(computer_science)">generators</a>&nbsp;are Python's mechanism for&nbsp;<a title="Lazy evaluation" href="https://en.wikipedia.org/wiki/Lazy_evaluation">lazy evaluation</a>&nbsp;of a function that would otherwise return a space-prohibitive or computationally intensive list.</p>
<p>This is an example to lazily generate the prime numbers:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="kn">from</span> <span class="nn">itertools</span> <span class="kn">import</span> <span class="n">count</span>

<span class="k">def</span> <span class="nf">generate_primes</span><span class="p">(</span><span class="n">stop_at</span><span class="o">=</span><span class="mi">0</span><span class="p">):</span>
    <span class="n">primes</span> <span class="o">=</span> <span class="p">[]</span>
    <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="n">count</span><span class="p">(</span><span class="mi">2</span><span class="p">):</span>
        <span class="k">if</span> <span class="mi">0</span> <span class="o">&lt;</span> <span class="n">stop_at</span> <span class="o">&lt;</span> <span class="n">n</span><span class="p">:</span>
            <span class="k">return</span> <span class="c1"># raises the StopIteration exception</span>
        <span class="n">composite</span> <span class="o">=</span> <span class="kc">False</span>
        <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">primes</span><span class="p">:</span>
            <span class="k">if</span> <span class="ow">not</span> <span class="n">n</span> <span class="o">%</span> <span class="n">p</span><span class="p">:</span>
                <span class="n">composite</span> <span class="o">=</span> <span class="kc">True</span>
                <span class="k">break</span>
            <span class="k">elif</span> <span class="n">p</span> <span class="o">**</span> <span class="mi">2</span> <span class="o">&gt;</span> <span class="n">n</span><span class="p">:</span>
                <span class="k">break</span>
        <span class="k">if</span> <span class="ow">not</span> <span class="n">composite</span><span class="p">:</span>
            <span class="n">primes</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">n</span><span class="p">)</span>
            <span class="k">yield</span> <span class="n">n</span>
</pre>
</div>
<p>To use this function simply call, e.g.:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">generate_primes</span><span class="p">():</span>  <span class="c1"># iterate over ALL primes</span>
    <span class="k">if</span> <span class="n">i</span> <span class="o">&gt;</span> <span class="mi">100</span><span class="p">:</span>
        <span class="k">break</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
</pre>
</div>
<p>The definition of a generator appears identical to that of a function, except the keyword&nbsp;<code>yield</code>&nbsp;is used in place of&nbsp;<code>return</code>. However, a generator is an object with persistent state, which can repeatedly enter and leave the same scope. A generator call can then be used in place of a list, or other structure whose elements will be iterated over. Whenever the&nbsp;<code>for</code>&nbsp;loop in the example requires the next item, the generator is called, and yields the next item.</p>
<p>Generators don't have to be infinite like the prime-number example above. When a generator terminates, an internal exception is raised which indicates to any calling context that there are no more values. A&nbsp;<code>for</code>&nbsp;loop or other iteration will then terminate.</p>
<h3><span id="Generator_expressions" class="mw-headline">Generator expressions</span></h3>
<div class="hatnote navigation-not-searchable">Further information:&nbsp;<a title="List comprehension" href="https://en.wikipedia.org/wiki/List_comprehension">List comprehension</a></div>
<p>Introduced in Python 2.4, generator expressions are the lazy evaluation equivalent of list comprehensions. Using the prime number generator provided in the above section, we might define a lazy, but not quite infinite collection.</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="kn">from</span> <span class="nn">itertools</span> <span class="kn">import</span> <span class="n">islice</span>

<span class="n">primes_under_million</span> <span class="o">=</span> <span class="p">(</span><span class="n">i</span> <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">generate_primes</span><span class="p">()</span> <span class="k">if</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="mi">1000000</span><span class="p">)</span>
<span class="n">two_thousandth_prime</span> <span class="o">=</span> <span class="n">islice</span><span class="p">(</span><span class="n">primes_under_million</span><span class="p">,</span> <span class="mi">1999</span><span class="p">,</span> <span class="mi">2000</span><span class="p">)</span><span class="o">.</span><span class="n">next</span><span class="p">()</span>
</pre>
</div>
<p>Most of the memory and time needed to generate this many primes will not be used until the needed element is actually accessed. Unfortunately, you cannot perform simple indexing and slicing of generators, but must use the&nbsp;<em>itertools</em>&nbsp;modules or "roll your own" loops. In contrast, a list comprehension is functionally equivalent, but is&nbsp;<em>greedy</em>&nbsp;in performing all the work:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="n">primes_under_million</span> <span class="o">=</span> <span class="p">[</span><span class="n">i</span> <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">generate_primes</span><span class="p">(</span><span class="mi">2000000</span><span class="p">)</span> <span class="k">if</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="mi">1000000</span><span class="p">]</span>
<span class="n">two_thousandth_prime</span> <span class="o">=</span> <span class="n">primes_under_million</span><span class="p">[</span><span class="mi">1999</span><span class="p">]</span>
</pre>
</div>
<p>The list comprehension will immediately create a large list (with 78498 items, in the example, but transiently creating a list of primes under two million), even if most elements are never accessed. The generator comprehension is more parsimonious.</p>
<h3><span id="Dictionary_and_set_comprehensions" class="mw-headline">Dictionary and set comprehensions</span></h3>
<p>While lists and generators had comprehensions/expressions, in Python versions older than 2.7 the other Python built-in collection types (dicts and sets) had to be kludged in using lists or generators:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="o">&gt;&gt;&gt;</span> <span class="nb">dict</span><span class="p">((</span><span class="n">n</span><span class="p">,</span> <span class="n">n</span><span class="o">*</span><span class="n">n</span><span class="p">)</span> <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">5</span><span class="p">))</span>
<span class="p">{</span><span class="mi">0</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">:</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">:</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">3</span><span class="p">:</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">4</span><span class="p">:</span> <span class="mi">16</span><span class="p">}</span>
</pre>
</div>
<p>Python 2.7 and 3.0 unify all collection types by introducing dict and set comprehensions, similar to list comprehensions:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="o">&gt;&gt;&gt;</span> <span class="p">[</span><span class="n">n</span><span class="o">*</span><span class="n">n</span> <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">5</span><span class="p">)]</span>  <span class="c1"># regular list comprehension</span>
<span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">16</span><span class="p">]</span>
<span class="o">&gt;&gt;&gt;</span>
<span class="o">&gt;&gt;&gt;</span> <span class="p">{</span><span class="n">n</span><span class="o">*</span><span class="n">n</span> <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">5</span><span class="p">)}</span>  <span class="c1"># set comprehension</span>
<span class="p">{</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">16</span><span class="p">}</span>
<span class="o">&gt;&gt;&gt;</span>
<span class="o">&gt;&gt;&gt;</span> <span class="p">{</span><span class="n">n</span><span class="p">:</span> <span class="n">n</span><span class="o">*</span><span class="n">n</span> <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">5</span><span class="p">)}</span>  <span class="c1"># dict comprehension</span>
<span class="p">{</span><span class="mi">0</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">:</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">:</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">3</span><span class="p">:</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">4</span><span class="p">:</span> <span class="mi">16</span><span class="p">}</span>
</pre>
</div>
<h2><span id="Objects" class="mw-headline">Objects</span></h2>
<p>Python supports most object oriented programming techniques. It allows&nbsp;<a title="Polymorphism (computer science)" href="https://en.wikipedia.org/wiki/Polymorphism_(computer_science)">polymorphism</a>, not only within a&nbsp;<a title="Class hierarchy" href="https://en.wikipedia.org/wiki/Class_hierarchy">class hierarchy</a>&nbsp;but also by&nbsp;<a title="Duck typing" href="https://en.wikipedia.org/wiki/Duck_typing">duck typing</a>. Any object can be used for any type, and it will work so long as it has the proper methods and attributes. And everything in Python is an object, including classes, functions, numbers and modules. Python also has support for&nbsp;<a title="Metaclass" href="https://en.wikipedia.org/wiki/Metaclass">metaclasses</a>, an advanced tool for enhancing classes' functionality. Naturally,&nbsp;<a class="mw-redirect" title="Inheritance (computer science)" href="https://en.wikipedia.org/wiki/Inheritance_(computer_science)">inheritance</a>, including&nbsp;<a title="Multiple inheritance" href="https://en.wikipedia.org/wiki/Multiple_inheritance">multiple inheritance</a>, is supported. It has limited support for private variables using&nbsp;<a title="Name mangling" href="https://en.wikipedia.org/wiki/Name_mangling#Python">name mangling.</a>&nbsp;See&nbsp;<a class="external text" href="https://docs.python.org/2/tutorial/classes.html" rel="nofollow">the "Classes" section of the tutorial</a>&nbsp;for details. Many Python users don't feel the need for private variables, though. The slogan "We're all responsible users here" is used to describe this attitude.&nbsp;Some consider&nbsp;<a title="Information hiding" href="https://en.wikipedia.org/wiki/Information_hiding">information hiding</a>&nbsp;to be&nbsp;<a title="Python (programming language)" href="https://en.wikipedia.org/wiki/Python_(programming_language)#Name_and_neologisms">unpythonic</a>, in that it suggests that the class in question contains unaesthetic or ill-planned internals. However, the strongest argument for name mangling is prevention of unpredictable breakage of programs: introducing a new public variable in a superclass can break subclasses if they don't use "private" variables.</p>
<p>From the tutorial:&nbsp;<em>As is true for modules, classes in Python do not put an absolute barrier between definition and user, but rather rely on the politeness of the user not to "break into the definition."</em></p>
<p>OOP doctrines such as the use of accessor methods to read data members are not enforced in Python. Just as Python offers functional-programming constructs but does not attempt to demand&nbsp;<a title="Referential transparency" href="https://en.wikipedia.org/wiki/Referential_transparency">referential transparency</a>, it offers an object system but does not demand OOP behavior. Moreover, it is always possible to redefine the class using&nbsp;<em>properties</em>&nbsp;so that when a certain variable is set or retrieved in calling code, it really invokes a function call, so that&nbsp;<code>spam.eggs = toast</code>&nbsp;might really invoke&nbsp;<code>spam.set_eggs(toast)</code>. This nullifies the practical advantage of accessor functions, and it remains OOP because the property&nbsp;<code>eggs</code>&nbsp;becomes a legitimate part of the object's interface: it need not reflect an implementation detail.</p>
<p>In version 2.2 of Python, "new-style" classes were introduced. With new-style classes, objects and types were unified, allowing the subclassing of types. Even entirely new types can be defined, complete with custom behavior for infix operators. This allows for many radical things to be done syntactically within Python. A new&nbsp;<a class="external text" href="https://www.python.org/download/releases/2.3/mro/" rel="nofollow">method resolution order</a>&nbsp;for&nbsp;<a title="Multiple inheritance" href="https://en.wikipedia.org/wiki/Multiple_inheritance">multiple inheritance</a>&nbsp;was also adopted with Python 2.3. It is also possible to run custom code while accessing or setting attributes, though the details of those techniques have evolved between Python versions.</p>
<h3><span id="With_statements" class="mw-headline">With statements</span></h3>
<p>The "with" statement handles resources.&nbsp;One function is called when entering scope and another when leaving. This prevents forgetting to remove the resource and also handles more complicated situations such as exceptions.</p>
<h3><span id="Properties" class="mw-headline">Properties</span></h3>
<p>Properties allow specially defined methods to be invoked on an object instance by using the same syntax as used for attribute access. An example of a class defining some properties is:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">

```python language
class MyClass:
    def __init__(self):
        self._a = None

    @property
    def a(self):
        return self._a

    @a.setter  # makes the property writable
    def a(self, value):
        self._a = value

```

</div>
<h3><span id="Descriptors" class="mw-headline">Descriptors</span></h3>
<p>A class that defines one or more of the special methods&nbsp;<code>__get__(self, instance, owner)</code>,&nbsp;<code>__set__(self, instance, value)</code>,&nbsp;<code>__delete__(self, instance)</code>&nbsp;can be used as a descriptor. Creating an instance of a descriptor as a class member of a second class makes the instance a property of the second class.</p>
<h3><span id="Class_and_static_methods" class="mw-headline">Class and static methods</span></h3>
<p>Python allows the creation of class methods and static method via the use of the&nbsp;<code>@classmethod</code>&nbsp;and&nbsp;<code>@staticmethod</code>&nbsp;<a href="https://en.wikipedia.org/wiki/Python_syntax_and_semantics#Decorators">decorators</a>. The first argument to a class method is the class object instead of the self-reference to the instance. A static method has no special first argument. Neither the instance, nor the class object is passed to a static method.</p>
<h2><span id="Exceptions" class="mw-headline">Exceptions</span></h2>
<p>Python supports (and extensively uses)&nbsp;<a title="Exception handling" href="https://en.wikipedia.org/wiki/Exception_handling">exception handling</a>&nbsp;as a means of testing for error conditions and other "exceptional" events in a program. Indeed, it is even possible to trap the exception caused by a&nbsp;<a title="Syntax error" href="https://en.wikipedia.org/wiki/Syntax_error">syntax error</a>.</p>
<p>Python style calls for the use of exceptions whenever an error condition might arise. Rather than testing for access to a file or resource before actually using it, it is conventional in Python to just go ahead and try to use it, catching the exception if access is rejected.</p>
<p>Exceptions can also be used as a more general means of non-local transfer of control, even when an error is not at issue. For instance, the&nbsp;<a title="GNU Mailman" href="https://en.wikipedia.org/wiki/GNU_Mailman">Mailman</a>&nbsp;mailing list software, written in Python, uses exceptions to jump out of deeply nested message-handling logic when a decision has been made to reject a message or hold it for moderator approval.</p>
<p>Exceptions are often used as an alternative to the&nbsp;<code>if</code>-block, especially in&nbsp;<a class="mw-redirect" title="Thread (computer science)" href="https://en.wikipedia.org/wiki/Thread_(computer_science)">threaded</a>&nbsp;situations. A commonly invoked motto is EAFP, or "It is Easier to Ask for Forgiveness than Permission,"&nbsp;which is attributed to&nbsp;<a title="Grace Hopper" href="https://en.wikipedia.org/wiki/Grace_Hopper#Anecdotes">Grace Hopper</a>. The alternative, known as LBYL, or "Look Before You Leap", explicitly tests for pre-conditions.</p>
<p>In this first code sample, following the LBYL approach, there is an explicit check for the attribute before access:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">spam</span><span class="p">,</span> <span class="s1">'eggs'</span><span class="p">):</span>
    <span class="n">ham</span> <span class="o">=</span> <span class="n">spam</span><span class="o">.</span><span class="n">eggs</span>
<span class="k">else</span><span class="p">:</span>
    <span class="n">handle_error</span><span class="p">()</span>
</pre>
</div>
<p>This second sample follows the EAFP paradigm:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">try</span><span class="p">:</span>
    <span class="n">ham</span> <span class="o">=</span> <span class="n">spam</span><span class="o">.</span><span class="n">eggs</span>
<span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
    <span class="n">handle_error</span><span class="p">()</span>
</pre>
</div>
<p>These two code samples have the same effect, although there will be performance differences. When&nbsp;<code>spam</code>&nbsp;has the attribute&nbsp;<code>eggs</code>, the EAFP sample will run faster. When&nbsp;<code>spam</code>&nbsp;does not have the attribute&nbsp;<code>eggs</code>&nbsp;(the "exceptional" case), the EAFP sample will run slower. The Python&nbsp;<a class="external text" href="https://docs.python.org/library/profile.html" rel="nofollow">profiler</a>&nbsp;can be used in specific cases to determine performance characteristics. If exceptional cases are rare, then the EAFP version will have superior&nbsp;<a class="mw-redirect" title="Average performance" href="https://en.wikipedia.org/wiki/Average_performance">average performance</a>&nbsp;than the alternative. In addition, it avoids the whole class of&nbsp;<a class="mw-redirect" title="Time-of-check-to-time-of-use" href="https://en.wikipedia.org/wiki/Time-of-check-to-time-of-use">time-of-check-to-time-of-use</a>&nbsp;(TOCTTOU) vulnerabilities, other&nbsp;<a class="mw-redirect" title="Race conditions" href="https://en.wikipedia.org/wiki/Race_conditions">race conditions</a>,&nbsp;and is compatible with&nbsp;<a title="Duck typing" href="https://en.wikipedia.org/wiki/Duck_typing">duck typing</a>. A drawback of EAFP is that it can be used only with statements; an exception cannot be caught in a generator expression, list comprehension, or lambda function.</p>
<h2><span id="Comments_and_docstrings" class="mw-headline">Comments and docstrings</span></h2>
<p>Python has two ways to annotate Python code. One is by using comments to indicate what some part of the code does. Single-line comments begin with the hash character ("#") and are terminated by the end of line. Comments spanning more than one line are achieved by inserting a multi-line string (with&nbsp;<code>"""</code>&nbsp;as the delimiter on each end) that is not used in assignment or otherwise evaluated, but sits in between other statements.</p>
<p>Commenting a piece of code:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">getline</span><span class="p">():</span>
    <span class="k">return</span> <span class="n">sys</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>  <span class="c1"># Get one line and return it</span>
</pre>
</div>
<p>Commenting a piece of code with multiple lines:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">getline</span><span class="p">():</span>
    <span class="k">return</span> <span class="n">sys</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>    <span class="s2">"""this function</span>
<span class="s2">                                      gets one line</span>
<span class="s2">                                      and returns it"""</span>
</pre>
</div>
<p><a title="Docstring" href="https://en.wikipedia.org/wiki/Docstring">Docstrings</a>&nbsp;(documentation strings), that is, strings that are located alone without assignment as the first indented line within a module, class, method or function, automatically set their contents as an attribute named&nbsp;<code>__doc__</code>, which is intended to store a human-readable description of the object's purpose, behavior, and usage. The built-in&nbsp;<code>help</code>&nbsp;function generates its output based on&nbsp;<code>__doc__</code>&nbsp;attributes. Such strings can be delimited with&nbsp;<code>"</code>&nbsp;or&nbsp;<code>'</code>&nbsp;for single line strings, or may span multiple lines if delimited with either&nbsp;<code>"""</code>&nbsp;or&nbsp;<code>'''</code>&nbsp;which is Python's notation for specifying multi-line strings. However, the style guide for the language specifies that triple double quotes (<code>"""</code>) are preferred for both single and multi-line docstrings.</p>
<p>Single line docstring:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">getline</span><span class="p">():</span>
    <span class="sd">"""Get one line from stdin and return it."""</span>
    <span class="k">return</span> <span class="n">sys</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>
</pre>
</div>
<p>Multi-line docstring:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">getline</span><span class="p">():</span>
    <span class="sd">"""Get one line</span>
<span class="sd">       from stdin</span>
<span class="sd">       and return it."""</span>
    <span class="k">return</span> <span class="n">sys</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>
</pre>
</div>
<p>Docstrings can be as large as the programmer wants and contain&nbsp;<a title="Newline" href="https://en.wikipedia.org/wiki/Newline">line breaks</a>. In contrast with comments, docstrings are themselves Python objects and are part of the interpreted code that Python runs. That means that a running program can retrieve its own docstrings and manipulate that information. But the normal usage is to give other programmers information about how to invoke the object being documented in the docstring.</p>
<p>There are tools available that can extract the docstrings to generate an&nbsp;<a title="Application programming interface" href="https://en.wikipedia.org/wiki/Application_programming_interface">API</a>&nbsp;documentation from the code. Docstring documentation can also be accessed from the interpreter with the&nbsp;<code>help()</code>&nbsp;function, or from the shell with the&nbsp;<a title="Pydoc" href="https://en.wikipedia.org/wiki/Pydoc">pydoc</a>&nbsp;command&nbsp;<code>pydoc</code>.</p>
<p>The&nbsp;<a title="Doctest" href="https://en.wikipedia.org/wiki/Doctest">doctest</a>&nbsp;standard module uses interactions copied from Python shell sessions into docstrings, to create tests, whereas the&nbsp;<a class="external text" href="http://docopt.org/" rel="nofollow">docopt</a>&nbsp;module uses them to define command-line options.</p>
<h2><span id="Function_annotations" class="mw-headline">Function annotations</span></h2>
<p>Function annotations are defined in&nbsp;<a class="external text" href="https://www.python.org/dev/peps/pep-3107/" rel="nofollow">PEP 3107</a>. They allow attaching data to the arguments and return of a function. The behaviour of annotations is not defined by the language, and is left to third party frameworks. For example, a library could be written to handle static typing:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">haul</span><span class="p">(</span><span class="n">item</span><span class="p">:</span> <span class="n">Haulable</span><span class="p">,</span> <span class="o">*</span><span class="n">vargs</span><span class="p">:</span> <span class="n">PackAnimal</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Distance</span>
</pre>
</div>
<h2><span id="Decorators" class="mw-headline">Decorators</span></h2>
<div class="hatnote navigation-not-searchable">See also:&nbsp;<a class="mw-redirect" title="Advice (computer science)" href="https://en.wikipedia.org/wiki/Advice_(computer_science)">Advice (computer science)</a></div>
<p>A decorator is any callable Python object that is used to modify a function, method or class definition. A decorator is passed the original object being defined and returns a modified object, which is then bound to the name in the definition. Python decorators were inspired in part by&nbsp;<a title="Java annotation" href="https://en.wikipedia.org/wiki/Java_annotation">Java annotations</a>, and have a similar syntax; the decorator syntax is pure&nbsp;<a title="Syntactic sugar" href="https://en.wikipedia.org/wiki/Syntactic_sugar">syntactic sugar</a>, using&nbsp;<code>@</code>&nbsp;as the keyword:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="nd">@viking_chorus</span>
<span class="k">def</span> <span class="nf">menu_item</span><span class="p">():</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">"spam"</span><span class="p">)</span>
</pre>
</div>
<p><strong>is equivalent to</strong></p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">menu_item</span><span class="p">():</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">"spam"</span><span class="p">)</span>
<span class="n">menu_item</span> <span class="o">=</span> <span class="n">viking_chorus</span><span class="p">(</span><span class="n">menu_item</span><span class="p">)</span>
</pre>
</div>
<p>Decorators are a form of&nbsp;<a title="Metaprogramming" href="https://en.wikipedia.org/wiki/Metaprogramming">metaprogramming</a>; they enhance the action of the function or method they decorate. For example, in the sample below,&nbsp;<code>viking_chorus</code>&nbsp;might cause&nbsp;<code>menu_item</code>&nbsp;to be run 8 times (see&nbsp;<a title="Spam (Monty Python)" href="https://en.wikipedia.org/wiki/Spam_(Monty_Python)">Spam sketch</a>) for each time it is called:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">viking_chorus</span><span class="p">(</span><span class="n">myfunc</span><span class="p">):</span>
    <span class="k">def</span> <span class="nf">inner_func</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">8</span><span class="p">):</span>
            <span class="n">myfunc</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">inner_func</span>
</pre>
</div>
<p>Canonical uses of function decorators are for creating&nbsp;<a class="mw-redirect" title="Class method" href="https://en.wikipedia.org/wiki/Class_method">class methods</a>&nbsp;or&nbsp;<a class="mw-redirect" title="Static method" href="https://en.wikipedia.org/wiki/Static_method">static methods</a>, adding function attributes,&nbsp;<a title="Tracing (software)" href="https://en.wikipedia.org/wiki/Tracing_(software)">tracing</a>, setting&nbsp;<a title="Precondition" href="https://en.wikipedia.org/wiki/Precondition">pre-</a>&nbsp;and&nbsp;<a title="Postcondition" href="https://en.wikipedia.org/wiki/Postcondition">postconditions</a>, and&nbsp;<a title="Synchronization" href="https://en.wikipedia.org/wiki/Synchronization">synchronization</a>,&nbsp;but can be used for far more besides, including&nbsp;<a class="mw-redirect" title="Tail recursion elimination" href="https://en.wikipedia.org/wiki/Tail_recursion_elimination">tail recursion elimination</a>,&nbsp;<a title="Memoization" href="https://en.wikipedia.org/wiki/Memoization">memoization</a>&nbsp;and even improving the writing of decorators.</p>
<p>Decorators can be chained by placing several on adjacent lines:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="nd">@invincible</span>
<span class="nd">@favourite_colour</span><span class="p">(</span><span class="s2">"Blue"</span><span class="p">)</span>
<span class="k">def</span> <span class="nf">black_knight</span><span class="p">():</span>
    <span class="k">pass</span>
</pre>
</div>
<p>is equivalent to</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">black_knight</span><span class="p">():</span>
    <span class="k">pass</span>
<span class="n">black_knight</span> <span class="o">=</span> <span class="n">invincible</span><span class="p">(</span><span class="n">favourite_colour</span><span class="p">(</span><span class="s2">"Blue"</span><span class="p">)(</span><span class="n">black_knight</span><span class="p">))</span>
</pre>
</div>
<p>or, using intermediate variables</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">black_knight</span><span class="p">():</span>
    <span class="k">pass</span>
<span class="n">blue_decorator</span> <span class="o">=</span> <span class="n">favourite_colour</span><span class="p">(</span><span class="s2">"Blue"</span><span class="p">)</span>
<span class="n">decorated_by_blue</span> <span class="o">=</span> <span class="n">blue_decorator</span><span class="p">(</span><span class="n">black_knight</span><span class="p">)</span>
<span class="n">black_knight</span> <span class="o">=</span> <span class="n">invincible</span><span class="p">(</span><span class="n">decorated_by_blue</span><span class="p">)</span>
</pre>
</div>
<p>In the example above, the&nbsp;<code>favourite_colour</code>&nbsp;decorator&nbsp;<a class="mw-redirect" title="Factory (software concept)" href="https://en.wikipedia.org/wiki/Factory_(software_concept)">factory</a>&nbsp;takes an argument. Decorator factories must return a decorator, which is then called with the object to be decorated as its argument:</p>
<div class="mw-highlight mw-highlight-lang-python mw-content-ltr" dir="ltr">
<pre><span class="k">def</span> <span class="nf">favourite_colour</span><span class="p">(</span><span class="n">colour</span><span class="p">):</span>
    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span><span class="n">func</span><span class="p">):</span>
        <span class="k">def</span> <span class="nf">wrapper</span><span class="p">():</span>
            <span class="nb">print</span><span class="p">(</span><span class="n">colour</span><span class="p">)</span>
            <span class="n">func</span><span class="p">()</span>
        <span class="k">return</span> <span class="n">wrapper</span>
    <span class="k">return</span> <span class="n">decorator</span>
</pre>
</div>
<p>This would then decorate the&nbsp;<code>black_knight</code>&nbsp;function such that the colour,&nbsp;<code>"Blue"</code>, would be printed prior to the&nbsp;<code>black_knight</code>&nbsp;function running.&nbsp;<a title="Closure (computer programming)" href="https://en.wikipedia.org/wiki/Closure_(computer_programming)">Closure</a>&nbsp;ensures that the colour argument is accessible to the innermost wrapper function even when it is returned and goes out of scope, which is what allows decorators to work.</p>
<p>Despite the name, Python decorators are not an implementation of the&nbsp;<a title="Decorator pattern" href="https://en.wikipedia.org/wiki/Decorator_pattern">decorator pattern</a>. The decorator pattern is a&nbsp;<a title="Design pattern" href="https://en.wikipedia.org/wiki/Design_pattern">design pattern</a>&nbsp;used in&nbsp;<a class="mw-redirect" title="Statically typed" href="https://en.wikipedia.org/wiki/Statically_typed">statically typed</a>&nbsp;<a class="mw-redirect" title="Object-oriented programming language" href="https://en.wikipedia.org/wiki/Object-oriented_programming_language">object-oriented programming languages</a>&nbsp;to allow functionality to be added to objects at run time; Python decorators add functionality to functions and methods at definition time, and thus are a higher-level construct than decorator-pattern classes. The decorator pattern itself is trivially implementable in Python, because the language is&nbsp;<a class="mw-redirect" title="Duck typed" href="https://en.wikipedia.org/wiki/Duck_typed">duck typed</a>, and so is not usually considered as such.</p>
<h2><span id="Easter_eggs" class="mw-headline">Easter eggs</span></h2>
<p>Users of&nbsp;<a class="mw-redirect" title="Curly bracket programming language" href="https://en.wikipedia.org/wiki/Curly_bracket_programming_language">curly bracket programming languages</a>, such as&nbsp;<a title="C (programming language)" href="https://en.wikipedia.org/wiki/C_(programming_language)">C</a>&nbsp;or&nbsp;<a title="Java (programming language)" href="https://en.wikipedia.org/wiki/Java_(programming_language)">Java</a>, sometimes expect or wish Python to follow a block-delimiter convention. Brace-delimited block syntax has been repeatedly requested, and consistently rejected by core developers. The Python interpreter contains an&nbsp;<a class="mw-redirect" title="Easter egg (virtual)" href="https://en.wikipedia.org/wiki/Easter_egg_(virtual)">easter egg</a>&nbsp;that summarizes its developers' feelings on this issue. The code&nbsp;<code>from __future__ import braces</code>&nbsp;raises the exception&nbsp;<code>SyntaxError: not a chance</code>. The&nbsp;<code>__future__</code>&nbsp;module is normally used to&nbsp;<a title="Backporting" href="https://en.wikipedia.org/wiki/Backporting">provide features from future versions</a>&nbsp;of Python.</p>
<p>Another hidden message, The Zen of Python (a summary of&nbsp;<a title="Python (programming language)" href="https://en.wikipedia.org/wiki/Python_(programming_language)#Features_and_philosophy">Python philosophy</a>), is displayed when trying to&nbsp;<code>import this</code>.</p>
<p>The message&nbsp;<code>Hello world!</code>&nbsp;is printed when the import statement&nbsp;<code>import __hello__</code>&nbsp;is used. In Python 2.7, instead of&nbsp;<code>Hello world!</code>&nbsp;it prints&nbsp;<code>Hello world...</code>.</p>
<p>An&nbsp;<code><a class="mw-redirect" title="Antigravity" href="https://en.wikipedia.org/wiki/Antigravity">antigravity</a></code>&nbsp;module was added to Python 2.7 and 3.0. Importing it opens a web browser to&nbsp;<a title="Xkcd" href="https://en.wikipedia.org/wiki/Xkcd">xkcd</a>&nbsp;comic&nbsp;<a class="external text" href="https://xkcd.com/353/" rel="nofollow">353</a>&nbsp;that portrays a humorous fictional use for such a module, intended to demonstrate the ease with which Python modules enable additional functionality.&nbsp;In Python 3.0, this module also contains an implementation of the "geohash" algorithm, a reference to&nbsp;<a title="Xkcd" href="https://en.wikipedia.org/wiki/Xkcd">xkcd</a>&nbsp;comic&nbsp;<a class="external text" href="https://xkcd.com/426/" rel="nofollow">426</a>.</p>
</br>
<ul>
<li><a href="https://github.com/manjunath5496/Python-Tutorial/blob/master/Notes/pyk(18).pdf" rel="nofollow">Functional Programming in Python</a></li>
<li><a href="https://github.com/manjunath5496/Python-Tutorial/blob/master/Notes/pyk(19).pdf" rel="nofollow">Only the Limits of Our Imagination: An exclusive interview with
Grace M. Hopper</a></li>
<li><a href="https://github.com/manjunath5496/Python-Tutorial/blob/master/Notes/pyk(20).pdf">The decorator module (old version)</a></li>
 <li><a href="https://github.com/manjunath5496/Python-Tutorial/blob/master/Notes/pyk(21).pdf">Python 3 MCQ - Multiple Choice Questions n Answers for Tests, Quizzes - Python Students and Teachers</a></li>
    
    
    
    
</ul>
</br>
