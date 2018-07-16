# guppy@1.0.0  [![translate-svg]][translate-list]

[translate-svg]: http://llever.com/translate.svg
[translate-list]: https://github.com/chinanf-boy/chinese-translate-list
    
「 React.js的友好应用程序管理器和任务运行器 」

[github source commit](https://github.com/joshwcomeau/guppy/tree/73a9f68702d44fe03dad118bd1b112f1998ef454)

欢迎 `Issue` 和 `Pull` ❤️, 最好 `Pull` 👏

[更多其他中文翻译](https://github.com/chinanf-boy/chinese-translate-list)

---

## 生活

[help me live , live need money 💰](https://github.com/chinanf-boy/live-need-money)

---

<!-- START doctoc -->
<!-- END doctoc -->

---

## 校对🀄️

- ⏰ 2018 7.16 开始

**0/5**


# 🐠孔雀鱼

### React.js的友好应用程序管理器和任务运行器

![Guppy project screen](https://github.com/joshwcomeau/guppy/raw/master/docs/images/main-image.png)

React Web开发有很多"元"技能,与构建优秀的Web产品并没有任何关系. 

例如,终端. 对于我们这些没有在unix shell上长大的人来说,终端是一个神秘而难以理解的命令. 它无疑是强大的,也是开发的宝贵技能......但是它真的应该成为现代网络开发的先决条件吗?

Guppy是一款免费的桌面应用程序,旨在让您更轻松地开始构建React Web产品. 它为React开发人员面临的许多典型任务提供了友好的GUI: 

-   创建新项目
-   运行开发服务器
-   执行任务 (构建生产,运行测试) 
-   管理依赖项 (添加,更新,搜索) 

Guppy是为初学者而设计的 - 刚开始使用Web开发的人. 我们希望它对于高级用户来说足够强大,但我们始终会优先考虑新开发人员的体验. 我们永远不会为Guppy收钱,它总是免费使用. 

> **注意**:  这是*超早期预发布alpha*. 说实话,它可能尚未准备好初学者使用 (可能有令人沮丧的错误,而且它只能在MacOS上运行) . 我们的目标是建立一个人们的社区来为此工作,并为初学者创造真正有用和美妙的东西. 

### 当前状态

这个项目是早期发布的Alpha版. 

想帮助为新手创造一些美好的东西吗?我们正在积极寻找贡献者,以帮助将这个预发行版alpha开发成令人惊奇的东西. 这是一个参与并帮助塑造Guppy未来的好时机!

另外,需要注意的是: 这是一个在业余时间工作的副项目. 我们感谢任何错误报告,但实际上我们可能无法及时解决问题 (尽管可以随时提供修复!) 

### 安装

马上,**Guppy仅适用于MacOS**. 我们希望尽快支持Windows和Linux. 

要使用Guppy,首先需要安装一个现代版本的Node (一个Javascript运行时) . [下载节点](https://nodejs.org/en/download/current/). 由于NPM 5.6.0中可能破坏依赖性的错误,建议使用"当前"版本而不是LTS. 

安装Node后,即可[下载Guppy](https://github.com/joshwcomeau/guppy/releases/download/v0.0.1/Guppy-MacOS.zip)

双击下载的可执行文件以打开Guppy. 如果MacOS抱怨这是从互联网上下载的事实,您可能需要右键单击并选择"打开". 

> 注意: 在将来的稳定版本中,我希望通过使用Guppy附带的Node运行时来消除下载Node的需要 (参见[#44](https://github.com/joshwcomeau/guppy/issues/44)) . 我还计划创建一个合适的安装程序,以便将Guppy复制到Applications文件夹 (参见[#26](https://github.com/joshwcomeau/guppy/issues/26)) . 欢迎捐款!

### 入门

详细了解如何在我们的网站中使用Guppy[入门指南](https://github.com/joshwcomeau/guppy/blob/master/docs/getting-started.md). 

### 怎么运行的

Guppy是一个电子应用程序,在后台秘密运行终端命令. 它用**CREATE-反应应用内**和**盖茨比-CLI**. 可以想象为Next和其他项目类型 (包括非React项目) 添加支持

Guppy为您添加了一个新的顶级密钥`package.json`存储与项目相关的信息. 它也读取`package.json`找出当前的依赖关系,看看哪些任务可用 (通过`scripts`) . 

Guppy拥有围绕任务类型构建的智能模块. 例如,开发服务器不是普通任务,它应该在整个项目工作期间运行,因此它在页面顶部给出了自己的模块. 

有关了解更多关于Guppy和贡献的更多信息,请参阅我们的[贡献文档](https://github.com/joshwcomeau/guppy/blob/master/CONTRIBUTING.md)

### 未来愿景

现在,Guppy的功能集非常有限. 它由3个模块组成: "开发服务器"窗格,"任务"窗格和"依赖关系"窗格. 

我希望看到的第一个重大变化是更好地支持常见的开发工具,如运行测试,linting,代码格式化等等. 一些潜在改进的例子: 

-   测试不应该只是列表中的一个细行,它应该有自己的模块,就像Dev Server那样. 它应该以"交互"模式运行,并允许用户通过单击按钮重新运行测试. 

-   依赖性应该易于更新. 我想象一个"更新核心依赖项"按钮,它可以通过内置的codemod支持来更新react,react-dom和任何相关的包. 我想它能够找到安全问题 (通过[`npm audit`](https://docs.npmjs.com/getting-started/running-a-security-audit)) . 

我还希望看到Guppy在教育用户关于Web开发方面变得更加有用. Guppy的理念是任何人都可以学习Web开发,它应该提供资源来帮助学习者. Guppy可以完全访问项目代码和设置,因此我想知道是否有机会为用户遇到的问题提出解决方案......我还没有任何具体的想法,但考虑一下这很有意思. 