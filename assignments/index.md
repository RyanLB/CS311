---
title: "Assignments"
layout: default
---

# Assignments

{% for file in site.static_files %}
{% if file.path contains "/assignments/" %}
[{{ file.path | remove_first:"/assignments/" }}]({{ site.github.url }}{{ file.path | uri_escape }})
{% endif %}
{% endfor %}
