---
layout: page
title: 自学与自我价值成长
permalink: /self-growth/
---

# 自学与自我价值成长

*Self-Learning & Personal Growth*

这里记录我对自主学习、个人成长与自我价值的长期探索。

## 相关文章

{% assign articles = site.posts | where_exp: "post", "post.categories contains 'self-growth'" %}

{% for post in articles %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
