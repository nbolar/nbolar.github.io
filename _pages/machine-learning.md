---
layout: posts
permalink: /machine-learning/
title: "Machine Learning"
author_profile: true
tags: [tweets, sentiment classifier]
header:
  image: "/images/photo4.jpg"
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
---
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
