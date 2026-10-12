# 邓睿哲个人主页

面向求职投递的中文单页主页。使用原生 HTML 和 CSS，可直接由 GitHub Pages 托管。

## 本地预览

在 `portfolio-site` 目录打开 `index.html`，或使用任意静态文件服务器预览。

## 发布到 GitHub Pages

当前账号为 `piblockarc`，仓库为 `pizpi`，已发布地址为 `https://piblockarc.github.io/pizpi/`。

1. 使用公开仓库 `pizpi`。
2. 将 `index.html`、`styles.css`、`.nojekyll` 和本说明放入仓库根目录。
3. 打开仓库 **Settings → Pages**，在 **Build and deployment** 中选择 **Deploy from a branch**，分支选 `main`，目录选 `/(root)`，保存。
4. 等待 GitHub Pages 发布成功后访问 `https://piblockarc.github.io/pizpi/`。

页面不依赖构建工具或服务端。`preview-desktop.png` 和 `preview-mobile.png` 是本地检查截图，无需上传。

## 修改内容

- 个人介绍、教育背景、项目、技能和奖项：编辑 `index.html`。
- 颜色、字号和移动端布局：编辑 `styles.css`。
- 在线修改：打开 GitHub 仓库中的 `index.html`，点击编辑按钮修改并提交，Pages 会重新发布。
- 正式公开前，请核对联系方式与项目资料的公开权限。

当前文字根据个人简历和自我介绍 PPT 整理。三个项目均包含目标、系统方案、个人工作、结果，以及可展开的技术实现与调试难点。

## 添加项目图片

将图片放入 `assets/`，在对应项目 HTML 注释位置加入 `figure`，使用 `project-media` 样式。图片默认 `width: 100%`、`height: auto`，保持原始比例，图注写明实物或运行结果。

目前尚未插入图片，收到整理好的素材后补充。奖学金比例、数学竞赛年份在两份材料中存在差异，页面暂未列出这些细节。
