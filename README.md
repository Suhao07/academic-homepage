# 个人学术主页

本主页直接复用了 [Jon Barron 学术主页模板](https://github.com/jonbarron/jonbarron.github.io) 的版式与未修改的 `stylesheet.css`。原仓库 README 明确允许将代码用于个人主页。

模板没有包含 Jon Barron 的个人介绍、论文条目、图片、视频或数据文件；本目录同样没有生成任何图片或个人文案。

## 手动填写内容

只需编辑 [index.html](index.html)：

1. 将所有 `[ ... ]` 占位文字替换为自己的信息；
2. 将自己的头像放到 `images/profile.jpg`，或直接删除头像所在的表格单元；
3. 若需保留简历链接，将个人 CV 放到 `data/CV.pdf`；
4. 每篇论文复制标记好的论文表格行，并只在 `images/` 内使用自己拥有的论文缩略图。

## GitHub Pages 部署

本目录是与技术博客完全独立的 Git 仓库，已包含 GitHub Actions 发布工作流：`.github/workflows/deploy-pages.yml`。

现有技术博客占用根网址 <https://suhao07.github.io/>。为了两者并存，建议将学术主页发布到独立项目仓库，例如 `Suhao07/academic-homepage`。发布网址为：

```text
https://suhao07.github.io/academic-homepage/
```

将本目录推送到新仓库的 `main` 分支后，打开 GitHub 仓库的 **Settings → Pages**，在 **Build and deployment → Source** 中选择 **GitHub Actions**。之后每次推送 `main`，网站都会自动更新。
