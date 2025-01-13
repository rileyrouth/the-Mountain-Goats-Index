---
layout: default
title: Shows
permalink: /shows/
---
# Shows

{% for show in site.shows %}
[{{ show.date | date: "%d %B %Y" }}, {{ show.city }} ({{ show.venue }})]({{ show.url | relative_url }})
{% endfor %}