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

Hi! I am Zhiwei. I am a fourth-year PhD student in the Department of Philosophy at <a href="https://www.pku.edu.cn">Peking University</a>. I mostly write about philosophy of mind and philosophy of perception.<br><br>

Much of my recent work forms part of a broader project aimed at advancing the claim that, roughly speaking, direct awareness of the world need not be unmediated: mediation can itself be a means by which we are directly aware of the world.<br><br>

I’m advised by <a href="https://phil.pku.edu.cn/szdw/szll/wgzxjys/274743.htm" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Qilin Li</a> at <a href="https://www.pku.edu.cn">Peking University</a> and, during my visit at <a href="https://www.mit.edu">MIT</a>, by <a href="http://www.alexbyrne.org" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Alex Byrne</a>.<br><br>

I enjoy cooking, wandering aimlessly, cycling, exploring narrative cinema, and reading personal biographies. I'm also a fan of the band <a href="https://music.apple.com/us/artist/twenty-one-pilots/349736311?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Twenty One Pilots</a> and Hong Kong singer <a href="https://music.apple.com/us/artist/%E8%AE%B8%E5%86%A0%E6%9D%B0/41642722?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Sam Hui</a>.


<style>

  /* =========================================================
     TALKS
     ========================================================= */

  .home-talks {
    /*
      清除上方 profile image 的 float，
      talks 从头像下方开始，并重新使用完整正文宽度。
    */
    clear: both;
    width: 100%;

    margin-top: 2.7rem;
    margin-bottom: 2.2rem;
  }


  /* =========================================================
     HEADING
     ========================================================= */

  .home-talks-header {
    margin: 0 0 1.45rem 0;
  }

  .home-talks-header h2 {
    margin: 0;
    padding: 0;
  }

  /*
    talks 保持链接到完整 talks 页面。
    默认不显示下划线，hover 时才显示。
  */
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


  /* =========================================================
     PAPER GROUP
     ========================================================= */

  .talk-group {
    margin: 0 0 1.65rem 0;
  }

  .talk-group:last-child {
    margin-bottom: 0;
  }


  /*
    论文题目。
    稍微突出，但不做成太重的 subsection heading。
  */
  .talk-title {
    margin: 0 0 0.55rem 0;

    font-size: 1.02rem;
    font-weight: 500;
    line-height: 1.42;

    letter-spacing: -0.005em;

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
    每一场会议独立显示。

    不使用 grid，
    不使用两栏布局，
    不让地点和时间人为纵向对齐。

    所有东西自然左对齐。
  */
  .talk-item {
    margin: 0 0 0.68rem 0;
    padding: 0;
  }

  .talk-item:last-child {
    margin-bottom: 0;
  }


  /* =========================================================
     CONFERENCE NAME
     ========================================================= */

  .talk-main {
    margin: 0;

    font-size: 0.94rem;
    font-weight: 400;
    line-height: 1.48;

    color: var(--global-text-color, inherit);
  }


  /*
    会议名称轻微斜体，
    保持 academic talks / CV 风格。
  */
  .talk-venue {
    font-style: italic;
    font-weight: 400;
  }


  /* =========================================================
     STATUS
     ========================================================= */

  /*
    REFEREED / ONLINE 直接跟在会议名后。

    不做 badge：
    - 无背景
    - 无边框
    - 无圆角

    仅作为非常轻的辅助信息。
  */
  .talk-status {
    display: inline;

    margin-left: 0.42rem;

    font-size: 0.66rem;
    font-style: normal;
    font-weight: 500;
    line-height: 1;

    letter-spacing: 0.055em;
    text-transform: uppercase;

    color: var(--global-text-color-light, #7c8187);

    white-space: nowrap;
  }

  .talk-status + .talk-status {
    margin-left: 0.3rem;
  }


  /* =========================================================
     PLACE + DATE
     ========================================================= */

  /*
    第二行正常左对齐：

    Vancouver, Canada · May 2026

    不做任何列式对齐。
  */
  .talk-meta {
    margin-top: 0.05rem;

    font-size: 0.82rem;
    font-weight: 400;
    line-height: 1.45;

    color: var(--global-text-color-light, #74787d);
  }


  /*
    地点与日期之间使用一个轻量 middle dot。
  */
  .talk-date.with-place::before {
    content: " · ";

    color: var(--global-text-color-light, #a2a2a2);
  }


  /* =========================================================
     CANCELLED
     ========================================================= */

  /*
    取消说明跟在地点和日期后面，
    用较淡文字，避免过度抢眼。
  */
  .talk-cancelled {
    margin-left: 0.38rem;

    font-size: 0.92em;
    font-style: italic;
    font-weight: 400;

    color: var(--global-text-color-light, #8a8a8a);
  }


  /* =========================================================
     DARK MODE
     ========================================================= */

  @media (prefers-color-scheme: dark) {

    .talk-status {
      color: rgba(229, 231, 235, 0.58);
    }

    .talk-meta {
      color: rgba(229, 231, 235, 0.64);
    }

    .talk-date.with-place::before {
      color: rgba(229, 231, 235, 0.32);
    }

    .talk-cancelled {
      color: rgba(229, 231, 235, 0.5);
    }

  }


  /* =========================================================
     MOBILE
     ========================================================= */

  @media (max-width: 576px) {

    .home-talks {
      margin-top: 2.3rem;
      margin-bottom: 2rem;
    }

    .home-talks-header {
      margin-bottom: 1.25rem;
    }

    .talk-group {
      margin-bottom: 1.5rem;
    }

    .talk-title {
      margin-bottom: 0.52rem;

      font-size: 1rem;
      line-height: 1.42;
    }

    .talk-item {
      margin-bottom: 0.68rem;
    }

    .talk-main {
      font-size: 0.91rem;
      line-height: 1.48;
    }

    .talk-status {
      font-size: 0.62rem;
    }

    .talk-meta {
      margin-top: 0.06rem;

      font-size: 0.79rem;
      line-height: 1.45;
    }

    .talk-cancelled {
      white-space: normal;
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

  </div>


  {% for talk in page.talks %}

    <section class="talk-group">


      <!-- Paper title -->
      <div class="talk-title">
        “{{ talk.title }}”
      </div>


      <!-- Conference list -->
      <div class="talk-list">

        {% for item in talk.items %}

          <div class="talk-item">


            <!-- Conference name + status -->
            <div class="talk-main">

              <span class="talk-venue">
                {{ item.venue }}
              </span>

              {% if item.refereed %}
                <span class="talk-status">
                  refereed
                </span>
              {% endif %}

              {% if item.online %}
                <span class="talk-status">
                  online
                </span>
              {% endif %}

            </div>


            <!-- Place + date + cancellation -->
            <div class="talk-meta">

              {% if item.place %}
                <span class="talk-place">
                  {{ item.place }}
                </span>
              {% endif %}

              {% if item.date %}
                <span class="talk-date{% if item.place %} with-place{% endif %}">
                  {{ item.date }}
                </span>
              {% endif %}

              {% if item.cancelled %}
                <span class="talk-cancelled">
                  cancelled — dissertation defense
                </span>
              {% endif %}

            </div>


          </div>

        {% endfor %}

      </div>


    </section>

  {% endfor %}

</div>
