---
layout: page
title: talks
permalink: /talks/
description: 
nav: true
nav_order: 5

# ✅ 同一个 title 可以重复出现；每条 talk 只放一个会议（items 里只有 1 条）
talks:
  
  - title: "Situated Object and Illusion"
    selected: true
    items:
      - venue: "APA Eastern Division Meeting (122nd)"
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
      - venue: "APA Pacific Division Meeting (98th)"
        place: "San Francisco, USA"
        date: "Apr 2025"

  - title: "Do Semantic Properties Involve the Future?"
    selected: false
    items:
      - venue: "Talk"
        place: "Beijing, China"
        date: "2025"

  - title: "Is Rich Phenomenology Fragmented?"
    selected: true
    items:
      - venue: "APA Central Division Meeting (122nd)"
        place: "Online"
        date: "Feb/Mar 2025"

  - title: "Do Semantic Properties Involve the Future?"
    selected: true
    items:
      - venue: "APA Eastern Division Meeting (121st)"
        place: "New York, USA"
        date: "Jan 2025"

  - title: "MCICCR"
    selected: false
    items:
      - venue: "Australasian Association of Philosophy (AAP) Conference 2024"
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
.talks-refined {
  max-width: 900px;
  margin-top: 1.7rem;
}

.talk-entry {
  position: relative;
  display: grid;
  grid-template-columns: 6.5rem 1fr;
  gap: 1.6rem;
  padding: 1.15rem 0;
}

.talk-entry::before {
  content: "";
  position: absolute;
  left: 6.5rem;
  top: 0;
  bottom: 0;
  width: 1px;
  background: linear-gradient(
    to bottom,
    transparent,
    var(--global-divider-color) 18%,
    var(--global-divider-color) 82%,
    transparent
  );
}

.talk-entry::after {
  content: "";
  position: absolute;
  left: calc(6.5rem - 4px);
  top: 1.55rem;
  width: 9px;
  height: 9px;
  border-radius: 999px;
  background: var(--global-theme-color);
  box-shadow: 0 0 0 5px color-mix(in srgb, var(--global-theme-color) 12%, transparent);
}

.talk-date {
  padding-top: 0.16rem;
  font-size: 0.82rem;
  line-height: 1.28;
  color: var(--global-text-color-light);
  text-align: right;
  letter-spacing: 0.02em;
}

.talk-date strong {
  display: block;
  font-size: 0.88rem;
  font-weight: 500;
  color: var(--global-text-color);
}

.talk-body {
  padding-left: 0.25rem;
}

.talk-title {
  margin: 0;
  font-size: 1.02rem;
  font-weight: 500;
  line-height: 1.42;
  letter-spacing: -0.01em;
  color: var(--global-text-color);
}

.talk-meta {
  margin-top: 0.28rem;
  font-size: 0.9rem;
  line-height: 1.55;
  color: var(--global-text-color-light);
}

.talk-venue {
  color: var(--global-text-color);
}

.talk-place::before {
  content: " · ";
  color: var(--global-text-color-light);
}

.talk-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.38rem;
  margin-top: 0.55rem;
}

.talk-tag {
  font-size: 0.67rem;
  line-height: 1;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  border-radius: 999px;
  padding: 0.22rem 0.52rem;
  border: 1px solid transparent;
}

.talk-tag.peer {
  color: #6f4e00;
  background: #fff6df;
  border-color: #ead89b;
}

.talk-tag.abstract {
  color: #6b3b16;
  background: #fff0e6;
  border-color: #efc7aa;
}

.talk-tag.wip {
  color: #3d5f4a;
  background: #edf7f0;
  border-color: #c9e4d0;
}

.talk-tag.workshop {
  color: #34537a;
  background: #edf4fc;
  border-color: #c7d9ee;
}

@media (prefers-color-scheme: dark) {
  .talk-tag.peer {
    color: #f3d37a;
    background: rgba(126, 91, 12, 0.22);
    border-color: rgba(243, 211, 122, 0.32);
  }

  .talk-tag.abstract {
    color: #f0b084;
    background: rgba(128, 68, 29, 0.22);
    border-color: rgba(240, 176, 132, 0.32);
  }

  .talk-tag.wip {
    color: #a8d8b4;
    background: rgba(46, 99, 61, 0.22);
    border-color: rgba(168, 216, 180, 0.32);
  }

  .talk-tag.workshop {
    color: #a9c7ef;
    background: rgba(47, 83, 129, 0.22);
    border-color: rgba(169, 199, 239, 0.32);
  }
}

html[data-theme="dark"] .talk-tag.peer,
html.dark .talk-tag.peer,
body.dark .talk-tag.peer,
body.theme-dark .talk-tag.peer {
  color: #f3d37a;
  background: rgba(126, 91, 12, 0.22);
  border-color: rgba(243, 211, 122, 0.32);
}

html[data-theme="dark"] .talk-tag.abstract,
html.dark .talk-tag.abstract,
body.dark .talk-tag.abstract,
body.theme-dark .talk-tag.abstract {
  color: #f0b084;
  background: rgba(128, 68, 29, 0.22);
  border-color: rgba(240, 176, 132, 0.32);
}

