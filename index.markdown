---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<style>
#main {
  margin-left: 10%;
  margin-right: 10%;
}
  
</style>

<head>
  <title>Neotoma Community Stories</title>
</head>
<div id="main">
<div style="display:grid;grid-template-rows: 1fr 1fr; margin: 3%; margin-bottom: 0%;">
<div style="position: relative; border: 1px solid var(--neotoma-brown-450); background: linear-gradient(135deg, var(--neotoma-gray-150) 0%, var(--neotoma-brown-0) 100%); width: 136%; padding-top: 20px; display:grid; grid-template-columns: 1fr 5fr; align-items:center; justify-items: center; justify-self:center;">
  <img style="width:100px;padding-bottom:15px;" src="https://raw.githubusercontent.com/NeotomaCommunity/NeotomaCommunity.github.io/278cda48e3d7f51e90188bc0fa89fb4fa73f43b2/images/packrat-logo.svg"/>
<h1>{{ site.title }}</h1>
</div>
<div style="text-align: center; margin-left: 5%; margin-right: 5%;">
<p> This website is a repository of stories contributed by members of Neotoma's community, organized by Neotoma's <a href="https://www.neotomadb.org/outreach" target="_blank"> Outreach and Community Engagement</a> team.</p>
</div>
</div>

<div style="display: grid; grid-template-rows: 1fr 10fr;">
  <h2 style="margin-top: 0px; padding-top: 0px;">Contributed Posts</h2>
<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%B %-d, %Y" }}</span>
  </li>
{% endfor %}

</div>
</ul>
</div>
