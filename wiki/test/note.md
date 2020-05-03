---
layout: default
title: Test
date: 2020-05-03
updated: May 03, 2020
---

<h2>{{ page.title }}</h2>
<p class="first">
        {% assign crumbs = page.url | remove:'/index.html' | split: '/' %}
        <a href="/">home</a> / 
        {% for crumb in crumbs offset: 1 %}
          {% if forloop.last %}
            {{ crumb | replace:'-',' ' | remove:'.html' }}
          {% else %}
            <a href="{% assign crumb_limit = forloop.index | plus: 1 %}{% for crumb in crumbs limit: crumb_limit %}{{ crumb | append: '/' }}{% endfor %}">{{ crumb | replace:'-',' ' | remove:'.html' }}</a> /
          {% endif %}
        {% endfor %}
<p>
<p>This is a test</p>
<div class="spacer"></div>
