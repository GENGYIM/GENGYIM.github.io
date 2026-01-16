---
# front matter 中的 title 仅用于 portfolio 列表页展示，无正文跳转作用，可保留
title: "Portfolio item number 2"
# excerpt 中的图片可选用 Markdown 原生语法（更贴合 md 模式），也可保留简化 HTML
excerpt: "Short description of portfolio item number 2\n![项目缩略图](/images/500x300.png \"Portfolio Item 2\")"
collection: portfolio
---

# Portfolio item number 2 （Markdown 一级标题，无跳转，纯静态）

## 项目展示图片（可选：Markdown 二级标题，用于分隔内容）
# 核心：Markdown 原生图片语法（无 HTML，纯 md 模式）
![项目详情图片](/images/500x300.png "Portfolio Item 2 详情图")

# 可选：如果需要简单调整图片大小（兼顾 md 兼容性，少量内联样式）
![项目详情图片](/images/500x300.png "Portfolio Item 2 详情图"){: style="width: 80%; max-width: 600px; display: block; margin: 0 auto;"}
