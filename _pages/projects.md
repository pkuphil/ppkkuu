---
layout: page
title: talks
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

  /* 去掉 list-group-item 默认白底块 + 强制撑满整行宽度（防止右侧日期无法贴边） */
  .list-group-item,
  .list-group-flush > .list-group-item{
    display: block !important;
    width: 100% !important;
    background: transparent !important;
  }

  /* 标题行 */
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

  /* 用 grid 保证右侧日期永远贴紧右边且所有条目对齐 */
  .talk-item{
    width: 100% !important;
    display: grid !important;
    grid-template-columns: 1fr 9.5rem; /* 右侧日期列固定宽度，统一对齐 */
    column-gap: 1rem;
    align-items: start;
  }

  .talk-main{
    min-width: 0;
  }

  /* 名称 + tags 同一行，tags 紧贴名称右侧 */
  .talk-venue-line{
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: .35rem .5rem;
  }

  .talk-item .text-muted{ color: var(--muted) !important; }

  /* tags 紧贴会议名称右侧 */
  .talk-tags{
    display: flex;
    flex-wrap: wrap;
    gap: .35rem;
    align-items: center;
    padding-top: 0;
  }
  .talk-tags--inline{
    justify-content: flex-start;
  }

  /* 右侧日期：贴紧最右 + 右对齐 */
  .talk-right{
    width: 9.5rem;
    justify-self: end;
    display: flex;
    justify-content: flex-end;
    text-align: right;
    padding-top: .05rem;
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

  /* list-group 边线更柔和 */
  .list-group-item{
    border-color: rgba(232, 226, 217, .75) !important;
  }

  /* 小屏适配：日期换到下一行（不想要可删） */
  @media (max-width: 520px){
    .talk-item{
      grid-template-columns: 1fr;
      row-gap: .35rem;
    }
    .talk-right{
      width: auto;
      justify-self: start;
      justify-content: flex-start;
      text-align: left;
    }
  }

  /* =========================
     Dark mode（夜间模式优化）
     - 自动：prefers-color-scheme: dark
     - 兼容：html[data-theme="dark"] / html.dark / body.dark / body.theme-dark
     ========================= */

  /* 1) 自动跟随系统夜间模式 */
  @media (prefers-color-scheme: dark){
    :root{
      --ink: #e5e7eb;
      --muted: #9ca3af;

      /* 卡片像“深色纸张”而不是纯黑 */
      --paper: #0b1220;
      --paper-border: #1f2a3a;

      /* 日期 */
      --date-bg: #121a24;
      --date-bd: #243146;
      --date-tx: #d1d5db;

      /* forthcoming */
      --status-bg: #2a1f10;
      --status-bd: #7c4a14;
      --status-tx: #fcd34d;

      /* colloquium */
      --type-bg: #122132;
      --type-bd: #2c4b66;
      --type-tx: #93c5fd;

      /* peer-reviewed */
      --review-bg: #10251d;
      --review-bd: #245743;
      --review-tx: #86efac;

      /* W.I.P. */
      --wip-bg: #121827;
      --wip-bd: #2a3447;
      --wip-tx: #cbd5e1;
    }

    /* 分隔线在深色下别太亮 */
    .list-group-item{
      border-color: rgba(255,255,255,.12) !important;
    }

    /* 深色下 shadow 克制一点 */
    .talk-card.shadow-sm{
      box-shadow: 0 1px 0 rgba(255,255,255,.04) !important;
    }
  }

  /* 2) 兼容“站点按钮切换暗色”的情况（不一定触发 prefers-color-scheme） */
  html[data-theme="dark"],
  html.dark,
  body.dark,
  body.theme-dark{
    --ink: #e5e7eb;
    --muted: #9ca3af;

    --paper: #0b1220;
    --paper-border: #1f2a3a;

    --date-bg: #121a24;
    --date-bd: #243146;
    --date-tx: #d1d5db;

    --status-bg: #2a1f10;
    --status-bd: #7c4a14;
    --status-tx: #fcd34d;

    --type-bg: #122132;
    --type-bd: #2c4b66;
    --type-tx: #93c5fd;

    --review-bg: #10251d;
    --review-bd: #245743;
    --review-tx: #86efac;

    --wip-bg: #121827;
    --wip-bd: #2a3447;
    --wip-tx: #cbd5e1;
  }

  html[data-theme="dark"] .list-group-item,
  html.dark .list-group-item,
  body.dark .list-group-item,
  body.theme-dark .list-group-item{
    border-color: rgba(255,255,255,.12) !important;
  }

  html[data-theme="dark"] .talk-card.shadow-sm,
  html.dark .talk-card.shadow-sm,
  body.dark .talk-card.shadow-sm,
  body.theme-dark .talk-card.shadow-sm{
    box-shadow: 0 1px 0 rgba(255,255,255,.04) !important;
  }
</style>

<div class="container px-0">

<!-- Talk 1 -->
  <div class="card talk-card shadow-sm mb-4">
    <div class="card-body">
      <div class="talk-header">
        <h2 class="h5 talk-title">“New Object Theory and Illusion”</h2>
      </div>

      <div class="list-group list-group-flush mt-3">
        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">Eastern APA</div>
                <div class="talk-tags talk-tags--inline">
                  <span class="tag tag--type">Colloquium</span>
                  <span class="tag tag--review">paper peer-reviewed</span>
                </div>
              </div>
              <div class="text-muted small">Baltimore, USA</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">Jan 2026</span>
            </div>
          </div>
        </div>
      </div>

    </div>
  </div>

  <!-- Talk 2 -->
  <div class="card talk-card shadow-sm mb-4">
    <div class="card-body">
      <div class="talk-header">
        <h2 class="h5 talk-title">“Mediated Direct Realism”</h2>
      </div>

      <div class="list-group list-group-flush mt-3">
        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">PKU Philosophy R&amp;W</div>
                <div class="talk-tags talk-tags--inline"></div>
              </div>
              <div class="text-muted small">Beijing, China</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">Dec 2025</span>
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
      </div>

      <div class="list-group list-group-flush mt-3">

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">Pacific APA</div>
                <div class="talk-tags talk-tags--inline">
                  <span class="tag tag--type">Colloquium</span>
                  <span class="tag tag--review">paper peer-reviewed</span>
                </div>
              </div>
              <div class="text-muted small">San Francisco, USA</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">Apr 2025</span>
            </div>
          </div>
        </div>

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">Eastern APA</div>
                <div class="talk-tags talk-tags--inline">
                  <span class="tag tag--wip">W.I.P.</span>
                </div>
              </div>
              <div class="text-muted small">New York, USA</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">Jan 2025</span>
            </div>
          </div>
        </div>

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">Talk</div>
                <div class="talk-tags talk-tags--inline"></div>
              </div>
              <div class="text-muted small">Beijing, China</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">2025</span>
            </div>
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
      </div>

      <div class="list-group list-group-flush mt-3">
        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">Central APA</div>
                <div class="talk-tags talk-tags--inline">
                  <span class="tag tag--type">Colloquium</span>
                  <span class="tag tag--review">paper peer-reviewed</span>
                </div>
              </div>
              <div class="text-muted small">Online</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">Feb/Mar 2025</span>
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
      </div>

      <div class="list-group list-group-flush mt-3">

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">Annual Conference of the Australasian Association of Philosophy</div>
                <div class="talk-tags talk-tags--inline">
                  <span class="tag tag--type">Colloquium</span>
                </div>
              </div>
              <div class="text-muted small">Perth, Australia</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">Jul 2024</span>
            </div>
          </div>
        </div>

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">Workshop for Young Scholars in Science and Philosophy</div>
                <div class="talk-tags talk-tags--inline">
                  <span class="tag tag--type">Colloquium</span>
                  <span class="tag tag--review">paper peer-reviewed</span>
                </div>
              </div>
              <div class="text-muted small">Beijing, China</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">Apr 2024</span>
            </div>
          </div>
        </div>

        <div class="list-group-item px-0">
          <div class="talk-item">
            <div class="talk-main">
              <div class="talk-venue-line">
                <div class="fw-semibold">PKU Philosophy R&amp;W</div>
                <div class="talk-tags talk-tags--inline"></div>
              </div>
              <div class="text-muted small">Beijing, China</div>
            </div>

            <div class="talk-right">
              <span class="tag tag--date">Mar 2024</span>
            </div>
          </div>
        </div>

      </div>
    </div>
  </div>

</div>
