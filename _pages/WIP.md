---
layout: default
title: research
permalink: /research/
nav: true
nav_order: 2
description: Research in philosophy of perception, emotion, and language.
---

<style>

  /* =========================================================
     RESEARCH PAGE — EDITORIAL LAYOUT
     Hero above; vertical research index + active project below.
     ========================================================= */

  @import url('https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500;1,600&family=Noto+Serif+SC:wght@400;500;600&display=swap');

  body,
  .navbar,
  .navbar-brand,
  .navbar-nav,
  .research-page {
    font-family:
      "EB Garamond",
      "Songti SC",
      STSong,
      "Noto Serif SC",
      SimSun,
      Garamond,
      Georgia,
      "Times New Roman",
      serif !important;
  }

  /*
    Give this page more horizontal breathing room than a normal article.
  */
  main.container {
    max-width: 1260px !important;
    padding-left: clamp(1.35rem, 3vw, 3rem);
    padding-right: clamp(1.35rem, 3vw, 3rem);
  }

  .research-page {
    --research-blue: #315f94;
    --research-green: #70854d;
    --research-orange: #c3653d;

    --research-text: #47443f;
    --research-heading: #34312d;
    --research-muted: #817c75;
    --research-soft: #a29d96;
    --research-rule: rgba(52, 49, 45, 0.13);

    width: 100%;
    max-width: 1160px;

    margin: -1rem auto 0;
    padding: 0 0 4.2rem;

    color: var(--research-text);
  }


  /* =========================================================
     HERO
     ========================================================= */

  .research-hero {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 300px;
    align-items: center;

    gap: clamp(2.8rem, 5vw, 4.6rem);

    margin-bottom: 2.45rem;
  }

  .research-hero-copy {
    min-width: 0;
  }

  .research-title {
    margin: 0 0 0.95rem 0;

    font-family: inherit;
    font-size: clamp(3.2rem, 5.8vw, 4.55rem);
    font-weight: 400;
    line-height: 0.98;

    letter-spacing: -0.037em;

    color: var(--research-heading);
  }

  .research-intro {
    max-width: 720px;

    margin: 0;

    font-size: 1.04rem;
    font-weight: 400;
    line-height: 1.64;

    color: var(--research-text);
  }


  /* =========================================================
     HERO IMAGE
     ========================================================= */

  .research-diagram {
    width: 286px;
    height: 286px;

    justify-self: end;
  }

  .research-diagram img {
    display: block;

    width: 100%;
    height: 100%;

    object-fit: contain;
    object-position: center;
  }


  /* =========================================================
     BODY — INDEX + PROJECT
     ========================================================= */

  .research-body {
    display: grid;
    grid-template-columns: 210px minmax(0, 1fr);
    align-items: start;

    column-gap: clamp(3rem, 4.5vw, 4.6rem);

    padding-top: 0;
  }


  /* =========================================================
     RESEARCH INDEX
     ========================================================= */

  .research-tabs {
    grid-column: 1;
    grid-row: 1;

    position: sticky;
    top: 6.2rem;

    width: 100%;

    margin: 0;
    padding: 0;

    border-top: 1px solid var(--research-rule);
  }

  .research-tabs-label {
    padding: 0.8rem 0 0.68rem;

    font-size: 0.76rem;
    font-weight: 500;
    line-height: 1.35;

    letter-spacing: 0.055em;
    text-transform: uppercase;

    color: var(--research-soft);

    border-bottom: 1px solid var(--research-rule);
  }

  .research-tab {
    appearance: none;
    -webkit-appearance: none;

    position: relative;

    display: block;

    width: 100%;
    min-width: 0;

    margin: 0;
    padding: 0.82rem 0.15rem 0.82rem 1rem;

    font-family: inherit;
    font-size: 0.98rem;
    font-weight: 400;
    line-height: 1.34;

    text-align: left;

    color: var(--research-muted);

    background: transparent !important;

    border: 0;
    border-bottom: 1px solid var(--research-rule);
    border-radius: 0;

    box-shadow: none !important;

    cursor: pointer;

    transition:
      color 0.16s ease,
      padding-left 0.16s ease;
  }

  .research-tab::before {
    content: "";

    position: absolute;
    left: 0.05rem;
    top: 1.17rem;

    width: 0.28rem;
    height: 0.28rem;

    border: 1px solid currentColor;
    border-radius: 50%;

    opacity: 0.42;

    transition:
      background-color 0.16s ease,
      opacity 0.16s ease;
  }

  .research-tab:hover,
  .research-tab:focus {
    color: var(--research-heading);

    padding-left: 1.08rem;

    background: transparent !important;

    outline: none;

    box-shadow: none !important;
  }

  .research-tab.active::before {
    background: currentColor;
    opacity: 1;
  }

  .research-tab-blue.active {
    color: var(--research-blue);
  }

  .research-tab-green.active {
    color: var(--research-green);
  }

  .research-tab-orange.active {
    color: var(--research-orange);
  }

  .research-tab-other.active {
    color: var(--research-muted);
  }


  /* =========================================================
     PANELS
     ========================================================= */

  .research-panel {
    --accent: var(--research-blue);

    grid-column: 2;
    grid-row: 1;

    display: none;

    width: 100%;
    max-width: 820px;

    animation: researchFadeIn 0.22s ease;
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
    --accent: var(--research-muted);
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
    max-width: 800px;

    margin: -0.05rem 0 0.28rem 0;

    font-family: inherit;
    font-size: clamp(1.7rem, 2.4vw, 1.95rem);
    font-weight: 500;
    line-height: 1.2;

    letter-spacing: -0.018em;

    color: var(--research-heading);
  }

  .research-project-question {
    max-width: 770px;

    margin: 0 0 1.05rem 0;

    font-size: 1.02rem;
    font-style: italic;
    font-weight: 400;
    line-height: 1.5;

    color: var(--accent);
  }


  /* =========================================================
     PROJECT OVERVIEW
     ========================================================= */

  .research-project-overview {
    max-width: 790px;

    margin-bottom: 1.55rem;
  }

  .research-project-overview p {
    margin: 0;

    font-size: 1rem;
    font-weight: 400;
    line-height: 1.64;

    color: var(--research-text);
  }


  /* =========================================================
     SECTION LABELS
     ========================================================= */

  .research-subheading {
    display: flex;
    align-items: center;

    gap: 0.68rem;

    margin: 1.55rem 0 0.42rem 0;

    font-size: 0.84rem;
    font-weight: 500;
    line-height: 1.4;

    letter-spacing: 0.025em;

    color: var(--research-muted);
  }

  .research-subheading::after {
    content: "";

    flex: 1 1 auto;

    height: 1px;

    background: var(--research-rule);
  }


  /* =========================================================
     WORK LIST
     ========================================================= */

  .research-work-list {
    width: 100%;
    max-width: 820px;

    margin: 0;
    padding: 0;

    border-top: 0;
  }

  .research-work {
    position: relative;

    margin: 0;

    padding: 0.72rem 0 0.78rem;

    border-bottom: 1px solid var(--research-rule);
  }

  .research-work:last-child {
    border-bottom: 0;
  }


  /* =========================================================
     PUBLISHED PAPERS — APA-STYLE SINGLE-LINE REFERENCES
     Title. Journal, forthcoming/year. [link]
     ========================================================= */

  .published-work {
    padding-top: 0.68rem;
    padding-bottom: 0.7rem;
  }

  .research-citation-line {
    display: block;
    width: 100%;
    padding-right: 1.55rem;

    font-size: 0.98rem;
    font-weight: 400;
    line-height: 1.5;
    letter-spacing: -0.001em;

    color: var(--research-text);

    white-space: nowrap;
  }

  .research-citation-title {
    font-weight: 500;
    color: var(--research-heading);
  }

  .research-citation-journal {
    font-style: italic;
    font-weight: 400;
    color: var(--research-text);
  }

  .research-citation-status {
    font-style: italic;
    font-weight: 400;
    color: var(--research-muted);
  }

  .research-citation-year {
    font-style: normal;
  }

  .published-work .research-work-link {
    margin-left: 0.12em;
    font-size: inherit;
  }

  .published-work .research-work-link::before {
    content: "";
    margin: 0;
  }

  .published-work .research-abstract summary {
    top: 0.79rem;
    right: 0;
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

    font-size: 1.01rem;
    font-weight: 500;
    line-height: 1.42;

    letter-spacing: -0.002em;

    color: var(--research-heading);
  }

  .research-work-status {
    flex: 0 0 auto;

    margin-left: auto;

    font-size: 0.86rem;
    font-weight: 400;
    font-style: italic;
    line-height: 1.4;

    white-space: nowrap;

    color: var(--research-muted);
  }


  /* =========================================================
     META
     ========================================================= */

  .research-work-meta {
    margin-top: 0.08rem;

    font-size: 0.91rem;
    font-weight: 400;
    line-height: 1.45;

    color: var(--research-muted);
  }

  .research-work-journal {
    font-style: italic;

    color: var(--research-text);
  }

  .research-work-link::before {
    content: " · ";

    margin-right: 0.12rem;

    color: var(--research-soft);
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
    box-shadow: none !important;

    transition: text-decoration-color 0.15s ease;
  }

  .research-work-link a:hover,
  .research-work-link a:focus {
    color: var(--accent) !important;

    background: transparent !important;

    text-decoration-color: currentColor !important;

    box-shadow: none !important;
  }


  /* =========================================================
     COLLAPSIBLE ABSTRACT
     A single + / − symbol; closed by default.
     ========================================================= */

  .research-abstract {
    margin: 0;
    padding: 0;
  }

  .research-abstract summary {
    list-style: none;

    position: absolute;
    right: 0;
    top: 2.02rem;

    display: grid;
    place-items: center;

    width: 1.08rem;
    height: 1.08rem;

    margin: 0;
    padding: 0;

    color: var(--accent);

    background: transparent !important;

    border: 0;
    border-radius: 0;

    cursor: pointer;

    user-select: none;

    transition:
      opacity 0.15s ease,
      transform 0.15s ease;
  }

  /*
    Current-work entries have no journal/meta line.
    Keep the symbol on the title/status line instead.
  */
  .research-work.private-work .research-work-head {
    padding-right: 1.4rem;
  }

  .research-work.private-work .research-abstract summary {
    top: 0.76rem;
  }

  .research-abstract summary::-webkit-details-marker {
    display: none;
  }

  .research-abstract summary::marker {
    content: "";
  }

  .research-abstract summary:hover,
  .research-abstract summary:focus {
    opacity: 0.68;
    transform: translateY(-1px);

    outline: none;
  }

  .research-toggle-symbol {
    display: block;

    font-family: inherit;
    font-size: 1.02rem;
    font-weight: 400;
    line-height: 1;
  }

  .research-toggle-symbol::before {
    content: "+";
  }

  .research-abstract[open] .research-toggle-symbol::before {
    content: "−";
  }

  .research-abstract-body {
    animation: researchAbstractIn 0.18s ease;
  }

  @keyframes researchAbstractIn {
    from {
      opacity: 0;
      transform: translateY(-2px);
    }

    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  .research-work-summary {
    max-width: 760px;

    margin: 0.42rem 0 0 0;

    font-size: 0.93rem;
    font-weight: 400;
    line-height: 1.62;

    color: var(--research-muted);
  }

  .research-sr-only {
    position: absolute !important;

    width: 1px !important;
    height: 1px !important;

    padding: 0 !important;
    margin: -1px !important;

    overflow: hidden !important;
    clip: rect(0, 0, 0, 0) !important;
    white-space: nowrap !important;

    border: 0 !important;
  }


  /* =========================================================
     CURRENT / PRIVATE WORK
     ========================================================= */

  .research-work.private-work .research-work-title {
    font-weight: 500;
  }

  .research-work.private-work .research-work-summary {
    max-width: 750px;
  }


  /* =========================================================
     OTHERS
     ========================================================= */

  .project-other .research-project-heading {
    margin-bottom: 0.45rem;

    font-size: 1.72rem;
    font-weight: 400;
  }

  .project-other .research-project-overview {
    max-width: 760px;

    margin-bottom: 2rem;
  }

  .project-other .research-work-title {
    font-weight: 500;
  }


  /* =========================================================
     DARK MODE
     ========================================================= */

  html[data-theme="dark"] .research-page,
  body[data-theme="dark"] .research-page {
    --research-blue: #7ea2d1;
    --research-green: #a0b97b;
    --research-orange: #df8b68;

    --research-text: #d6d2cd;
    --research-heading: #ece8e3;
    --research-muted: #aaa59e;
    --research-soft: #807b75;
    --research-rule: rgba(236, 232, 227, 0.12);
  }

  @media (prefers-color-scheme: dark) {
    .research-page {
      --research-blue: #7ea2d1;
      --research-green: #a0b97b;
      --research-orange: #df8b68;

      --research-text: #d6d2cd;
      --research-heading: #ece8e3;
      --research-muted: #aaa59e;
      --research-soft: #807b75;
      --research-rule: rgba(236, 232, 227, 0.12);
    }
  }


  /* =========================================================
     TABLET
     ========================================================= */

  @media (max-width: 960px) {

    .research-citation-line {
      white-space: normal;
    }


    main.container {
      max-width: 980px !important;
    }

    .research-hero {
      grid-template-columns: minmax(0, 1fr) 225px;

      gap: 2.6rem;
    }

    .research-diagram {
      width: 220px;
      height: 220px;
    }

    .research-body {
      grid-template-columns: 180px minmax(0, 1fr);

      column-gap: 2.8rem;
    }

    .research-tab {
      font-size: 0.93rem;
    }

  }


  /* =========================================================
     MOBILE
     ========================================================= */

  @media (max-width: 700px) {

    main.container {
      max-width: 100% !important;

      padding-left: 1.2rem;
      padding-right: 1.2rem;
    }

    .research-page {
      margin-top: -0.35rem;
      padding-top: 0;
      padding-bottom: 3rem;
    }

    .research-hero {
      display: block;

      margin-bottom: 1.9rem;
    }

    .research-title {
      margin-bottom: 0.82rem;

      font-size: 2.85rem;
      line-height: 1.02;
    }

    .research-intro {
      font-size: 1rem;
      line-height: 1.66;
    }

    .research-diagram {
      width: 190px;
      height: 190px;

      margin: 1.25rem auto 0;
    }


    /* ---------- Index ---------- */

    .research-body {
      display: block;
    }

    .research-tabs {
      position: static;

      display: flex;

      overflow-x: auto;
      overflow-y: hidden;

      width: 100%;

      margin: 0 0 1.7rem 0;

      border-top: 1px solid var(--research-rule);
      border-bottom: 1px solid var(--research-rule);

      scrollbar-width: none;

      -webkit-overflow-scrolling: touch;
    }

    .research-tabs::-webkit-scrollbar {
      display: none;
    }

    .research-tabs-label {
      display: none;
    }

    .research-tab {
      flex: 0 0 auto;

      width: auto;

      padding: 0.8rem 0.9rem;

      font-size: 0.88rem;

      white-space: nowrap;

      border-bottom: 2px solid transparent;
    }

    .research-tab:first-of-type {
      padding-left: 0;
    }

    .research-tab::before {
      display: none;
    }

    .research-tab:hover,
    .research-tab:focus {
      padding-left: 0.9rem;
    }

    .research-tab:first-of-type:hover,
    .research-tab:first-of-type:focus {
      padding-left: 0;
    }

    .research-tab-blue.active {
      border-bottom-color: var(--research-blue);
    }

    .research-tab-green.active {
      border-bottom-color: var(--research-green);
    }

    .research-tab-orange.active {
      border-bottom-color: var(--research-orange);
    }

    .research-tab-other.active {
      border-bottom-color: var(--research-muted);
    }


    /* ---------- Project ---------- */

    .research-panel {
      max-width: none;
    }

    .research-project-heading {
      font-size: 1.58rem;
      line-height: 1.24;
    }

    .research-project-question {
      margin-bottom: 0.95rem;

      font-size: 0.96rem;
    }

    .research-project-overview {
      margin-bottom: 1.35rem;
    }

    .research-project-overview p {
      font-size: 0.98rem;
      line-height: 1.66;
    }

    .research-subheading {
      margin-top: 1.45rem;

      font-size: 0.82rem;
    }


    /* ---------- Work ---------- */

    .research-work {
      padding-top: 0.68rem;
      padding-bottom: 0.74rem;
    }

    .research-work-head {
      display: block;
    }

    .research-work-title {
      font-size: 0.98rem;
      line-height: 1.42;
    }

    .research-work-status {
      display: block;

      margin: 0.12rem 0 0 0;

      font-size: 0.82rem;
    }

    .research-work-meta {
      margin-top: 0.13rem;

      font-size: 0.87rem;
    }

    .research-abstract {
      margin-top: 0;
    }

    .research-abstract summary {
      top: 1.95rem;
      right: 0;
    }

    .research-work.private-work .research-abstract summary {
      top: 0.7rem;
    }

    .research-work-summary {
      margin-top: 0.28rem;

      font-size: 0.9rem;
      line-height: 1.58;
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
        My primary research interest is the problem of perceptual objects: what the
        objects of perceptual experience are and how they can be directly present to us.
        I also work in the philosophy of emotion, especially on institutional formal
        objects and fittingness, and in the philosophy of language, especially on
        reference and temporal externalism.
      </p>

    </div>



    <!-- Three main research programs -->

    <div
      class="research-diagram"
      aria-hidden="true"
    >

      <img
        src="{{ '/assets/img/boy.png' | relative_url }}"
        alt=""
      >

    </div>

  </header>



  <div class="research-body">


  <!-- =======================================================
       TABS
       ======================================================= -->

  <div
    class="research-tabs"
    role="tablist"
    aria-label="Research projects"
  >


    <div class="research-tabs-label" aria-hidden="true">
      Research areas
    </div>


    <button
      class="research-tab research-tab-blue active"
      id="tab-perception"
      type="button"
      role="tab"
      aria-selected="true"
      aria-controls="research-perception"
      data-project="perception"
    >
      Perceptual Objects
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
      Others
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
        I am developing a broader account of perceptual objects and direct awareness.
        I want to understand how ordinary worldly objects figure in perceptual
        experience across different sensory modalities and perceptual contexts, and
        how a form of direct realism can accommodate illusion, hallucination, and
        other difficult cases while preserving the idea that perception genuinely
        puts us in touch with the world.
      </p>

    </div>



    <!-- Papers -->

    <div class="research-subheading">
      Papers
    </div>


    <div class="research-work-list">


      <!-- Tactile -->

      <article class="research-work published-work">

        <div class="research-citation-line">
          <span class="research-citation-title">A Tactile Screening-Off Problem for Naïve Realism.</span>
          <span class="research-citation-journal"> Analysis</span>,
          <span class="research-citation-status"> forthcoming</span>.
          <span class="research-work-link">
            <a
              href="https://doi.org/10.1093/analys/anag033"
              target="_blank"
              rel="noopener noreferrer"
            >[OUP]</a>
          </span>
        </div>


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I develop a screening-off problem for naïve realism that begins with
          ordinary tactile perception rather than hallucination. Using cases involving
          touch and realistic haptic simulation, I argue that the particular external
          object can become explanatorily redundant with respect to phenomenal
          character, putting pressure on the constitutive role assigned to worldly objects.
            </p>

          </div>

        </details>

      </article>



      <!-- Cross-modal -->

      <article class="research-work published-work">

        <div class="research-citation-line">
          <span class="research-citation-title">Cross-Modal Experiences and the Problem of Phenomenal Overlap.</span>
          <span class="research-citation-journal"> Journal of Consciousness Studies</span>,
          <span class="research-citation-status"> forthcoming</span>.
          <span class="research-work-link">
            <a
              href="https://philpapers.org/rec/YANCEA-3"
              target="_blank"
              rel="noopener noreferrer"
            >[manuscript]</a>
          </span>
        </div>


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I examine whether naïve realism can explain cases in which the same object
          is perceived through different sensory modalities but the resulting experiences
          seem phenomenally very different. I argue that appeals to abstract spatial
          commonality do not provide the relevant phenomenal overlap, leaving a
          significant problem for strong forms of naïve realism.
            </p>

          </div>

        </details>

      </article>


    </div>



    <!-- Current work -->

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


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I develop the central positive account of this research project and use it
          to clarify what it takes for perceptual awareness of ordinary objects to count
          as genuinely direct. The manuscript brings together several of the questions
          about perceptual objects that motivate my work in philosophy of perception.
            </p>

          </div>

        </details>

      </article>



      <!-- Hallucination manuscript -->

      <article class="research-work private-work">

        <div class="research-work-head">

          <div class="research-work-title">
            A manuscript on hallucination and direct realism
          </div>

          <div class="research-work-status">
            manuscript
          </div>

        </div>


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I examine the direction of the argument from hallucination and ask what
          justifies moving from a bad case to conclusions about veridical perception.
          I compare several ways of motivating that move and consider what the debate
          reveals about the pressure hallucination places on naïve realism.
            </p>

          </div>

        </details>

      </article>



      <!-- Illusion manuscript -->

      <article class="research-work private-work">

        <div class="research-work-head">

          <div class="research-work-title">
            A manuscript on illusion and perceptual correctness
          </div>

          <div class="research-work-status">
            manuscript
          </div>

        </div>


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I examine how judgments of perceptual error in color depend on the
          background conditions used to assess correctness. I use these cases to ask
          whether familiar arguments from illusion rely on assumptions about
          perceptual correctness that need to be made explicit before they can support
          conclusions about the objects of perception.
            </p>

          </div>

        </details>

      </article>


    </div>


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
        I am interested in how institutions and social practices shape the evaluative
        objects of our emotions. My aim is to understand when socially constituted
        standings such as prestige and stigma become part of what emotions respond to,
        and how the reality of such standings should be distinguished from the further
        question of whether they make admiration, contempt, or related emotions fitting.
      </p>

    </div>



    <!-- Papers -->

    <div class="research-subheading">
      Papers
    </div>


    <div class="research-work-list">


      <article class="research-work published-work">

        <div class="research-citation-line">
          <span class="research-citation-title">Institutional Formal Objects and Two-Level Fittingness.</span>
          <span class="research-citation-journal"> The Philosophical Quarterly</span>,
          <span class="research-citation-status"> forthcoming</span>.
          <span class="research-work-link">
            <a
              href="https://philpapers.org/rec/YANIFO"
              target="_blank"
              rel="noopener noreferrer"
            >[manuscript]</a>
          </span>
        </div>


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I introduce the idea of institutional formal objects and argue that socially
          constituted evaluative properties such as prestige and stigma can themselves
          enter the evaluative content of emotion, rather than merely serving as evidence
          of personal excellence or defect. I then develop a two-level account of
          fittingness for emotions directed at such institutional standings.
            </p>

          </div>

        </details>

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
            A manuscript on social context and institutional emotions
          </div>

          <div class="research-work-status">
            manuscript
          </div>

        </div>


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I examine how an emotion can respond to a social standing that varies across
          different social settings. I use these cases to ask how social context bears
          on which institutional standing an emotion attributes to its target, and how
          this in turn affects questions about emotional accuracy and fittingness.
            </p>

          </div>

        </details>

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
        I am interested in how reference is fixed and maintained across time,
        particularly when a community's present linguistic practice appears compatible
        with more than one candidate interpretation. I want to understand how much
        work can be done by present public practice before future use enters the
        metasemantic story, and what this tells us about semantic continuity,
        indeterminacy, and change.
      </p>

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


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I examine cases in which the applications of a public term are compatible
          with more than one candidate extension and ask what fixes its reference
          before later separating cases appear. I compare the role of present public
          practice with appeals to future linguistic use, with particular attention to
          semantic continuity and change across time.
            </p>

          </div>

        </details>

      </article>


    </div>


  </section>



  <!-- =======================================================
       OTHERS
       ======================================================= -->

  <section
    class="research-panel project-other"
    id="research-other"
    data-panel="other"
    role="tabpanel"
    aria-labelledby="tab-other"
  >


    <h2 class="research-project-heading">
      Others
    </h2>



    <div class="research-project-overview">

      <p>
        I wrote the paper below during my master's studies. I remain interested in
        questions about consciousness, attention, and phenomenal richness, but this
        is no longer one of the main directions of my current research.
      </p>

    </div>



    <div class="research-work-list">


      <article class="research-work published-work">

        <div class="research-citation-line">
          <span class="research-citation-title">Is Rich Phenomenology Fragmented?.</span>
          <span class="research-citation-journal"> Synthese</span>,
          <span class="research-citation-status research-citation-year"> 2025</span>.
          <span class="research-work-link">
            <a
              href="https://doi.org/10.1007/s11229-025-05058-8"
              target="_blank"
              rel="noopener noreferrer"
            >[Springer]</a>
          </span>
        </div>


        <details class="research-abstract">

          <summary aria-label="Toggle abstract">

            <span class="research-toggle-symbol" aria-hidden="true"></span>
            <span class="research-sr-only">Toggle abstract</span>

          </summary>

          <div class="research-abstract-body">

            <p class="research-work-summary">
          I revisit the debate between rich and fragmented views of phenomenal
          consciousness using evidence from the Sperling paradigm and related work
          on attention. I argue that data often taken to favour the Fragment View can
          also be accommodated by the Rich View, and that the latter retains important
          theoretical advantages.
            </p>

          </div>

        </details>

      </article>


    </div>


  </section>


  </div>


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

        item.setAttribute(
          "tabindex",
          "-1"
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

      tab.setAttribute(
        "tabindex",
        "0"
      );


      const targetPanel = document.querySelector(
        '.research-panel[data-panel="' + project + '"]'
      );


      if (targetPanel) {

        targetPanel.classList.add("active");

      }

    }



    tabs.forEach(function (tab, index) {

      if (!tab.classList.contains("active")) {

        tab.setAttribute(
          "tabindex",
          "-1"
        );

      }


      tab.addEventListener("click", function () {

        activateResearchTab(tab);

      });



      tab.addEventListener("keydown", function (event) {

        if (
          event.key !== "ArrowLeft" &&
          event.key !== "ArrowRight" &&
          event.key !== "ArrowUp" &&
          event.key !== "ArrowDown"
        ) {
          return;
        }


        event.preventDefault();


        let newIndex;


        if (
          event.key === "ArrowRight" ||
          event.key === "ArrowDown"
        ) {

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
