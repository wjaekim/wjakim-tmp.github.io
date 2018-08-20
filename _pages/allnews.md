---
title: "News - Quantitative Psychology Active Learning Lab"
layout: gridlay
excerpt: "News in Quantitative Psychology Active Learning Lab"
permalink: /allnews/
---

# News

{% for article in site.data.news %}
<p><h1>{{ article.headline }} </h1> <br>
{{ article.date }}</p>
{% endfor %}
