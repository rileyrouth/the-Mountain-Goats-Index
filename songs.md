---
layout: default
title: Songs
permalink: /songs/
---
# Songs

{% for song in site.data.songs %}
{% assign slug = song.title | slugify %}
* [{{ song.title }}]({{ "/songs/" | append: slug | relative_url }})
{% endfor %}