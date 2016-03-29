---
title: Lecture Notes
layout: default
---

# Lecture Notes

{% for file in site.static_files %}
{% if file.path contains "/lectures/" %}
[{{ file.path | remove_first:"/lectures/" }}]({{ file.path | uri_escape }})
{% endif %}
{% endfor %}
