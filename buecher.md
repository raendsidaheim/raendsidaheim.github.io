---
layout: page
title: Bücher
permalink: /buecher/
---

<ul class="post-list">
  {% for post in site.posts %}
    {% if post.subtype == 'buecher' %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    </li>
    {% endif %}
  {% endfor %}
</ul>
