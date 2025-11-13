---
title: "People"
permalink: /people.html
layout: collection
collection: people
entries_layout: grid
author_profile: false # Hides the default author sidebar for a cleaner look
---

## Lab Head
{% raw %} {% assign lab_head = site.people | where: "position", "Assistant Professor (Lab Head)" | sort: "name" %} {% for person in lab_head %} {% include author-profile.html author=person type="grid" %} {% endfor %} {% endraw %}

<hr>

##PhD Students
{% raw %}
{% assign phd_students = site.people | where: "position", "PhD Student" | sort: "name" %}
{% for person in phd_students %}
  {% include author-profile.html author=person type="grid" %}
{% endfor %}
{% endraw %}
<hr>

## M.Tech Students
{% raw %} {% assign mtech_students = site.people | where: "position", "M.Tech Student" | sort: "name" %} {% for person in mtech_students %} {% include author-profile.html author=person type="grid" %} {% endfor %} {% endraw %}
<hr>

##Project Staff
{% raw %}
{% assign project_staff = site.people | where: "position", "Project Staff" | sort: "name" %}
{% for person in project_staff %}
  {% include author-profile.html author=person type="grid" %}
{% endfor %}
{% endraw %}
