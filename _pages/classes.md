---
layout: page
title: Classes
image: '/assets/images/seated-dancer.svg'
---

{% for class in site.classes %}<div class="class">
  <h3 class="class-title">{{ class.title }}</h3>
  <div class="class-description">{{ class.content | markdownify }}</div>
  {% if class.url %}
    <a class="button" href="{{ class.book_url }}">Sign up</a>
  {% endif %}
</div>{% endfor %}
