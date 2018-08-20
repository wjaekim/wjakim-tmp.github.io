---
title: "News - Quantitative Psychology Active Learning Lab"
layout: gridlay
excerpt: "News in Quantitative Psychology Active Learning Lab"
permalink: /allnews/
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<font size="5">{{ article.headline }}</font><br>
  <font size="1">{{ article.content }}</font></p>
{% endfor %}
