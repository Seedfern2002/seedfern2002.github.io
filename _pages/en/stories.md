---
layout: archive
title: "Miscellany"
permalink: /en/stories/
author_profile: true
lang: en
---

{% include base_path %}

Stories, essays, and occasional reflections.

{% assign stories = site.stories | where: "lang", "en" | sort: "date" | reverse %}

{% if stories.size > 0 %}
  {% for post in stories %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
No writing posted yet.
{% endif %}
