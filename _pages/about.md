---
layout: about
title: about
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
---

Hi! I am Zhiwei. I am a third-year PhD student in the Department of Philosophy at <a href='https://www.pku.edu.cn'>Peking University</a>. I mostly write about philosophy of mind and philosophy of perception.<br><br>
I’m advised by <a href="https://phil.pku.edu.cn/szdw/szll/wgzxjys/274743.htm" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Qilin Li</a> at <a href='https://www.pku.edu.cn'>Peking University</a> and, during my visit at <a href='https://www.mit.edu'>MIT</a>, by <a href="http://www.alexbyrne.org" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Alex Byrne</a>.<br><br>
I enjoy cooking, wandering aimlessly, cycling, exploring narrative cinema, and reading personal biographies. I'm also a fan of the band <a href="https://music.apple.com/us/artist/twenty-one-pilots/349736311?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Twenty One Pilots</a> and Hong Kong singer <a href="https://music.apple.com/us/artist/%E8%AE%B8%E5%86%A0%E6%9D%B0/41642722?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Sam Hui</a>.

{% assign talks_page = site.pages | where_exp: "p", "p.url == '/talks/' or p.url == '/talks'" | first %}

<style>
  /* 只影响首页 talks 这一块：修复暗色模式 list-group 白底 */
  .home-talks .list-group,
  .home-talks .list-group-item{
    background: transparent !important;
  }

  .home-talks .list-group-item{
    border-color: rgba(150,150,150,.18) !important;
  }

  /* muted 颜色跟随主题（变量不存在时也不影响） */
  .home-talks .text-muted{
    color: var(--global-text-color-light, #6b7280) !important;
  }

  /* ✅ latest talks：hover 时出现下划线（兼容主题伪下划线实现） */
  .home-talks h2 a{
    text-decoration: none;
    border-bottom: 0;
    box-shadow: none;
  }
  /* ✅ latest talks：下划线不抖动（始终占位，默认透明） */
.home-talks h2 a{
  text-decoration: underline;
  text-decoration-color: transparent;     /* 默认看不见 */
  text-underline-offset: .18em;
  text-decoration-thickness: 1px;         /* 可选：固定粗细更稳 */
  border-bottom: 0 !important;
  box-shadow: none !important;
}

.home-talks h2 a:hover,
.home-talks h2 a:focus{
  text-decoration-color: currentColor;    /* hover 才显示 */
  border-bottom: 0 !important;
  box-shadow: none !important;
}

  /* 深色模式下的边线与文字更柔和 */
  @media (prefers-color-scheme: dark){
    .home-talks .list-group-item{
      border-color: rgba(255,255,255,.12) !important;
    }
    .home-talks .text-muted{
      color: rgba(229,231,235,.72) !important;
    }
  }
</style>

<div class="home-talks">
  <h2>
    <!-- ✅ 去掉 text-decoration-none，让 hover 下划线生效 -->
    <a href="{{ '/talks/' | relative_url }}" class="text-reset">
      latest talks
    </a>
  </h2>

  {% if talks_page and talks_page.talks %}
    {% assign selected_talks = talks_page.talks | where: "selected", true %}

    {%- comment -%}
      兜底：如果 talks 页面没有标 selected，则展示前 5 条
    {%- endcomment -%}
    {% if selected_talks == nil or selected_talks.size == 0 %}
      {% assign selected_talks = talks_page.talks %}
    {% endif %}

    <div class="list-group list-group-flush mt-2 mb-2">
      {% for talk in selected_talks limit:5 %}
        {% assign first_item = talk.items | first %}
        <div class="list-group-item px-0">
          <div class="d-flex flex-wrap justify-content-between gap-2">
            <div class="fw-semibold">“{{ talk.title }}”</div>
            <div class="text-muted small">{{ first_item.date }}</div>
          </div>
          <div class="text-muted small">
            {{ first_item.venue }}{% if first_item.place %} · {{ first_item.place }}{% endif %}
          </div>
        </div>
      {% endfor %}
    </div>
  {% endif %}
</div>
