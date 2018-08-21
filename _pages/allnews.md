---
title: "News - Quantitative Psychology Active Learning Lab"
layout: newslay
excerpt: "News from Quantitative Psychology Active Learning Lab"
permalink: /allnews/
---
# News

{% for article in site.data.news %}
<p style="padding: 0.6em 0 0 0">
<font size="+2">{{ article.headline }}</font><br>
{{ article.date }} <br>
{{ article.content }}</p>
<p align="center" style="padding: 0 0 0.6em 0"> {{ article.link }} </p>
{% endfor %}
