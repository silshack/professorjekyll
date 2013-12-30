---
layout: post
author: einstein
duedate: 2014-04-20
categories: assignment
title: Assignment 1
---

## Assignment #1

{% if site.python == true do %}

<form> 
	<textarea id="code" rows="12" cols="80">
print "Write python code for your students to run here."
	</textarea>
	<button type="button" onclick="runit()">Run</button> 
</form> 

<pre id="output">Press Run to see the output of the code above</pre>

{% else %}

Your assignments, formatted in markdown, go here!

{% endif %}