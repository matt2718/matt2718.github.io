---
title: "List of Post Categories"
layout: page
---
{% assign sorted_cats = site.categories | sort %}
{% for cat in sorted_cats %}

{% capture catname %}{{ cat | first }}{% endcapture %}

[{{catname}} ({{ site.categories[catname] | size }} posts)](/categories/{{catname}})

{% endfor %}
