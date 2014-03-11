## Add some style 

<hr />

<p class="file">File: <span class="file-name">index.html</span></p>

<pre><code class="django" data-trim>
{% extends "_base.html" %}

{% block css %}
<link rel="stylesheet" href="css/style.css" />
<style>
  #tarbell-headline { font-size: 90px; }
</style>
{% endblock %}

{% block content %}
<div class="container">
  <!-- content -->;
</div>
{% endblock content %}
</code></pre>
