---
title: 如何将hexo推送到github
date: '2026-03-09 17:01:53'
updated: '2026-03-09 17:35:51'
permalink: /post/how-to-push-hexo-to-github-zs4upa.html
comments: true
toc: true
---



# 如何将hexo推送到github

好的，我们来做一次 ​**Git 仓库的全面初始化**，包括清理之前的推送记录，重新建立一个干净的仓库并推送到 GitHub Pages。以下是完整流程：

---

### 🔧 全面初始化步骤

1. **进入博客目录**

   ```bash
   cd E:\BaiduSyncdisk\博客\my-blog
   ```
2. **删除旧的**  **​`.git`​**​ **文件夹（如果存在）** 这一步会清除之前的 Git 配置和推送记录：

   ```bash
   rd /s /q .git
   ```

   （Windows 下用 `rd`​，Linux/macOS 下用 `rm -rf .git`）
3. **重新初始化 Git 仓库**

   ```bash
   git init
   ```
4. **添加远程仓库**

   ```bash
   git remote add origin https://github.com/GinPd/GinPd.github.io.git
   ```
5. **切换到 main 分支**

   ```bash
   git branch -M main
   ```
6. **添加文件并提交**

   ```bash
   git add .
   git commit -m "初始化博客仓库"
   ```
7. **推送到远程仓库**如果远程仓库已有内容，可以选择强制覆盖：

   ```bash
   git push -u origin main --force
   ```

   ⚠️ 注意：这会覆盖远程仓库的历史记录，只保留你本地的内容。

---

### 🔑 总结

- 删除 `.git` → 清理旧仓库记录
- ​`git init` → 重新初始化
- ​`git remote add origin` → 关联远程
- ​`git branch -M main` → 统一分支名称
- ​`git add . && git commit` → 提交代码
- ​`git push -u origin main --force` → 推送到 GitHub Pages

这样你就能得到一个 ​**全新的 Git 仓库**，并且远程仓库会完全同步你的本地内容。

要不要我帮你再整理一份 ​**Hexo 博客部署到 GitHub Pages的完整流程清单**​（包括 `hexo generate`​ 和 `hexo deploy`），这样你就能一步步完成博客上线？

[基于 Hexo 和 GitHub Pages 搭建博客并实现思源笔记一键发布 - DUKE'S BLOG](https://duke-zhu.top/post/build-a-blog-based-on-hexo-and-github-pages-and-realize-oneclick-release-of-siyuan-notes-z1ji8uo.html)

[在 GitHub Pages 上部署 Hexo | Hexo](https://hexo.io/zh-cn/docs/github-pages)
