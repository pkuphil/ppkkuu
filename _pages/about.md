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

selected_papers: true # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

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
     TALKS
     ========================================================= */

  .home-talks {
    /*
      清除上方 profile image 的 float。
      Talks 从头像下方开始，占满整个正文区域，
      所以最右侧日期与上方头像右边缘对齐。
    */
    clear: both;
    width: 100%;

    margin-top: 2.4rem;
    margin-bottom: 2rem;
  }


  /* =========================================================
     TALKS HEADING
     ========================================================= */

  .home-talks-header {
    margin: 0 0 1.1rem 0;
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


  /* =========================================================
     PAPER GROUP
     ========================================================= */

  .talk-group {
    margin: 0 0 1.22rem 0;
  }

  .talk-group:last-child {
    margin-bottom: 0;
  }


  /*
    论文标题是这一组最明显的信息：
    稍微加粗、略微放大，但不做得过重。
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
    每场报告一行：

    — Conference (refereed colloquium) · Place          Date

    会议相关信息自然左对齐，
    只有日期贴到最右边。
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


  /* =========================================================
     LEFT SIDE
     ========================================================= */

  .talk-info {
    min-width: 0;
    flex: 1 1 auto;

    padding-right: 1.25rem;
  }


  /*
    使用 em dash，而不是 bullet。
  */
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

  /*
    只把 refereed 信息作为轻量说明：

      (refereed colloquium)

    不使用 badge、大写标签、角标或框。
  */
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

  /*
    地点与会议名保持在同一行。
  */
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
     DATE
     ========================================================= */

  /*
    日期单独贴到最右边。

    因为 .home-talks 占满整个正文容器，
    所以日期的右边缘就是该容器的右边缘，
    也会与上方头像的右边缘保持一致。
  */
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

  /*
    cancellation 是辅助信息，
    所以做得更轻，不抢论文标题和会议名。
  */
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

    .home-talks {
      margin-top: 2.15rem;
      margin-bottom: 1.8rem;
    }

    .home-talks-header {
      margin-bottom: 0.95rem;
    }

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
