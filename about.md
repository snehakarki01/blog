---
layout: default
title: Welcome
permalink: /
---

<div style="text-align: center; margin-top: 40px;">
  <img src="{{ site.avatar }}" alt="Avatar" style="border-radius: 50%; width: 120px;" />
  <h1>👋 Hello, I'm {{ site.name }}</h1>
  <p>{{ site.description }}</p>
</div>

<br />

## ✍️ Latest Posts

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><br />
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

<br />

## 🔗 Explore

- [About](/about/)
- [Projects](/projects/)  
- [Contact](mailto:{{ site.email }})

