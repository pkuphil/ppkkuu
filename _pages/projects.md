---
layout: page
title: Talks
permalink: /talks/
description: Talks and presentations.
nav: true
nav_order: 3
---

<style>
  /* 温润学术配色（偏纸张/墨蓝/鼠尾草） */
  :root{
    --ink: #1f2937;
    --muted: #6b7280;

    --paper: #fbfaf8;
    --paper-border: #e8e2d9;

    --date-bg: #f7f3eb;
    --date-bd: #e8ddcf;
    --date-tx: #5b4636;

    --status-bg: #fff4e6;   /* forthcoming */
    --status-bd: #ffd8a8;
    --status-tx: #8a4b00;

    --type-bg: #eaf2f8;     /* colloquium */
    --type-bd: #cfe3f1;
    --type-tx: #235a7a;

    --review-bg: #eaf6f1;   /* peer-reviewed */
    --review-bd: #caead9;
    --review-tx: #1f5c43;

    --wip-bg: #f1f5f9;      /* W.I.P. */
    --wip-bd: #d8e1ec;
    --wip-tx: #334155;
  }

  /* 卡片整体更“纸感”一点 */
  .talk-card{
    border: 1px solid var(--paper-border);
    border-radius: 14px;
    background: var(--paper);
  }

  /* 标题行：左标题 + 右侧标签，统一对齐 */
  .talk-header{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: baseline;
    gap: .75rem;
  }
  .talk-title{
    margin: 0;
    color: var(--ink);
    letter-spacing: .1px;
  }
  .talk-meta{
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-end;
    gap: .4rem;
    align-items: center;
  }

  /* 每条 venue 行：左信息 + 右 tags */
  .talk-item{
    display: flex;
    justify-content: space-between;
    gap: .75rem;
    align-items: flex-start;
  }
  .talk-item .text-muted{ color: var(--muted) !important; }

  .talk-tags{
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-end;
    gap: .35rem;
    align-items: center;
    padding-top: .05rem;
    flex: 0 0 auto;
  }

  /* 统一 tag 视觉 */
  .tag{
    border: 1px solid transparent;
    border-radius: 999px;
    padding: .35rem .6rem;
    font-weight: 550;
    font-size: .78rem;
    line-height: 1;
    letter-spacing: .2px;
    white-space: nowrap;
  }

  .tag--date   { background: var(--date-bg);   border-color: var(--date-bd);   color: var(--date-tx); }
  .tag--status { background: var(--status-bg); border-color: var(--status-bd); color: var(--status-tx); }
  .tag--type   { background: var(--type-bg);   border-color: var(--type-bd);   color: var(--type-tx); }
  .tag--review { background: var(--review-bg); border-color: var(--review-bd); color: var(--review-tx); }
  .tag--wip    { background: var(--wip-bg);    border-color: var(--wip-bd);    color: var(--wip-tx); }

  /* list-group 更干净一些 */
  .list-group-item{
    border-color: rgba(232, 226, 217, .75) !important;
  }
</style>

<div class="container px-0">

  <!-- Talk 1 -->
  <div class="card talk-card shadow-sm mb-4">
    <div class="card-body">
      <div class="talk-header">
        <h2 class="h5 talk-title">“Mediated Direct Realism”</h2>
        <div class="talk-meta">
          <span class="tag tag--date">Dec 2025</span>
        </div>
      </div>

      <div class="list-group list-group-flush mt-3">
        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">PKU Philosophy R&amp;W</div>
              <div class="text-muted small">Beijing, China · December 2025</div>
            </div>
            <div class="talk-tags"></div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Talk 2 -->
  <div class="card talk-card shadow-sm mb-4">
    <div class="card-body">
      <div class="talk-header">
        <h2 class="h5 talk-title">“New Object Theory and Illusion”</h2>
        <div class="talk-meta">
          <span class="tag tag--date">Jan 2026</span>
          <span class="tag tag--status">Forthcoming</span>
          <span class="tag tag--type">Colloquium</span>
          <span class="tag tag--review">peer-reviewed</span>
        </div>
      </div>

      <div class="list-group list-group-flush mt-3">
        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">Eastern APA</div>
              <div class="text-muted small">Baltimore, USA · January 2026</div>
            </div>
            <div class="talk-tags">
              <span class="tag tag--status">Forthcoming</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Talk 3 -->
  <div class="card talk-card shadow-sm mb-4">
    <div class="card-body">
      <div class="talk-header">
        <h2 class="h5 talk-title">“Do Semantic Properties Involve the Future?”</h2>
        <div class="talk-meta">
          <span class="tag tag--date">2025</span>
        </div>
      </div>

      <div class="list-group list-group-flush mt-3">

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">Pacific APA</div>
              <div class="text-muted small">San Francisco, USA · April 2025</div>
            </div>
            <div class="talk-tags">
              <span class="tag tag--type">Colloquium</span>
              <span class="tag tag--review">peer-reviewed</span>
            </div>
          </div>
        </div>

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">Eastern APA</div>
              <div class="text-muted small">New York, USA · January 2025</div>
            </div>
            <div class="talk-tags">
              <span class="tag tag--wip">W.I.P.</span>
            </div>
          </div>
        </div>

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">Talk</div>
              <div class="text-muted small">Beijing, China · 2025</div>
            </div>
            <div class="talk-tags"></div>
          </div>
        </div>

      </div>
    </div>
  </div>

  <!-- Talk 4 -->
  <div class="card talk-card shadow-sm mb-4">
    <div class="card-body">
      <div class="talk-header">
        <h2 class="h5 talk-title">“Is Rich Phenomenology Fragmented?”</h2>
        <div class="talk-meta">
          <span class="tag tag--date">Feb/Mar 2025</span>
          <span class="tag tag--type">Colloquium</span>
          <span class="tag tag--review">peer-reviewed</span>
        </div>
      </div>

      <div class="list-group list-group-flush mt-3">
        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">Central APA</div>
              <div class="text-muted small">Online · February/March 2025</div>
            </div>
            <div class="talk-tags">
              <span class="tag tag--type">Colloquium</span>
              <span class="tag tag--review">peer-reviewed</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Talk 5 -->
  <div class="card talk-card shadow-sm mb-4">
    <div class="card-body">
      <div class="talk-header">
        <h2 class="h5 talk-title">“MCICCR”</h2>
        <div class="talk-meta">
          <span class="tag tag--date">2024</span>
        </div>
      </div>

      <div class="list-group list-group-flush mt-3">

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">Annual Conference of the Australasian Association of Philosophy</div>
              <div class="text-muted small">Perth, Australia · July 2024</div>
            </div>
            <div class="talk-tags">
              <span class="tag tag--type">Colloquium</span>
              <span class="tag tag--review">abstract peer-reviewed</span>
            </div>
          </div>
        </div>

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">Workshop for Young Scholars in Science and Philosophy</div>
              <div class="text-muted small">Beijing, China · April 2024</div>
            </div>
            <div class="talk-tags">
              <span class="tag tag--type">Colloquium</span>
              <span class="tag tag--review">paper peer-reviewed</span>
            </div>
          </div>
        </div>

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div>
              <div class="fw-semibold">PKU Philosophy R&amp;W</div>
              <div class="text-muted small">Beijing, China · March 2024</div>
            </div>
            <div class="talk-tags"></div>
          </div>
        </div>

      </div>
    </div>
  </div>

</div>
