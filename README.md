# MARTIN · 为想象赋予形状

正式网站：https://martinyuan.com/

`docs/` 是当前 React 网站的生产构建文件。GitHub Pages 从 `main` 分支的 `/docs` 目录发布，`docs/CNAME` 记录自有域名，`docs/.nojekyll` 让静态文件直接发布。

本地源工程位于 `E:\Projects\个人网站\terra-nova`，发布检出位于同级 `github-pages`。后续修改源工程并构建，将 `dist/` 内文件更新到本仓库的 `docs/`，提交推送后等待 Pages 发布完成。`docs/` 中的哈希文件名由构建生成，不要直接编辑压缩后的 JavaScript。

下方的原生 HTML 模板说明和原来的 `dist/` 继续保留作为早期版本记录；当前 Pages 使用的是 `docs/`。

## 打开网站

双击 `dist/index.html`，即可在浏览器里打开。也可以把 `dist` 内的文件一起上传到静态网站托管服务。

## 文件说明

- `dist/index.html`：页面内容，包括名字、简介、兴趣和联系方式。
- `dist/style.css`：页面样式，包括配色、布局和手机适配。
- `dist/script.js`：切换浅色 / 深色模式、记住配色选择、自动更新年份。
- `dist/favicon.svg`：浏览器标签页图标。

## 换成自己的资料

1. 将 `index.html` 中的“你的名字”替换成真实姓名，包括标题和页脚。
2. 修改“关于我”中的简介和兴趣标签。
3. 将 `hello@example.com` 替换成自己的邮箱，记得同时修改显示文字和 `mailto:` 链接。
4. 如果需要更换颜色，修改 `style.css` 开头的 CSS 变量。

当前姓名、简介、兴趣和邮箱是示例内容。邮箱链接会打开访客的邮件应用，网站本身不代发邮件。
