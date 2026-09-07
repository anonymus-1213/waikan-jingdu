# 外刊精读 · 每日一篇英文外刊学习

一个纯静态的英文外刊精读网站，每日一篇，含原文精读、重点词汇、长难句、全文翻译。

## 目录结构

- `index.html` — 首页（最新文章 hero + 往期归档列表 + 关键词搜索）
- `articles/` — 文章页，每天一篇独立 HTML，命名 `外刊精读_YYYY-MM-DD.html`

## 新增一篇文章

1. 在 `articles/` 下新建 `外刊精读_YYYY-MM-DD.html`，复制现有文章页改内容即可。
2. 在 `index.html` 的往期归档区（`#list`）新增一个 `<article>` 条目，填好日期、标题、英文副标题、摘要、标签和链接，并更新 `data-search` 关键词。

## 本地预览

- 方式一：直接双击 `index.html`。
- 方式二：`python -m http.server 8765 --directory .` 后打开 http://localhost:8765/

## 发布

纯静态站点，无构建步骤、无依赖，可直接发布到 Cloudflare Pages / Netlify / GitHub Pages。
