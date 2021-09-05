---
title: 使用 Hexo 和 Hugo 來架設部落格
date: 2021-09-05T17:25:17+08:00
tags: [教學系列]
draft: true
---
本篇教學將使用 Hexo 和 Hugo 兩款非常受歡迎的工具來建立自己的靜態部落格，並且也會根據小弟操作起來的感受來給予評價

## Hexo

[Hexo 官網](https://hexo.io/zh-tw/)

Hexo 是一款基於 Node.js 所製作的網誌框架，官網內的中文文件相當完善，且 Google 上也可以找到許多關於 Hexo 的教學，我認為這點相當的加分

以下將介紹如何在 Ubuntu 中安裝和操作

### 安裝教學

#### 前置作業

首先我們需要安裝 Node.js 和 git ，這邊推薦使用 nvm 來安裝 Node.js
如何安裝可以參考 nvm 的 Github

[連結](https://github.com/nvm-sh/nvm#install--update-script)

nvm 安裝好後再安裝最新版 Node.js

```bash
nvm install node
```

git 的安裝方式可以直接下指令安裝

```bash
sudo add-apt-repository ppa:git-core/ppa
sudo apt update
sudo apt install git
```

都安裝好後直接使用 npm 來安裝 Hexo

```bash
npm install -g hexo-cli
```

## Hugo 操作教學

[Hugo 官網](https://gohugo.io/)

## 網域基本概念與註冊購買
