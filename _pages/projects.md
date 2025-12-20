---
layout: page
title: talks
permalink: /talks/
description: Talks and presentations.
nav: true
nav_order: 3

# ✅ 同一个 title 可以重复出现；每条 talk 只放一个会议（items 里只有 1 条）
talks:
  - title: "New Object Theory and Illusion"
    selected: true
    items:
      - venue: "Eastern APA"
        place: "Baltimore, USA"
        date: "Jan 2026"

  - title: "Mediated Direct Realism"
    selected: true
    items:
      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "Dec 2025"

  - title: "Do Semantic Properties Involve the Future?"
    selected: true
    items:
      - venue: "Pacific APA"
        place: "San Francisco, USA"
        date: "Apr 2025"

  - title: "Do Semantic Properties Involve the Future?"
    selected: true
    items:
      - venue: "Eastern APA"
        place: "New York, USA"
        date: "Jan 2025"

  - title: "Do Semantic Properties Involve the Future?"
    selected: false
    items:
      - venue: "Talk"
        place: "Beijing, China"
        date: "2025"

  - title: "Is Rich Phenomenology Fragmented?"
    selected: true
    items:
      - venue: "Central APA"
        place: "Online"
        date: "Feb/Mar 2025"

  - title: "MCICCR"
    selected: false
    items:
      - venue: "Annual Conference of the Australasian Association of Philosophy"
        place: "Perth, Australia"
        date: "Jul 2024"

  - title: "MCICCR"
    selected: false
    items:
      - venue: "Workshop for Young Scholars in Science and Philosophy"
        place: "Beijing, China"
        date: "Apr 2024"

  - title: "MCICCR"
    selected: false
    items:
      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "Mar 2024"
---

<style>
  /* =========================
     Classic Jekyll/CV-style talks list
     - no cards, no colored pills
     - clean separators
     - right-aligned date column
     ========================= */

  .talks-classic{
    margin-top: 1.25rem;
  }

  .talk-block{
    margin: 0 0 1.8rem 0;
  }

  .talk-title{
    margin: 0 0 .55rem 0;
    font-weight: 600;
    letter-spacing: .1px;
  }

  .talk-list{
    list-style: none;
    margin: 0;
    padding: 0;
    border-top: 1px solid rgba(0,0,0,.12);
  }

  .talk-li{
    padding: .65rem 0;
    border-bottom: 1px solid rgba(0,0,0,.10);
  }

  /* two-column row: left info + right date */
  .talk-row{
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 9.5rem;
    column-gap: 1rem;
    align-items: start;
  }

  .talk-left{ min-width: 0; }

  .talk-venue-line{
    display: flex;
    flex-wrap: wrap;
    align-items: baseline;
    gap: .35rem .5rem;
    line-height: 1.25;
  }

  .talk-venue{
    font-weight: 600;
  }

  .talk-place{
    margin-top: .15rem;
    font-size: .92rem;
    opacity: .75;
    line-height: 1.25;
  }

  .talk-date{
    text-align: right;
    white-space: nowrap;
    font-variant-numeric: tabular-nums;
    opacity: .85;
    padding-top: .02rem;
  }

  /* make your existing .tag spans look like classic inline text */
  .talk-tags{
    font-size: .92rem;
    opacity: .75;
  }
  .talk-tags::before{ content: "("; }
  .talk-tags::after{ content: ")"; }

  .talk-tags .tag{
    background: transparent !important;
    border: 0 !important;
    padding: 0 !important;
    border-radius: 0 !important;
    font-weight: 400 !important;
    font-size: inherit !important;
    color: inherit !important;
    line-height: inherit !important;
    letter-spacing: 0 !important;
    white-space: normal !important;
  }

  /* separators between tags */
  .talk-tags .tag + .tag::before{
    content: "; ";
  }

  /* mobile: date drops below */
  @media (max-width: 520px){
    .talk-row{
      grid-template-columns: 1fr;
      row-gap: .25rem;
    }
    .talk-date{
      text-align: left;
    }
  }

  /* dark mode: softer borders */
  @media (prefers-color-scheme: dark){
    .talk-list{ border-top-color: rgba(255,255,255,.16); }
    .talk-li{ border-bottom-color: rgba(255,255,255,.14); }
  }

  html[data-theme="dark"] .talk-list,
  html.dark .talk-list,
  body.dark .talk-list,
  body.theme-dark .talk-list{
    border-top-color: rgba(255,255,255,.16);
  }

  html[data-theme="dark"] .talk-li,
  html.dark .talk-li,
  body.dark .talk-li,
  body.theme-dark .talk-li{
    border-bottom-color: rgba(255,255,255,.14);
  }
