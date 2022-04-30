---
title: "使用 Hugo + Netlify + Gandi 來架設部落格 Part 1"
date: 2022-04-29T13:25:17+08:00
tags: [教學系列]
draft: false
---

## 前言

終於開始來寫技術文章了，這項工作也是拖了半年許久，終於開始動工(感動

但在寫其他技術文章前，想先來分享我是如何來架設部落格的，也順便練練寫文章的感覺

此教學會分成三個部份來介紹：

1. Hugo
2. Netlify
3. Gandi

那麼就開始吧

## Hugo 介紹

[Hugo 官網](https://gohugo.io/)

Hugo 是基於 Go 語言所開發的網誌工具，官網首頁大大寫著 「`The world’s fastest framework for building websites`」，看來他們團隊對於 Hugo 的打包速度相當自豪

以下介紹如何在 Ubuntu 上安裝和操作

## Hugo 安裝教學

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

## Hello World

安裝成功後不免俗也要來執行一下 Hello World，也就是建立部落格

Hugo 也有提供相關的指令

```bash
hugo new site quickstart
```

執行後可以看到 quickstart 的資料夾被建立，裡面的內容正是我們的部落格架構

接著來發布我們部落格的第一篇貼文

```bash
cd quickstart
hugo new post/my-first-post.md
hugo server -D
```

執行後可以看到 content/post 內多了 my-first-post.md 的文件

接著在瀏覽器上開啟 <http://localhost:1313/> 便可以看到初步架設好的部落格啦

## 後記

Hugo 算是蠻主流的靜態網站框架，架設起來也不會很困難

而且還有很多主題與外掛插件可以選擇，這部份就留待你們自己去挖掘囉

下一篇將會來介紹如何將我們的部落格發布到 Netlify 上

### References

<https://gohugo.io/getting-started/quick-start/>

<https://ithelp.ithome.com.tw/articles/10235097>
