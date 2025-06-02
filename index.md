---
layout: default
title: Home
---

# 개발 일지

업무 중 생긴 문제 해결과 기록을 남기는 공간입니다.

# 📚 Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>
