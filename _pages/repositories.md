---
layout: page
permalink: /repositories/
title: repositories
description: Welcome to my repository page! Here you'll find a collection of my projects, code snippets, and experiments. Each repository showcases my work in various domains, from data analysis and machine learning to web development and automation. Feel free to explore, fork, and contribute!
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}


## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
