---
title: "News - Quantitative Psychology Active Learning Lab"
layout: newslay
excerpt: "News from Quantitative Psychology Active Learning Lab"
permalink: /news/
---
# News

{% for article in site.data.news %}
<p style="padding: 0.6em 0 0 0">
<font size="+2">{{ article.headline }}</font><br>
{{ article.date }} </p>
<p>{{ article.content }}</p>
<p align="center" style="padding: 0 0 0.6em 0; margin-top:-12px"> {{ article.link }} </p>
{% endfor %}
