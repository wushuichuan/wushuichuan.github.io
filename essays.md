---
layout: page
title: Essays
permalink: /essays/
---

# 思想文章

这里收录哲学、心理学与社会科学方面的专题分析和独立思考。

{% assign articles = site.posts | where_exp: "post", "post.categories contains 'essays'" %}

{% for post in articles %}
- [{{ post.title }}]({{ post.url | relative_url }}) · {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
