---
layout: default
title: Updates
permalink: /posts/
---

Catch up on the latest notes from our meetups and announcements.

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small>{{ post.date | date: "%d %B %Y" }}</small>

{{ post.excerpt | strip_html }}

{% endfor %}
