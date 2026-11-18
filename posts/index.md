---
layout: page
title: Posts
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      <small><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %d, %Y" }}</time></small>
    </li>
  {% endfor %}
</ul>
