---
layout: default
title: Tennis Blog
permalink: /blog/
---

# Tennis Blog 🎾

<div class="posts">
  {% for post in site.categories.Tennis %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>