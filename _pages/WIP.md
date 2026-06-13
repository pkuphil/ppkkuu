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
}

.wip-intro {
  max-width: 690px;
  margin-bottom: 2.4rem;
  font-size: 0.98rem;
  line-height: 1.75;
  color: var(--global-text-color-light);
}

.wip-list {
  display: flex;
  flex-direction: column;
  gap: 1.15rem;
}

.wip-item {
  display: grid;
  grid-template-columns: 56px 1fr;
  gap: 1.4rem;
  padding: 1.45rem 1.55rem;
  border: 1px solid var(--global-divider-color);
  border-radius: 18px;
  background: var(--global-card-bg-color);
  transition: transform 0.18s ease, box-shadow 0.18s ease, border-color 0.18s ease;
}

.wip-item:hover {
  transform: translateY(-2px);
  border-color: color-mix(in srgb, var(--global-theme-color) 45%, var(--global-divider-color));
  box-shadow: 0 12px 28px rgba(0, 0, 0, 0.06);
}

.wip-number {
  font-size: 0.78rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--global-text-color-light);
  padding-top: 0.22rem;
}

.wip-content {
  min-width: 0;
}

.wip-topline {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 1rem;
  margin-bottom: 0.55rem;
}

.wip-title {
  margin: 0;
  font-size: 1.18rem;
  font-weight: 500;
  line-height: 1.38;
  letter-spacing: -0.01em;
}

.wip-status {
  flex-shrink: 0;
  font-size: 0.68rem;
  font-weight: 600;
  letter-spacing: 0.045em;
  text-transform: uppercase;
  padding: 0.24rem 0.62rem;
  border-radius: 999px;
  color: var(--global-theme-color);
  background: color-mix(in srgb, var(--global-theme-color) 9%, transparent);
  border: 1px solid color-mix(in srgb, var(--global-theme-color) 35%, transparent);
  white-space: nowrap;
}

.wip-status.subtle {
  color: var(--global-text-color-light);
  background: transparent;
  border-color: var(--global-divider-color);
}

.wip-description {
  max-width: 760px;
  margin: 0.2rem 0 0.85rem;
  font-size: 0.96rem;
  line-height: 1.72;
  color: var(--global-text-color);
}

.wip-meta {
  display: flex;
  flex-wrap: wrap;
  gap: 0.45rem;
  margin-top: 0.15rem;
}

.wip-tag {
  font-size: 0.7rem;
  letter-spacing: 0.025em;
  color: var(--global-text-color-light);
  padding: 0.16rem 0.52rem;
  border-radius: 999px;
  border: 1px solid var(--global-divider-color);
  background: rgba(127, 127, 127, 0.035);
}

@media (max-width: 700px) {
  .wip-item {
    grid-template-columns: 1fr;
    gap: 0.55rem;
    padding: 1.25rem 1.2rem;
  }

  .wip-topline {
    flex-direction: column;
    gap: 0.45rem;
  }

  .wip-number {
    padding-top: 0;
  }
}
</style>

<div class="wip-container">

  <p class="wip-intro">
    This page lists selected research projects currently in progress. The descriptions are intentionally brief and non-technical, highlighting the broad questions behind each project.
  </p>

  <div class="wip-list">

    <article class="wip-item">
      <div class="wip-number">01</div>

      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">A paper about institutional status and social emotions</h2>
          <span class="wip-status">R&amp;R at Philosophical Quarterly</span>
        </div>

        <p class="wip-description">
          This paper asks why certain social labels, roles, and credentials can shape our emotional responses to people so powerfully. 
          It develops a framework for understanding how emotions may track institutionally constituted forms of status, while also asking when such responses are genuinely fitting and when they become normatively questionable.
        </p>

        <div class="wip-meta">
          <span class="wip-tag">philosophy of emotion</span>
          <span class="wip-tag">social ontology</span>
          <span class="wip-tag">fittingness</span>
        </div>
      </div>
    </article>

    <article class="wip-item">
      <div class="wip-number">02</div>

      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">A paper about perception and mediation</h2>
          <span class="wip-status subtle">manuscript</span>
        </div>

        <p class="wip-description">
          This paper revisits the contrast between direct and indirect realism in the philosophy of perception. 
          It argues that mediation need not block direct awareness of ordinary objects, and explores a model on which perceptual experience can involve a mediating element without placing the world behind a veil.
        </p>

        <div class="wip-meta">
          <span class="wip-tag">philosophy of perception</span>
          <span class="wip-tag">direct realism</span>
          <span class="wip-tag">hallucination</span>
        </div>
      </div>
    </article>

    <article class="wip-item">
      <div class="wip-number">03</div>

      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">A paper about reference and linguistic practice</h2>
          <span class="wip-status subtle">manuscript</span>
        </div>

        <p class="wip-description">
          This paper examines how a community's existing linguistic practice can help determine what its words refer to, even when several possible extensions initially look equally compatible with use. 
          It offers a practice-based account of how patterns of judgment, correction, and projection can already favor one interpretation over others.
        </p>

        <div class="wip-meta">
          <span class="wip-tag">philosophy of language</span>
          <span class="wip-tag">reference</span>
          <span class="wip-tag">metasemantics</span>
        </div>
      </div>
    </article>

  </div>
</div>
