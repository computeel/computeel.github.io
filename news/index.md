---
layout: page
title: News
eyebrow: Updates
subtitle: Announcements, achievements and events at ComputEEL/MatSci.
hero_image: /assets/images/hero-group.jpeg
hero_tags:
  - Events
  - Defenses & exams
  - Superconductivity
---

### Latest news

{% assign news_posts = site.categories.news | sort: "date" | reverse %}
<div class="grid" style="grid-template-columns: repeat(auto-fit,minmax(260px,1fr));">
{% for post in news_posts %}
  <div class="card">
    <div class="tag">{{ post.date | date: "%d %b %Y" }}</div>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="muted">{{ post.subtitle | default: post.excerpt | strip_html | truncate: 120 }}</p>
    <a class="pill" href="{{ post.url | relative_url }}">Read</a>
  </div>
{% endfor %}
</div>

### Blog

{% assign blog_posts = site.categories.blog | sort: "date" | reverse %}
<div class="grid" style="grid-template-columns: repeat(auto-fit,minmax(260px,1fr));">
{% for post in blog_posts %}
  <div class="card">
    <div class="tag">{{ post.date | date: "%d %b %Y" }}</div>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="muted">{{ post.subtitle | default: post.excerpt | strip_html | truncate: 120 }}</p>
    <a class="pill" href="{{ post.url | relative_url }}">Read</a>
  </div>
{% else %}
  <p class="muted">No blog posts yet.</p>
{% endfor %}
</div>
