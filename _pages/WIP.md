---
layout: page
permalink: /WIP/
title: work in progress
nav_title: wip
nav: true
nav_order: 3
---

<style>
.wip-container {
  max-width: 920px;
  margin-top: 2.2rem;
  counter-reset: wip-counter;
}

.wip-list {
  display: block;
}

.wip-item {
  position: relative;
  counter-increment: wip-counter;
  padding-left: 3.05rem;
  padding-bottom: 1.15rem;
  margin-bottom: 1.15rem;
  border-bottom: 1px solid var(--global-divider-color);
}

.wip-item:last-child {
  border-bottom: none;
}

.wip-item::before {
  content: counter(wip-counter);
  position: absolute;
  left: 0;
  top: 0.03rem;
  width: 1.6rem;
  text-align: right;
  color: var(--global-theme-color);
  font-weight: 500;
  letter-spacing: 0.04em;
}

.wip-content {
  min-width: 0;
}

.wip-topline {
  display: block;
  margin-bottom: 0.28rem;
}

.wip-title {
  margin: 0;
  font-size: inherit;
  font-weight: bolder;
  line-height: inherit;
  color: var(--global-text-color);
}

.wip-status {
  display: inline-block;
  margin-top: 0.28rem;
  color: var(--global-theme-color);
  font-family: "Cormorant Garamond", "EB Garamond", "Georgia", serif;
  font-style: italic;
  font-weight: 500;
  letter-spacing: 0.015em;
  text-decoration: none !important;
}

.wip-status.subtle {
  color: var(--global-text-color-light);
}

.wip-description {
  max-width: 760px;
  margin: 0.55rem 0 0.7rem;
  color: var(--global-text-color);
  line-height: 1.62;
}

@media (max-width: 576px) {
  .wip-container {
    max-width: 100%;
  }

  .wip-item {
    padding-left: 2.35rem;
    margin-bottom: 1.05rem;
    padding-bottom: 1.05rem;
  }

  .wip-item::before {
    width: 1.35rem;
  }
}
</style>

<div class="wip-container">
  <div class="wip-list">

    <article class="wip-item">
      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">A paper about institutional status and social emotions</h2>
          <span class="wip-status">R&amp;R at The Philosophical Quarterly</span>
        </div>

        <p class="wip-description">
          I ask why certain social labels, roles, and credentials can shape our emotional responses to people so powerfully.
          I develop a framework for understanding how emotions may track institutionally constituted forms of status, while also asking when such responses are genuinely fitting and when they become normatively questionable.
        </p>
      </div>
    </article>

    <article class="wip-item">
      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">A paper about perception and mediation</h2>
          <span class="wip-status subtle">manuscript</span>
        </div>

        <p class="wip-description">
          I revisit the contrast between direct and indirect realism in the philosophy of perception.
          I argue that mediation need not block direct awareness of ordinary objects, and explore a model on which perceptual experience can involve a mediating element without placing the world behind a veil.
        </p>
      </div>
    </article>

    <article class="wip-item">
      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">A paper about reference and linguistic practice</h2>
          <span class="wip-status subtle">manuscript</span>
        </div>

        <p class="wip-description">
          I examine how a community's existing linguistic practice can help determine what its words refer to, even when several possible extensions initially look equally compatible with use.
          I offer a practice-based account of how patterns of judgment, correction, and projection can already favor one interpretation over others.
        </p>
      </div>
    </article>

  </div>
</div>
