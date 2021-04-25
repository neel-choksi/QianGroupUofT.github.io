---
title: "Qian Group - Publications"
layout: gridlay
excerpt: "Qian Group-- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Group highlights

For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.ca/citations?hl=en&user=sLHyO1wAAAAJ&view_op=list_works&sortby=pubdate).

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Full List

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
