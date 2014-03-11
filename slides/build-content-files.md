## Read a file

<hr />

<p class="file">File: <span class="file-name">content.md</span></p>

<pre><code class="markdown" data-trim>
# My glorious content

* A glorious one item list
</code></pre>

<hr/>

<p class="file">File: <span class="file-name">index.html</span></p>
 
<pre><code class="django" data-trim>
{% extends "_base.html" %}

{% block content %}
<div class="container">
  {{ read_file("content.md")|markdown }}
</div>
{% endblock %}
</code></pre>

