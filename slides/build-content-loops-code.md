## Add some Javascript 

<hr />

<p class="file">File: <span class="file-name">index.html</span></p>

<pre><code class="django" data-trim>
{% extends "_base.html" %}

{% block content %}
  {% for journalist in journalists %}
  <h1>{{ journalist.name }}</h1>
  <img src="{{ journalist.image }}" />
  <p><a href="{{ journalist.url }}">Wikipedia</a></p>
  {% endfor %}
{% endblock content %}
</code></pre>
