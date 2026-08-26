---
layout: about
title: hi!
permalink: /
subtitle: "allenminesky ⟡ gmail · com"

profile:
  align: right
  image: prof_pic_color.jpg
  image_circular: false
  more_info: >
    <p></p>
    <p></p>

selected_papers: true
social: false

talks:
  - title: "Situated Objects and Illusion"
    items:
      - venue: "Society for Exact Philosophy Annual Meeting"
        place: "Vancouver, Canada"
        date: "May 2026"
        refereed: true
        cancelled: true
      - venue: "APA Eastern Division Meeting (122nd)"
        place: "Baltimore, USA"
        date: "Jan 2026"
        refereed: true

  - title: "Mediated Direct Realism"
    items:
      - venue: "Institute of Philosophy, Chinese Academy of Sciences"
        place: "Beijing, China"
        date: "Apr 2026"
      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "Dec 2025"

  - title: "Do Semantic Properties Involve the Future?"
    items:
      - venue: "APA Pacific Division Meeting (98th)"
        place: "San Francisco, USA"
        date: "Apr 2025"
        refereed: true
      - venue: "APA Eastern Division Meeting (121st)"
        place: "New York, USA"
        date: "Jan 2025"
      - venue: "Talk"
        place: "Beijing, China"
        date: "2025"

  - title: "Is Rich Phenomenology Fragmented?"
    items:
      - venue: "APA Central Division Meeting (122nd)"
        place: "Online"
        date: "Feb/Mar 2025"
        online: true
        refereed: true

  - title: "MCICCR"
    items:
      - venue: "Australasian Association of Philosophy Conference"
        place: "Perth, Australia"
        date: "Jul 2024"
        refereed: true
      - venue: "Workshop for Young Scholars in Science and Philosophy"
        place: "Beijing, China"
        date: "Apr 2024"
        refereed: true
      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "Mar 2024"
---

Hi! I am Zhiwei. I am a fourth-year PhD student in the Department of Philosophy at <a href='https://www.pku.edu.cn'>Peking University</a>. I mostly write about philosophy of mind and philosophy of perception.<br><br>

Much of my recent work forms part of a broader project aimed at advancing the claim that, roughly speaking, direct awareness of the world need not be unmediated: mediation can itself be a means by which we are directly aware of the world.<br><br>

I’m advised by <a href="https://phil.pku.edu.cn/szdw/szll/wgzxjys/274743.htm" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Qilin Li</a> at <a href='https://www.pku.edu.cn'>Peking University</a> and, during my visit at <a href='https://www.mit.edu'>MIT</a>, by <a href="http://www.alexbyrne.org" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Alex Byrne</a>.<br><br>

I enjoy cooking, wandering aimlessly, cycling, exploring narrative cinema, and reading personal biographies. I'm also a fan of the band <a href="https://music.apple.com/us/artist/twenty-one-pilots/349736311?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Twenty One Pilots</a> and Hong Kong singer <a href="https://music.apple.com/us/artist/%E8%AE%B8%E5%86%A0%E6%9D%B0/41642722?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Sam Hui</a>.


