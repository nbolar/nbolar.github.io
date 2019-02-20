---
layout: archive
permalink: /vanet/
title: "VANET"
author_profile: true
header:
  image: "/images/vanet.jpg"
  caption: "Photo credit: [**Spiro**](http://spiroprojects.com/blog/cat-view-more.php?blogname=What-is-Vehicular-Ad-hoc-Network-(VANET)?&id=29)"
---
<ul>
  {% for post in site.categories.vanet %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} {{ post.date | date_to_string }}</a>
    </li>
  {% endfor %}
</ul>
