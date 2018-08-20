---
title: "News - Quantitative Psychology Active Learning Lab"
layout: newslay
excerpt: "News in Quantitative Psychology Active Learning Lab"
permalink: /allnews/
---
# News

{% for article in site.data.news %}
<p style="padding: 0.7em 0 0 0">{{ article.date }} <br>
<font size="5">{{ article.headline }}</font><br>
{{ article.content }}</p>
<p align="center" style="padding: 0 0 0.7em 0"> {{ article.link }} </p>
{% endfor %}
