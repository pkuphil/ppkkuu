/* =========================================================
   PUBLICATION
   ========================================================= */

.publication-list {
  margin: 0;
  padding: 0;
}


/*
  每篇 publication 保持舒展但不松散。
*/
.publication-item {
  margin: 0 0 1.05rem 0;
  padding: 0;
}

.publication-item:last-child {
  margin-bottom: 0;
}


/*
  论文标题：
  至少与个人介绍正文一样大，
  并稍微加粗，作为第一视觉层级。
*/
.publication-title {
  margin: 0 0 0.16rem 0;

  font-size: 1.04rem;
  font-weight: 600;
  line-height: 1.45;

  letter-spacing: -0.006em;

  color: var(--global-text-color, inherit);
}


/*
  第二行：
  Journal · [publisher/manuscript]                forthcoming / 2025

  整行字号不再缩小，
  与首页个人介绍正文处于同一量级。
*/
.publication-meta {
  display: flex;
  align-items: baseline;

  width: 100%;
  gap: 1.2rem;

  font-size: 1rem;
  line-height: 1.45;
}


/*
  左侧 journal + link
*/
.publication-details {
  min-width: 0;
  flex: 1 1 auto;
}


/*
  期刊名：
  使用更有书刊感、更流畅的 serif 字体。

  优先顺序：
  Iowan Old Style → Palatino → Georgia → serif

  不需要另外加载字体，
  在 macOS / Windows / Linux 上都有合理 fallback。
*/
.publication-journal {
  font-family:
    "Iowan Old Style",
    "Palatino Linotype",
    "Book Antiqua",
    Palatino,
    Georgia,
    serif;

  font-size: 1.08rem;
  font-style: italic;
  font-weight: 500;
  line-height: 1.35;

  letter-spacing: -0.008em;

  color: var(--global-text-color, inherit);
}


/*
  [Oxford Academic]
  [Springer]
  [manuscript]

  明显是链接，但不做成按钮。
*/
.publication-link {
  margin-left: 0.28em;

  font-family: inherit;
  font-size: 0.84em;
  font-style: normal;
  font-weight: 400;

  color: var(--global-text-color-light, #747a80);

  white-space: nowrap;
}

.publication-link::before {
  content: " · ";

  color: var(--global-text-color-light, #aaa);
}


.publication-link a {
  color: inherit !important;

  text-decoration-line: underline;
  text-decoration-color: rgba(115, 120, 125, 0.38);
  text-decoration-thickness: 1px;
  text-underline-offset: 0.16em;

  border-bottom: 0 !important;
  box-shadow: none !important;

  transition:
    color 0.15s ease,
    text-decoration-color 0.15s ease;
}

.publication-link a:hover,
.publication-link a:focus {
  color: var(--global-text-color, inherit) !important;
  text-decoration-color: currentColor;

  border-bottom: 0 !important;
  box-shadow: none !important;
}


/*
  forthcoming / year

  不做得太小。
  它和期刊处于同一行，但视觉权重稍低。
*/
.publication-status {
  flex: 0 0 auto;

  margin-left: auto;

  font-size: 0.96rem;
  font-weight: 400;
  font-style: normal;

  color: var(--global-text-color-light, #6f757a);

  white-space: nowrap;
  text-align: right;
}


/* =========================================================
   DARK MODE
   ========================================================= */

@media (prefers-color-scheme: dark) {

  .publication-journal {
    color: var(--global-text-color, inherit);
  }

  .publication-link {
    color: rgba(229, 231, 235, 0.58);
  }

  .publication-link::before {
    color: rgba(229, 231, 235, 0.3);
  }

  .publication-status {
    color: rgba(229, 231, 235, 0.66);
  }

}


/* =========================================================
   MOBILE
   ========================================================= */

@media (max-width: 576px) {

  .publication-item {
    margin-bottom: 0.95rem;
  }

  .publication-title {
    font-size: 1rem;
    line-height: 1.43;
  }

  .publication-meta {
    gap: 0.65rem;

    font-size: 0.96rem;
  }

  .publication-journal {
    font-size: 1.04rem;
  }

  .publication-status {
    font-size: 0.9rem;
  }

}
