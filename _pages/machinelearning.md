---
layout: archive
permalink: /machine-learning/
title: "Machine Learning Posts"
author_profile: true
header:
  image = "/images/photo5.jpg"
---
{% include base_path %}
{% include group-by-array collections.posts field="tags" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  {% for post in posts %}
    {% include archive-single.html%}
  {% endfor %}
{% endfor %}
