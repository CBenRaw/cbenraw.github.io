---
title:  "cbenraw"
---

# Greetings, and a hearty welcome

## Blog posts

<span>
  {% for post in site.posts %}
    <p>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </p>
  {% endfor %}
</span>


### Tags

{% for tag in site.tags %}
  <h4>{{ tag[0] }}</h4>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}