---
layout: about
title: hi!
permalink: /
subtitle: "allenminesky ⟡ gmail · com"

profile:
  align: right
  image: prof_pic_color.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p></p>
    <p></p>

selected_papers: false # custom Publication section below
social: false # includes social icons at the bottom of the page

publications:
  - title: "Institutional Formal Objects and Two-Level Fittingness."
    journal: "The Philosophical Quarterly"
    status: "forthcoming"

  - title: "A Tactile Screening-Off Problem for Naïve Realism."
    journal: "Analysis"
    doi: "10.1093/analys/anag033"
    doi_url: "https://doi.org/10.1093/analys/anag033"
    status: "forthcoming"

  - title: "Cross-Modal Experiences and the Problem of Phenomenal Overlap."
    journal: "Journal of Consciousness Studies"
    status: "forthcoming"

  - title: "Is Rich Phenomenology Fragmented?"
    journal: "Synthese"
    doi: "10.1007/s11229-025-05058-8"
    doi_url: "https://doi.org/10.1007/s11229-025-05058-8"
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

Hi! I am Zhiwei. I am a fourth-year PhD student in the Department of Philosophy at <a href='https://www.pku.edu.cn'>Peking University</a>. I mostly write about philosophy of mind and philosophy of perception.<br><br>
Much of my recent work forms part of a broader project aimed at advancing the claim that, roughly speaking, direct awareness of the world need not be unmediated: mediation can itself be a means by which we are directly aware of the world.<br><br>
I’m advised by <a href="https://phil.pku.edu.cn/szdw/szll/wgzxjys/274743.htm" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Qilin Li</a> at <a href='https://www.pku.edu.cn'>Peking University</a> and, during my visit at <a href='https://www.mit.edu'>MIT</a>, by <a href="http://www.alexbyrne.org" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Alex Byrne</a>.<br><br>
I enjoy cooking, wandering aimlessly, cycling, exploring narrative cinema, and reading personal biographies. I'm also a fan of the band <a href="https://music.apple.com/us/artist/twenty-one-pilots/349736311?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Twenty One Pilots</a> and Hong Kong singer <a href="https://music.apple.com/us/artist/%E8%AE%B8%E5%86%A0%E6%9D%B0/41642722?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Sam Hui</a>.


