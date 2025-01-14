---
layout: default
title: Records
permalink: /records/
---
# Records
This is a list of records by the Mountain Goats, including EPs, cassettes, albums, and compilations. Click on a record to see its songs and other information.

{% assign discography = site.records | sort: "year" %}
{% for record in discography %}
* [{{ record.title }}]({{ record.url | relative_url }})
{% endfor %}