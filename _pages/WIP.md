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
    max-width: 740px;

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
    max-width: 800px;

    margin: 0 0 0.38rem 0;

    font-family: inherit;
    font-size: 1.65rem;
    font-weight: 500;
    line-height: 1.25;

    letter-spacing: -0.018em;

    color: var(--global-text-color, inherit);
  }

  .research-project-question {
    max-width: 760px;

    margin: 0 0 1.45rem 0;

    font-size: 0.98rem;
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

    margin-bottom: 2.25rem;
  }

  .research-project-overview p {
    margin: 0;

    font-size: 0.96rem;
    font-weight: 400;
    line-height: 1.7;

    color: var(--global-text-color, inherit);
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
    max-width: 850px;

    margin: 0;
    padding: 0;

    border-top: 1px solid var(--global-divider-color, #e2e2e2);
  }

  .research-work {
    margin: 0;

    padding: 0.95rem 0 1.05rem 0;

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

    font-size: 0.98rem;
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
    margin-top: 0.14rem;

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
     PAPER DESCRIPTION
     ========================================================= */

  .research-work-summary {
    max-width: 780px;

    margin: 0.48rem 0 0 0;

    font-size: 0.87rem;
    font-weight: 400;
    line-height: 1.62;

    color: var(--global-text-color-light, #686d72);
  }


  /* =========================================================
     CURRENT / PRIVATE WORK
     ========================================================= */

  .research-work.private-work .research-work-title {
    font-weight: 500;
  }

  .research-work.private-work .research-work-summary {
    max-width: 760px;
  }


  /* =========================================================
     OTHER WORK
     ========================================================= */

  .project-other .research-project-heading {
    margin-bottom: 0.45rem;

    font-size: 1.5rem;
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

    .research-project-overview {
      margin-bottom: 1.8rem;
    }

    .research-project-overview p {
      font-size: 0.92rem;
      line-height: 1.62;
    }


    /* Work */

    .research-subheading {
      margin-top: 1.7rem;
    }

    .research-work {
      padding-top: 0.8rem;
      padding-bottom: 0.9rem;
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
      margin-top: 0.4rem;

      font-size: 0.83rem;
      line-height: 1.56;
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
        I am developing a broader account of perceptual objects and direct awareness.
        I want to understand how ordinary worldly objects figure in perceptual
        experience across different sensory modalities and perceptual contexts, and
        how a form of direct realism can accommodate illusion, hallucination, and
        other difficult cases while preserving the idea that perception genuinely
        puts us in touch with the world.
      </p>

    </div>



    <!-- Published & forthcoming -->

    <div class="research-subheading">
      Published &amp; forthcoming
    </div>


    <div class="research-work-list">


      <!-- Tactile -->

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
          I develop a screening-off problem for naïve realism that begins with
          ordinary tactile perception rather than hallucination. Using cases involving
          touch and realistic haptic simulation, I argue that the particular external
          object can become explanatorily redundant with respect to phenomenal
          character, putting pressure on the constitutive role assigned to worldly objects.
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
          I examine whether naïve realism can explain cases in which the same object
          is perceived through different sensory modalities but the resulting experiences
          seem phenomenally very different. I argue that appeals to abstract spatial
          commonality do not provide the relevant phenomenal overlap, leaving a
          significant problem for strong forms of naïve realism.
        </p>

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


        <p class="research-work-summary">
          I develop the central positive account of this research project and use it
          to clarify what it takes for perceptual awareness of ordinary objects to count
          as genuinely direct. The manuscript brings together several of the questions
          about perceptual objects that motivate my work in philosophy of perception.
        </p>

      </article>



      <!-- Context manuscript -->

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
          I examine how changes in perceptual context bear on the objects and
          phenomenal character of experience. I use these cases to ask how a theory
          of perceptual objects should accommodate contextual variation without
          losing sight of the worldly objects that perception appears to present.
        </p>

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
          I introduce the idea of institutional formal objects and argue that socially
          constituted evaluative properties such as prestige and stigma can themselves
          enter the evaluative content of emotion, rather than merely serving as evidence
          of personal excellence or defect. I then develop a two-level account of
          fittingness for emotions directed at such institutional standings.
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


        <p class="research-work-summary">
          I examine cases in which the applications of a public term are compatible
          with more than one candidate extension and ask what fixes its reference
          before later separating cases appear. I compare the role of present public
          practice with appeals to future linguistic use, with particular attention to
          semantic continuity and change across time.
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



    <div class="research-project-overview">

      <p>
        I wrote the paper below during my master's studies. I remain interested in
        questions about consciousness, attention, and phenomenal richness, but this
        is no longer one of the main directions of my current research.
      </p>

    </div>



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
          I revisit the debate between rich and fragmented views of phenomenal
          consciousness using evidence from the Sperling paradigm and related work
          on attention. I argue that data often taken to favour the Fragment View can
          also be accommodated by the Rich View, and that the latter retains important
          theoretical advantages.
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
