---
layout: default
title: Thoughts and Abstracts
permalink: /blogs/
---

<section class="blog-section">
  <h1>Thoughts and Abstracts</h1>
  <hr>

  <!-- Technical Section -->
  <div class="blog-category">
    <h2>Technical</h2>
    <div class="blog-list">
      {% for post in site.posts %}
        {% if post.category == "technical" %}
        <div class="blog-item">
          <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
          <p>{{ post.excerpt | strip_html }}</p>
          <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
        </div>
        {% endif %}
      {% endfor %}
    </div>
  </div>

  <hr>

  <!-- Psychological Section -->
  <div class="blog-category">
    <h2>Psychological</h2>
    <div class="blog-list">
      {% for post in site.posts %}
        {% if post.category == "psychology" %}
        <div class="blog-item">
          <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
          <p>{{ post.excerpt | strip_html }}</p>
          <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
        </div>
        {% endif %}
      {% endfor %}
    </div>
  </div>
</section>
