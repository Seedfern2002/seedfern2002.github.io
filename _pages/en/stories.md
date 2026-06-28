---
layout: archive
title: "Stories"
permalink: /en/stories/
author_profile: true
lang: en
---

{% include base_path %}

A place for short fiction and occasional narrative sketches.

{% assign stories = site.stories | where: "lang", "en" | sort: "date" | reverse %}

{% if stories.size > 0 %}
  {% for post in stories %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
No stories posted yet.
{% endif %}
