---
layout: page
permalink: /WIP/
nav_title: w.i.p.
nav: true
nav_order: 3
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
