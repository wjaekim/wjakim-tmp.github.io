---
title: "News - Quantitative Psychology Active Learning Lab"
layout: gridlay
excerpt: "News in Quantitative Psychology Active Learning Lab"
permalink: /allnews/
---

{% for article in site.data.news %}
<p style="padding: 1em 1em 1em 0">{{ article.date }} <br>
<font size="5">{{ article.headline }}</font><br>
<font size="4">{{ article.content }}</font></p>
{% endfor %}
