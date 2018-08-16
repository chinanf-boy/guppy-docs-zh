# [guppy@0.0.1][commit]  [![translate-svg]][translate-list]

[translate-svg]: http://llever.com/translate.svg
[translate-list]: https://github.com/chinanf-boy/chinese-translate-list
    
「 React.js的友好应用程序管理器和任务运行器 」

[commit]: https://github.com/joshwcomeau/guppy/tree/73a9f68702d44fe03dad118bd1b112f1998ef454
[more]: https://github.com/chinanf-boy/chinese-translate-list

---

## 校对 ✅

<!-- doc-templite START generated -->
<!-- time = '2018 7.16' -->

翻译的原文 | 与日期 | 最新更新 | 更多
---|---|---|---
[commit] | ⏰ 2018 7.16 | ![last] | [中文翻译][more]
<!-- doc-templite END generated -->

[last]: https://img.shields.io/github/last-commit/joshwcomeau/guppy.svg

### 贡献

欢迎 👏 勘误/校对/更新贡献 😊 [具体贡献请看](https://github.com/chinanf-boy/chinese-translate-list#贡献)

## 生活

[help me live , live need money 💰](https://github.com/chinanf-boy/live-need-money)


## 目录

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [🐠孔雀鱼-Guppy](#%E5%AD%94%E9%9B%80%E9%B1%BC-guppy)
    - [React.js的友好应用程序管理器和任务运行器](#reactjs%E7%9A%84%E5%8F%8B%E5%A5%BD%E5%BA%94%E7%94%A8%E7%A8%8B%E5%BA%8F%E7%AE%A1%E7%90%86%E5%99%A8%E5%92%8C%E4%BB%BB%E5%8A%A1%E8%BF%90%E8%A1%8C%E5%99%A8)
    - [当前状态](#%E5%BD%93%E5%89%8D%E7%8A%B6%E6%80%81)
    - [安装](#%E5%AE%89%E8%A3%85)
    - [入门](#%E5%85%A5%E9%97%A8)
    - [它是如何工作的](#%E5%AE%83%E6%98%AF%E5%A6%82%E4%BD%95%E5%B7%A5%E4%BD%9C%E7%9A%84)
    - [未来愿景](#%E6%9C%AA%E6%9D%A5%E6%84%BF%E6%99%AF)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

---

# 🐠孔雀鱼-Guppy

### React.js的友好应用程序管理器和任务运行器

![Guppy project screen](https://github.com/joshwcomeau/guppy/raw/master/docs/images/main-image.png)

React Web开发有很多"元"技能,与构建优秀的Web产品并没有任何关系. 

例如,终端. 对于我们这些没有在 unix shell 上长大的人来说,终端是一个神秘而难以理解的命令. 它无疑是强大的,也是开发的宝贵技能......但是它真的应该成为现代网络开发的先决条件吗?

Guppy是一款免费的桌面应用程序,旨在让您更轻松地开始构建 React Web 产品. 它为 React开发人员 面临的许多典型任务提供了友好的 GUI: 

-   创建新项目
-   运行开发服务器
-   执行任务 (构建生产,运行测试) 
-   管理依赖项 (添加,更新,搜索) 

Guppy是为 初学者 而设计的 - 刚开始使用 Web开发 的人. 我们希望它对于高级用户来说足够强大,但我们始终会优先考虑 新开发人员 的体验. 我们永远不会为Guppy收钱,它总是免费使用. 

> **注意**:  这是*超早期预发布alpha版本*. 说实话,它可能尚未准备好初学者使用 (可能有令人沮丧的错误,而且它只能在MacOS上运行) . 我们的目标是建立一个社区来为此工作,并为 初学者 创造真正有用和美妙的东西. 

### 当前状态

这个项目是早期发布的Alpha版. 

想帮助 萌新 创造一些美好的东西吗? 我们正在积极寻找贡献者,以帮助将这个预发行版开发成令人惊奇的东西. 这是一个参与并帮助塑造Guppy未来的好时机!

另外,需要注意的是: 这是一个在业余时间工作的副项目. 我们感谢任何错误报告,但实际上我们可能无法及时解决问题 (尽管可以随时提供修复!) 

### 安装

现在,**Guppy仅适用于MacOS**. 我们希望尽快支持 Windows和Linux. 

要使用 Guppy,首先需要安装一个现代版本的Node (一个Javascript运行时) . [下载节点](https://nodejs.org/en/download/current/). 由于 NPM 5.6.0中可能破坏依赖性的错误,建议使用"当前"版本而不是LTS. 

安装Node后,即可[下载Guppy](https://github.com/joshwcomeau/guppy/releases/download/v0.0.1/Guppy-MacOS.zip)

双击下载的可执行文件以打开Guppy. 如果MacOS,抱怨这是从互联网上下载的事实,您可能需要右键单击并选择"打开". 

> 注意: 在将来的稳定版本中,我希望通过使用 Guppy包裹Node 来消除下载Node的需要 (参见[#44](https://github.com/joshwcomeau/guppy/issues/44)) . 我还计划创建一个合适的安装程序,以便将 Guppy 复制到 Applications文件夹 (参见[#26](https://github.com/joshwcomeau/guppy/issues/26)) . 欢迎捐款!

### 入门

详细了解如何在我们的网站中使用Guppy[入门指南](./docs/getting-started.md). 

### 它是如何工作的

Guppy是一个 `electron` 应用程序,在后台秘密运行终端命令. 它用 **create-react-app** 和 **gatsby-cli**. 可以想象为Next和其他项目类型 (包括非React项目) 添加支持

Guppy为您添加了一个新的顶级密钥`package.json`存储与项目相关的信息. 它也读取`package.json`找出当前的依赖关系,看看哪些任务可用 (通过`scripts`) . 

Guppy拥有围绕 任务类型构建智能模块. 例如,开发服务器不是普通任务,它应该在整个项目工作期间运行,因此它在页面顶部给出了自己的模块. 

有关了解更多关于  Guppy和贡献的更多信息,请参阅我们的[贡献文档](CONTRIBUTING.md)

### 未来愿景

现在,Guppy 的功能集非常有限. 它由3个模块组成: "开发服务器"窗格,"任务"窗格和"依赖关系"窗格. 

我希望看到的第一个重大变化是更好地支持常见的开发工具,如 运行测试,linting,代码格式化 等等. 一些潜在改进的例子: 

-   测试不应该只是列表中的一个细行,它应该有自己的模块,就像 Dev Server 那样. 它应该以"交互"模式运行,并允许用户通过单击按钮重新运行测试. 

-   依赖模块 应该易于更新. 我想象一个"更新 核心 依赖项"按钮,它可以通过 built-in-codemod 支持更新 react,react-dom和任何相关的包. 我想它能够找到安全问题 (通过[`npm audit`](https://docs.npmjs.com/getting-started/running-a-security-audit)) . 

我还希望看到 Guppy 在 教育用户关于 Web开发方面 变得更加有用. Guppy 的理念是 任何人都可以学习Web开发,它应该提供资源来帮助学习者. Guppy 可以完全访问 项目代码和设置,因此我想知道是否有机会,为用户遇到的问题提出解决方案......我还没有任何具体的想法,但考虑一下这很有意思. 
