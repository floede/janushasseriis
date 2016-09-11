---
layout: page
permalink: /articles/
title: articles
description: My thoughts on code, development, projects and everything surrounding that.
---

<ul class="post-list">
{% for poem in site.articles reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
