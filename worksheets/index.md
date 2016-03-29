---
title: "Worksheets"
layout: default
---

# Worksheets

{% for file in site.static_files %}
{% if file.path contains "/worksheets/" %}
[{{ file.path | remove_first:"/worksheets/" }}]({{ file.path | uri_escape }})
{% endif %}
{% endfor %}
