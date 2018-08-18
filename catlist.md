---
title: "List of Post Categories"
layout: page
---

{% for cat in site.categories %}

{% capture catname %}{{ cat | first }}{% endcapture %}

[{{catname}} ({{ site.categories[catname] | size }} posts)](/categories/{{catname}})

{% endfor %}
