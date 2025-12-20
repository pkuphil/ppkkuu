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

<h2>
  <a href="{{ '/talks/' | relative_url }}" class="text-decoration-none">
    talks
  </a>
</h2>

<div class="list-group list-group-flush mt-2 mb-2">
  {% for t in site.data.talks limit:3 %}
    <div class="list-group-item px-0">
      <div class="d-flex flex-wrap justify-content-between gap-2">
        <div class="fw-semibold">“{{ t.title }}”</div>
        <div class="text-muted small">{{ t.date }}</div>
      </div>
      <div class="text-muted small">{{ t.venue }}</div>
    </div>
  {% endfor %}
</div>

