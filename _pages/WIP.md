---
layout: page
permalink: /WIP/
title: W.I.P.
nav: true
nav_order: 5
abs_open: true
---

# Work in Progress


<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

{% if page.abs_open %}
<script>
  window.addEventListener("load", () => {
    document.querySelectorAll(".publications a.abstract.btn").forEach((btn) => {
      if (btn.textContent.trim().toLowerCase() === "abs") btn.click();
    });
  });
</script>
{% endif %}

</div>
