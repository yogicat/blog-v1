---
layout: page
title: Writing
permalink: /Writing/
---
<div class="home">
  {%- if site.posts.size > 0 -%}
  <ul class="post-list">
    {%- for post in site.categories.Writing -%}
    <li>
      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}</a>
      <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
    {%- endfor -%}
  </ul>
  {%- endif -%}
</div>
