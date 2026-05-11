# blog.limewolf.top
Visit my website: [blog.limewolf.top](https://blog.limewolf.top).

---
Written using both **Org Mode** and **Markdown**.

Powered by 
- [Hugo](https://github.com/gohugoio/hugo)
- [monochrome](https://github.com/kaiiiz/hugo-theme-monochrome)
- [vercel](https://vercel.com/)
- [giscus](https://github.com/giscus/giscus)

---

## `hermes-neolog` 分支

> 本分支由 **柚木（阿普）** 操刀打造 ✨
> 视觉重构、主题搭建、短代码适配、前端资源整合，一条龙。
> 柚木是莱姆的 Hermes Agent，是莱姆的好助手 🐺🤝

### 与 master 分支的区别

| 维度 | master | hermes-neolog |
|------|--------|---------------|
| 主题 | Hugo 官方 monochrome 主题 | 自建 `neo-log` 定制主题 |
| 视觉风格 | 简洁极简风 | 毛玻璃 (glassmorphism) 质感、圆角卡片、现代暗色美学 |
| 短代码 | monochrome 内置 | 基于原始短代码做了适配与风格对齐 |
| 前端资源 | — | 引入 Prism 代码高亮、Fuse.js 搜索、Zooming 图片缩放等前端库 |
| 导航 | 默认 hamburger 菜单 | 重构后的 hamburger + 毛玻璃遮罩层 |
| config | YAML 格式 | TOML 重构，结构更清晰 |

### 创建目的

在不动 `master` 稳定内容的前提下，对博客进行一次彻底的视觉升级实验。改的不仅仅是 CSS——从布局模板、短代码适配到前端依赖全部重做，需要一个独立分支来承载这些破坏性变更。

### 工作流

1. **写文章** — 在 `content/` 下正常新增 `.md` 或 `.org` 文件
2. **本地预览** — 执行 `hugo server -D` 启动开发服务器，实时预览效果
3. **构建** — 确认无误后执行 `hugo`，静态文件输出到 `public/` 目录
4. **部署** — 将 `public/` 同步到 nginx 根目录 `/var/www/blog/`
5. **提交推送** — `git add . && git commit -m "..." && git push origin hermes-neolog`

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a></br>
This work is licensed under the <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
