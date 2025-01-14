---
layout: default
title: Shows
permalink: /shows/
---
# Shows
This is a list of live shows played by the Mountain Goats. Click on a date to see the setlist and other information.

{% for show in site.shows %}
[{{ show.date | date: "%d %B %Y" }}, {{ show.city }} ({{ show.venue }})]({{ show.url | relative_url }})
{% endfor %}