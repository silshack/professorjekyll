---
layout: default
title: "People"
---


### {{ site.course.title }} Instructors  
{% for a in site.authors do %}
  {% assign adata = a[0] %}
  {% assign thisauthor = site.authors[adata] %}
  
  {% if thisauthor.prof == true %}
#### {{ thisauthor.name }}
{{ thisauthor.about }}

<ul class="posts">
    {% for p in site.posts do %}
      {% if p.author == adata %}
<li><span>=>  <a href="{{ site.url }}{{p.url}}">{{p.title}}</a> - {{ p.date | date_to_string }}</span></li>
      {% endif %}
    {% endfor %}
</ul>

  {% endif %}
{% endfor %}

### {{ site.course.title }} Participants
{% for a in site.authors do %}
  {% assign adata = a[0] %}
  {% assign thisauthor = site.authors[adata] %}
  
  {% if thisauthor.prof != true %}
#### {{ thisauthor.name }}
{{ thisauthor.about }}
    {% for p in site.posts do %}
      {% if p.author == adata %}
* [{{ p.title }}]({{ site.url }}{{p.url}})
      {% endif %}
    {% endfor %}
  {% endif %}
<br/>
{% endfor %}


