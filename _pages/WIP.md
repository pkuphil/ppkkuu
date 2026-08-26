---
layout: page
title: research
permalink: /research/
nav: true
nav_order: 2
description: Research in philosophy of perception, emotion, and language.
---

<style>

  /* =========================================================
     RESEARCH PAGE
     ========================================================= */

  .research-page {
    --research-blue: #315f94;
    --research-green: #70854d;
    --research-orange: #c3653d;

    width: 100%;
    max-width: 1040px;

    margin: 0 auto;
    padding: 1.5rem 0 4rem 0;

    font-family: inherit;
    color: var(--global-text-color, inherit);
  }


  /* =========================================================
     HERO
     ========================================================= */

  .research-hero {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 220px;
    align-items: center;

    gap: 4rem;

    margin-bottom: 2.8rem;
  }

  .research-hero-copy {
    min-width: 0;
  }

  .research-title {
    margin: 0 0 1.25rem 0;

    font-family: inherit;
    font-size: clamp(3rem, 6vw, 4.25rem);
    font-weight: 400;
    line-height: 1;

    letter-spacing: -0.035em;

    color: var(--global-text-color, inherit);
  }

  .research-intro {
    max-width: 710px;

    margin: 0;

    font-size: 1rem;
    font-weight: 400;
    line-height: 1.7;

    color: var(--global-text-color, inherit);
  }


  /* =========================================================
     RESEARCH DIAGRAM
     ========================================================= */

  .research-diagram {
    width: 210px;
    height: 210px;

    justify-self: end;

    opacity: 0.9;
  }

  .research-diagram svg {
    display: block;

    width: 100%;
    height: 100%;
  }


  /* =========================================================
     TABS
     ========================================================= */

  .research-tabs {
    display: grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));

    width: 100%;

    margin: 0 0 2.65rem 0;

    border-top: 1px solid var(--global-divider-color, #dedede);
    border-bottom: 1px solid var(--global-divider-color, #dedede);
  }

  .research-tab {
    position: relative;

    appearance: none;
    -webkit-appearance: none;

    display: flex;
    align-items: center;
    justify-content: center;

    min-width: 0;
    min-height: 3.75rem;

    margin: 0;
    padding: 0.9rem 1rem;

    font-family: inherit;
    font-size: 0.87rem;
    font-weight: 400;
    line-height: 1.35;

    text-align: center;

    color: var(--global-text-color-light, #777);

    background: transparent !important;

    border: 0;
    border-bottom: 2px solid transparent;

    border-radius: 0;

    box-shadow: none !important;

    cursor: pointer;

    transition:
      color 0.16s ease,
      border-color 0.16s ease;
  }

  .research-tab:hover,
  .research-tab:focus {
    color: var(--global-text-color, inherit);

    background: transparent !important;

    outline: none;

    box-shadow: none !important;
  }


  /* Active tabs */

  .research-tab-blue.active {
    color: var(--research-blue);

    border-bottom-color: var(--research-blue);
  }

  .research-tab-green.active {
    color: var(--research-green);

    border-bottom-color: var(--research-green);
  }

  .research-tab-orange.active {
    color: var(--research-orange);

    border-bottom-color: var(--research-orange);
  }

  .research-tab-other {
    color: var(--global-text-color-light, #999);
  }

  .research-tab-other.active {
    color: var(--global-text-color, inherit);

    border-bottom-color: var(--global-text-color-light, #999);
  }


  /* =========================================================
     PANELS
     ========================================================= */

  .research-panel {
    --accent: var(--research-blue);

    display: none;

    width: 100%;

    animation: researchFadeIn 0.2s ease;
  }

  .research-panel.active {
    display: block;
  }

  .research-panel.project-blue {
    --accent: var(--research-blue);
  }

  .research-panel.project-green {
    --accent: var(--research-green);
  }

  .research-panel.project-orange {
    --accent: var(--research-orange);
  }

  .research-panel.project-other {
    --accent: var(--global-text-color-light, #888);
  }


  @keyframes researchFadeIn {

    from {
      opacity: 0;
      transform: translateY(3px);
    }

    to {
      opacity: 1;
      transform: translateY(0);
    }

  }


  /* =========================================================
     PROJECT HEADER
     ========================================================= */

  .research-project-heading {
    max-width: 780px;

    margin: 0 0 0.38rem 0;

    font-family: inherit;
    font-size: 1.65rem;
    font-weight: 500;
    line-height: 1.25;

    letter-spacing: -0.018em;

    color: var(--global-text-color, inherit);
  }

  .research-project-question {
    max-width: 730px;

    margin: 0 0 1.4rem 0;

    font-size: 0.98rem;
    font-style: italic;
    font-weight: 400;
    line-height: 1.5;

    color: var(--accent);
  }


  /* =========================================================
     OVERVIEW
     ========================================================= */

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
     RESEARCH FOCUS
     ========================================================= */

  .research-focus {
    display: flex;
    flex-wrap: wrap;

    gap: 0;

    max-width: 800px;

    margin: 1.25rem 0 2rem 0;

    font-size: 0.69rem;
    font-weight: 500;
    line-height: 1.5;

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

    color: var(--global-text-color-light, #aaa);
  }


  /* =========================================================
     SUBHEADINGS
     ========================================================= */

  .research-subheading {
    margin: 2rem 0 0.7rem 0;

    font-size: 0.71rem;
    font-weight: 500;
    line-height: 1.35;

    letter-spacing: 0.085em;
    text-transform: uppercase;

    color: var(--global-text-color-light, #777);
  }


  /* =========================================================
     WORK LIST
     ========================================================= */

  .research-work-list {
    width: 100%;

    max-width: 830px;

    margin: 0;
    padding: 0;

    border-top: 1px solid var(--global-divider-color, #e2e2e2);
  }

  .research-work {
    margin: 0;

    padding: 0.85rem 0 0.9rem 0;

    border-bottom: 1px solid var(--global-divider-color, #e8e8e8);
  }

  .research-work:last-child {
    border-bottom: 0;
  }


  /* =========================================================
     WORK HEADER
     ========================================================= */

  .research-work-head {
    display: flex;
    align-items: baseline;

    width: 100%;

    gap: 1.25rem;
  }

  .research-work-title {
    flex: 1 1 auto;

    min-width: 0;

    margin: 0;

    font-size: 0.97rem;
    font-weight: 600;
    line-height: 1.42;

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

    color: var(--global-text-color-light, #777);
  }


  /* =========================================================
     META
     ========================================================= */

  .research-work-meta {
    margin-top: 0.13rem;

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

    margin-right: 0.15rem;

    color: var(--global-text-color-light, #aaa);
  }

  .research-work-link a,
  .research-work-link a:link,
  .research-work-link a:visited {
    color: var(--accent) !important;

    background: transparent !important;

    text-decoration: underline !important;
    text-decoration-color: transparent !important;
    text-decoration-thickness: 1px !important;
    text-underline-offset: 0.17em;

    border: 0 !important;

    box-shadow: none !important;
  }

  .research-work-link a:hover,
  .research-work-link a:focus {
    color: var(--accent) !important;

    background: transparent !important;

    text-decoration-color: currentColor !important;

    box-shadow: none !important;
  }


  /* =========================================================
     PAPER SUMMARY
     ========================================================= */

  .research-work-summary {
    max-width: 740px;

    margin: 0.36rem 0 0 0;

    font-size: 0.86rem;
    font-weight: 400;
    line-height: 1.55;

    color: var(--global-text-color-light, #686d72);
  }


  /* =========================================================
     CURRENT / PRIVATE WORK
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
    max-width: 760px;

    margin: 1.4rem 0 0 0;
    padding: 0;
  }

  .research-more summary {
    display: inline-flex;
    align-items: center;

    gap: 0.45rem;

    margin: 0;
    padding: 0;

    cursor: pointer;

    list-style: none;

    font-size: 0.83rem;
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
    max-width: 720px;

    margin-top: 1rem;
    padding-left: 1rem;

    border-left: 1px solid var(--global-divider-color, #dedede);
  }

  .research-more-content p {
    margin: 0 0 0.8rem 0;

    font-size: 0.89rem;
    font-weight: 400;
    line-height: 1.62;

    color: var(--global-text-color, inherit);
  }

  .research-more-content p:last-child {
    margin-bottom: 0;
  }


  /* =========================================================
     OTHER WORK
     ========================================================= */

  .project-other .research-project-heading {
    margin-bottom: 1.25rem;

    font-size: 1.45rem;
    font-weight: 400;
  }

  .project-other .research-work-list {
    max-width: 830px;
  }

  .project-other .research-work-title {
    font-weight: 500;
  }

  .project-other .research-work-summary {
    max-width: 690px;
  }


  /* =========================================================
     DARK MODE
     ========================================================= */

  html[data-theme="dark"] .research-page,
  body[data-theme="dark"] .research-page {
    --research-blue: #7ea2d1;
    --research-green: #a0b97b;
    --research-orange: #df8b68;
  }


  @media (prefers-color-scheme: dark) {

    .research-page {
      --research-blue: #7ea2d1;
      --research-green: #a0b97b;
      --research-orange: #df8b68;
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
      grid-template-columns: minmax(0, 1fr) 180px;

      gap: 2rem;
    }

    .research-diagram {
      width: 175px;
      height: 175px;
    }

    .research-tab {
      padding-left: 0.65rem;
      padding-right: 0.65rem;

      font-size: 0.82rem;
    }

  }


  /* =========================================================
     MOBILE
     ========================================================= */

  @media (max-width: 650px) {

    .research-page {
      padding-top: 0.5rem;
      padding-bottom: 3rem;
    }


    /* Hero */

    .research-hero {
      display: block;

      margin-bottom: 2rem;
    }

    .research-title {
      margin-bottom: 1.1rem;

      font-size: 2.7rem;
      line-height: 1.04;
    }

    .research-intro {
      font-size: 0.95rem;
      line-height: 1.63;
    }

    .research-diagram {
      width: 145px;
      height: 145px;

      margin: 1.45rem auto 0 auto;
    }


    /* Tabs */

    .research-tabs {
      display: flex;

      overflow-x: auto;
      overflow-y: hidden;

      margin-bottom: 2rem;

      scrollbar-width: none;

      -webkit-overflow-scrolling: touch;
    }

    .research-tabs::-webkit-scrollbar {
      display: none;
    }

    .research-tab {
      flex: 0 0 auto;

      min-height: auto;

      padding: 0.82rem 1rem;

      font-size: 0.82rem;

      white-space: nowrap;
    }

    .research-tab:first-child {
      padding-left: 0;
    }


    /* Project */

    .research-project-heading {
      font-size: 1.4rem;
      line-height: 1.28;
    }

    .research-project-question {
      margin-bottom: 1.15rem;

      font-size: 0.92rem;
    }

    .research-project-overview p {
      font-size: 0.92rem;
      line-height: 1.6;
    }

    .research-focus {
      margin-top: 1rem;
      margin-bottom: 1.65rem;

      font-size: 0.64rem;
      line-height: 1.55;
    }


    /* Work */

    .research-subheading {
      margin-top: 1.7rem;
    }

    .research-work {
      padding-top: 0.75rem;
      padding-bottom: 0.8rem;
    }

    .research-work-head {
      display: block;
    }

    .research-work-title {
      font-size: 0.93rem;
      line-height: 1.42;
    }

    .research-work-status {
      display: block;

      margin: 0.15rem 0 0 0;

      font-size: 0.74rem;
    }

    .research-work-meta {
      margin-top: 0.15rem;

      font-size: 0.8rem;
    }

    .research-work-summary {
      margin-top: 0.3rem;

      font-size: 0.83rem;
      line-height: 1.52;
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

      <h1 class="research-title">
        Research
      </h1>

      <p class="research-intro">
        My research focuses primarily on the objects of perception and the nature of
        direct awareness. I also work in the philosophy of emotion, especially on
        formal objects and fittingness, and in the philosophy of language, especially
        on reference and temporal externalism.
      </p>

    </div>



    <!-- Three main research programs -->

    <div
      class="research-diagram"
      aria-hidden="true"
    >

      <svg
        viewBox="0 0 240 240"
        xmlns="http://www.w3.org/2000/svg"
      >


        <!-- Guides -->

        <circle
          cx="120"
          cy="120"
          r="89"
          fill="none"
          stroke="currentColor"
          stroke-width="0.8"
          stroke-dasharray="2.2 3.5"
          opacity="0.17"
        />


        <line
          x1="20"
          y1="120"
          x2="220"
          y2="120"
          stroke="currentColor"
          stroke-width="0.7"
          opacity="0.13"
        />


        <line
          x1="120"
          y1="20"
          x2="120"
          y2="220"
          stroke="currentColor"
          stroke-width="0.7"
          opacity="0.13"
        />



        <!-- Perception -->

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



        <!-- Emotion -->

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



        <!-- Language -->

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



        <!-- Accent points -->

        <circle
          cx="120"
          cy="31"
          r="3.4"
          fill="#315f94"
        />

        <circle
          cx="198"
          cy="62"
          r="3"
          fill="#c3653d"
        />

        <circle
          cx="120"
          cy="209"
          r="3.2"
          fill="#70854d"
        />


      </svg>

    </div>

  </header>



  <!-- =======================================================
       TABS
       ======================================================= -->

  <div
    class="research-tabs"
    role="tablist"
    aria-label="Research projects"
  >


    <button
      class="research-tab research-tab-blue active"
      id="tab-perception"
      type="button"
      role="tab"
      aria-selected="true"
      aria-controls="research-perception"
      data-project="perception"
    >
      Perceptual Objects &amp; Direct Realism
    </button>



    <button
      class="research-tab research-tab-green"
      id="tab-emotion"
      type="button"
      role="tab"
      aria-selected="false"
      aria-controls="research-emotion"
      data-project="emotion"
    >
      Institutional Formal Objects
    </button>



    <button
      class="research-tab research-tab-orange"
      id="tab-language"
      type="button"
      role="tab"
      aria-selected="false"
      aria-controls="research-language"
      data-project="language"
    >
      Temporal Externalism
    </button>



    <button
      class="research-tab research-tab-other"
      id="tab-other"
      type="button"
      role="tab"
      aria-selected="false"
      aria-controls="research-other"
      data-project="other"
    >
      Other Work
    </button>


  </div>



  <!-- =======================================================
       PERCEPTION
       ======================================================= -->

  <section
    class="research-panel project-blue active"
    id="research-perception"
    data-panel="perception"
    role="tabpanel"
    aria-labelledby="tab-perception"
  >


    <h2 class="research-project-heading">
      Perceptual Objects and Direct Realism
    </h2>


    <div class="research-project-question">
      What are the objects of perception, and what makes our awareness of them direct?
    </div>



    <div class="research-project-overview">

      <p>
        My main research concerns the objects of perceptual experience and the nature
        of direct awareness. I am interested in how ordinary objects figure in
        experience and in what a satisfactory form of direct realism should preserve.
      </p>

      <p>
        I approach these questions through work on perceptual objects, touch,
        cross-modal experience, perceptual context, illusion, and hallucination.
        A central manuscript develops the positive framework of this project.
      </p>

    </div>



    <div class="research-focus">

      <span>perceptual objects</span>

      <span>direct awareness</span>

      <span>naïve realism</span>

      <span>perceptual context</span>

      <span>cross-modal perception</span>

    </div>



    <!-- Published & forthcoming -->

    <div class="research-subheading">
      Published &amp; forthcoming
    </div>


    <div class="research-work-list">


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
          I argue that ordinary tactile perception creates a screening-off problem
          for naïve realism without relying on hallucination.
        </p>

      </article>



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
          I argue that cross-modal phenomenal heterogeneity creates a problem for
          strong forms of naïve realism.
        </p>

      </article>


    </div>



    <!-- Current work -->

    <div class="research-subheading">
      Current work
    </div>


    <div class="research-work-list">


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
          Develops the central positive account of this research project.
        </p>

      </article>



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
          Examines how perceptual context bears on the objects and phenomenal
          character of experience.
        </p>

      </article>


    </div>



    <details class="research-more">

      <summary>
        More on this project
      </summary>


      <div class="research-more-content">

        <p>
          Across this work, I use problems concerning sensory variation, perceptual
          context, and the relation between experience and worldly objects to ask
          what a theory of direct perception needs to explain.
        </p>

        <p>
          The individual papers develop different parts of this broader project,
          while the central positive account is currently under review.
        </p>

      </div>

    </details>


  </section>



  <!-- =======================================================
       PHILOSOPHY OF EMOTION
       ======================================================= -->

  <section
    class="research-panel project-green"
    id="research-emotion"
    data-panel="emotion"
    role="tabpanel"
    aria-labelledby="tab-emotion"
  >


    <h2 class="research-project-heading">
      Institutional Formal Objects
    </h2>


    <div class="research-project-question">
      How can socially constituted standings enter the evaluative structure of emotion?
    </div>



    <div class="research-project-overview">

      <p>
        My work in the philosophy of emotion examines how social standings such as
        prestige and stigma can enter emotional evaluation. I am especially interested
        in formal objects, fittingness, and the relation between social reality and
        emotional normativity.
      </p>

    </div>



    <div class="research-focus">

      <span>philosophy of emotion</span>

      <span>formal objects</span>

      <span>fittingness</span>

      <span>social ontology</span>

      <span>institutional status</span>

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
          I argue that socially constituted evaluative properties can themselves be
          formal objects of emotion, and develop a two-level account of their fittingness.
        </p>

      </article>


    </div>


  </section>



  <!-- =======================================================
       PHILOSOPHY OF LANGUAGE
       ======================================================= -->

  <section
    class="research-panel project-orange"
    id="research-language"
    data-panel="language"
    role="tabpanel"
    aria-labelledby="tab-language"
  >


    <h2 class="research-project-heading">
      Temporal Externalism
    </h2>


    <div class="research-project-question">
      How can reference depend on linguistic practice across time?
    </div>



    <div class="research-project-overview">

      <p>
        My work in the philosophy of language focuses on reference and temporal
        externalism. I am interested in how present and future linguistic practice
        bear on reference, semantic continuity, and change across time.
      </p>

    </div>



    <div class="research-focus">

      <span>philosophy of language</span>

      <span>metasemantics</span>

      <span>reference</span>

      <span>temporal externalism</span>

      <span>linguistic practice</span>

    </div>



    <div class="research-subheading">
      Current work
    </div>


    <div class="research-work-list">


      <article class="research-work private-work">

        <div class="research-work-head">

          <div class="research-work-title">
            A manuscript on reference and linguistic practice across time
          </div>

          <div class="research-work-status">
            under review
          </div>

        </div>


        <p class="research-work-summary">
          Examines how present and future linguistic practice bear on the
          determination of reference.
        </p>

      </article>


    </div>


  </section>



  <!-- =======================================================
       OTHER WORK
       ======================================================= -->

  <section
    class="research-panel project-other"
    id="research-other"
    data-panel="other"
    role="tabpanel"
    aria-labelledby="tab-other"
  >


    <h2 class="research-project-heading">
      Other Work
    </h2>


    <div class="research-work-list">


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
          I argue that evidence commonly taken to support a fragmented view of
          phenomenal consciousness is also compatible with a richer view.
        </p>

      </article>


    </div>


  </section>


</div>



<!-- =========================================================
     TAB SWITCHING
     ========================================================= -->

<script>

  document.addEventListener("DOMContentLoaded", function () {

    const tabs = Array.from(
      document.querySelectorAll(".research-tab")
    );

    const panels = Array.from(
      document.querySelectorAll(".research-panel")
    );


    function activateResearchTab(tab) {

      const project = tab.dataset.project;


      tabs.forEach(function (item) {

        item.classList.remove("active");

        item.setAttribute(
          "aria-selected",
          "false"
        );

      });


      panels.forEach(function (panel) {

        panel.classList.remove("active");

      });


      tab.classList.add("active");

      tab.setAttribute(
        "aria-selected",
        "true"
      );


      const targetPanel = document.querySelector(
        '.research-panel[data-panel="' + project + '"]'
      );


      if (targetPanel) {

        targetPanel.classList.add("active");

      }

    }



    tabs.forEach(function (tab, index) {

      tab.addEventListener("click", function () {

        activateResearchTab(tab);

      });



      /*
        Keyboard support:
        left / right arrows switch tabs
      */

      tab.addEventListener("keydown", function (event) {

        if (
          event.key !== "ArrowLeft" &&
          event.key !== "ArrowRight"
        ) {
          return;
        }


        event.preventDefault();


        let newIndex;


        if (event.key === "ArrowRight") {

          newIndex =
            (index + 1) % tabs.length;

        } else {

          newIndex =
            (index - 1 + tabs.length) % tabs.length;

        }


        const nextTab = tabs[newIndex];


        nextTab.focus();

        activateResearchTab(nextTab);

      });

    });

  });

</script>
