---
layout: page-w-avatar
title: Blog Posts
excerpt: "An archive of blog posts sorted by date."
image:
  feature: cottonwood.png
  credit: 
  creditlink: 
search_omit: true
---



---

<ul class="post-list">
{% for post in site.categories.blog %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul> 

<a markdown="0" href="/tags/" class="btn">Tag index</a>
