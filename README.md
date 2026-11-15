# Cheristar 的个人博客

站点：<https://cheristar.github.io>。由 GitHub Pages + Jekyll 构建，不需要额外购买服务器。

## 发布新文章

1. 在 GitHub 仓库打开 `_posts`，点击 **Add file → Create new file**。
2. 文件名使用 `年-月-日-英文短名.md`，例如 `2026-11-16-my-note.md`。
3. 按下面的格式写文章，提交到 `main`，等待 Pages 构建完成。

```markdown
---
title: "文章标题"
date: 2026-11-16 12:00:00 +0800
categories: [学习与技术]
tags: [物理, 笔记]
description: "一两句话介绍这篇文章，会显示在首页。"
---

这里开始写正文。

## 小标题

支持 **加粗**、列表、引用、链接、代码块以及 LaTeX 公式。

行内公式：\(E = mc^2\)。

独立公式：

$$
i\hbar\frac{\partial}{\partial t}\Psi = \hat H\Psi
$$
```

分类建议使用 `学习与技术`、`生活随笔`、`摄影`，与首页筛选一致。标签可以自由填写。未来日期的文章会等到对应时间之后再次触发构建时显示；普通发布请用当前或过去的日期。

## 放照片

在仓库创建 `assets/images` 文件夹并上传照片，在文章中使用 `![照片说明](/assets/images/照片名.jpg)`。公开发布前请自行确认照片内容和定位信息是否适合公开。

## 日常修改

- 博客名称、简介：`_config.yml`
- 首页介绍：`index.html`
- 关于页面：`about.md`
- 配色、布局和交互：`_layouts/default.html`
- 文章：`_posts/`

归档、标签、RSS 和站点地图会在构建时自动更新。搜索在本地浏览器完成，不向外部服务提交关键词。深色模式设置保存在当前浏览器。公式通过 jsDelivr 加载 MathJax；若加载受限，公式源码仍可阅读。

## 部署

仓库 Settings → Pages → Deploy from a branch → `main` / `(root)`。提交后可在 Actions 中查看 `pages build and deployment`。不要添加 `.nojekyll`，本博客需要 Jekyll 渲染。
