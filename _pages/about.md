---
layout: default
title: hi!
permalink: /
subtitle: "allenminesky ⟡ gmail · com"

selected_papers: false
social: false

publications:
  - title: "Institutional Formal Objects and Two-Level Fittingness."
    journal: "The Philosophical Quarterly"
    link_label: "manuscript"
    link_url: "https://philpapers.org/rec/YANIFO"
    status: "forthcoming"

  - title: "A Tactile Screening-Off Problem for Naïve Realism."
    journal: "Analysis"
    link_label: "OUP"
    link_url: "https://doi.org/10.1093/analys/anag033"
    status: "forthcoming"

  - title: "Cross-Modal Experiences and the Problem of Phenomenal Overlap."
    journal: "Journal of Consciousness Studies"
    link_label: "manuscript"
    link_url: "https://philpapers.org/rec/YANCEA-3"
    status: "forthcoming"

  - title: "Is Rich Phenomenology Fragmented?"
    journal: "Synthese"
    link_label: "Springer"
    link_url: "https://doi.org/10.1007/s11229-025-05058-8"
    status: "2025"

talks:
  - title: "Situated Objects and Illusion"
    items:
      - venue: "Society for Exact Philosophy Annual Meeting"
        place: "Vancouver, Canada"
        date: "May 2026"
        refereed: true
        cancelled: true

      - venue: "APA Eastern Division Meeting"
        place: "Baltimore, USA"
        date: "Jan. 2026"
        refereed: true

  - title: "Mediated Direct Realism"
    items:
      - venue: "Department of Philosophy, Sun Yat-sen University"
        online: true
        date: "Jun. 2026"

      - venue: "Institute of Philosophy, Chinese Academy of Sciences"
        place: "Beijing, China"
        date: "Apr. 2026"

      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "Dec. 2025"

  - title: "Do Semantic Properties Involve the Future?"
    items:
      - venue: "APA Pacific Division Meeting"
        place: "San Francisco, USA"
        date: "Apr. 2025"
        refereed: true

      - venue: "APA Eastern Division Meeting"
        place: "New York, USA"
        date: "Jan. 2025"

      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "2025"

  - title: "Is Rich Phenomenology Fragmented?"
    items:
      - venue: "APA Central Division Meeting"
        online: true
        date: "Feb./Mar. 2025"
        refereed: true

  - title: "MCICCR"
    items:
      - venue: "Australasian Association of Philosophy Conference"
        place: "Perth, Australia"
        date: "Jul. 2024"
        refereed: true

      - venue: "Workshop for Young Scholars in Science and Philosophy"
        place: "Beijing, China"
        date: "Apr. 2024"
        refereed: true

      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "Mar. 2024"
---

