---
layout: page
title: Archive
permalink: /archive/
---


{% for post in site.posts %}
- [{{ post.date | date: "%-d." }} {% assign m = post.date | date: "%-m" %}{% case m %}{% when '1' %}Januar{% when '2' %}Februar{% when '3' %}M&auml;rz{% when '4' %}April{% when '5' %}Mai{% when '6' %}Juni{% when '7' %}Juli{% when '8' %}August{% when '9' %}September{% when '10' %}Oktober{% when '11' %}November{% when '12' %}Dezember{% endcase %} {{ post.date | date: "%Y" }} {{ post.title }}]({{ post.url }})
{% endfor %}
