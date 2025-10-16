---
layout: default
title: Team
permalink: /people/
---

# Project Team

Welcome — below are people contributing to this project.

<ul class="team-list">
  {% for person in site.data.people %}
  <li class="team-member">
    {% if person.photo %}
    <img src="{{ person.photo }}" alt="{{ person.name }}" class="team-avatar" />
    {% endif %}
    <h3>{{ person.name }}</h3>
    <p><strong>{{ person.role }}</strong> — {{ person.institution }}</p>
    <p>{{ person.bio }}</p>
  </li>
  {% endfor %}
</ul>
