# MARTIN · 为想象赋予形状

Martin 的个人网站，展示个人介绍、项目与思考。自定义域名：**martinyuan.com**。

## 发布链路

本地 React / TypeScript / Vite 源工程 → 构建生成 dist → 本仓库 docs → GitHub Pages → martinyuan.com。

GitHub Pages 设置为 `main` 分支、`/docs` 目录。域名已配置 GitHub Pages 的四条 A 记录，日常更新网站不需要重复修改 DNS。

## 后续如何更新

1. 在本地 `terra-nova` 源工程修改 `src/content.ts` 或页面代码。它与发布仓库的本地检出 `github-pages` 位于同一个父目录。
2. 在源工程运行 `npm run build`，完成类型检查和生产构建。
3. 将源工程 `dist/` 中的文件同步到本仓库 `docs/`，保留 `CNAME` 与 `.nojekyll`。
4. 提交并推送 `main`，在仓库 Actions / Settings → Pages 查看发布状态。

`docs/assets/` 是构建生成的压缩文件，应回到源工程修改内容。当前聊天入口为固定问答，尚未连接真正的个人 Agent。

## 目录说明

- `docs/index.html`：正式网站入口。
- `docs/assets/`、`docs/images/`：脚本、样式与公开展示素材。
- `docs/CNAME`：自定义域名。
- `docs/.nojekyll`：直接发布静态文件。
- 根目录原有的 `dist/`、`.openai/`：早期课程模板，保留历史记录，不作为当前 Pages 的发布内容。

本仓库仅存放发布文件；完整源工程及部署维护说明位于本地 `terra-nova`。
