---
layout: default
title: Books
permalink: /books/
---

<div class="books">
  {%- if site.posts.size > 0 -%}
  <ul class="post-list">
    {%- for post in site.categories.Books -%}
    <li>
      <a class="post-link" href="{{ post.url | relative_url }}">
        <img width="160" src="{{ post.img }}" />
        <span class="post-name">{{ post.title | escape }}</span>
      </a>
      <span class="post-date">{{ post.ratings }}</span>
      <span class="post-date post-author">by {{ post.author }}</span>
      <span class="post-date">{{ post.date | date: "%Y.%m.%d" }}</span>
    </li>
    {%- endfor -%}
  </ul>
  {%- endif -%}
</div>
