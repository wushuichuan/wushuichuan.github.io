---
layout: page
title: Notes
permalink: /notes/
---

# 阅读与学习笔记

记录书籍阅读、概念学习、知识整理和日常思考。

{% assign articles = site.posts | where_exp: "post", "post.categories contains 'notes'" %}

{% for post in articles %}
- [{{ post.title }}]({{ post.url | relative_url }}) · {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
