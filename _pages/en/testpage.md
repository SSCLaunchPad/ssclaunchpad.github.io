---
altLangPrefix: testpage
description: Testing things out
title: TEST
last_updated: 2025-11-26T21:43:11Z
---

<!-- <ul>
  {% for page in site.pages %}
    <li><a href="{{ page.url }}">{{ page.title }}</a>
    <span>{{ page.path }}</span>
    <span>{{ page.url }}</span>
    </li>
  {% endfor %}
</ul> -->

{% assign latest = site.pages | sort: "last_updated" | reverse %}

{% for p in latest %}
  <p><a href="{{ p.url }}">{{ p.title }}</a>;{{ p.path }}; {{ p.last_updated | date: "%s"  }}; {{ p.last_updated }}</p>
{% endfor %}
