---
layout: default
title: Records
permalink: /records/
---
# Records

{% for record in site.records %}
* [{{ record.title }}]({{ record.url }})
{% endfor %}