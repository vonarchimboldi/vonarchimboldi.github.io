---
layout: archive
permalink: /posts/
title: "Posts"
author_profile: "true"
---


{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.extract }}
  </article>
{% endfor %}