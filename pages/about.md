---
layout: page
title: About
description: 过犹不及，事缓则圆
keywords: 于是，
comments: true
menu: 关于
permalink: /about/
---

过犹不及，事缓则圆。



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