</style>

<div class="talks-classic">

  <!-- Talk 1 -->
  <section class="talk-block">
    <h2 class="talk-title">“New Object Theory and Illusion”</h2>
    <ul class="talk-list">
      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">Eastern APA</span>
              <span class="talk-tags">
                <span class="tag tag--type">Colloquium</span>
                <span class="tag tag--review">paper peer-reviewed</span>
              </span>
            </div>
            <div class="talk-place">Baltimore, USA</div>
          </div>
          <div class="talk-date">Jan 2026</div>
        </div>
      </li>
    </ul>
  </section>

  <!-- Talk 2 -->
  <section class="talk-block">
    <h2 class="talk-title">“Mediated Direct Realism”</h2>
    <ul class="talk-list">
      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">PKU Philosophy R&amp;W</span>
            </div>
            <div class="talk-place">Beijing, China</div>
          </div>
          <div class="talk-date">Dec 2025</div>
        </div>
      </li>
    </ul>
  </section>

  <!-- Talk 3 -->
  <section class="talk-block">
    <h2 class="talk-title">“Do Semantic Properties Involve the Future?”</h2>
    <ul class="talk-list">

      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">Pacific APA</span>
              <span class="talk-tags">
                <span class="tag tag--type">Colloquium</span>
                <span class="tag tag--review">paper peer-reviewed</span>
              </span>
            </div>
            <div class="talk-place">San Francisco, USA</div>
          </div>
          <div class="talk-date">Apr 2025</div>
        </div>
      </li>

      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">Eastern APA</span>
              <span class="talk-tags">
                <span class="tag tag--wip">W.I.P.</span>
              </span>
            </div>
            <div class="talk-place">New York, USA</div>
          </div>
          <div class="talk-date">Jan 2025</div>
        </div>
      </li>

      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">Talk</span>
            </div>
            <div class="talk-place">Beijing, China</div>
          </div>
          <div class="talk-date">2025</div>
        </div>
      </li>

    </ul>
  </section>

  <!-- Talk 4 -->
  <section class="talk-block">
    <h2 class="talk-title">“Is Rich Phenomenology Fragmented?”</h2>
    <ul class="talk-list">
      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">Central APA</span>
              <span class="talk-tags">
                <span class="tag tag--type">Colloquium</span>
                <span class="tag tag--review">paper peer-reviewed</span>
              </span>
            </div>
            <div class="talk-place">Online</div>
          </div>
          <div class="talk-date">Feb/Mar 2025</div>
        </div>
      </li>
    </ul>
  </section>

  <!-- Talk 5 -->
  <section class="talk-block">
    <h2 class="talk-title">“MCICCR”</h2>
    <ul class="talk-list">

      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">Annual Conference of the Australasian Association of Philosophy</span>
              <span class="talk-tags">
                <span class="tag tag--type">Colloquium</span>
              </span>
            </div>
            <div class="talk-place">Perth, Australia</div>
          </div>
          <div class="talk-date">Jul 2024</div>
        </div>
      </li>

      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">Workshop for Young Scholars in Science and Philosophy</span>
              <span class="talk-tags">
                <span class="tag tag--type">Colloquium</span>
                <span class="tag tag--review">paper peer-reviewed</span>
              </span>
            </div>
            <div class="talk-place">Beijing, China</div>
          </div>
          <div class="talk-date">Apr 2024</div>
        </div>
      </li>

      <li class="talk-li">
        <div class="talk-row">
          <div class="talk-left">
            <div class="talk-venue-line">
              <span class="talk-venue">PKU Philosophy R&amp;W</span>
            </div>
            <div class="talk-place">Beijing, China</div>
          </div>
          <div class="talk-date">Mar 2024</div>
        </div>
      </li>

    </ul>
  </section>

</div>
