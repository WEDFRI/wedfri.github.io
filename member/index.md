---
layout: default
title: Members
description: WEDFRI Members
main: true
project-header: true
header-img: img/about.jpg
---

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
    {% if page.member == true %}
        {% include member-list.html %}
    {% endif %}
{% endfor %}

</ul>
