---
layout: default
title: Songs
permalink: /songs/
---
# Songs
This is a list of songs by the Mountain Goats. Click on a song to see lyrics and more information.

{% for song in site.data.songs %}
{% assign slug = song.title | slugify %}
* [{{ song.title }}]({{ "/songs/" | append: slug | relative_url }})
{% endfor %}