---
layout: post-index
permalink: /talks/
title: Talks
tagline: Talks that I have given
tags: [talks]
comments: false
---

<h4 style="margin-bottom:0px;padding-top:10px;">Talks</h4>
<ul class="talks_list">

{% assign number_printed = 0 %}
{% for talk in site.data.talks %}

<li ><p>
<b>{{ talk.month }} / {{ talk.year }}:</b> ({{talk.type}}) "{{ talk.title }}"
Talk at {{talk.venue}} ({{talk.location}}). [{{ <a href="/docs/slides/{{ talk.slides }}" target="_blank">slides</a> }}]
</p>
</li>

{% endfor %}

</ul>