---
layout: publications
permalink: /talks/
title: Talks
tagline: Talks that I have given
tags: [talks]
comments: false
---

<h4 style="margin-bottom:0px;padding-top:10px;">Talks</h4>
<ul class="talks_list">

{% assign number_printed = 0 %}
{% assign sorted_talks = (site.data.talks | sort: 'year') | reverse %}

{% for talk in sorted_talks %}

<li><p>
<b>{{ talk.month }}/{{ talk.year }}:</b> ({{talk.type}}) "{{ talk.title }}".
Talk at {{talk.venue}} ({{talk.location}}). [<a href="/docs/slides/{{ talk.slides }}" target="_blank">{{ talk.slidetype }}</a>]
</p>
</li>

{% endfor %}

</ul>