---
layout: page
title: 关于
description: 你的指尖有改变世界的力量
keywords: 周博文
comments: true
menu: 关于
permalink: /about/
---

我是周博文。

一个理想主义的文艺青年。


## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## 技能关键词

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
