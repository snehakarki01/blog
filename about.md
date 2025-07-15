---
layout: page
title: Welcome
permalink: /
---

<img src="{{ site.avatar }}" alt="Avatar" style="border-radius: 50%; width: 100px;">

# 👋 Hello, I'm {{ site.name }}

{{ site.description }}

---

## ✍️ Latest Posts

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><br>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

---

## 🔗 Explore
- [About](/about/)
- [Projects](/projects/)
- [Contact](mailto:{{ site.footer-links.email }})
