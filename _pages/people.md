---
title: "People"
layout: single
permalink: /people/
---

## Principal Investigator

{% assign pi = site.data.authors.scott %}

{% include people-card.html
  name=pi.name
  role=pi.role
  bio=pi.bio
  avatar=pi.avatar
  links=pi.links
%}

---

## PhD Students

<div class="people-grid">

{% assign students = site.data.authors | where: "role", "PhD Student" %}

{% for person in students %}
  {% include people-card.html
    name=person.name
    role=person.role
    bio=person.bio
    avatar=person.avatar
    links=person.links
  %}
{% endfor %}

</div>
