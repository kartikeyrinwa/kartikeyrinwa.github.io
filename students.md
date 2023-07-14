---
layout: publications
permalink: /students/
title: My Students
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
{% if "kartikey.sharma" in sdeg.internal_advisor %}

<li ><p>
<b>{{ stud.first_name stud.last_name}}</b> 
<b>Thesis: {{ sdeg.thesis.title }}</b> 
</li>

{% endif %}
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
{% if "kartikey.sharma" in sdeg.internal_advisor %}

<li ><p>
<b>{{ stud.first_name stud.last_name}}</b> 
<b>Thesis: {{ sdeg.thesis.title }}</b> 
</li>

{% endif %}
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
{% if "kartikey.sharma" in sdeg.internal_advisor %}

<li ><p>
<b>{{ stud.first_name stud.last_name}}</b> 
<b>Thesis: {{ sdeg.thesis.title }}</b> 
</li>

{% endif %}
{% endif %}
{% endfor %}
{% endfor %}

</ul>