<style>

  /* =========================================================
     SHARED SECTION STYLE
     ========================================================= */

  .home-publications,
  .home-talks {
    clear: both;
    width: 100%;
  }

  .home-publications {
    margin-top: 2.45rem;
    margin-bottom: 2.45rem;
  }

  .home-talks {
    margin-top: 0;
    margin-bottom: 2rem;
  }


  /* =========================================================
     SECTION HEADINGS
     ========================================================= */

  .home-section-header {
    margin: 0 0 1.05rem 0;
  }

  .home-section-header h2 {
    margin: 0;
    padding: 0;
  }

  .home-section-header h2 a {
    color: inherit !important;

    text-decoration-line: underline;
    text-decoration-color: transparent;
    text-decoration-thickness: 1px;
    text-underline-offset: 0.18em;

    border-bottom: 0 !important;
    box-shadow: none !important;

    transition: text-decoration-color 0.15s ease;
  }

  .home-section-header h2 a:hover,
  .home-section-header h2 a:focus {
    text-decoration-color: currentColor;

    border-bottom: 0 !important;
    box-shadow: none !important;
  }


  /* =========================================================
     PUBLICATION
     ========================================================= */

  .publication-list {
    margin: 0;
    padding: 0;
  }


  /*
    每篇 publication 保持紧凑。

    第一行：
      论文标题

    第二行：
      Journal · DOI                              forthcoming

    不使用卡片、边框或背景。
  */
  .publication-item {
    margin: 0 0 0.86rem 0;
    padding: 0;
  }

  .publication-item:last-child {
    margin-bottom: 0;
  }


  /*
    论文标题是 publication section 的主要视觉重点。
  */
  .publication-title {
    margin: 0 0 0.12rem 0;

    font-size: 0.96rem;
    font-weight: 600;
    line-height: 1.42;

    letter-spacing: -0.006em;

    color: var(--global-text-color, inherit);
  }


  /*
    第二行使用 flex：

    左边：
      Journal · DOI

    右边：
      forthcoming / 2025

    这样状态形成非常干净的右侧视觉轴。
  */
  .publication-meta {
    display: flex;
    align-items: baseline;

    width: 100%;

    gap: 1rem;

    font-size: 0.82rem;
    line-height: 1.45;

    color: var(--global-text-color-light, #6d7378);
  }


  .publication-details {
    min-width: 0;
    flex: 1 1 auto;
  }


  /*
    Journal 用 italic。
    一篇 publication 只有一个期刊名，因此不会像 talks 中
    大量会议名称全部斜体那样显得凌乱。
  */
  .publication-journal {
    font-style: italic;
    font-weight: 400;
  }


  /*
    DOI 是三级信息，进一步降低对比度。
  */
  .publication-doi {
    margin-left: 0.18em;

    font-size: 0.92em;

    color: var(--global-text-color-light, #85898d);
  }

  .publication-doi::before {
    content: " · ";

    color: var(--global-text-color-light, #aaa);
  }

  .publication-doi a {
    color: inherit !important;

    text-decoration: none;

    border-bottom: 0 !important;
    box-shadow: none !important;
  }

  .publication-doi a:hover,
  .publication-doi a:focus {
    text-decoration: underline;
    text-underline-offset: 0.16em;

    border-bottom: 0 !important;
    box-shadow: none !important;
  }


  /*
    forthcoming / year 最右对齐。
  */
  .publication-status {
    flex: 0 0 auto;

    margin-left: auto;

    font-size: 0.96em;
    font-weight: 400;
    font-style: normal;

    color: var(--global-text-color-light, #73787d);

    white-space: nowrap;
    text-align: right;
  }


  /* =========================================================
     TALKS — PAPER GROUP
     ========================================================= */

  .talk-group {
    margin: 0 0 1.22rem 0;
  }

  .talk-group:last-child {
    margin-bottom: 0;
  }


  /*
    Talk 的论文题目稍微突出。
  */
  .talk-title {
    margin: 0 0 0.34rem 0;

    font-size: 1.03rem;
    font-weight: 600;
    line-height: 1.4;

    letter-spacing: -0.008em;

    color: var(--global-text-color, inherit);
  }


  /* =========================================================
     TALK LIST
     ========================================================= */

  .talk-list {
    margin: 0;
    padding: 0;
  }


  /*
    每场 talk 一行：

    — Conference (refereed colloquium) · Place           Date
  */
  .talk-item {
    display: flex;
    align-items: baseline;

    width: 100%;

    margin: 0;
    padding: 0.12rem 0;

    font-size: 0.89rem;
    font-weight: 400;
    line-height: 1.5;

    color: var(--global-text-color, inherit);
  }


  .talk-info {
    min-width: 0;
    flex: 1 1 auto;

    padding-right: 1.25rem;
  }


  /* =========================================================
     DASH
     ========================================================= */

  .talk-dash {
    display: inline-block;

    width: 1.05rem;

    color: var(--global-text-color-light, #8d8d8d);
  }


  /* =========================================================
     VENUE
     ========================================================= */

  .talk-venue {
    font-style: normal;
    font-weight: 400;

    color: var(--global-text-color, inherit);
  }


  /* =========================================================
     REFEREED COLLOQUIUM
     ========================================================= */

  .talk-status {
    margin-left: 0.18em;

    font-size: 0.8em;
    font-weight: 400;
    font-style: normal;

    color: var(--global-text-color-light, #838383);

    white-space: nowrap;
  }


  /* =========================================================
     PLACE / ONLINE
     ========================================================= */

  .talk-place,
  .talk-online {
    color: var(--global-text-color-light, #686e73);
  }

  .talk-place::before,
  .talk-online::before {
    content: " · ";

    color: var(--global-text-color-light, #aaa);
  }


  /* =========================================================
     TALK DATE
     ========================================================= */

  .talk-date {
    flex: 0 0 auto;

    margin-left: auto;

    font-size: 0.88em;
    font-weight: 400;

    color: var(--global-text-color-light, #686e73);

    white-space: nowrap;
    text-align: right;
  }


  /* =========================================================
     CANCELLED
     ========================================================= */

  .talk-cancelled {
    margin-left: 0.2em;

    font-size: 0.79em;
    font-weight: 400;
    font-style: italic;

    color: var(--global-text-color-light, #929292);
  }

  .talk-cancelled::before {
    content: " · ";

    font-style: normal;

    color: var(--global-text-color-light, #aaa);
  }


  /* =========================================================
     DARK MODE
     ========================================================= */

  @media (prefers-color-scheme: dark) {

    .publication-meta,
    .publication-status {
      color: rgba(229, 231, 235, 0.64);
    }

    .publication-doi {
      color: rgba(229, 231, 235, 0.5);
    }

    .publication-doi::before {
      color: rgba(229, 231, 235, 0.3);
    }

    .talk-dash {
      color: rgba(229, 231, 235, 0.38);
    }

    .talk-status {
      color: rgba(229, 231, 235, 0.5);
    }

    .talk-place,
    .talk-online,
    .talk-date {
      color: rgba(229, 231, 235, 0.64);
    }

    .talk-place::before,
    .talk-online::before,
    .talk-cancelled::before {
      color: rgba(229, 231, 235, 0.3);
    }

    .talk-cancelled {
      color: rgba(229, 231, 235, 0.46);
    }

  }


  /* =========================================================
     MOBILE
     ========================================================= */

  @media (max-width: 576px) {

    .home-publications {
      margin-top: 2.15rem;
      margin-bottom: 2.15rem;
    }

    .home-section-header {
      margin-bottom: 0.95rem;
    }


    /* Publications */

    .publication-item {
      margin-bottom: 0.82rem;
    }

    .publication-title {
      font-size: 0.92rem;
      line-height: 1.42;
    }

    .publication-meta {
      gap: 0.65rem;

      font-size: 0.78rem;
    }

    .publication-status {
      font-size: 0.92em;
    }


    /* Talks */

    .talk-group {
      margin-bottom: 1.05rem;
    }

    .talk-title {
      margin-bottom: 0.3rem;

      font-size: 0.98rem;
      line-height: 1.4;
    }

    .talk-item {
      align-items: baseline;

      padding-top: 0.11rem;
      padding-bottom: 0.11rem;

      font-size: 0.85rem;
      line-height: 1.48;
    }

    .talk-info {
      padding-right: 0.7rem;
    }

    .talk-dash {
      width: 0.92rem;
    }

    .talk-date {
      font-size: 0.84em;
    }

  }

</style>


<!-- =========================================================
     PUBLICATION
     ========================================================= -->

<div class="home-publications">

  <div class="home-section-header">

    <h2>
      <a href="{{ '/publications/' | relative_url }}">
        Publication
      </a>
    </h2>

  </div>


  <div class="publication-list">

    {% for publication in page.publications %}

      <div class="publication-item">


        <!-- Paper title -->
        <div class="publication-title">
          {{ publication.title }}
        </div>


        <!-- Journal / DOI / status -->
        <div class="publication-meta">


          <div class="publication-details">

            <span class="publication-journal">
              {{ publication.journal }}
            </span>


            {% if publication.doi %}
              <span class="publication-doi">

                {% if publication.doi_url %}

                  <a
                    href="{{ publication.doi_url }}"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                    doi: {{ publication.doi }}
                  </a>

                {% else %}

                  doi: {{ publication.doi }}

                {% endif %}

              </span>
            {% endif %}

          </div>


          <div class="publication-status">
            {{ publication.status }}
          </div>


        </div>

      </div>

    {% endfor %}

  </div>

</div>



<!-- =========================================================
     TALKS
     ========================================================= -->

<div class="home-talks">

  <div class="home-section-header">

    <h2>
      <a href="{{ '/talks/' | relative_url }}">
        Talks
      </a>
    </h2>

  </div>


  {% for talk in page.talks %}

    <section class="talk-group">


      <!-- Paper title -->
      <div class="talk-title">
        “{{ talk.title }}”
      </div>


      <!-- Talks -->
      <div class="talk-list">

        {% for item in talk.items %}

          <div class="talk-item">


            <!-- LEFT SIDE -->
            <div class="talk-info">


              <!-- Dash -->
              <span class="talk-dash">
                —
              </span>


              <!-- Venue -->
              <span class="talk-venue">
                {{ item.venue }}
              </span>


              <!-- Refereed colloquium -->
              {% if item.refereed %}
                <span class="talk-status">
                  (refereed colloquium)
                </span>
              {% endif %}


              <!-- Place -->
              {% if item.place %}
                <span class="talk-place">
                  {{ item.place }}
                </span>
              {% endif %}


              <!-- Online -->
              {% if item.online %}
                <span class="talk-online">
                  Online
                </span>
              {% endif %}


              <!-- Cancellation -->
              {% if item.cancelled %}
                <span class="talk-cancelled">
                  cancelled — dissertation defense
                </span>
              {% endif %}


            </div>


            <!-- RIGHT SIDE: DATE -->
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

</div>
