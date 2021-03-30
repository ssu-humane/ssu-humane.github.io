---
title: "HUMANE Lab - Publications"
layout: gridlay
excerpt: "HUMANE Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Selected Publications

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.com/citations?user=xiZ1ImoAAAAJ&hl=en))

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
