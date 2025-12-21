---
layout: page
permalink: /zhiweitalks/
title: zhiweitalks
description:
nav: false
nav_order: 3
abs_open: true
---

<!-- _pages/zhiweitalks.md -->

{% include bib_search.liquid %}

<div class="publications talks-page">

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

<style>
/* =========================================================
   zhiweitalks: Hide left thumbnail / journal image
   Only applies to this page because of .talks-page
   ========================================================= */

/* 1) Try to hide common thumbnail containers/imgs used by academic Jekyll themes */
.publications.talks-page img,
.publications.talks-page .pub-image,
.publications.talks-page .publication-image,
.publications.talks-page .teaser,
.publications.talks-page .thumbnail,
.publications.talks-page .preview,
.publications.talks-page .image,
.publications.talks-page .left,
.publications.talks-page .media-left,
.publications.talks-page .paper-thumbnail,
.publications.talks-page .venue-thumbnail {
  display: none !important;
}

/* 2) Remove leftover spacing if the layout reserved a left column */
.publications.talks-page .pub-content,
.publications.talks-page .publication-content,
.publications.talks-page .entry-content,
.publications.talks-page .bib-entry,
.publications.talks-page .bib-entry .content,
.publications.talks-page .reference,
.publications.talks-page .reference .content {
  margin-left: 0 !important;
  padding-left: 0 !important;
}

/* 3) If each item is a grid/flex with 2 columns, force it to 1 column */
.publications.talks-page .publication,
.publications.talks-page .pub,
.publications.talks-page .entry,
.publications.talks-page .reference {
  grid-template-columns: 1fr !important;
}

/* 4) In case some themes wrap image in a <figure> */
.publications.talks-page figure {
  display: none !important;
}
</style>
