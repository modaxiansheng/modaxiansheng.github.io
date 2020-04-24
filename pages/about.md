---
layout: page
title: About
description: 人工智能拥抱世界
keywords: modaxiansheng, 莫大先生，宋子盈
comments: true
menu: 关于
permalink: /about/
---

我是宋子盈，花名：莫大先生，
河北科技大学2019硕士，计算机专业，机器学习方向

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'modaxiansheng.org' %}
{% endif %}
<li> 手机号：18395622998</li>
<li> 微信：   18395622998</li>
</ul>


## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

## professional experience

<ul>
{% for work in site.data.works %}
<li>{{work.time }}：{{work.company}}--{{work.work}}</li>
{% endfor %}
{% if site.url contains 'modaxiansheng.org' %}
{% endif %}
</ul>