---
layout: publications
permalink: /other/
title: Other
tags: [other]
modified: 15-4-2026
comments: false
---

<!-- BTP -->

<h4 style="margin-bottom:0px;padding-top:10px;">Bachelor Thesis Projects</h4>
<ul class="_list">

{% assign number_printed = 0 %}
{% for proj in site.data.project_list %}
{% if proj.type == "btp" %}
{% if proj.year == 2026 %}

<li ><p>
<b>{{ proj.title }}</b> 
<br>
<b>Description</b> : {{ proj.description }}
</p>
</li>

{% endif %}
{% endif %}
{% endfor %}

</ul>






