---
title: "Jenkins Suite"
layout: category
permalink: /categories/
author_profile: true
taxonomy: jenkinssuite
sidebar:
  nav: "categories"
---

{% if site.tag_archive.type and page.tags[0] %}
  {% include tag-list.html %}
{% endif %}

{% if site.category_archive.type and page.categories[0] %}
  {% include category-list.html %}
{% endif %}
