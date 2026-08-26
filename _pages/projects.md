---
layout: page
title: talks
permalink: /talks/
description:
nav: false
nav_order: 5

talks:
  - title: "Situated Objects and Illusion"
    selected: false
    type: "peer-reviewed colloquium"
    items:
      - venue: "Society for Exact Philosophy Annual Meeting"
        place: "Vancouver, Canada"
        date: "May 2026"
        note: "Cancelled due to dissertation defense."

  - title: "Mediated Direct Realism"
    selected: false
    items:
      - venue: "Institute of Philosophy, Chinese Academy of Sciences"
        place: "Beijing, China"
        date: "Apr 2026"

  - title: "Situated Object and Illusion"
    selected: true
    type: "peer-reviewed colloquium"
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
    type: "peer-reviewed colloquium"
    items:
      - venue: "APA Pacific Division Meeting (98th)"
        place: "San Francisco, USA"
        date: "Apr 2025"

  - title: "Is Rich Phenomenology Fragmented?"
    selected: true
    type: "peer-reviewed colloquium"
    items:
      - venue: "APA Central Division Meeting (122nd)"
        place: "Online"
        date: "Feb/Mar 2025"

  - title: "Do Semantic Properties Involve the Future?"
    selected: true
    type: "w.i.p."
    items:
      - venue: "APA Eastern Division Meeting (121st)"
        place: "New York, USA"
        date: "Jan 2025"

  - title: "Do Semantic Properties Involve the Future?"
    selected: false
    items:
      - venue: "Talk"
        place: "Beijing, China"
        date: "2025"

  - title: "MCICCR"
    selected: false
    type: "abstract peer-reviewed colloquium"
    items:
      - venue: "Australasian Association of Philosophy Conference"
        place: "Perth, Australia"
        date: "Jul 2024"

  - title: "MCICCR"
    selected: false
    type: "peer-reviewed colloquium"
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
.talks-container {
  max-width: 920px;
  margin-top: 2.2rem;
  counter-reset: talk-counter;
}

.talks-list {
  display: block;
}

.talk-item {
  position: relative;
  counter-increment: talk-counter;
  padding-left: 3.05rem;
  padding-bottom: 1.15rem;
  margin-bottom: 1.15rem;
  border-bottom: 1px solid var(--global-divider-color);
}

.talk-item:last-child {
  border-bottom: none;
}

.talk-item::before {
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

.talk-content {
  min-width: 0;
}

.talk-topline {
  display: flex;
  align-items: baseline;
  flex-wrap: wrap;
  gap: 0.45rem 0.6rem;
  margin-bottom: 0.28rem;
}

.talk-title {
  margin: 0;
  font-size: inherit;
  font-weight: bolder;
  line-height: inherit;
  color: var(--global-text-color);
}

.talk-kind {
  display: inline-flex;
  align-items: center;
  transform: translateY(-0.04rem);
  padding: 0.14rem 0.48rem;
  border: 1px solid var(--global-divider-color);
  border-radius: 999px;
  color: var(--global-text-color-light);
  background: transparent;
  font-size: 0.64rem;
  line-height: 1;
  letter-spacing: 0.055em;
  text-transform: uppercase;
  white-space: nowrap;
}

.talk-meta {
  margin-top: 0.32rem;
  color: var(--global-text-color-light);
  line-height: 1.45;
}

.talk-venue {
  color: var(--global-theme-color);
  font-family: "Cormorant Garamond", "EB Garamond", "Georgia", serif;
  font-size: inherit;
  font-style: italic;
  font-weight: 400;
  letter-spacing: 0.012em;
  text-decoration: none !important;
}

.talk-place,
.talk-date {
  color: var(--global-text-color-light);
}

.talk-place::before,
.talk-date::before {
  content: " · ";
  color: var(--global-text-color-light);
}

.talk-note {
  max-width: 760px;
  margin-top: 0.45rem;
  color: var(--global-text-color-light);
  font-style: italic;
  line-height: 1.55;
}

@media (max-width: 576px) {
  .talks-container {
    max-width: 100%;
  }

  .talk-item {
    padding-left: 2.35rem;
    margin-bottom: 1.05rem;
    padding-bottom: 1.05rem;
  }

  .talk-item::before {
    width: 1.35rem;
  }

  .talk-topline {
    display: block;
  }

  .talk-kind {
    margin-top: 0.36rem;
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

<div class="talks-container">
  <div class="talks-list">
    {% for talk in page.talks %}
      {% assign item = talk.items | first %}
      {% assign type_class = talk.type | downcase | replace: " ", "-" | replace: ".", "" %}

      <article class="talk-item">
        <div class="talk-content">
          <div class="talk-topline">
            <h2 class="talk-title">“{{ talk.title }}”</h2>
            {% if talk.type %}
              <span class="talk-kind {{ type_class }}">{{ talk.type }}</span>
            {% endif %}
          </div>

          <div class="talk-meta">
            <span class="talk-venue">{{ item.venue }}</span>
            {% if item.place %}
              <span class="talk-place">{{ item.place }}</span>
            {% endif %}
            {% if item.date %}
              <span class="talk-date">{{ item.date }}</span>
            {% endif %}
          </div>

          {% if item.note %}
            <div class="talk-note">{{ item.note }}</div>
          {% endif %}
        </div>
      </article>
    {% endfor %}
  </div>
</div>
