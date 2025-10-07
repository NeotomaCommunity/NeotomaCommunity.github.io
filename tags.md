---
layout: default
title: Tags
---

<style>

  #main {
    margin-left: 10%;
    margin-right: 10%;
    border-bottom: 1px solid var(--neotoma-brown-200);
  }
  
</style>

<div id="main">
<h1>Tags</h1>

<ul>
  {% for tag in site.tags %}
    <li>
      <a href="#{{ tag[0] }}">{{ tag[0] }}</a> ({{ tag[1].size }} posts)
    </li>
  {% endfor %}
</ul>

{% for tag in site.tags %}
  <h2 id="{{ tag[0] }}">{{ tag[0] }}</h2>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
</div>

<div style="display:grid;grid-template-columns:2fr 1fr; margin-left:10%;margin-right:10%;">
<div id="return">
  <p>Return to Neotoma Community Stories <a href="https://neotomacommunity.github.io/">main page.</a></p>
</div>
</div>
