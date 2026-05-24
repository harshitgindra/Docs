---
layout: default
title: Home
---

# App Docs

Welcome to the public documentation hub for all apps by Harshit Gindra. Select an app below to view its documentation.

<div class="app-grid">
{% for app in site.data.apps %}
  <div class="app-card">
    <a href="{{ app.url | relative_url }}">{{ app.name }}</a>
    <p>{{ app.description }}</p>
  </div>
{% endfor %}
</div>
