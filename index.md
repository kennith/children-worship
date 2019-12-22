---
layout: default
---
## 2019-09-22

[PPT](https://docs.google.com/presentation/d/1M65Y8BtOjLbMkIrCwABv_LMCVIygp6Ol0ukEG6v78iE/edit?usp=drivesdk)


<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | absolute_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