html[data-theme="dark"] .talk-tag.wip,
html.dark .talk-tag.wip,
body.dark .talk-tag.wip,
body.theme-dark .talk-tag.wip {
  color: #a8d8b4;
  background: rgba(46, 99, 61, 0.22);
  border-color: rgba(168, 216, 180, 0.32);
}

html[data-theme="dark"] .talk-tag.workshop,
html.dark .talk-tag.workshop,
body.dark .talk-tag.workshop,
body.theme-dark .talk-tag.workshop {
  color: #a9c7ef;
  background: rgba(47, 83, 129, 0.22);
  border-color: rgba(169, 199, 239, 0.32);
}

@media (max-width: 650px) {
  .talk-entry {
    grid-template-columns: 1fr;
    gap: 0.35rem;
    padding: 1.05rem 0;
  }

  .talk-entry::before,
  .talk-entry::after {
    display: none;
  }

  .talk-date {
    text-align: left;
    padding-top: 0;
  }

  .talk-date strong {
    display: inline;
  }

  .talk-body {
    padding-left: 0;
  }

  .talk-place::before {
    content: "";
  }

  .talk-place {
    display: block;
  }
}
</style>

<div class="talks-refined">

  <article class="talk-entry">
    <div class="talk-date">
      <strong>Jan</strong>
      2026
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“New Object Theory and Illusion”</h2>
      <div class="talk-meta">
        <span class="talk-venue">Eastern APA</span>
        <span class="talk-place">Baltimore, USA</span>
      </div>
      <div class="talk-tags">
        <span class="talk-tag peer">Paper peer reviewed</span>
      </div>
    </div>
  </article>

  <article class="talk-entry">
    <div class="talk-date">
      <strong>Dec</strong>
      2025
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“Mediated Direct Realism”</h2>
      <div class="talk-meta">
        <span class="talk-venue">PKU Philosophy R&amp;W</span>
        <span class="talk-place">Beijing, China</span>
      </div>
    </div>
  </article>

  <article class="talk-entry">
    <div class="talk-date">
      <strong>Apr</strong>
      2025
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“Do Semantic Properties Involve the Future?”</h2>
      <div class="talk-meta">
        <span class="talk-venue">Pacific APA</span>
        <span class="talk-place">San Francisco, USA</span>
      </div>
      <div class="talk-tags">
        <span class="talk-tag peer">Paper peer reviewed</span>
      </div>
    </div>
  </article>

  <article class="talk-entry">
    <div class="talk-date">
      <strong>Jan</strong>
      2025
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“Do Semantic Properties Involve the Future?”</h2>
      <div class="talk-meta">
        <span class="talk-venue">Eastern APA</span>
        <span class="talk-place">New York, USA</span>
      </div>
      <div class="talk-tags">
        <span class="talk-tag wip">W.I.P.</span>
      </div>
    </div>
  </article>

  <article class="talk-entry">
    <div class="talk-date">
      <strong>2025</strong>
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“Do Semantic Properties Involve the Future?”</h2>
      <div class="talk-meta">
        <span class="talk-venue">Talk</span>
        <span class="talk-place">Beijing, China</span>
      </div>
    </div>
  </article>

  <article class="talk-entry">
    <div class="talk-date">
      <strong>Feb/Mar</strong>
      2025
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“Is Rich Phenomenology Fragmented?”</h2>
      <div class="talk-meta">
        <span class="talk-venue">Central APA</span>
        <span class="talk-place">Online</span>
      </div>
      <div class="talk-tags">
        <span class="talk-tag peer">Paper peer reviewed</span>
      </div>
    </div>
  </article>

  <article class="talk-entry">
    <div class="talk-date">
      <strong>Jul</strong>
      2024
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“MCICCR”</h2>
      <div class="talk-meta">
        <span class="talk-venue">Annual Conference of the Australasian Association of Philosophy</span>
        <span class="talk-place">Perth, Australia</span>
      </div>
      <div class="talk-tags">
        <span class="talk-tag abstract">Abstract peer reviewed</span>
      </div>
    </div>
  </article>

  <article class="talk-entry">
    <div class="talk-date">
      <strong>Apr</strong>
      2024
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“MCICCR”</h2>
      <div class="talk-meta">
        <span class="talk-venue">Workshop for Young Scholars in Science and Philosophy</span>
        <span class="talk-place">Beijing, China</span>
      </div>
      <div class="talk-tags">
        <span class="talk-tag peer">Paper peer reviewed</span>
      </div>
    </div>
  </article>

  <article class="talk-entry">
    <div class="talk-date">
      <strong>Mar</strong>
      2024
    </div>

    <div class="talk-body">
      <h2 class="talk-title">“MCICCR”</h2>
      <div class="talk-meta">
        <span class="talk-venue">PKU Philosophy R&amp;W</span>
        <span class="talk-place">Beijing, China</span>
      </div>
    </div>
  </article>

</div>
