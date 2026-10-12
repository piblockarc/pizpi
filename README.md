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

现有图片已放入各项目的 `project-gallery` 图片组。每张图片使用独立的 `figure` 和 `img`，按原始比例显示，点击后打开原图。

1. 将新图片上传到仓库根目录；也可以放在 `assets/` 中。
2. 在 `index.html` 对应项目的 `project-gallery` 内，复制以下代码。
3. 将两处 `new-image.png` 替换为真实图片路径，并修改图注。
4. 提交到 `main`，等待 GitHub Pages 自动更新。

```html
<figure class="project-media">
  <a class="image-link" href="new-image.png" target="_blank" rel="noopener noreferrer" aria-label="查看原图：图片说明">
    <img src="new-image.png" alt="图片说明" loading="lazy" decoding="async" />
  </a>
  <figcaption>图片说明</figcaption>
</figure>
```

- 一个 `img` 只填写一个 `src`；多张图片复制多段 `figure`。
- 需要横跨整行的流程图，将 `class="project-media"` 改为 `class="project-media project-media--wide"`。
- 电脑端根据可用宽度排成一列或两列，手机端自动使用单列。
- 图片保持 `height: auto`，不使用固定高度或裁切。
- 荣誉图片放在荣誉部分的 `section__body` 内。

奖学金比例、数学竞赛年份在两份文字材料中存在差异，页面暂未列出这些细节。
