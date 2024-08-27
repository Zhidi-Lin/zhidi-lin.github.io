---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 2
pubs:

### Topic: IoT Network Security

  - author: "**Zhidi LIN**"
    title: "See my my full list of publications on Google Scholar"
    month: "Aug"
    year: "2024"
    booktitle: ""
    url: "https://scholar.google.com/citations?user=8BmRXqMAAAAJ&hl=en"


---

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}<br>
    {% if pub.address %}{{pub.address}}
    {% endif %} {{pub.month}}, {{pub.year}} {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}
