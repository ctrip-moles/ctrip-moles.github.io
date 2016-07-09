---
layout: page
title: 新闻
title-en: News
permalink: /news/
---

<ul>
{% for news in site.data.news %}
    <li style="margin-top:.5em;">
        <a href="{{ news.url }}">{{ news.title }}</a>
        <br/>
        <small style="color:gray;">
            {{ news.sitename }}，
            {{ news.date }}
        </small>
        {% if news.icon %}
            <img src="{{ news.icon }}" style="height:1.2em; margin-left:.5em;"/>
        {% endif %}
    </li>
{% endfor %}
</ul>
