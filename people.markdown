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

{{ thisauthor.about }}  Find {{ thisauthor.name }} on <a href="http://twitter.com/{{thisauthor.twitter}}">Twitter</a>, <a href="http://github.com/{{thisauthor.github}}">Github</a>, and <a href="{{thisauthor.website}}">on the web</a>.

<ul class="posts">
    {% for p in site.posts do %}
	{% for authors in p.author %}
      {% if authors == adata %}
<li><span>=>  <a href="{{ site.baseurl }}{{p.url}}">{{p.title}}</a> - {{ p.date | date_to_string }}</span></li>
      {% endif %}
	{% endfor %}
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

{{ thisauthor.about }}  Find {{ thisauthor.name }} on <a href="http://twitter.com/{{thisauthor.twitter}}">Twitter</a>, <a href="http://github.com/{{thisauthor.github}}">Github</a>, and <a href="{{thisauthor.website}}">on the web</a>.

    {% for p in site.posts do %}
      {% for authors in p.author %}
      {% if authors == adata %}
* [{{ p.title }}]({{ site.baseurl }}{{p.url}})
      {% endif %}
	{% endfor %}
    {% endfor %}
  {% endif %}
{% endfor %}


