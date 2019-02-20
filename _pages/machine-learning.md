---
layout: archive
permalink: /machine-learning/
title: "Machine Learning"
author_profile: true
header:
  image: "/images/photo4.jpg"
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
---
<!-- {% for post in site.categories.machine %}
  <a href="{{ post.url }}">
    <h2>{{ post.title }}</h2>
    <p>{{ post.date | date_to_string }}</p>
  </a>
{% endfor %} -->
<ul>
  {% for post in site.categories.machine %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
