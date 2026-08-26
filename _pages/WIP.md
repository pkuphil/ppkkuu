---
layout: default
title: research
permalink: /research/
nav: true
nav_order: 2
description: Research in philosophy of perception, institutional objects, and temporal externalism.
---

<style>
  /* =========================================================
     RESEARCH PAGE
     ========================================================= */

  html {
    scroll-behavior: smooth;
  }

  .research-page {
    --research-blue: #315f94;
    --research-blue-soft: rgba(49, 95, 148, 0.055);

    --research-green: #70854d;
    --research-green-soft: rgba(112, 133, 77, 0.055);

    --research-orange: #c3653d;
    --research-orange-soft: rgba(195, 101, 61, 0.055);

    width: 100%;
    max-width: 1080px;

    margin: 0 auto;
    padding: 1.65rem 0 4rem 0;

    font-family: inherit;
    color: var(--global-text-color, inherit);
  }


  /* =========================================================
     HERO
     ========================================================= */

  .research-hero {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 245px;
    align-items: center;

    gap: 4rem;

    margin: 0 0 3.15rem 0;
  }

  .research-hero-copy {
    min-width: 0;
  }

  .research-title {
    margin: 0 0 1.45rem 0;

    font-family: inherit;
    font-size: clamp(3rem, 6vw, 4.35rem);
    font-weight: 400;
    line-height: 1.02;

    letter-spacing: -0.035em;

    color: var(--global-text-color, inherit);
  }

  .research-intro {
    max-width: 720px;

    margin: 0;

    font-size: 1rem;
    font-weight: 400;
    line-height: 1.72;

    color: var(--global-text-color, inherit);
  }


  /* =========================================================
     RESEARCH DIAGRAM
     ========================================================= */

  .research-diagram {
    width: 230px;
    height: 230px;

    justify-self: end;

    opacity: 0.95;
  }

  .research-diagram svg {
    display: block;

    width: 100%;
    height: 100%;
  }


  /* =========================================================
     TOP PROJECT INDEX
     ========================================================= */

  .research-index {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));

    width: 100%;

    margin: 0 0 0 0;

    border-top: 1px solid var(--global-divider-color, #dedede);
    border-bottom: 1px solid var(--global-divider-color, #dedede);
  }

  .research-index-item {
    position: relative;

    display: flex;
    align-items: baseline;

    gap: 0.75rem;

    min-width: 0;

    padding: 0.95rem 1rem 0.92rem 0;

    color: var(--global-text-color, inherit) !important;

    background: transparent !important;

    text-decoration: none !important;

    border: 0 !important;
    border-bottom: 2px solid transparent !important;

    box-shadow: none !important;

    transition:
      border-color 0.16s ease,
      color 0.16s ease;
  }

  .research-index-item + .research-index-item {
    padding-left: 1.25rem;
  }

  .research-index-item:hover,
  .research-index-item:focus {
    background: transparent !important;

    text-decoration: none !important;

    border-bottom-color: currentColor !important;

    box-shadow: none !important;
  }

  .research-index-number {
    flex: 0 0 auto;

    font-size: 1.02rem;
    font-weight: 400;
    line-height: 1;
  }

  .research-index-label {
    min-width: 0;

    font-size: 0.9rem;
    font-weight: 400;
    line-height: 1.35;
  }

  .research-index-item.blue {
    color: var(--research-blue) !important;
  }

  .research-index-item.green {
    color: var(--research-green) !important;
  }

  .research-index-item.orange {
    color: var(--research-orange) !important;
  }


  /* =========================================================
     PROJECT SECTION
     ========================================================= */

  .research-project {
    --accent: var(--research-blue);
    --accent-soft: var(--research-blue-soft);

    display: grid;
    grid-template-columns: 170px minmax(0, 1fr);

    width: 100%;

    border-bottom: 1px solid var(--global-divider-color, #dedede);

    scroll-margin-top: 5.5rem;
  }

  .research-project.project-blue {
    --accent: var(--research-blue);
    --accent-soft: var(--research-blue-soft);
  }

  .research-project.project-green {
    --accent: var(--research-green);
    --accent-soft: var(--research-green-soft);
  }

  .research-project.project-orange {
    --accent: var(--research-orange);
    --accent-soft: var(--research-orange-soft);
  }


  /* =========================================================
     LEFT RAIL
     ========================================================= */

  .research-project-rail {
    position: relative;

    padding: 2.15rem 1.6rem 2.5rem 1.35rem;

    background: var(--accent-soft);
  }

  .research-project-rail-inner {
    position: sticky;
    top: 5.4rem;
  }

  .research-project-number {
    margin: 0 0 1rem 0;

    font-size: 3.05rem;
    font-weight: 300;
    line-height: 1;

    letter-spacing: -0.04em;

    color: var(--accent);
  }

  .research-project-rail-line {
    width: 3.2rem;
    height: 1px;

    margin: 0 0 0.85rem 0;

    background: var(--accent);

    opacity: 0.48;
  }

  .research-project-kicker {
    margin: 0;

    font-size: 0.71rem;
    font-weight: 500;
    line-height: 1.35;

    letter-spacing: 0.09em;
    text-transform: uppercase;

    color: var(--accent);
  }


  /* =========================================================
     PROJECT BODY
     ========================================================= */

  .research-project-body {
    min-width: 0;

    padding: 2.15rem 0 2.7rem 2.7rem;
  }

  .research-project-heading {
    margin: 0 0 0.35rem 0;

    font-family: inherit;
    font-size: 1.6rem;
    font-weight: 500;
    line-height: 1.25;

    letter-spacing: -0.018em;

    color: var(--global-text-color, inherit);
  }

  .research-project-question {
    max-width: 710px;

    margin: 0 0 1.4rem 0;

    font-size: 0.98rem;
    font-style: italic;
    font-weight: 400;
    line-height: 1.5;

    color: var(--accent);
  }

  .research-project-overview {
    max-width: 760px;
  }

  .research-project-overview p {
    margin: 0 0 0.9rem 0;

    font-size: 0.96rem;
    font-weight: 400;
    line-height: 1.66;

    color: var(--global-text-color, inherit);
  }

  .research-project-overview p:last-child {
    margin-bottom: 0;
  }


  /* =========================================================
     KEYWORDS / RESEARCH FOCUS
     ========================================================= */

  .research-focus {
    display: flex;
    flex-wrap: wrap;

    gap: 0.25rem 0;

    margin: 1.25rem 0 2.15rem 0;

    font-size: 0.7rem;
    font-weight: 500;
    line-height: 1.45;

    letter-spacing: 0.055em;
    text-transform: uppercase;

    color: var(--accent);
  }

  .research-focus span {
    white-space: nowrap;
  }

  .research-focus span:not(:last-child)::after {
    content: " · ";

    margin: 0 0.55rem;

    color: var(--global-text-color-light, #a3a3a3);
  }


  /* =========================================================
     SMALL SECTION LABEL
     ========================================================= */

  .research-subheading {
    margin: 2.15rem 0 0.72rem 0;

    font-size: 0.72rem;
    font-weight: 500;
    line-height: 1.35;

    letter-spacing: 0.085em;
    text-transform: uppercase;

    color: var(--global-text-color-light, #777);
  }


  /* =========================================================
     PUBLIC / CURRENT WORK LIST
     ========================================================= */

  .research-work-list {
    width: 100%;

    margin: 0;
    padding: 0;

    border-top: 1px solid var(--global-divider-color, #e2e2e2);
  }

  .research-work {
    margin: 0;
    padding: 0.82rem 0 0.88rem 0;

    border-bottom: 1px solid var(--global-divider-color, #e7e7e7);
  }

  .research-work:last-child {
    border-bottom: 0;
  }

  .research-work-head {
    display: flex;
    align-items: baseline;

    width: 100%;

    gap: 1rem;
  }

  .research-work-title {
    min-width: 0;
    flex: 1 1 auto;

    margin: 0;

    font-size: 0.97rem;
    font-weight: 600;
    line-height: 1.43;

    color: var(--global-text-color, inherit);
  }

  .research-work-status {
    flex: 0 0 auto;

    margin-left: auto;

    font-size: 0.78rem;
    font-weight: 400;
    font-style: italic;

    line-height: 1.4;

    white-space: nowrap;
    text-align: right;

    color: var(--global-text-color-light, #777);
  }

  .research-work-meta {
    margin-top: 0.12rem;

    font-size: 0.84rem;
    font-weight: 400;
    line-height: 1.45;

    color: var(--global-text-color-light, #747474);
  }

  .research-work-journal {
    font-style: italic;

    color: var(--global-text-color, inherit);
  }

  .research-work-link::before {
    content: " · ";

    color: var(--global-text-color-light, #aaa);
  }

  .research-work-link {
    margin-left: 0.15rem;
  }

  .research-work-link a,
  .research-work-link a:link,
  .research-work-link a:visited {
    color: var(--accent) !important;

    background: transparent !important;

    text-decoration-line: underline !important;
    text-decoration-color: transparent !important;
    text-decoration-thickness: 1px !important;
    text-underline-offset: 0.17em;

    border: 0 !important;
    border-bottom: 0 !important;

    box-shadow: none !important;
  }

  .research-work-link a:hover,
  .research-work-link a:focus {
    color: var(--accent) !important;

    background: transparent !important;

    text-decoration-color: currentColor !important;

    border: 0 !important;
    border-bottom: 0 !important;

    box-shadow: none !important;
  }

  .research-work-summary {
    max-width: 735px;

    margin: 0.36rem 0 0 0;

    font-size: 0.86rem;
    font-weight: 400;
    line-height: 1.55;

    color: var(--global-text-color-light, #686d72);
  }


  /* =========================================================
     CURRENT / UNPUBLISHED WORK
     ========================================================= */

  .research-work.private-work .research-work-title {
    font-weight: 500;
  }

  .research-work.private-work .research-work-summary {
    max-width: 690px;
  }


  /* =========================================================
     MORE DETAILS
     ========================================================= */

  .research-more {
    margin: 1.45rem 0 0 0;
    padding: 0;
  }

  .research-more summary {
    display: inline-flex;
    align-items: center;

    gap: 0.48rem;

    margin: 0;
    padding: 0;

    cursor: pointer;

    list-style: none;

    font-size: 0.84rem;
    font-weight: 400;

    color: var(--accent);

    user-select: none;
  }

  .research-more summary::-webkit-details-marker {
    display: none;
  }

  .research-more summary::after {
    content: "+";

    font-size: 1rem;
    font-weight: 300;
    line-height: 1;
  }

  .research-more[open] summary::after {
    content: "−";
  }

  .research-more summary:hover {
    text-decoration: underline;
    text-decoration-thickness: 1px;
    text-underline-offset: 0.18em;
  }

  .research-more-content {
    max-width: 735px;

    margin: 1rem 0 0 0;
    padding-left: 1rem;

    border-left: 1px solid var(--global-divider-color, #dedede);
  }

  .research-more-content p {
    margin: 0 0 0.85rem 0;

    font-size: 0.9rem;
    font-weight: 400;
    line-height: 1.64;

    color: var(--global-text-color, inherit);
  }

  .research-more-content p:last-child {
    margin-bottom: 0;
  }


  /* =========================================================
     COMPACT SECONDARY PROJECT
     ========================================================= */

  .research-project.compact .research-project-body {
    padding-top: 2.05rem;
    padding-bottom: 2.4rem;
  }

  .research-project.compact .research-focus {
    margin-bottom: 1.6rem;
  }


  /* =========================================================
     DARK MODE
     ========================================================= */

  html[data-theme="dark"] .research-page,
  body[data-theme="dark"] .research-page {
    --research-blue: #7ea2d1;
    --research-blue-soft: rgba(126, 162, 209, 0.055);

    --research-green: #a0b97b;
    --research-green-soft: rgba(160, 185, 123, 0.055);

    --research-orange: #df8b68;
    --research-orange-soft: rgba(223, 139, 104, 0.055);
  }

  @media (prefers-color-scheme: dark) {
    .research-page {
      --research-blue: #7ea2d1;
      --research-blue-soft: rgba(126, 162, 209, 0.055);

      --research-green: #a0b97b;
      --research-green-soft: rgba(160, 185, 123, 0.055);

      --research-orange: #df8b68;
      --research-orange-soft: rgba(223, 139, 104, 0.055);
    }

    .research-work-summary {
      color: rgba(229, 231, 235, 0.67);
    }

    .research-work-status,
    .research-work-meta,
    .research-subheading {
      color: rgba(229, 231, 235, 0.58);
    }
  }


  /* =========================================================
     TABLET
     ========================================================= */

  @media (max-width: 900px) {

    .research-hero {
      grid-template-columns: minmax(0, 1fr) 190px;
      gap: 2rem;
    }

    .research-diagram {
      width: 185px;
      height: 185px;
    }

    .research-project {
      grid-template-columns: 135px minmax(0, 1fr);
    }

    .research-project-rail {
      padding-left: 1rem;
      padding-right: 1rem;
    }

    .research-project-body {
      padding-left: 2rem;
    }

  }


  /* =========================================================
     MOBILE
     ========================================================= */

  @media (max-width: 650px) {

    .research-page {
      padding-top: 0.6rem;
      padding-bottom: 3rem;
    }


    /* ---------- Hero ---------- */

    .research-hero {
      display: block;

      margin-bottom: 2.25rem;
    }

    .research-title {
      margin-bottom: 1.15rem;

      font-size: 2.75rem;
      line-height: 1.04;
    }

    .research-intro {
      font-size: 0.96rem;
      line-height: 1.65;
    }

    .research-diagram {
      width: 155px;
      height: 155px;

      margin: 1.55rem auto 0 auto;
    }


    /* ---------- Index ---------- */

    .research-index {
      display: block;

      margin-bottom: 0;
    }

    .research-index-item,
    .research-index-item + .research-index-item {
      width: 100%;

      padding: 0.72rem 0;

      border-bottom: 1px solid var(--global-divider-color, #e2e2e2) !important;
    }

    .research-index-item:last-child {
      border-bottom: 0 !important;
    }

    .research-index-item:hover,
    .research-index-item:focus {
      border-bottom-color: var(--global-divider-color, #e2e2e2) !important;
    }

    .research-index-number {
      width: 1.55rem;

      font-size: 0.92rem;
    }

    .research-index-label {
      font-size: 0.88rem;
    }


    /* ---------- Projects ---------- */

    .research-project,
    .research-project.compact {
      display: block;

      scroll-margin-top: 4.5rem;
    }

    .research-project-rail {
      padding: 1.75rem 0 0.6rem 0;

      background: transparent;
    }

    .research-project-rail-inner {
      position: static;

      display: flex;
      align-items: baseline;

      gap: 0.75rem;
    }

    .research-project-number {
      margin: 0;

      font-size: 1.52rem;
      font-weight: 400;
    }

    .research-project-rail-line {
      display: none;
    }

    .research-project-kicker {
      font-size: 0.68rem;
    }

    .research-project-body,
    .research-project.compact .research-project-body {
      padding: 0 0 2.25rem 0;
    }

    .research-project-heading {
      margin-top: 0.15rem;

      font-size: 1.38rem;
      line-height: 1.28;
    }

    .research-project-question {
      margin-bottom: 1.2rem;

      font-size: 0.93rem;
    }

    .research-project-overview p {
      font-size: 0.93rem;
      line-height: 1.62;
    }

    .research-focus {
      margin-top: 1.05rem;
      margin-bottom: 1.7rem;

      font-size: 0.65rem;
      line-height: 1.55;
    }


    /* ---------- Work ---------- */

    .research-work {
      padding-top: 0.76rem;
      padding-bottom: 0.8rem;
    }

    .research-work-head {
      display: block;
    }

    .research-work-title {
      font-size: 0.94rem;
      line-height: 1.42;
    }

    .research-work-status {
      display: block;

      margin: 0.16rem 0 0 0;

      font-size: 0.75rem;

      text-align: left;
    }

    .research-work-meta {
      margin-top: 0.15rem;

      font-size: 0.81rem;
    }

    .research-work-summary {
      margin-top: 0.32rem;

      font-size: 0.84rem;
      line-height: 1.53;
    }

    .research-subheading {
      margin-top: 1.8rem;
    }

    .research-more-content {
      padding-left: 0.8rem;
    }

  }

</style>



<div class="research-page">


  <!-- =======================================================
       HERO
       ======================================================= -->

  <header class="research-hero">

    <div class="research-hero-copy">

      <h1 class="research-title">Research</h1>

      <p class="research-intro">
        My research is organized around three projects concerning perceptual objects and direct realism,
        institutional formal objects, and temporal externalism. Although they arise in different areas,
        each project asks how the nature or significance of something may depend on structures extending
        beyond what is immediately given.
      </p>

    </div>


    <!--
      Decorative research map.
      Pure SVG: no image file required.
    -->
    <div class="research-diagram" aria-hidden="true">

      <svg
        viewBox="0 0 240 240"
        xmlns="http://www.w3.org/2000/svg"
      >

        <!-- guides -->
        <circle
          cx="120"
          cy="120"
          r="89"
          fill="none"
          stroke="currentColor"
          stroke-width="0.8"
          stroke-dasharray="2.2 3.5"
          opacity="0.18"
        />

        <line
          x1="20"
          y1="120"
          x2="220"
          y2="120"
          stroke="currentColor"
          stroke-width="0.7"
          opacity="0.14"
        />

        <line
          x1="120"
          y1="20"
          x2="120"
          y2="220"
          stroke="currentColor"
          stroke-width="0.7"
          opacity="0.14"
        />


        <!-- blue -->
        <circle
          cx="88"
          cy="135"
          r="52"
          fill="#315f94"
          fill-opacity="0.10"
          stroke="#315f94"
          stroke-opacity="0.28"
          stroke-width="1"
        />


        <!-- green -->
        <circle
          cx="151"
          cy="135"
          r="52"
          fill="#70854d"
          fill-opacity="0.10"
          stroke="#70854d"
          stroke-opacity="0.28"
          stroke-width="1"
        />


        <!-- orange -->
        <circle
          cx="120"
          cy="87"
          r="52"
          fill="#c3653d"
          fill-opacity="0.10"
          stroke="#c3653d"
          stroke-opacity="0.28"
          stroke-width="1"
        />


        <!-- small accent points -->
        <circle cx="120" cy="31" r="3.4" fill="#315f94" />

        <circle cx="198" cy="62" r="3" fill="#c3653d" />

        <circle cx="120" cy="209" r="3.2" fill="#70854d" />

      </svg>

    </div>

  </header>



  <!-- =======================================================
       PROJECT INDEX
       ======================================================= -->

  <nav class="research-index" aria-label="Research projects">

    <a
      class="research-index-item blue"
      href="#perception"
    >
      <span class="research-index-number">01</span>

      <span class="research-index-label">
        Perceptual Objects &amp; Direct Realism
      </span>
    </a>


    <a
      class="research-index-item green"
      href="#institutional-objects"
    >
      <span class="research-index-number">02</span>

      <span class="research-index-label">
        Institutional Formal Objects
      </span>
    </a>


    <a
      class="research-index-item orange"
      href="#temporal-externalism"
    >
      <span class="research-index-number">03</span>

      <span class="research-index-label">
        Temporal Externalism
      </span>
    </a>

  </nav>



  <!-- =======================================================
       01
       PERCEPTUAL OBJECTS & DIRECT REALISM
       ======================================================= -->

  <section
    class="research-project project-blue"
    id="perception"
  >


    <!-- LEFT RAIL -->
    <aside class="research-project-rail">

      <div class="research-project-rail-inner">

        <div class="research-project-number">
          01
        </div>

        <div class="research-project-rail-line"></div>

        <div class="research-project-kicker">
          Perception
        </div>

      </div>

    </aside>



    <!-- BODY -->
    <div class="research-project-body">


      <h2 class="research-project-heading">
        Perceptual Objects and Direct Realism
      </h2>


      <div class="research-project-question">
        What does it take for perceptual awareness of the world to be genuinely direct?
      </div>


      <div class="research-project-overview">

        <p>
          My main project in the philosophy of perception concerns the objects of perceptual
          experience and the nature of direct awareness. I am interested in what makes our
          awareness of ordinary objects genuinely direct, and in whether familiar ways of
          drawing the distinction between direct and indirect perception are sufficiently
          fine-grained.
        </p>

        <p>
          I approach these questions through work on naïve realism, perceptual objects,
          illusion and hallucination, cross-modal perception, touch, and the role of perceptual
          context. A recurring concern is how much explanatory work should be assigned to
          ordinary objects themselves, and which commitments a satisfactory form of direct
          realism must preserve.
        </p>

        <p>
          The positive part of this project develops a systematic account of direct awareness
          and its relation to perceptual mediation. Because the central manuscript is currently
          under review, I keep its technical formulation and argumentative machinery off this
          page.
        </p>

      </div>



      <!-- Research vocabulary -->
      <div class="research-focus">

        <span>direct awareness</span>

        <span>perceptual objects</span>

        <span>naïve realism</span>

        <span>illusion</span>

        <span>hallucination</span>

        <span>cross-modal perception</span>

      </div>



      <!-- ===================================================
           PUBLISHED & FORTHCOMING
           =================================================== -->

      <div class="research-subheading">
        Published &amp; forthcoming
      </div>


      <div class="research-work-list">


        <!-- Tactile screening-off -->
        <article class="research-work">

          <div class="research-work-head">

            <div class="research-work-title">
              A Tactile Screening-Off Problem for Naïve Realism
            </div>

            <div class="research-work-status">
              forthcoming
            </div>

          </div>


          <div class="research-work-meta">

            <span class="research-work-journal">
              Analysis
            </span>

            <span class="research-work-link">
              <a
                href="https://doi.org/10.1093/analys/anag033"
                target="_blank"
                rel="noopener noreferrer"
              >
                [OUP]
              </a>
            </span>

          </div>


          <p class="research-work-summary">
            I argue that naïve realism faces a screening-off problem arising within
            ordinary tactile perception and realistic haptic simulation, without relying
            on the traditional appeal to hallucination.
          </p>

        </article>



        <!-- Cross-modal -->
        <article class="research-work">

          <div class="research-work-head">

            <div class="research-work-title">
              Cross-Modal Experiences and the Problem of Phenomenal Overlap
            </div>

            <div class="research-work-status">
              forthcoming
            </div>

          </div>


          <div class="research-work-meta">

            <span class="research-work-journal">
              Journal of Consciousness Studies
            </span>

            <span class="research-work-link">
              <a
                href="https://philpapers.org/rec/YANCEA-3"
                target="_blank"
                rel="noopener noreferrer"
              >
                [manuscript]
              </a>
            </span>

          </div>


          <p class="research-work-summary">
            I argue that the heterogeneity of cross-modal experience places pressure
            on strong forms of naïve realism, and that abstract spatial similarity does
            not provide the kind of phenomenal overlap such views require.
          </p>

        </article>



        <!-- Rich phenomenology -->
        <article class="research-work">

          <div class="research-work-head">

            <div class="research-work-title">
              Is Rich Phenomenology Fragmented?
            </div>

            <div class="research-work-status">
              2025
            </div>

          </div>


          <div class="research-work-meta">

            <span class="research-work-journal">
              Synthese
            </span>

            <span class="research-work-link">
              <a
                href="https://doi.org/10.1007/s11229-025-05058-8"
                target="_blank"
                rel="noopener noreferrer"
              >
                [Springer]
              </a>
            </span>

          </div>


          <p class="research-work-summary">
            This paper examines whether rich phenomenal character should be understood
            as fragmented across different aspects of perceptual experience.
          </p>

        </article>

      </div>



      <!-- ===================================================
           CURRENT WORK
           =================================================== -->

      <div class="research-subheading">
        Current work
      </div>


      <div class="research-work-list">


        <!-- Core manuscript -->
        <article class="research-work private-work">

          <div class="research-work-head">

            <div class="research-work-title">
              A manuscript on direct awareness in perception
            </div>

            <div class="research-work-status">
              under review
            </div>

          </div>


          <p class="research-work-summary">
            Develops the central positive account of this research program.
            Further details are omitted while the manuscript is under review.
          </p>

        </article>



        <!-- Context / perceptual objects -->
        <article class="research-work private-work">

          <div class="research-work-head">

            <div class="research-work-title">
              A manuscript on perceptual context and perceptual objects
            </div>

            <div class="research-work-status">
              manuscript
            </div>

          </div>


          <p class="research-work-summary">
            Examines how perceptual context bears on questions about perceptual objects
            and the explanation of context-sensitive phenomenal variation.
          </p>

        </article>



        <!-- Boundary -->
        <article class="research-work private-work">

          <div class="research-work-head">

            <div class="research-work-title">
              A manuscript on the commitments of naïve realism
            </div>

            <div class="research-work-status">
              manuscript
            </div>

          </div>


          <p class="research-work-summary">
            Asks which commitments are essential to naïve realism and which may be
            revised without abandoning the view altogether.
          </p>

        </article>



        <!-- Hallucination -->
        <article class="research-work private-work">

          <div class="research-work-head">

            <div class="research-work-title">
              A manuscript on hallucination and direct realism
            </div>

            <div class="research-work-status">
              manuscript
            </div>

          </div>


          <p class="research-work-summary">
            Reconsiders what arguments from hallucination can establish about the
            nature of successful perceptual experience.
          </p>

        </article>



        <!-- Illusion -->
        <article class="research-work private-work">

          <div class="research-work-head">

            <div class="research-work-title">
              A manuscript on illusion and perceptual correctness
            </div>

            <div class="research-work-status">
              manuscript
            </div>

          </div>


          <p class="research-work-summary">
            Examines how theories of perceptual error should characterize correctness
            in cases where perceptual appearance is sensitive to background conditions.
          </p>

        </article>

      </div>



      <!-- ===================================================
           MORE
           =================================================== -->

      <details class="research-more">

        <summary>
          More on this project
        </summary>


        <div class="research-more-content">

          <p>
            Much of the project begins from a tension in contemporary philosophy of
            perception. Direct realist views capture the thought that ordinary worldly
            objects are genuinely present to us in successful perception, but familiar
            cases involving illusion, hallucination, sensory variation, and perceptual
            context place pressure on simple versions of that picture.
          </p>

          <p>
            Rather than treating these cases as isolated objections, I use them to ask
            a more general question about the architecture of perceptual awareness:
            which aspects of experience should be explained by the subject, which by
            the world, and how should these contributions be related in a theory that
            still deserves to count as direct realist?
          </p>

          <p>
            The papers in this project approach that question from different directions.
            Some develop pressure on orthodox relational views; others investigate
            perceptual objects, contextual variation, and the structure of the familiar
            bad cases. Together they form the background for a more systematic positive
            account currently under review.
          </p>

        </div>

      </details>


    </div>

  </section>



  <!-- =======================================================
       02
       INSTITUTIONAL FORMAL OBJECTS
       ======================================================= -->

  <section
    class="research-project project-green compact"
    id="institutional-objects"
  >


    <!-- LEFT RAIL -->
    <aside class="research-project-rail">

      <div class="research-project-rail-inner">

        <div class="research-project-number">
          02
        </div>

        <div class="research-project-rail-line"></div>

        <div class="research-project-kicker">
          Institutional<br>
          Objects
        </div>

      </div>

    </aside>



    <!-- BODY -->
    <div class="research-project-body">


      <h2 class="research-project-heading">
        Institutional Formal Objects
      </h2>


      <div class="research-project-question">
        How do institutional structures shape the objects to which normative responses are directed?
      </div>


      <div class="research-project-overview">

        <p>
          My second project concerns institutional formal objects and the normative
          structures associated with them. I am interested in objects whose identity or
          significance depends partly on institutional practices, and in how those
          structures bear on questions about fitting responses.
        </p>

        <p>
          More broadly, the project asks how object-level facts and institutional
          background conditions interact when we assess what attitudes or responses
          are appropriate.
        </p>

      </div>



      <div class="research-focus">

        <span>formal objects</span>

        <span>institutions</span>

        <span>fittingness</span>

        <span>normativity</span>

      </div>



      <div class="research-subheading">
        Published &amp; forthcoming
      </div>


      <div class="research-work-list">

        <article class="research-work">

          <div class="research-work-head">

            <div class="research-work-title">
              Institutional Formal Objects and Two-Level Fittingness
            </div>

            <div class="research-work-status">
              forthcoming
            </div>

          </div>


          <div class="research-work-meta">

            <span class="research-work-journal">
              The Philosophical Quarterly
            </span>

            <span class="research-work-link">
              <a
                href="https://philpapers.org/rec/YANIFO"
                target="_blank"
                rel="noopener noreferrer"
              >
                [manuscript]
              </a>
            </span>

          </div>


          <p class="research-work-summary">
            I develop an account of institutional formal objects and examine how
            fittingness can operate at two connected levels.
          </p>

        </article>

      </div>


    </div>

  </section>



  <!-- =======================================================
       03
       TEMPORAL EXTERNALISM
       ======================================================= -->

  <section
    class="research-project project-orange compact"
    id="temporal-externalism"
  >


    <!-- LEFT RAIL -->
    <aside class="research-project-rail">

      <div class="research-project-rail-inner">

        <div class="research-project-number">
          03
        </div>

        <div class="research-project-rail-line"></div>

        <div class="research-project-kicker">
          Temporal<br>
          Externalism
        </div>

      </div>

    </aside>



    <!-- BODY -->
    <div class="research-project-body">


      <h2 class="research-project-heading">
        Temporal Externalism
      </h2>


      <div class="research-project-question">
        To what extent can the determination of present semantic properties depend on temporally extended facts?
      </div>


      <div class="research-project-overview">

        <p>
          My third project concerns temporal externalism, especially questions about
          the temporal structure of semantic determination. I am interested in whether
          properties instantiated at a time must be fixed entirely by facts available at
          that time, and in what follows if semantic dependence extends across time.
        </p>

        <p>
          This project connects issues in the philosophy of language and metaphysics,
          with particular attention to the relation between present semantic properties
          and temporally extended patterns or conditions.
        </p>

      </div>



      <div class="research-focus">

        <span>temporal externalism</span>

        <span>semantics</span>

        <span>metaphysics</span>

        <span>determination</span>

      </div>



      <div class="research-subheading">
        Current work
      </div>


      <div class="research-work-list">

        <article class="research-work private-work">

          <div class="research-work-head">

            <div class="research-work-title">
              A manuscript on temporal externalism and semantic properties
            </div>

            <div class="research-work-status">
              manuscript
            </div>

          </div>


          <p class="research-work-summary">
            Examines questions about temporally extended dependence and the
            determination of semantic properties.
          </p>

        </article>

      </div>


    </div>

  </section>


</div>
