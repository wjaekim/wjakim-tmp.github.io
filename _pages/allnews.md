---
title: "News - Quantitative Psychology Active Learning Lab"
layout: newslay
excerpt: "News in Quantitative Psychology Active Learning Lab"
permalink: /allnews/
---
# News

{% for article in site.data.news %}
<p style="padding: 1em 1em 0 0">{{ article.date }} <br>
<font size="5">{{ article.headline }}</font><br>
<font size="3">{{ article.content }}</font></p>
<p align="center" style="padding: 0 1em 1em 0"><font size="3">{{ article.link }}</font></p>
{% endfor %}
