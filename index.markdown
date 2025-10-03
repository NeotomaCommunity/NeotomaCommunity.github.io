---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<style>
body {
  margin-left: 10%;
  margin-right: 10%;
}
  
</style>

<div style="display:grid;grid-template-rows: 1fr 1fr; margin: 3%;">
<div style="position: relative; border: 1px solid var(--neotoma-brown-450); background: linear-gradient(135deg, var(--neotoma-gray-150) 0%, var(--neotoma-brown-0) 100%); width: 150%; left: -25%; padding-top: 20px;">
<h1>{{ site.title }}</h1>
</div>
<div style="text-align: center; margin-left: 5%; margin-right: 5%;">
<p> {{ site.description }} </p>
</div>
</div>

<div style="display: grid; grid-template-rows: 1fr 10fr;">
  <h2 style="">Contributed Posts</h2>
<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%B %-d, %Y" }}</span>
  </li>
{% endfor %}
</ul>
</div>
