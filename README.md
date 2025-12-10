# HugoWind Starter

[English](#english) | [简体中文](#简体中文)

---

## English

🚀 Quick start template for [HugoWind](https://github.com/ouraihub-hugo-themes/hugowind) theme - A modern Hugo theme inspired by AstroWind.

### Features

- ✅ Pre-configured with Hugo Modules
- ✅ Uses pre-compiled theme (no build tools needed)
- ✅ GitHub Actions deployment included
- ✅ Multilingual support (English/Chinese)
- ✅ Ready to use out of the box

### Prerequisites

- Hugo Extended v0.120.0+
- Git 2.0+
- Go 1.20+
- Node.js v18.0+ (for Pagefind search)
- pnpm v8.0+

### Quick Start

1. **Use this template** (click the green button above) or clone:

```bash
git clone https://github.com/ouraihub-hugo-themes/hugowind-starter.git my-site
cd my-site
```

2. **Initialize Hugo Modules**:

```bash
hugo mod get -u
```

3. **Install dependencies** (for search):

```bash
pnpm install
```

4. **Start development server**:

```bash
pnpm dev
```

5. **Visit** http://localhost:1313

### Creating Content

```bash
# English post
hugo new content/en/posts/my-post.md

# Chinese post
hugo new content/zh/posts/my-post.md
```

### Deployment

This starter includes GitHub Actions for automatic deployment to GitHub Pages.

1. Go to repository Settings → Pages
2. Set Source to "GitHub Actions"
3. Push to main branch

### Updating Theme

```bash
hugo mod get -u
hugo mod tidy
```

### Links

- [HugoWind Theme](https://github.com/ouraihub-hugo-themes/hugowind)
- [Hugo Documentation](https://gohugo.io/documentation/)

---

## 简体中文

🚀 [HugoWind](https://github.com/ouraihub-hugo-themes/hugowind) 主题的快速启动模板 - 一个受 AstroWind 启发的现代 Hugo 主题。

### 特性

- ✅ 预配置 Hugo Modules
- ✅ 使用预编译主题（无需构建工具）
- ✅ 包含 GitHub Actions 部署
- ✅ 多语言支持（中文/英文）
- ✅ 开箱即用

### 前置要求

- Hugo Extended v0.120.0+
- Git 2.0+
- Go 1.20+
- Node.js v18.0+（用于 Pagefind 搜索）
- pnpm v8.0+

### 快速开始

1. **使用此模板**（点击上方绿色按钮）或克隆：

```bash
git clone https://github.com/ouraihub-hugo-themes/hugowind-starter.git my-site
cd my-site
```

2. **初始化 Hugo 模块**：

```bash
hugo mod get -u
```

3. **安装依赖**（用于搜索）：

```bash
pnpm install
```

4. **启动开发服务器**：

```bash
pnpm dev
```

5. **访问** http://localhost:1313

### 创建内容

```bash
# 英文文章
hugo new content/en/posts/my-post.md

# 中文文章
hugo new content/zh/posts/my-post.md
```

### 部署

此 starter 包含 GitHub Actions，可自动部署到 GitHub Pages。

1. 进入仓库 Settings → Pages
2. 将 Source 设置为 "GitHub Actions"
3. 推送到 main 分支

### 更新主题

```bash
hugo mod get -u
hugo mod tidy
```

### 相关链接

- [HugoWind 主题](https://github.com/ouraihub-hugo-themes/hugowind)
- [Hugo 文档](https://gohugo.io/documentation/)

---

## License

MIT License - see [LICENSE](LICENSE) for details.
