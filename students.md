---
layout: publications
permalink: /students/
title: Students
tags: [students]
modified: 14-7-2023
comments: false
---

List of students I have worked with:

<!-- Bachelors -->

<h4 style="margin-bottom:0px;padding-top:10px;">Bachelors</h4>
<ul class="bachelor_list">

{% assign number_printed = 0 %}
{% for stud in site.data.student_list %}
{% for sdeg in stud.degrees %}
{% if sdeg.type == "bsc" %}

<li ><p>
<b>{{ stud.first_name }} {{ stud.last_name }}</b> 
<br>
<b>Thesis</b> : {{ sdeg.thesis.title }}
</p>
</li>

{% endif %}
{% endfor %}
{% endfor %}

</ul>

<!-- Masters -->

<h4 style="margin-bottom:0px;padding-top:10px;">Masters</h4>
<ul class="master_list">

{% assign number_printed = 0 %}
{% for stud in site.data.student_list %}
{% for sdeg in stud.degrees %}
{% if sdeg.type == "msc" %}

<li ><p>
<b>{{ stud.first_name }} {{ stud.last_name}}</b> 
<br>
<b>Thesis</b>: {{ sdeg.thesis.title }} 
</p>
</li>

{% endif %}
{% endfor %}
{% endfor %}

</ul>


<!-- Ph.D. -->

<h4 style="margin-bottom:0px;padding-top:10px;">Ph.D.</h4>
<ul class="phd_list">

{% assign number_printed = 0 %}
{% for stud in site.data.student_list %}
{% for sdeg in stud.degrees %}
{% if sdeg.type == "phd" %}

<li ><p>
<b>{{ stud.first_name }} {{ stud.last_name}}</b> 
<br>
<b>Thesis</b>: {{ sdeg.thesis.title }} 
</p>
</li>

{% endif %}
{% endfor %}
{% endfor %}

</ul>






