---
layout: page
title: Blog
permalink: /blog/
---

<ul>
  {% raw %}{% for post in site.posts %}{% endraw %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small> — {{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% raw %}{% endfor %}{% endraw %}
</ul>
