# Gengyuan Hu · 学术主页

这是基于 [al-folio v1.2](https://github.com/alshedivat/al-folio/releases/tag/v1.2) 的 Jekyll 学术站点，使用官方 `al_folio_core` 主题 gem。网站包含英文首页、论文、项目及中文简介；内容取自公开的 [GitHub 账号](https://github.com/ChengFeng233)、[ELTLM-Bench](https://github.com/ChengFeng233/ELTLM-Bench)、[ACL Anthology](https://aclanthology.org/2026.findings-acl.772/) 和 [ROBOGAME 视觉仓库](https://github.com/ChengFeng233/USTC_ROBOGAME2025_CV)。主页没有添加未经确认的学位或年级，也未添加邮箱或 Scholar ID。

## 本地预览

安装 Ruby 3.4（Windows 推荐 RubyInstaller with Devkit），在此目录运行：

```sh
bundle install
bundle exec jekyll serve
```

浏览器打开 `http://127.0.0.1:4000`。

## 发布到 GitHub Pages

1. 在 `ChengFeng233` 账号下创建公开仓库 `ChengFeng233.github.io`。
2. 将本目录的**源码**放到仓库 `main` 分支根目录，保留 `.github/workflows/pages.yml`；不要上传 `_site/`，也不要在仓库里多套一层 `academic-homepage/`。
3. 在仓库 **Settings → Pages → Build and deployment → Source** 选择 **GitHub Actions**（不是 **Deploy from a branch**）。
4. 在 **Actions → Deploy academic homepage** 点击 **Run workflow**。成功后访问 `https://chengfeng233.github.io`。后续推送至 `main` 会自动部署。

## 更新内容

| 内容 | 文件 |
| --- | --- |
| 英文简介、首页链接 | `_pages/about.md` |
| 中文简介 | `_pages/zh.md` |
| 论文元数据、论文链接及首页精选 | `_bibliography/papers.bib` |
| 项目介绍 | `_projects/` |
| 站点名称、地址、主题设置 | `_config.yml` |

如需使用照片，将图片放到 `assets/img/` 并修改 `_pages/about.md` 的 `profile.image`。图形素材是站点配图，不是临床影像或比赛实拍。
