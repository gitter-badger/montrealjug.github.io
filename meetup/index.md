---
layout: page
title: Meetups
excerpt: "Tous les Meetups du Montreal JUG"
---

<ul class="post-list">
{% for post in site.categories.meetup %}
 {% if post.hidden != true %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
  {% endif %}
{% endfor %}
</ul>
