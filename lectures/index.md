---
title: Lecture Notes
layout: default
---

# Lecture Notes

{% for file in site.static_files %}
{% if file.path contains "/lectures/" %}
[{{ file.path | remove_first:"/lectures/" }}]({{ site.github.url }}{{ file.path | uri_encode }})
{% endif %}
{% endfor %}
