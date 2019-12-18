---
layout: single
title: 'THE LOOPS BROTHER'
tags: testing 
---

<div>
<h1> PHOTOS </h1>
{% for file in site.static_files %}
    {% if file.path contains 'photos' %}
        {% if file.extname contains '.jpg' %}
            <div><a href="https://michaelscottkittenco.github.io/{{ file.path }}">{{ file.basename }}</a></div>
        {% endif %}
    {% endif %}
{% endfor %}
</div>