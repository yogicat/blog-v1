---
layout: page
title: Books
permalink: /Books/
---
<ul class="post-list">
  {%- for post in site.categories.Books -%}
  <li>
    <a class="post-link" href="{{ post.url | relative_url }}">
      {{ post.title | escape }}</a>
    <span class="post-categories">{{ post.categories }}</span>
    <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
  {%- endfor -%}
</ul>

