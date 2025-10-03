---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<div style="display:grid;grid-template-rows: 1fr 1fr;">
<div style="border: 1px solid var(--neotoma-brown-450);">
<h1>{{ site.title }}</h1>
</div>
<div style="border: 1px solid var(--neotoma-brown-450);">
<p> {{ site.description }} </p>
</div>
</div>

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%B %-d, %Y" }}</span>
  </li>
{% endfor %}
</ul>
