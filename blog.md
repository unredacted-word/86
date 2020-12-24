---
title: Articles
displayTitle: "Articles"
---


<ol class="c-Index">
{% for post in site.posts %}
  <li class="c-Index--Item">
    <a href="/86{{ post.url }}" title="{{ post.title }}">
      {{ post.title }}
    </a>
    <br>

    {% if post.metaDescription %}
      <span>{{ post.metaDescription }}</span>
      <br>
    {% endif %}

    <time class="published" datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date: "%A %B %-d, %Y" }}</time>
  </li>
{% endfor %}
</ol>
