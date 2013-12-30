---
layout: post
title: "Assignment Support!"
author: mccarthy
date: 2013-08-01 12:00:00 PM
categories: jekyll update
---

Professor Jekyll supports assignment posts!

Just include `assignment` in the post's categories and it will be listed on the [assignments page]({{ site.baseurl }}/assignments.html) instead of the home page.  Assignment posts will treat the post's date as the assignment's due date.

{% if site.python == true %}

You can also include executable Python code throughout the site.  Check [this example]({{ site.baseurl }}/assignment/2012/12/31/Assignment1.html) for more!
<div style="text-align: center">
  <img src="{{ site.baseurl}}/img/mccarthy.jpg/">
</div>
{% endif %}

Want to queue up a whole bunch of assignments but keep your students focused on only a few?  Just set `published: false` on the ones in the far future and then change it to `true` when you want students to see them.