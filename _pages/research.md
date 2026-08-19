---
layout: page
permalink: /research/
title: research
nav: true
nav_order: 2
display_categories: [work, fun]
horizontal: false
---

<div class="publications">

<h2>Peer-Reviewed Articles</h2>
{% bibliography --query @*[category=peer-reviewed] %}

<h2>Book Chapters</h2>
{% bibliography --query @*[category=book-chapter] %}

</div>

<div class="projects">
<h2>Current Projects</h2>
{% assign sorted_projects = site.projects | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3">
{% for project in sorted_projects %}
  {% include projects.liquid %}
{% endfor %}
</div>
</div>