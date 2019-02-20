---
layout: archive
permalink: /swift/
title: "Swift Work"
author_profile: true
header:
  image: "/images/swift.jpg"
---
<ul>
  {% for post in site.categories.swift %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} {{ post.date | date_to_string }}</a>
    </li>
  {% endfor %}
</ul>
