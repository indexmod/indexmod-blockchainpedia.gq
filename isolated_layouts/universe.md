---
title: The Indexmod universe
shortname: This universe
permalink: universe
birth: 2018
layout: tech-universe
exclude: true
---

<wrap>

{% assign mypages = site.html_pages | sort: "order" %} {% for page in mypages %}
{% unless page.exclude %}

<a href="{{ page.permalink | absolute_url }}">{% include indexmod-indicator-2.html %}</a>

{% endunless %}
{% endfor %}

</wrap>