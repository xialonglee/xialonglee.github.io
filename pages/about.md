---
layout: page
title: About
description: Xialong Lee的个人博客
keywords: xialonglee, Xialonglee, Xialong Lee
comments: true
menu: 关于
permalink: /about/
---

经验心得、人生感悟汇总

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
