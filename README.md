# 贵州黔行 - 快速上手

## 📂 项目结构

```
GuiZhouRen/
├── _config.yml          # Hexo 主配置（已配好）
├── package.json         # 依赖清单
├── scaffolds/           # 文章模板
├── source/
│   ├── _posts/          # 所有文章放这里
│   │   ├── hello-guizhou.md          # 中文欢迎页
│   │   ├── welcome-to-guizhou-en.md  # 英文欢迎页
│   │   └── guiyang.md                # 贵阳示例文章
│   ├── _data/
│   │   └── butterfly.yml # Butterfly 主题配置
│   └── about/
│       └── index.md      # 关于页面
└── themes/              # 主题目录（npm install 后会安装 Butterfly）
```

## 🚀 三步启动

### 1. 安装依赖
```powershell
cd D:\Code\GuiZhouRen
npm install
```

### 2. 本地预览
```powershell
npx hexo server
```

浏览器打开 `http://localhost:4000`

### 3. 预览正常后，生成静态文件
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

## 📝 贵州县市文章计划

按地区分批写：
- **黔中**：贵阳、安顺 → 文章放 `categories: 黔中`
- **黔北**：遵义、铜仁 → `categories: 黔北`
- **黔南**：黔南州、黔西南州 → `categories: 黔南`
- **黔东南**：黔东南州 → `categories: 黔东南`
- **黔西北**：毕节、六盘水 → `categories: 黔西北`
