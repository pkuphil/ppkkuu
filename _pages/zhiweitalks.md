---
layout: page
permalink: /zhiweitalks/
title: zhiweitalks
nav: true
nav_order: 3
abs_open: true
---

{% include bib_search.liquid %}

<div class="publications">

{% bibliography --file talks --sort_by year --order descending %}

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
