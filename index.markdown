---
layout: default
title: {{ site.data.linkedin_profile.name | default: "Home" }}
description: Personal portfolio website of {{ site.data.linkedin_profile.name }}, {{ site.data.linkedin_profile.title | default: "displaying professional experience, skills, and projects" }}.
---

<header class="profile-header">
  <h1>{{ site.data.linkedin_profile.name }}</h1>
  {% if site.data.linkedin_profile.pronouns %}
    <p><em>({{ site.data.linkedin_profile.pronouns }})</em></p>
  {% endif %}
  <p>{{ site.data.linkedin_profile.title }}</p>
  {% if site.data.linkedin_profile.location %}
    <p>{{ site.data.linkedin_profile.location }}</p>
  {% endif %}
  {% if site.data.linkedin_profile.contact_info %}
    <p>Contact: <a href="https://{{ site.data.linkedin_profile.contact_info }}" target="_blank">{{ site.data.linkedin_profile.contact_info }}</a></p>
  {% endif %}
</header>

{% include about.html %}
{% include skills.html %}
{% include experience.html %}
{% include education.html %}
{% include publications.html %}
{% include honors.html %}
