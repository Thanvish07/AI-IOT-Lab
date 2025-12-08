---
title: "News Archive"
permalink: /year-archive/
layout: archive
author_profile: false
classes: wide
---

<style>
  /* Force full width for this page too */
  .page__inner-wrap { width: 100% !important; max-width: 100% !important; }
  .page { padding-right: 0 !important; }
  @media (min-width: 64em) { .page { display: block !important; } }
</style>

{% for post in site.posts %}
  {% include archive-single.html type="grid" %}
{% endfor %}
