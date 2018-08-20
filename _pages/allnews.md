---
title: "News - Quantitative Psychology Active Learning Lab"
layout: gridlay
excerpt: "News in Quantitative Psychology Active Learning Lab"
permalink: /allnews/
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
### {{ article.headline }} </p>
{% endfor %}
