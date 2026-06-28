---
layout: archive
title: "短篇小说"
permalink: /zh/stories/
author_profile: true
lang: zh
---

{% include base_path %}

这里会放一些短篇小说、片段和偶尔的叙事练习。

{% assign stories = site.stories | where: "lang", "zh" | sort: "date" | reverse %}

{% if stories.size > 0 %}
  {% for post in stories %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
暂时还没有发布小说。
{% endif %}
