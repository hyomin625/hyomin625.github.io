---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  document.querySelectorAll("abbr.badge").forEach(function (badge) {
    const text = badge.textContent.trim();
    if (text === "Under Review") {
      badge.style.backgroundColor = "#e91e8c";
    } else if (text === "Domestic") {
      badge.style.backgroundColor = "#1565c0";
    }
  });
});
</script>
