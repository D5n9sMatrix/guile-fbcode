<!DOCTYPE html>
<!-- saved from url=(0082)https://www.gnu.org/software/emacs/manual/html_node/elisp/Evaluation-Notation.html -->
<html><!-- Created by GNU Texinfo 7.0.3, https://www.gnu.org/software/texinfo/ --><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">

<title>Evaluation Notation (GNU Emacs Lisp Reference Manual)</title>

<meta name="description" content="Evaluation Notation (GNU Emacs Lisp Reference Manual)">
<meta name="keywords" content="Evaluation Notation (GNU Emacs Lisp Reference Manual)">
<meta name="resource-type" content="document">
<meta name="distribution" content="global">
<meta name="Generator" content="makeinfo">
<meta name="viewport" content="width=device-width,initial-scale=1">

<link rev="made" href="mailto:bug-gnu-emacs@gnu.org">
<link rel="icon" type="image/png" href="https://www.gnu.org/graphics/gnu-head-mini.png">
<meta name="ICBM" content="42.256233,-71.006581">
<meta name="DC.title" content="gnu.org">
<style type="text/css">
@import url('/software/emacs/manual.css');
</style>
</head>

<body lang="en">
<div class="subsection-level-extent" id="Evaluation-Notation">
<div class="nav-panel">
<p>
Next: <a href="https://www.gnu.org/software/emacs/manual/html_node/elisp/Printing-Notation.html" accesskey="n" rel="next">Printing Notation</a>, Previous: <a href="https://www.gnu.org/software/emacs/manual/html_node/elisp/nil-and-t.html" accesskey="p" rel="prev"><code class="code">nil</code> and <code class="code">t</code></a>, Up: <a href="https://www.gnu.org/software/emacs/manual/html_node/elisp/Conventions.html" accesskey="u" rel="up">Conventions</a> &nbsp; [<a href="https://www.gnu.org/software/emacs/manual/html_node/elisp/index.html#SEC_Contents" title="Table of contents" rel="contents">Contents</a>][<a href="https://www.gnu.org/software/emacs/manual/html_node/elisp/Index.html" title="Index" rel="index">Index</a>]</p>
</div>
<hr>
<h4 class="subsection" id="Evaluation-Notation-1">1.3.3 Evaluation Notation</h4>
<a class="index-entry-id" id="index-evaluation-notation"></a>
<a class="index-entry-id" id="index-documentation-notation"></a>
<a class="index-entry-id" id="index-notation"></a>

<p>A Lisp expression that you can evaluate is called a <em class="dfn">form</em>.
Evaluating a form always produces a result, which is a Lisp object.  In
the examples in this manual, this is indicated with ‘<samp class="samp">⇒</samp>’:
</p>
<div class="example">
<pre class="example-preformatted">(car '(1 2))
     ⇒ 1
</pre></div>

<p>You can read this as “<code class="code">(car '(1 2))</code> evaluates to 1”.
</p>
<p>When a form is a macro call, it expands into a new form for Lisp to
evaluate.  We show the result of the expansion with
‘<samp class="samp">→</samp>’.  We may or may not show the result of the
evaluation of the expanded form.
</p>
<div class="example">
<pre class="example-preformatted">(third '(a b c))
     → (car (cdr (cdr '(a b c))))
     ⇒ c
</pre></div>

<p>To help describe one form, we sometimes show another form that
produces identical results.  The exact equivalence of two forms is
indicated with ‘<samp class="samp">≡</samp>’.
</p>
<div class="example">
<pre class="example-preformatted">(make-sparse-keymap) ≡ (list 'keymap)
</pre></div>

</div>





</body></html>