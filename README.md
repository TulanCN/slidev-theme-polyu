# slidev-theme-polyu

[![NPM version](https://img.shields.io/npm/v/slidev-theme-polyu?color=a6192e&label=)](https://www.npmjs.com/package/slidev-theme-polyu)

香港理工大学主题的 [Slidev](https://github.com/slidevjs/slidev) 幻灯片模板。

<!--
  Learn more about how to write a theme:
  https://sli.dev/guide/write-theme.html
--->

<!--
  run `npm run dev` to check out the slides for more details of how to start writing a theme
-->

## 特点

- 遵循香港理工大学的品牌标识
- 使用理大红色 (#a6192e) 作为主题色
- 包含理大标志和口号
- 简洁专业的设计风格

## 安装

在你的 `slides.md` 文件的前言部分添加以下内容。启动 Slidev 后，它会提示你自动安装主题。

<pre><code>---
theme: <b>polyu</b>
---</code></pre>

了解更多关于 [如何使用主题](https://sli.dev/guide/theme-addon#use-theme) 的信息。

## 布局

此主题提供以下布局:

- `cover` - 主页封面布局，带有理大标志和口号
- `intro` - 简介布局

## 组件

此主题提供以下组件:

- 标准 Slidev 组件

## 贡献

- `npm install`
- `npm run dev` 启动 `example.md` 的主题预览
- 编辑 `example.md` 和样式文件，查看更改效果
- `npm run export` 生成预览 PDF
- `npm run screenshot` 生成预览 PNG
