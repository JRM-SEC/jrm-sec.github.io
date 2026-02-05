---
layout: page
title: Blog
---

Aquí documento ideas, aprendizajes y reflexiones sobre ciberseguridad y proyectos prácticos.

---

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})

<span style="opacity:.7;font-size:.9em;">
  {{ post.date | date: "%d/%m/%Y" }}
</span>

{{ post.excerpt | strip_html | truncate: 220 }}

---

{% endfor %}
