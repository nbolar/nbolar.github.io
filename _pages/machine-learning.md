---
layout: archive
permalink: /machine-learning/
title: "Machine Learning"
author_profile: true
header:
  image: "/images/machine learning.png"
  caption: "Photo credit: [**SmartData Collective**](https://www.smartdatacollective.com/savvy-entrepreneurs-are-using-machine-learning-to-streamline-logo-design/)"
---

<ul>
  {% for post in site.categories.machine %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} {{ post.date | date_to_string }}</a>
    </li>
  {% endfor %}
</ul>
