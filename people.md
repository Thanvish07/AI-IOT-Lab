---
title: "People"
permalink: /people.html
layout: collection
collection: people
entries_layout: grid
author_profile: false # Hides the default author sidebar for a cleaner look
---

## Lab Head

{% assign lab_head = site.people | where: "position", "Assistant Professor (Lab Head)" | sort: "name" %}
{% for person in lab_head %}
  {% include author-profile.html author=person type="grid" %}
{% endfor %}

<hr>

## PhD Students

{% assign phd_students = site.people | where: "position", "PhD Student" | sort: "name" %}
{% for person in phd_students %}
  {% include author-profile.html author=person type="grid" %}
{% endfor %}

<hr>

## M.Tech Students

{% assign mtech_students = site.people | where: "position", "M.Tech Student" | sort: "name" %}
{% for person in mtech_students %}
  {% include author-profile.html author=person type="grid" %}
{% endfor %}

<hr>

## Project Staff

{% assign project_staff = site.people | where: "position", "Project Staff" | sort: "name" %}
{% for person in project_staff %}
  {% include author-profile.html author=person type="grid" %}
{% endfor %}
