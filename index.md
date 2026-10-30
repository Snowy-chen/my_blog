---
layout: default
---

# 最新文章

<ul style="list-style: none;padding: 15px 0; color: #333;">
  {% for post in site.posts %}
    <li style="display: flex;">
       {% if post.image %}
      <img src="{{post.image}}" style="width: 200px; margin-right: 10px; border: 1px solid #eee; border-radius: 5px; padding: 5px; background-color: #eee;">
      {% endif %}
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> 
      <span style="color: #999; font-size: 0.9em;">- {{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>
