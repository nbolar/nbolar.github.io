---
layout: archive
permalink: /machine-learning/
title: "Machine Learning"
author_profile: true
header:
  image: "/images/machine learning.png"
  caption: "Photo credit: [**IE Exponential Learning**](https://www.ie.edu/exponential-learning/blog/data-science/machine-learning-marketing/)"
---

<ul>
  {% for post in site.categories.machine %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} {{ post.date | date_to_string }}</a>
    </li>
  {% endfor %}
</ul>
