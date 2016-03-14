---
layout: page
title: Meet Us
permalink: /meet/
---

{% assign current-shambles = (site.data.shambles | where:"left", "false") %}
{% assign shamblumni = (site.data.shambles | where:"left", "true") %}

{% for shamble in current-shambles %}
    {{shamble.name}}
{% endfor %}

{% for shamble in shamblumni %}
    {{shamble.name}}
{% endfor %}