<style>
  /* =========================================================
     HOMEPAGE — THREE-COLUMN EDITORIAL LAYOUT
     Profile | Publications + Talks | Portrait
     Research remains in the site navigation only.
     ========================================================= */

  @import url('https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500;1,600&family=Noto+Serif+SC:wght@400;500;600&display=swap');

  body,
  .navbar,
  .navbar-brand,
  .navbar-nav,
  .home-shell {
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

  /* Let the homepage breathe beyond the theme's normal article width. */
  main.container {
    max-width: 1320px !important;
    padding-left: clamp(1.35rem, 3vw, 3rem);
    padding-right: clamp(1.35rem, 3vw, 3rem);
  }

  .home-shell {
    --home-text: #47443f;
    --home-heading: #34312d;
    --home-muted: #817c75;
    --home-soft: #a29d96;
    --home-rule: rgba(52, 49, 45, 0.13);
    --home-accent: var(--global-theme-color, #735c8f);

    width: 100%;
    margin: 0 auto;
    padding: 0.35rem 0 4.8rem;

    color: var(--home-text);
  }

  .home-shell a,
  .home-shell a:link,
  .home-shell a:visited {
    color: var(--home-accent);
  }

  .home-shell a:hover,
  .home-shell a:focus {
    color: var(--home-accent);
  }


  /* =========================================================
     HOMEPAGE NAME
     ========================================================= */

  .home-name {
    margin: 0 0 2.35rem 0;

    font-family:
      "EB Garamond",
      "Songti SC",
      STSong,
      "Noto Serif SC",
      SimSun,
      Garamond,
      Georgia,
      "Times New Roman",
      serif;

    font-size: clamp(2.15rem, 3.4vw, 3rem);
    font-weight: 400;
    line-height: 1.04;

    letter-spacing: -0.024em;

    color: var(--home-heading);
  }


  /* =========================================================
     MAIN GRID
     ========================================================= */

  .home-grid {
    display: grid;
    grid-template-columns:
      minmax(205px, 0.82fr)
      minmax(500px, 1.9fr)
      minmax(220px, 0.9fr);

    column-gap: clamp(2.6rem, 4vw, 4.6rem);
    align-items: start;
  }

  .home-about,
  .home-academic,
  .home-portrait {
    min-width: 0;
  }


  /* =========================================================
     SECTION HEADINGS
     A quiet rule makes the structure clear without cards/boxes.
     ========================================================= */

  .home-section-heading {
    display: flex;
    align-items: center;

    gap: 0.8rem;

    margin: 0 0 1.35rem 0;
  }

  .home-section-heading::after {
    content: "";

    flex: 1 1 auto;

    height: 1px;

    background: var(--home-rule);
  }

  .home-section-heading h2 {
    flex: 0 0 auto;

    margin: 0;
    padding: 0;

    font-family: inherit;
    font-size: 1.42rem;
    font-weight: 500;
    line-height: 1.2;
    letter-spacing: -0.012em;

    color: var(--home-heading);
  }

  .home-section-heading h2 a,
  .home-section-heading h2 a:link,
  .home-section-heading h2 a:visited {
    color: var(--home-heading) !important;

    text-decoration-line: underline;
    text-decoration-color: transparent;
    text-decoration-thickness: 1px;
    text-underline-offset: 0.18em;

    border: 0 !important;
    box-shadow: none !important;

    transition: text-decoration-color 0.16s ease;
  }

  .home-section-heading h2 a:hover,
  .home-section-heading h2 a:focus {
    color: var(--home-heading) !important;
    text-decoration-color: currentColor;
  }


  /* =========================================================
     LEFT COLUMN — ABOUT
     ========================================================= */

  .home-about {
    padding-top: 0.1rem;
  }

  .home-about-copy {
    font-size: 1rem;
    font-weight: 400;
    line-height: 1.72;
  }

  .home-about-copy p {
    margin: 0 0 1.08rem 0;
  }

  .home-about-copy p:last-child {
    margin-bottom: 0;
  }

  .home-about-copy a,
  .home-about-copy a:link,
  .home-about-copy a:visited {
    color: var(--home-accent) !important;

    text-decoration-line: underline;
    text-decoration-color: transparent;
    text-decoration-thickness: 1px;
    text-underline-offset: 0.16em;

    border: 0 !important;
    box-shadow: none !important;

    transition: text-decoration-color 0.15s ease;
  }

  .home-about-copy a:hover,
  .home-about-copy a:focus {
    text-decoration-color: currentColor;
  }

  /* =========================================================
     ABOUT — COLLAPSIBLE MORE
     ========================================================= */

  .home-about-more {
    margin: 0.15rem 0 0 0;
    padding: 0;
  }

  .home-about-more summary {
    list-style: none;

    display: grid;
    place-items: center;

    width: 1.05rem;
    height: 1.05rem;

    margin: 0;
    padding: 0;

    font-family: inherit;
    font-size: 1.05rem;
    font-weight: 400;
    line-height: 1;

    color: var(--home-muted);

    background: transparent !important;
    border: 0;
    border-radius: 0;

    cursor: pointer;
    user-select: none;

    transition:
      color 0.15s ease,
      opacity 0.15s ease,
      transform 0.15s ease;
  }

  .home-about-more summary::-webkit-details-marker {
    display: none;
  }

  .home-about-more summary::marker {
    content: "";
  }

  .home-about-more summary::before {
    content: "+";
  }

  .home-about-more[open] summary::before {
    content: "−";
  }

  .home-about-more summary:hover,
  .home-about-more summary:focus {
    color: var(--home-text);
    opacity: 0.82;
    transform: translateY(-1px);

    outline: none;
  }

  .home-about-more[open] summary {
    margin-bottom: 0.78rem;
  }

  .home-about-more-body {
    animation: homeAboutMoreIn 0.18s ease;
  }

  .home-about-more-body p:last-child {
    margin-bottom: 0;
  }

  @keyframes homeAboutMoreIn {
    from {
      opacity: 0;
      transform: translateY(-2px);
    }

    to {
      opacity: 1;
      transform: translateY(0);
    }
  }


  .home-contact {
    margin-top: 1.35rem;
    padding-top: 1.05rem;

    border-top: 1px solid var(--home-rule);
  }

  .home-contact-label {
    margin: 0 0 0.18rem 0;

    font-size: 0.78rem;
    font-weight: 500;
    line-height: 1.35;

    letter-spacing: 0.045em;
    text-transform: uppercase;

    color: var(--home-soft);
  }

  .home-contact-value {
    margin: 0;

    font-size: 0.94rem;
    font-style: normal;
    font-weight: 400;
    line-height: 1.45;

    color: var(--home-muted);
  }


  /* =========================================================
     CENTER COLUMN — ACADEMIC CONTENT
     ========================================================= */

  .home-academic {
    min-width: 0;
  }

  .home-publications {
    margin: 0;
  }

  .home-talks {
    margin: 3rem 0 0 0;
    padding-top: 0;
  }


  /* =========================================================
     PUBLICATIONS
     ========================================================= */

  .publication-list {
    margin: 0;
    padding: 0;
  }

  .publication-item {
    margin: 0 0 1.28rem 0;
    padding: 0;
  }

  .publication-item:last-child {
    margin-bottom: 0;
  }

  .publication-title {
    margin: 0 0 0.13rem 0;

    font-size: 1.035rem;
    font-weight: 500;
    line-height: 1.43;
    letter-spacing: -0.002em;

    color: var(--home-heading);
  }

  .publication-meta {
    display: flex;
    align-items: baseline;

    width: 100%;

    gap: 1.1rem;

    line-height: 1.46;
  }

  .publication-details {
    min-width: 0;
    flex: 1 1 auto;
  }

  .publication-journal {
    font-size: 0.93rem;
    font-style: italic;
    font-weight: 400;

    color: var(--home-text);
  }

  .publication-link {
    margin-left: 0.22em;

    font-size: 0.87rem;
    font-style: normal;
    font-weight: 400;

    white-space: nowrap;
  }

  .publication-link::before {
    content: " · ";

    color: var(--home-soft);
  }

  .publication-link a,
  .publication-link a:link,
  .publication-link a:visited {
    color: var(--home-muted) !important;

    background: transparent !important;

    text-decoration-line: underline !important;
    text-decoration-color: transparent !important;
    text-decoration-thickness: 1px !important;
    text-underline-offset: 0.17em;

    border: 0 !important;
    box-shadow: none !important;

    transition:
      color 0.15s ease,
      text-decoration-color 0.15s ease;
  }

  .publication-link a:hover,
  .publication-link a:focus {
    color: var(--home-text) !important;
    text-decoration-color: currentColor !important;
  }

  .publication-status {
    flex: 0 0 auto;

    margin-left: auto;

    font-size: 0.88rem;
    font-weight: 400;
    font-style: normal;

    color: var(--home-muted);

    white-space: nowrap;
    text-align: right;
  }

  .publication-status-forthcoming {
    font-style: italic;
  }


  /* =========================================================
     TALKS
     ========================================================= */

  .talk-group {
    margin: 0 0 1.36rem 0;
  }

  .talk-group:last-child {
    margin-bottom: 0;
  }

  .talk-title {
    margin: 0 0 0.33rem 0;

    font-size: 1.03rem;
    font-weight: 600;
    line-height: 1.4;
    letter-spacing: -0.004em;

    color: var(--home-heading);
  }

  .talk-list {
    margin: 0;
    padding: 0;
  }

  .talk-item {
    position: relative;

    display: flex;
    align-items: baseline;

    width: 100%;

    margin: 0;
    padding: 0.105rem 0;

    font-size: 0.92rem;
    font-weight: 400;
    line-height: 1.5;

    color: var(--home-text);
  }

  .talk-info {
    min-width: 0;
    flex: 1 1 auto;

    padding-right: 1.2rem;
  }

  .talk-marker {
    position: absolute;

    left: -0.72rem;
    top: 0.76em;

    width: 0.16rem;
    height: 0.16rem;

    border-radius: 50%;

    background: var(--home-soft);
  }

  .talk-venue {
    font-style: normal;
    font-weight: 400;

    color: var(--home-text);
  }

  .talk-status {
    margin-left: 0.16em;

    font-size: 0.81em;
    font-weight: 400;

    color: var(--home-soft);

    white-space: nowrap;
  }

  .talk-place,
  .talk-online {
    color: var(--home-muted);
  }

  .talk-place::before,
  .talk-online::before {
    content: " · ";

    color: var(--home-soft);
  }

  .talk-date {
    flex: 0 0 auto;

    margin-left: auto;

    font-size: 0.88em;
    font-weight: 400;

    color: var(--home-muted);

    white-space: nowrap;
    text-align: right;
  }

  .talk-cancelled {
    margin-left: 0.18em;

    font-size: 0.78em;
    font-weight: 400;
    font-style: italic;

    color: var(--home-soft);
  }

  .talk-cancelled::before {
    content: " · ";

    font-style: normal;

    color: var(--home-soft);
  }


  /* =========================================================
     RIGHT COLUMN — PORTRAIT
     ========================================================= */

  .home-portrait {
    justify-self: end;

    width: 100%;
    max-width: 280px;

    position: sticky;
    top: 6.4rem;
  }

  .home-portrait-frame {
    margin: 0;
    padding: 0;
  }

  .home-portrait-frame img {
    display: block;

    width: 100%;
    height: auto;

    margin: 0;

    border-radius: 2px;

    box-shadow: none;
  }

  .home-portrait-caption {
    margin: 0.72rem 0 0 0;

    font-size: 0.82rem;
    font-style: italic;
    font-weight: 400;
    line-height: 1.45;

    text-align: right;

    color: var(--home-soft);
  }


  /* =========================================================
     DARK MODE
     ========================================================= */

  html[data-theme="dark"] .home-shell,
  body[data-theme="dark"] .home-shell {
    --home-text: #d6d2cd;
    --home-heading: #ece8e3;
    --home-muted: #aaa59e;
    --home-soft: #807b75;
    --home-rule: rgba(236, 232, 227, 0.12);
  }

  @media (prefers-color-scheme: dark) {
    .home-shell {
      --home-text: #d6d2cd;
      --home-heading: #ece8e3;
      --home-muted: #aaa59e;
      --home-soft: #807b75;
      --home-rule: rgba(236, 232, 227, 0.12);
    }
  }


  /* =========================================================
     TABLET
     Keep the portrait separate while allowing the academic
     column to remain comfortably wide.
     ========================================================= */

  @media (max-width: 1080px) {

    main.container {
      max-width: 940px !important;
    }

    .home-grid {
      grid-template-columns: minmax(0, 1fr) 220px;

      column-gap: 3rem;
      row-gap: 2.8rem;
    }

    .home-about {
      grid-column: 1;
      grid-row: 1;
    }

    .home-academic {
      grid-column: 1;
      grid-row: 2;
    }

    .home-portrait {
      grid-column: 2;
      grid-row: 1 / span 2;

      max-width: 220px;

      position: sticky;
      top: 6rem;
    }

    .home-about-copy {
      max-width: 640px;
    }
  }


  /* =========================================================
     MOBILE
     ========================================================= */

  @media (max-width: 720px) {

    main.container {
      max-width: 100% !important;

      padding-left: 1.2rem;
      padding-right: 1.2rem;
    }

    .home-shell {
      padding-top: 0.15rem;
      padding-bottom: 3.4rem;
    }

    .home-name {
      margin-bottom: 1.8rem;
      font-size: 2.25rem;
    }

    .home-grid {
      display: flex;
      flex-direction: column;

      gap: 0;
    }

    .home-about {
      order: 1;
    }

    .home-portrait {
      order: 2;

      width: min(72vw, 260px);
      max-width: none;

      margin: 2rem auto 0;

      position: static;
    }

    .home-academic {
      order: 3;

      width: 100%;

      margin-top: 2.8rem;
    }

    .home-section-heading {
      margin-bottom: 1.05rem;
    }

    .home-section-heading h2 {
      font-size: 1.34rem;
    }

    .home-about-copy {
      font-size: 0.98rem;
      line-height: 1.68;
    }

    .home-contact {
      margin-top: 1.35rem;
      padding-top: 0.9rem;
    }

    .publication-item {
      margin-bottom: 1.08rem;
    }

    .publication-title {
      font-size: 1rem;
      line-height: 1.43;
    }

    .publication-journal {
      font-size: 0.9rem;
    }

    .publication-link {
      font-size: 0.84rem;
    }

    .publication-status {
      font-size: 0.85rem;
    }

    .home-talks {
      margin-top: 2.5rem;
    }

    .talk-group {
      margin-bottom: 1.12rem;
    }

    .talk-title {
      font-size: 1rem;
      line-height: 1.4;
    }

    .talk-item {
      font-size: 0.88rem;
      line-height: 1.5;
    }

    .talk-info {
      padding-right: 0.7rem;
    }

    .talk-marker {
      left: -0.58rem;
    }

    .talk-date {
      font-size: 0.86em;
    }
  }


  /* =========================================================
     VERY SMALL SCREENS
     Long venue names can wrap without squeezing the date.
     ========================================================= */

  @media (max-width: 430px) {

    .publication-meta,
    .talk-item {
      align-items: flex-start;
    }

    .publication-meta {
      gap: 0.65rem;
    }

    .publication-status {
      padding-top: 0.04rem;
    }

    .talk-info {
      padding-right: 0.45rem;
    }

    .talk-date {
      padding-top: 0.08rem;
    }
  }
</style>


<div class="home-shell">

  <h1 class="home-name">
    Zhiwei Yang（杨嘉）
  </h1>

  <div class="home-grid">


    <!-- =====================================================
         LEFT — ABOUT
         ===================================================== -->

    <aside class="home-about" aria-label="About">

      <div class="home-section-heading">
        <h2>About</h2>
      </div>

      <div class="home-about-copy">

        <p>
          Hi! I am Zhiwei. I received my PhD in Philosophy from
          <a href="https://www.pku.edu.cn/" target="_blank" rel="noopener noreferrer">Peking University</a>
          in 2026. I mostly write about philosophy of mind and philosophy of perception.
        </p>

        <p>
          I’m advised by
          <a href="https://phil.pku.edu.cn/szdw/szll/wgzxjys/274743.htm" target="_blank" rel="noopener noreferrer">Qilin Li</a>
          at
          <a href="https://www.pku.edu.cn/" target="_blank" rel="noopener noreferrer">Peking University</a>
          (2022–2026) and, during my visit at
          <a href="https://www.mit.edu/" target="_blank" rel="noopener noreferrer">MIT</a>
          (2024–2025), by
          <a href="http://www.alexbyrne.org/" target="_blank" rel="noopener noreferrer">Alex Byrne</a>.
        </p>

        <details class="home-about-more">

          <summary aria-label="Show more about me"></summary>

          <div class="home-about-more-body">

            <p>
              Much of my recent work forms part of a broader project aimed at advancing the claim that,
              roughly speaking, direct awareness of the world need not be unmediated: mediation can itself
              be a means by which we are directly aware of the world.
            </p>

            <p>
              I enjoy cooking, wandering aimlessly, cycling, exploring narrative cinema, and reading
              personal biographies. I'm also a fan of the band
              <a href="https://music.apple.com/us/artist/twenty-one-pilots/349736311?l=zh-Hans-CN" target="_blank" rel="noopener noreferrer">Twenty One Pilots</a>
              and Hong Kong singer
              <a href="https://music.apple.com/us/artist/%E8%AE%B8%E5%86%A0%E6%9D%B0/41642722?l=zh-Hans-CN" target="_blank" rel="noopener noreferrer">Sam Hui</a>.
            </p>

          </div>

        </details>

      </div>

      <div class="home-contact">
        <div class="home-contact-label">contact</div>
        <p class="home-contact-value">
          allenminesky ⟡ gmail · com
        </p>
      </div>

    </aside>


    <!-- =====================================================
         CENTER — PUBLICATIONS + TALKS
         ===================================================== -->

    <main class="home-academic">


      <!-- PUBLICATIONS -->

      <section class="home-publications" aria-labelledby="home-publications-title">

        <div class="home-section-heading">
          <h2 id="home-publications-title">
            <a href="{{ '/publications/' | relative_url }}">
              Papers
            </a>
          </h2>
        </div>

        <div class="publication-list">

          {% for publication in page.publications %}

            <article class="publication-item">

              <div class="publication-title">
                {{ publication.title }}
              </div>

              <div class="publication-meta">

                <div class="publication-details">

                  <span class="publication-journal">
                    {{ publication.journal }}
                  </span>

                  {% if publication.link_url %}
                    <span class="publication-link">
                      <a
                        href="{{ publication.link_url }}"
                        target="_blank"
                        rel="noopener noreferrer"
                      >
                        [{{ publication.link_label }}]
                      </a>
                    </span>
                  {% endif %}

                </div>

                <div class="publication-status{% if publication.status == 'forthcoming' %} publication-status-forthcoming{% endif %}">
                  {{ publication.status }}
                </div>

              </div>

            </article>

          {% endfor %}

        </div>

      </section>


      <!-- TALKS -->

      <section class="home-talks" aria-labelledby="home-talks-title">

        <div class="home-section-heading">
          <h2 id="home-talks-title">
            <a href="{{ '/talks/' | relative_url }}">
              Talks
            </a>
          </h2>
        </div>

        {% for talk in page.talks %}

          <section class="talk-group">

            <div class="talk-title">
              “{{ talk.title }}”
            </div>

            <div class="talk-list">

              {% for item in talk.items %}

                <div class="talk-item">

                  <span class="talk-marker" aria-hidden="true"></span>

                  <div class="talk-info">

                    <span class="talk-venue">
                      {{ item.venue }}
                    </span>

                    {% if item.refereed %}
                      <span class="talk-status">
                        (refereed colloquium)
                      </span>
                    {% endif %}

                    {% if item.place %}
                      <span class="talk-place">
                        {{ item.place }}
                      </span>
                    {% endif %}

                    {% if item.online %}
                      <span class="talk-online">
                        Online
                      </span>
                    {% endif %}

                    {% if item.cancelled %}
                      <span class="talk-cancelled">
                        cancelled — dissertation defense
                      </span>
                    {% endif %}

                  </div>

                  {% if item.date %}
                    <div class="talk-date">
                      {{ item.date }}
                    </div>
                  {% endif %}

                </div>

              {% endfor %}

            </div>

          </section>

        {% endfor %}

      </section>

    </main>


    <!-- =====================================================
         RIGHT — PORTRAIT
         ===================================================== -->

    <aside class="home-portrait" aria-label="Portrait">

      <figure class="home-portrait-frame">

        <img
          src="{{ '/assets/img/prof_pic_color.jpg' | relative_url }}"
          alt="Portrait of Zhiwei Yang"
        >

      </figure>

    </aside>


  </div>

</div>
