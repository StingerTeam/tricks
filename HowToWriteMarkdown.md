# 如何撰写 Markdown

## 为什么使用 Markdown

Markdown 是一种轻量级标记语言，可以用于撰写文档、笔记、博客等。

Markdown 提供了许多优势，如易于学习和使用的语法、可移植性和兼容性、灵活性和可定制性，以及可读性和可维护性。它简单直观，可以使用各种工具和平台转换为 HTML、PDF 或其他格式。此外，它还可以使用扩展程序和插件扩展更多的功能和样式，并生成清晰一致的文本，便于编辑和更新。

## Markdown 语法

[GitHub 官方 Markdown 语法教程](https://docs.github.com/zh/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

## Markdown 排版规范

你可能会觉得这些规范很恼人，但事实上，遵守这些规范会让你在编写 Markdown 时更愉悦。

[基于 Markdown 的中文文档排版规范](https://zhuanlan.zhihu.com/p/144446995)

[GitHub 风格的 Markdown 规范](https://gfm.docschina.org/zh-hans/)

> 题外话：如果你对排版、设计等感兴趣，推荐 UP 主：[oooooohmygosh](https://space.bilibili.com/38053181)，有利于提升书写规范性和审美。

## 使用什么工具

市面上有很多优秀的 Markdown 编辑器，如 Obsidian、Typora、Notion、AFFiNE 等。

但是作者还是选择了 VS Code。

以下只是个人见解，具体用什么软件还是看个人喜好。

### 原因

1. 其他工具支持所见即所得（渲染效果和源码在同一位置），很酷，很方便，但是实际使用起来还是有些不适。VS Code 可以左边编写源代码，右边查看渲染效果，这样使用更加精准快速。

2. VS Code 的资源管理器或者说项目模式更加简单，无需创建仓库等概念，直接打开文件夹，使用最原始的资源管理概念即可。

3. VS Code 同时也是我的主力 IDE，有一种 All in One 的方便。

4. VS Code 可以安装很多插件，提供了很多其他工具无法比拟的功能，如 Git 集成（可以用于云端同步）、自定义主题、自动排版、自动格式化、AI 自动补全等。

### 推荐的 VS Code Markdown 插件

- GitHub Markdown Preview：包含很多插件的插件包，装完基本够用了。

- markdownlint：Markdown 语法检查，按下 Ctrl+S 自动格式化，让你的 markdown 更加优雅。

- pangu-markdown：自动排版，中英文混排时，自动在中文和英文之间添加空格，更加规范。

- GitHub Copilot：AI 自动补全，谁用谁知道。需要申请学生账号（过程较为艰辛，后续可能会出教程）。当然也有其他代替品。

- GitHub Copilot Chat：类似 ChatGPT，针对代码的 AI 对话系统，需要 GitHub Copilot 作为前提。

### 缺点

虽然用 VS Code 写 Markdown 很方便，但是阅读 Markdown 还是 Obsidian 等软件更好，包括但不限于效果更好看、有树状索引（VS Code 有大纲）、导出功能更好等。
