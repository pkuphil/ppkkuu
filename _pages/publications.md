---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 2
abs_open: false

scholar:
  sort_by: year
  order: descending
---

<!-- _pages/publications.md -->

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
