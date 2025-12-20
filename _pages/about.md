---
layout: about
title: about
permalink: /
subtitle: <a href='#'>Peking University</a>. allenminesky@gmail.com.

profile:
  align: right
  image: prof_pic_color.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p></p>
    <p></p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page
---

Hi! I am Zhiwei. I am a third-year PhD student in the Department of Philosophy at Peking University and currently a visiting student at MIT. I mostly write about philosophy of mind and philosophy of perception.<br><br>
I’m advised by <a href="https://phil.pku.edu.cn/szdw/szll/wgzxjys/274743.htm" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Qilin Li</a> at Peking University and, during my visit at MIT, by <a href="http://www.alexbyrne.org" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Alex Byrne</a>.<br><br>
I enjoy cooking, wandering aimlessly, cycling, exploring narrative cinema, and reading personal biographies. I'm also a fan of the band <a href="https://music.apple.com/us/artist/twenty-one-pilots/349736311?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Twenty One Pilots</a> and Hong Kong singer <a href="https://music.apple.com/us/artist/%E8%AE%B8%E5%86%A0%E6%9D%B0/41642722?l=zh-Hans-CN" class="custom-link" target="_blank" rel="noopener noreferrer" style="color: #2f4f6e;">Sam Hui</a>.

{% assign talks_page = site.pages | where: "url", "/talks/" | first %}

<style>
  /* 只影响首页 talks 这一块：修复暗色模式 list-group 白底 */
  .home-talks .list-group,
  .home-talks .list-group-item{
    background: transparent !important;
  }

  .home-talks .list-group-item{
    border-color: rgba(150,150,150,.18) !important;
  }

  /* 让 muted 颜色跟随主题（变量不存在时也不影响） */
  .home-talks .text-muted{
    color: var(--global-text-color-light, #6b7280) !important;
  }
</style>

<div class="home-talks">
  <h2>
    <a href="{{ '/talks/' | relative_url }}" class="text-reset text-decoration-none">
      latest talks
    </a>
  </h2>

  {% if talks_page and talks_page.talks %}
    <div class="list-group list-group-flush mt-2 mb-2">
      {% for talk in talks_page.talks limit:5 %}
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



