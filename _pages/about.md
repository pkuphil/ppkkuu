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
        colloquium: true
        cancelled: true

      - venue: "APA Eastern Division Meeting (122nd)"
        place: "Baltimore, USA"
        date: "Jan. 2026"
        refereed: true
        colloquium: true

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
      - venue: "APA Pacific Division Meeting (98th)"
        place: "San Francisco, USA"
        date: "Apr. 2025"
        refereed: true
        colloquium: true

      - venue: "APA Eastern Division Meeting (121st)"
        place: "New York, USA"
        date: "Jan. 2025"

      - venue: "Talk"
        place: "Beijing, China"
        date: "2025"

  - title: "Is Rich Phenomenology Fragmented?"
    items:
      - venue: "APA Central Division Meeting (122nd)"
        online: true
        date: "Feb./Mar. 2025"
        refereed: true
        colloquium: true

  - title: "MCICCR"
    items:
      - venue: "Australasian Association of Philosophy Conference"
        place: "Perth, Australia"
        date: "Jul. 2024"
        refereed: true
        colloquium: true

      - venue: "Workshop for Young Scholars in Science and Philosophy"
        place: "Beijing, China"
        date: "Apr. 2024"
        refereed: true
        colloquium: true

      - venue: "PKU Philosophy R&W"
        place: "Beijing, China"
        date: "Mar. 2024"
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
    clear: both;
    width: 100%;

    margin-top: 2.4rem;
    margin-bottom: 2rem;
  }


  /* =========================================================
     HEADING
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
    论文标题作为整个分组最明显的信息。

    稍微放大 + 600 weight，
    但不会重到像大标题。
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
    一场报告 = 一行。

    左侧自然排列：
      — Conference (refereed colloquium) · Place

    右侧：
      Date

    除日期以外，不做任何表格式字段对齐。
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
    用 em dash 代替圆点。

    视觉上更像 academic CV / talks list，
    也比 bullet 更安静。
  */
  .talk-dash {
    display: inline-block;

    width: 1.05rem;

    color: var(--global-text-color-light, #8d8d8d);
  }


  /* =========================================================
     VENUE
     ========================================================= */

  /*
    会议名称使用正常字体。

    因为论文标题已经负责视觉重点，
    这里不再使用大量 italic。
  */
  .talk-venue {
    font-style: normal;
    font-weight: 400;

    color: var(--global-text-color, inherit);
  }


  /* =========================================================
     REFEREED COLLOQUIUM / ONLINE
     ========================================================= */

  /*
    辅助信息只使用轻量括号文本：

      (refereed colloquium)
      (online)
      (refereed colloquium, online)

    不使用 badge、大写、小方框或角标。
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
     LOCATION
     ========================================================= */

  .talk-place {
    color: var(--global-text-color-light, #686e73);
  }

  .talk-place::before {
    content: " · ";

    color: var(--global-text-color-light, #aaa);
  }


  /*
    Online 作为地点性质的信息，
    因此也和 place 放在同一层级。
  */
  .talk-online {
    color: var(--global-text-color-light, #686e73);
  }

  .talk-online::before {
    content: " · ";

    color: var(--global-text-color-light, #aaa);
  }


  /* =========================================================
     DATE
     ========================================================= */

  /*
    只有日期右对齐。

    .home-talks 本身 width: 100%，
    所以日期最右端与 talks 容器的右边缘一致，
    也就是与上方 profile image 的右边缘对齐。
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


      <div class="talk-list">

        {% for item in talk.items %}

          <div class="talk-item">


            <!-- LEFT -->
            <div class="talk-info">

              <span class="talk-dash">—</span>

              <span class="talk-venue">
                {{ item.venue }}
              </span>


              <!-- refereed / colloquium status -->
              {% if item.refereed or item.online %}
                <span class="talk-status">
                  (
                  {%- if item.refereed and item.colloquium -%}
                    refereed colloquium
                  {%- elsif item.refereed -%}
                    refereed
                  {%- endif -%}

                  {%- if item.refereed and item.online -%}
                    ,&nbsp;
                  {%- endif -%}

                  {%- if item.online -%}
                    online
                  {%- endif -%}
                  )
                </span>
              {% endif %}


              <!-- place -->
              {% if item.place %}
                <span class="talk-place">
                  {{ item.place }}
                </span>
              {% endif %}


              <!-- online as location -->
              {% if item.online %}
                <span class="talk-online">
                  Online
                </span>
              {% endif %}


              <!-- cancellation -->
              {% if item.cancelled %}
                <span class="talk-cancelled">
                  cancelled — dissertation defense
                </span>
              {% endif %}

            </div>


            <!-- RIGHT: date only -->
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
