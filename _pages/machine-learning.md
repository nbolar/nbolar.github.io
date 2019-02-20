---
layout: archive
permalink: /machine-learning/
title: "Machine Learning"
author_profile: true
header:
  image: "/images/photo4.jpg"
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
---

<ul>
  {% for post in site.categories.machine %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} {{ post.date | date_to_string }}</a>
    </li>
  {% endfor %}
</ul>
