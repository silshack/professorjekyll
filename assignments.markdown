---
layout: default
title: "Assignments"
---

## {{ site.course.number }} Assignments

Any post that has "assignment" as a category will appear here:

<ul class="posts">

{% assign assignments = site.categories.assignment %}
{% for post in assignments %}
    <li><a href=" {{ site.baseurl }}{{ post.url }} "> {{ post.title }} </a> &raquo; <span>Due: {{ post.date | date: "%a, %b %d, %y" }} </span> </li>

{% endfor %}

</ul>
