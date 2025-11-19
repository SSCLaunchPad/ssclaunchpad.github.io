---
altLangPrefix: testpage
description: Testing things out
title: TEST
---

<!-- <ul>
  {% for page in site.pages %}
    <li><a href="{{ page.url }}">{{ page.title }}</a>
    <span>{{ page.path }}</span>
    <span>{{ page.url }}</span>
    </li>
  {% endfor %}
</ul> -->

{% assign latest = site.pages | sort: "last_modified_at_str" | reverse %}

{% for p in latest %}
  <p><a href="{{ p.url }}">{{ p.title }}</a>;{{ p.path }}; {{ p.last_modified_at }}</p>
{% endfor %}