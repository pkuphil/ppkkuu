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
  max-width: 680px;
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
  background:
    linear-gradient(
      135deg,
      rgba(255, 255, 255, 0.04),
      rgba(255, 255, 255, 0)
    ),
    var(--global-card-bg-color);
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
    This page lists selected research projects currently in progress, including manuscripts under review, revise-and-resubmit projects, and early-stage work.
  </p>

  <div class="wip-list">

    <article class="wip-item">
      <div class="wip-number">01</div>

      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">你的第一个研究主题标题</h2>
          <span class="wip-status">R&amp;R at Journal Name</span>
        </div>

        <p class="wip-description">
          This project examines how local political incentives shape development outcomes. 
          It studies the conditions under which officials prioritize long-term growth, public goods provision, 
          and institutional reform.
        </p>

        <div class="wip-meta">
          <span class="wip-tag">political economy</span>
          <span class="wip-tag">local governance</span>
          <span class="wip-tag">development</span>
        </div>
      </div>
    </article>

    <article class="wip-item">
      <div class="wip-number">02</div>

      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">你的第二个研究主题标题</h2>
          <span class="wip-status subtle">working paper</span>
        </div>

        <p class="wip-description">
          This paper investigates how bureaucratic capacity affects policy implementation across regions. 
          It combines administrative data with institutional analysis to explain variation in policy outcomes.
        </p>

        <div class="wip-meta">
          <span class="wip-tag">bureaucracy</span>
          <span class="wip-tag">institutions</span>
          <span class="wip-tag">policy implementation</span>
        </div>
      </div>
    </article>

    <article class="wip-item">
      <div class="wip-number">03</div>

      <div class="wip-content">
        <div class="wip-topline">
          <h2 class="wip-title">你的第三个研究主题标题</h2>
          <span class="wip-status subtle">early stage</span>
        </div>

        <p class="wip-description">
          This project explores how information flows shape accountability and public service delivery. 
          It focuses on how citizens, officials, and intermediaries respond to new forms of political information.
        </p>

        <div class="wip-meta">
          <span class="wip-tag">accountability</span>
          <span class="wip-tag">information</span>
          <span class="wip-tag">public services</span>
        </div>
      </div>
    </article>

  </div>
</div>
