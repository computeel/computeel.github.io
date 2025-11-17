---
layout: page
title: Team
eyebrow: ComputEEL/MatSci
subtitle: Researchers, alumni and collaborators of the group.
hero_image: /assets/images/hero-group.jpeg
hero_tags:
  - DFT
  - CALPHAD
  - Quantum materials
---

### Current members

<div class="team-grid">
{% assign members = site.data.team | where: "status", "member" %}
{% for person in members %}
  <div class="person">
    <img src="{{ person.image | relative_url }}" alt="{{ person.name }}">
    <div class="role">{{ person.role }}</div>
    <h3>{{ person.name }}</h3>
    {% if person.alias %}<p class="muted">{{ person.alias }}</p>{% endif %}
    <p class="muted">{{ person.focus }}</p>
    <div class="pill-row">
      <a class="pill" href="{{ person.url | relative_url }}">Profile</a>
    </div>
  </div>
{% endfor %}
</div>

### Former members

<div class="team-grid">
{% assign former = site.data.team | where: "status", "former" %}
{% for person in former %}
  <div class="person">
    <img src="{{ person.image | relative_url }}" alt="{{ person.name }}">
    <div class="role">{{ person.role }}</div>
    <h3>{{ person.name }}</h3>
    {% if person.alias %}<p class="muted">{{ person.alias }}</p>{% endif %}
    <p class="muted">{{ person.focus }}</p>
    <div class="pill-row">
      <a class="pill" href="{{ person.url | relative_url }}">Profile</a>
    </div>
  </div>
{% endfor %}
</div>

### Collaborators

<div class="team-grid">
{% assign collab = site.data.team | where: "status", "collaborator" %}
{% for person in collab %}
  <div class="person">
    <img src="{{ person.image | relative_url }}" alt="{{ person.name }}">
    <div class="role">{{ person.role }}</div>
    <h3>{{ person.name }}</h3>
    {% if person.alias %}<p class="muted">{{ person.alias }}</p>{% endif %}
    <p class="muted">{{ person.focus }}</p>
    <div class="pill-row">
      <a class="pill" href="{{ person.url | relative_url }}">Profile</a>
    </div>
  </div>
{% endfor %}
</div>

Looking for partnerships or positions? [Contact us]({{ '/contact/' | relative_url }}) for undergraduate research, graduate school or collaboration opportunities.
