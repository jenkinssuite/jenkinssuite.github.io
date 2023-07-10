---
title: "Jenkins Suite [en]"
layout: category
permalink: /categories/en
author_profile: true
taxonomy: jenkinssuite_en
sidebar:
  nav: "categories"
---

{% if site.tag_archive.type and page.tags[0] %}
  {% include tag-list.html %}
{% endif %}

{% if site.category_archive.type and page.categories[0] %}
  {% include category-list.html %}
{% endif %}
