---
layout: page
permalink: /publications/
title: publications
nav: false
nav_order: 2
---

<div class="publications">

<h2>Peer-Reviewed Articles</h2>
{% bibliography --query @*[category=peer-reviewed] %}

<h2>Book Chapters</h2>
{% bibliography --query @*[category=book-chapter] %}

</div>