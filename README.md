# 跟着豪士绅士 · 一片好吃吐司的诞生

一个单文件（`index.html`）的移动端 H5 互动营销体验，讲述「一片好吃吐司的诞生」故事。

## 功能特性

- **纯前端、零依赖**：所有逻辑、样式、素材（内嵌 base64）都打包在单个 `index.html` 中。
- **互动剧情**：多场景分镜（揉面、发酵、烘烤、出炉等），配合引导气泡逐步推进。
- **Web Audio 音效**：所有音效（点击、揉面、烘烤、胜利等）由 `AudioContext` 实时合成，无需音频文件。
- **移动端优化**：限制最大宽度 480px，适配安全区域（刘海屏），禁用缩放与文本选择，带触感震动反馈。
- **动画**：CSS keyframes 实现的 Ken Burns、漂浮、脉冲、爆破等动效。

## 本地预览

直接用浏览器打开 `index.html`，或启动一个静态服务器：

```bash
python -m http.server 8000
# 浏览器访问 http://localhost:8000
```

## 部署

通过 GitHub Actions 自动部署到 GitHub Pages，工作流见 `.github/workflows/deploy.yml`。
推送到 `main` 或 `deploy/github-pages` 分支即自动构建并发布。

部署完成后，访问地址形如：
`https://<用户名>.github.io/<仓库名>/`
