# Vacuum's Blog

个人博客，使用 [Hexo](https://hexo.io/) 8 + [Butterfly](https://butterfly.js.org/) 主题搭建。

## 本地开发

```bash
pnpm install          # 安装依赖（本项目使用 pnpm）
pnpm server           # 本地预览 http://localhost:4000
pnpm exec hexo new post "文章标题"   # 新建文章
pnpm build            # 生成静态文件到 public/
pnpm clean            # 清理缓存
```

## 目录说明

| 路径 | 说明 |
|---|---|
| `source/_posts/` | 博客文章（Markdown） |
| `source/about/` | 关于页面（可选） |
| `_config.yml` | Hexo 站点配置 |
| `_config.butterfly.yml` | Butterfly 主题配置 |
| `.github/workflows/pages.yml` | GitHub Pages 自动部署 |

## 部署

推送到 `main` 分支后，GitHub Actions 会自动构建并部署到 GitHub Pages：

https://chenyuliu06.github.io

首次使用需要在仓库 **Settings → Pages → Build and deployment → Source** 选择 **GitHub Actions**。
