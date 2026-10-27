# 主页迁移说明

基于 https://github.com/xyjoey/PRISM 的 PRISM 模板；保留 MIT LICENSE。

- 旧仓库：https://github.com/Janene-Li/Janene-Li.github.io，默认分支 master。
- 已沿用原站昵称 Janene 和公开邮箱 enhanli_cs@163.com，并修正 GitHub 链接。头像使用用户提供的图片，并加入用户确认的 Google Scholar 主页。
- 已保留 10 篇旧文章及其 URL、图片、分类、标签和归档。
- 首页支持中英文和深色模式，旧文章内容保持原样。
- 原 About 页为空；新简介仅概括旧站笔记主题，不包含未经提供的学历或任职。
- 论文、履历、奖项、教学、服务、新闻等模板示例已移除，等真实资料到齐后补充。
- 旧站索引另存于 public/legacy/index.html。

## 之后更新

- 简介：content/bio.md；中文：content_zh/bio.md。
- 姓名、身份、机构、邮箱、学术主页：两种语言的 config.toml。
- 首页栏目：两种语言的 about.toml。
- 论文：content/publications.bib；加入真实论文后再开启导航和首页论文区。
- 头像：public/avatar.png。

## 运行与部署

Node.js 22 及以上。运行 npm ci，npm run dev 本地预览；npm run build 生成 out/。

GitHub Pages 需将 Settings → Pages → Source 设为 GitHub Actions。工作流对 PR 只构建，合并到 master 后部署。

迁移稿通过独立分支和草稿 PR 保存，审核并合并后再启用 GitHub Pages 工作流。

## 验证

本地已通过 Next.js 15.5.28 生产构建与 TypeScript 类型检查，并检查中英文切换、深色模式和全部 10 篇笔记列表。头像已替换为用户提供的图片。
