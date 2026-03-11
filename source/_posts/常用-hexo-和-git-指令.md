---
title: 常用hexo和git指令
date: '2026-03-10 11:08:49'
updated: '2026-03-10 11:35:37'
permalink: /post/commonly-used-hexo-and-git-commands-z1r59ho.html
comments: true
toc: true
---





- 一键预览，本地`localhost:4000`

  ```shell
  hexo clean && hexo generate && hexo server
  ```

- 添加、提交文件

  ```shell
  git add .

  git commit -m "merge: 解决冲突（保留本地最新配置 + 远程新文章）"
  ```

- 推送

  ```shell
  git push origin main
  ```

- 拉取

  ```shell
  git pull origin main
  ```

‍
