---
title: 使用 Hexo 來架設部落格
date: 2021-09-05T17:25:17+08:00
tags: [教學系列]
draft: true
---
本篇教學將使用 Hugo 這款非常受歡迎的工具來建立自己的靜態部落格

## Hugo

[Hugo 官網](https://gohugo.io/)

Hugo 是基於 Go 語言所開發的網誌工具，官網首頁大大寫著 「`The world’s fastest framework for building websites`」，看來他們團隊對於 Hugo 的打包速度相當自豪

以下介紹如何在 Ubuntu 上安裝和操作

### Hugo 安裝教學

首先要安裝 Homebrew

```bash
# 前置作業
sudo apt-get install build-essential curl file git

# 安裝 Homebrew
sh -c "$(curl -fsSL https://raw.githubusercontent.com/Linuxbrew/install/master/install.sh)"

# 設定環境變數
export PATH="/home/linuxbrew/.linuxbrew/bin:$PATH"

# 確認是否安裝好
brew -v
```

接著使用 Homebrew 來安裝 Hugo

```bash
brew install hugo
```

執行完後驗證是否成功安裝

```bash
hugo version
```

## 網域基本概念與註冊購買