<style>
  /* =========================================================
     TALKS
     ========================================================= */

  .home-talks {
    clear: both;
    width: 100%;

    margin-top: 2.65rem;
    margin-bottom: 2.2rem;
  }


  /* =========================================================
     HEADER
     ========================================================= */

  .home-talks-header {
    display: flex;
    align-items: baseline;
    justify-content: space-between;

    gap: 1rem;

    width: 100%;
    margin-bottom: 1.2rem;
  }

  .home-talks-header h2 {
    margin: 0;
    padding: 0;
  }

  .home-talks-header h2 a {
    color: inherit !important;

    text-decoration-line: underline;
    text-decoration-color: transparent;
    text-decoration-thickness: 1px;
    text-underline-offset: 0.18em;

    border-bottom: 0 !important;
    box-shadow: none !important;

    transition: text-decoration-color 0.15s ease;
  }

  .home-talks-header h2 a:hover,
  .home-talks-header h2 a:focus {
    text-decoration-color: currentColor;

    border-bottom: 0 !important;
    box-shadow: none !important;
  }


  /* 右侧说明 */
  .home-talks-legend {
    flex: 0 0 auto;
    margin-left: auto;

    font-size: 0.76rem;
    font-weight: 400;
    line-height: 1.2;

    color: var(--global-text-color-light, #6b7280);

    white-space: nowrap;
  }


  /* =========================================================
     PAPER GROUP
     ========================================================= */

  .talk-group {
    margin: 0 0 1.32rem 0;
  }

  .talk-group:last-child {
    margin-bottom: 0;
  }

  .talk-title {
    margin: 0 0 0.28rem 0;

    font-size: 1.03rem;
    font-weight: 500;
    line-height: 1.4;

    color: var(--global-text-color, inherit);
  }


  /* =========================================================
     VENUES
     ========================================================= */

  .talk-venues {
    position: relative;

    margin: 0;
    padding-left: 1.18rem;

    font-size: 0.94rem;
    font-weight: 400;
    line-height: 1.68;

    color: var(--global-text-color, inherit);
  }

  .talk-venues::before {
    content: "·";

    position: absolute;
    left: 0.34rem;
    top: 0;

    color: var(--global-text-color-light, #737373);
  }

  /*
    每一场会议保持 inline。
    空间不足时由浏览器自然换行。
  */
  .talk-entry {
    display: inline;
  }

  /*
    同一篇论文的会议之间用 /
  */
  .talk-entry + .talk-entry::before {
    content: " / ";

    color: var(--global-text-color-light, #8a8a8a);
  }


  /* =========================================================
     VENUE / PLACE / DATE
     ========================================================= */

  .talk-venue {
    font-style: italic;
  }

  .talk-place,
  .talk-date {
    font-style: normal;
  }

  .talk-place {
    margin-left: 0.18rem;
  }

  .talk-date {
    margin-left: 0.18rem;
  }


  /* =========================================================
     SYMBOLS
     † = online
     ‡ = refereed
     ========================================================= */

  .talk-symbols {
    display: inline;
    margin-left: 0.06rem;

    font-size: 0.76em;
    font-weight: 400;
    vertical-align: 0.28em;

    letter-spacing: 0.02em;
  }


  /* =========================================================
     CANCELLED
     ========================================================= */

  .talk-cancelled {
    margin-left: 0.28rem;

    font-size: 0.82em;
    font-weight: 400;
    font-style: italic;

    color: var(--global-text-color-light, #777);
  }


  /* =========================================================
     DARK MODE
     ========================================================= */

  @media (prefers-color-scheme: dark) {

    .home-talks-legend,
    .talk-venues::before,
    .talk-entry + .talk-entry::before,
    .talk-cancelled {
      color: rgba(229, 231, 235, 0.62);
    }

  }


  /* =========================================================
     MOBILE
     ========================================================= */

  @media (max-width: 576px) {

    .home-talks {
      margin-top: 2.25rem;
      margin-bottom: 2rem;
    }

    .home-talks-header {
      gap: 0.75rem;
      margin-bottom: 1rem;
    }

    .home-talks-legend {
      font-size: 0.7rem;
    }

    .talk-group {
      margin-bottom: 1.15rem;
    }

    .talk-title {
      font-size: 1rem;
      line-height: 1.42;
    }

    .talk-venues {
      padding-left: 1rem;

      font-size: 0.91rem;
      line-height: 1.65;
    }

    .talk-venues::before {
      left: 0.22rem;
    }

    .talk-cancelled {
      font-size: 0.8em;
    }

  }
</style>


<div class="home-talks">

  <div class="home-talks-header">

    <h2>
      <a href="{{ '/talks/' | relative_url }}">
        talks
      </a>
    </h2>

    <span class="home-talks-legend">
      († = online; ‡ = refereed)
    </span>

  </div>


  {% for talk in page.talks %}

    <section class="talk-group">

      <div class="talk-title">
        “{{ talk.title }}”
      </div>

      <div class="talk-venues">

        {% for item in talk.items %}

          <span class="talk-entry">

            <span class="talk-venue">
              {{ item.venue }}
            </span>

            {% if item.place %}
              <span class="talk-place">
                {{ item.place }}
              </span>
            {% endif %}

            {% if item.online or item.refereed %}
              <sup class="talk-symbols">{% if item.online %}†{% endif %}{% if item.refereed %}‡{% endif %}</sup>
            {% endif %}

            {% if item.date %}
              <span class="talk-date">
                {{ item.date }}
              </span>
            {% endif %}

            {% if item.cancelled %}
              <span class="talk-cancelled">
                (cancelled — dissertation defense)
              </span>
            {% endif %}

          </span>

        {% endfor %}

      </div>

    </section>

  {% endfor %}

</div>
