---
layout: page
title: talks
permalink: /talks/
description:
nav: true
nav_order: 5

talks:
  - title: "Situated Objects and Illusion"
    selected: false
    items:
      - venue: "Society for Exact Philosophy Annual Meeting"
        place: "Vancouver, Canada"
        date: "May 2026"
        tag: "peer"
        tag_label: "Paper peer reviewed"
        note: "Cancelled due to dissertation defense."

  - title: "Mediated Direct Realism"
    selected: false
    items:
      - venue: "Institute of Philosophy, Chinese Academy of Sciences"
        place: "Beijing, China"
        date: "Apr 2026"

  - title: "Situated Object and Illusion"
    selected: true
    items:
      - venue: "APA Eastern Division Meeting (122nd)"
        place: "Baltimore, USA"
        date: "Jan 2026"
        tag: "peer"
        tag_label: "Paper peer reviewed"

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
        tag: "peer"
        tag_label: "Paper peer reviewed"

  - title: "Is Rich Phenomenology Fragmented?"
    selected: true
    items:
      - venue: "APA Central Division Meeting (122nd)"
        place: "Online"
        date: "Feb/Mar 2025"
        tag: "peer"
        tag_label: "Paper peer reviewed"

  - title: "Do Semantic Properties Involve the Future?"
    selected: true
    items:
      - venue: "APA Eastern Division Meeting (121st)"
        place: "New York, USA"
        date: "Jan 2025"
        tag: "wip"
        tag_label: "W.I.P."

  - title: "Do Semantic Properties Involve the Future?"
    selected: false
    items:
      - venue: "Talk"
        place: "Beijing, China"
        date: "2025"

  - title: "MCICCR"
    selected: false
    items:
      - venue: "Australasian Association of Philosophy Conference"
        place: "Perth, Australia"
        date: "Jul 2024"
        tag: "abstract"
        tag_label: "Abstract peer reviewed"

  - title: "MCICCR"
    selected: false
    items:
      - venue: "Workshop for Young Scholars in Science and Philosophy"
        place: "Beijing, China"
        date: "Apr 2024"
        tag: "peer"
        tag_label: "Paper peer reviewed"

  - title: "MCICCR"
    selected: false
    items:
      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "Mar 2024"
---

<style>
.talks-list {
  max-width: 920px;
  margin-top: 2.2rem;
  counter-reset: talk-counter;
}

.talk-entry {
  position: relative;
  counter-increment: talk-counter;
  padding-left: 3.05rem;
  padding-bottom: 1.15rem;
  margin-bottom: 1.15rem;
  border-bottom: 1px solid var(--global-divider-color);
}

.talk-entry:last-child {
  border-bottom: none;
}

.talk-entry::before {
  content: counter(talk-counter);
  position: absolute;
  left: 0;
  top: 0.03rem;
  width: 1.6rem;
  text-align: right;
  color: var(--global-theme-color);
  font-weight: 500;
  letter-spacing: 0.04em;
}

.talk-title {
  margin: 0;
  font-size: inherit;
  font-weight: bolder;
  line-height: inherit;
  color: var(--global-text-color);
}

.talk-meta {
  margin-top: 0.28rem;
  color: var(--global-text-color-light);
  line-height: 1.45;
}

.talk-venue {
  color: var(--global-theme-color);
  font-family: "Cormorant Garamond", "EB Garamond", "Georgia", serif;
  font-style: italic;
  font-weight: 500;
  letter-spacing: 0.015em;
  text-decoration: none !important;
}

.talk-date {
  color: var(--global-text-color-light);
}

.talk-place::before,
.talk-date::before {
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

.talk-note-muted {
  margin-top: 0.42rem;
  color: var(--global-text-color-light);
  font-style: italic;
  font-size: 0.875rem;
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

@media (max-width: 576px) {
  .talk-entry {
    padding-left: 2.35rem;
    margin-bottom: 1.05rem;
    padding-bottom: 1.05rem;
  }

  .talk-entry::before {
    width: 1.35rem;
  }

  .talk-place,
  .talk-date {
    display: block;
  }

  .talk-place::before,
  .talk-date::before {
    content: "";
  }
}
</style>

<div class="talks-list">
  {% for talk in page.talks %}
    {% assign item = talk.items | first %}

    <article class="talk-entry">
      <h2 class="talk-title">“{{ talk.title }}”</h2>

      <div class="talk-meta">
        <span class="talk-venue">{{ item.venue }}</span>
        {% if item.place %}
          <span class="talk-place">{{ item.place }}</span>
        {% endif %}
        {% if item.date %}
          <span class="talk-date">{{ item.date }}</span>
        {% endif %}
      </div>

      {% if item.tag_label %}
        <div class="talk-tags">
          <span class="talk-tag {{ item.tag }}">{{ item.tag_label }}</span>
        </div>
      {% endif %}

      {% if item.note %}
        <div class="talk-note-muted">{{ item.note }}</div>
      {% endif %}
    </article>
  {% endfor %}
</div>
