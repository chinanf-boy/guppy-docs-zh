
# 特约

感谢您对Guppy的兴趣!我们对社区的任何贡献表示欢迎和感激. 我们希望Guppy成为一项社区活动,我们所有人共同努力,让那些没有终端经验的人们更容易进行网页开发!

## 报告问题和提出问题

在打开问题之前,请搜索[问题跟踪器](https://github.com/joshwcomeau/guppy/issues)确保您的问题尚未报告. 

### 错误和改进

*Guppy是alpha软件*,你可能会遇到一些问题. 

我们使用问题跟踪器来跟踪Guppy本身,其示例和文档的错误和改进. 我们鼓励您打开讨论改进,架构,理论,内部实施等问题. 如果之前讨论过某个主题,我们将要求您加入之前的讨论. 

## 发展

访问[问题跟踪器](https://github.com/joshwcomeau/guppy/issues)找到需要注意的未决问题列表. 贡献的最佳方式是找到你能够并且愿意解决的问题. 随着项目的成熟,我们希望为更新的React开发人员添加更多"良好的第一贡献"问题. 

叉,然后克隆回购: 

    git clone https://github.com/your-username/guppy.git

### 运行

#### 地方发展

您可以通过运行本地开始本地开发`start`任务: 

    npm run start

这应该打开一个运行应用程序的Electron窗口. 

在开发过程中,所有项目都是在`~/guppy-projects-dev`

您可以运行以下命令来构建MacOS可执行文件: 

    npm run package

结果将在`release-builds`夹. 

### 测试和类型检查

不幸的是,很少有Guppy目前正在测试. 

我们希望在此期间添加更多测试,以及添加CI集成以在push上运行测试,但是现在您可以使用以下命令运行测试: 

    npm run test

该项目使用Flow,可以使用以下方法检查类型: 

    npm run flow

这个项目使用Prettier,这应该在提交时自动运行. 

### 文件

请在项目中了解更多关于Guppy的信息[自述](https://github.com/joshwcomeau/guppy/blob/master/README.md),或位于[/文档](https://github.com/joshwcomeau/guppy/tree/master/docs)目录. 

### 发送拉取请求

对于非平凡的更改,请在开始工作之前打开有关新功能或重构的提案的问题,或对现有的请求功能问题发表评论. 我们不希望您在我们不想接受的拉动请求上浪费您的努力. 

另一方面,有时是开始对话的最佳方式*是*发送拉取请求. 用你最好的判断!

通常,贡献工作流程如下所示: 

-   在中找到或打开一个新问题[问题跟踪器](https://github.com/joshwcomeau/guppy/issues). 
-   回购利用. 
-   基于的创建一个新的功能分支`master`科. 
-   确保所有测试都通过
-   提交拉取请求,引用它解决的任何问题. 

请尽量将拉取请求集中在范围内,避免包含不相关的提交. 

在您提交了拉取请求后,我们会尽快回复您. 我们可能会建议一些变化或改进. 

谢谢你的贡献!
