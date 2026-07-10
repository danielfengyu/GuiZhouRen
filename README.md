# 贵州黔行 - 快速上手

## 📂 项目结构

```
GuiZhouRen/
├── _config.yml              # Hexo 主配置
├── _config.butterfly.yml    # Butterfly 主题配置
├── package.json             # 依赖清单
├── netlify.toml             # Netlify 部署配置
├── scaffolds/               # 文章模板
├── source/
│   ├── _posts/              # 88县市文章（99篇）
│   ├── map/                 # 探索贵州页面
│   ├── about/               # 关于页面
│   ├── img/                 # 封面图（99张）
│   ├── manifest.json        # PWA 清单
│   └── sw.js                # Service Worker
├── public/                  # 生成静态文件
└── node_modules/            # 依赖
```

## 🚀 三步启动

### 1. 安装依赖
```powershell
npm install
```

### 2. 本地预览
```powershell
npx hexo server
```

浏览器打开 `http://localhost:4000`

### 3. 生成静态文件
```powershell
npx hexo generate
```

生成的网站在 `public/` 目录，可直接部署到任意服务器。

## ✍️ 写新文章

```powershell
# 在 D:\Code\GuiZhouRen 目录下
npx hexo new "遵义"
```

然后在 `source/_posts/遵义.md` 编辑即可。

### 文章模板
```markdown
---
title: 文章标题
date: 2026-07-04 23:00:00
tags:
  - 标签1
  - 标签2
categories: 分类名
description: 简短描述
---

正文内容（Markdown 格式）
```

## ✨ 网站特色功能

- 🗺️ **探索贵州** — 可视化分区展示 7 大地理板块，点击直达分类文章
- 📱 **PWA 支持** — 可添加到手机桌面，离线也能访问已缓存页面
- 🎲 **随机文章** — 右下角按钮一键随机跳转，发现未知角落
- 🌊 **页面动画** — 入场渐显动画，浏览体验更流畅
- 🏆 **必游榜单** — 探索页精选 TOP 10 目的地与美食

## 📝 贵州县市文章计划

按地区分批写：
- **黔中**：贵阳、安顺 → 文章放 `categories: 黔中`
- **黔北**：遵义、铜仁 → `categories: 黔北`
- **黔南**：黔南州、黔西南州 → `categories: 黔南`
- **黔东南**：黔东南州 → `categories: 黔东南`
- **黔西北**：毕节、六盘水 → `categories: 黔西北`
