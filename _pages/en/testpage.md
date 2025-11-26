---
altLangPrefix: testpage
description: Testing things out
title: TEST
last_updated: 2025-11-26T19:59:06Z
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
  <p><a href="{{ p.url }}">{{ p.title }}</a>;{{ p.path }}; {{ p.last_modified_at }}</p>
{% endfor %}
