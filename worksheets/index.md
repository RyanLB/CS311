---
title: "Worksheets"
layout: default
---

# Worksheets

{% for file in site.static_files %}
{% if file.path contains "/worksheets/" %}
[{{ file.path | remove_first:"/worksheets/" }}]({{ site.github.url }}{{ file.path | uri_escape }})
{% endif %}
{% endfor %}
