---
layout: archive
title: "杂谈"
permalink: /zh/stories/
author_profile: true
lang: zh
---

{% include base_path %}

故事、随笔，以及偶尔的思考。

{% assign stories = site.stories | where: "lang", "zh" | sort: "date" | reverse %}

{% if stories.size > 0 %}
  {% for post in stories %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
暂时还没有发布文章。
{% endif %}
