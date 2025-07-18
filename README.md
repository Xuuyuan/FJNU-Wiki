# 福建师范大学 Wiki

[项目站点](https://fjnu.nekoark.com) 这份指南由福建师范大学贴吧吧务组及全体吧友共同完成。

欢迎浏览，欢迎 Star，欢迎贡献。万分感激。

## 参与协作

我们非常欢迎您为 **福建师范大学 Wiki** 编写内容，将自己在福师大的生活经验与大家分享。

[项目站点](https://fjnu.nekoark.com) 使用了 CDN。由于 CDN 的缓存机制，对站点页面做出的改动最迟在 24 小时后才会被同步到各 CDN 节点。若您急需进行相关页面的同步，可以联系 @Xuuyuan 进行刷新预热。

本项目基于 MkDocs 框架构建，您可以以以下方式参与协作：

### 在 GitHub 上编辑单个页面的内容

参与本 Wiki 的编写需要一个 GitHub 账号（可以前往 [GitHub 的账号注册页面](https://github.com/signup) 进行注册）。

1. 根据 Wiki 文档的链接路径，在 GitHub 项目中找到对应文件。
2. 点击页面右上方的 **【Fork this repository and edit the file】** 按钮，即可进入到编辑页面。若弹出 **【Fork this repository】** 的提示，点击继续即可。
3. 在编辑框内编写你想要修改的内容。在修改和接下来的提交过程中，请 **关闭您的自动翻译软件** ，否则可能产生不必要的麻烦。 **编辑页面内容时，请遵循 [Markdown 语法规范](https://markdown.com.cn/basic-syntax/)** ，否则可能出现页面排版问题。
4. 编写完成后点击右上角的 **【Commit changes...】** 按钮，按照下文中的 **Commit 规范** 填写 commit 信息，之后点击 **【Propose changes】** 按钮提交修改。点击后， GitHub 会跳转到你的分支仓库页面，此时页面右上方会显示一个绿色的 **【Create pull request】** 按钮，点击后 GitHub 会跳转到一个创建 Pull Request 页面。向下滚动检查自己所作出的修改没有错误后，按照下文中的 **Pull Request 信息格式规范** 规范书写 Pull Request 信息，然后点击页面上的绿色的 **【Create pull request】** 按钮创建 Pull Request。
5. 此时，你的 Pull Request 就顺利提交到仓库，等待管理员审核并合并到主仓库中即可。

### 使用 Git 在本地进行编辑

使用本方式进行编辑可能需要一定基础，但有利于在本地进行调试、预览（在本地配置 MkDocs 环境即可）。

- 将主仓库 Fork 到自己的仓库中；
- 将 Fork 后的分支仓库克隆（clone）到本地；
- 在本地进行修改后提交（commit）这些更改；
- 将这些更改推送（push）到你克隆的分支仓库；
- 提交 Pull Request 至主仓库。

## 对于目录和引用的变更

通常情况下，如果您需要添加一个新页面，或者修改已有页面在目录中的链接，您就需要对 mkdocs.yml 文件作出相应改动，参考原有的格式即可。

## Commit 信息格式规范

~~**事实上，我们提交 Commit 时也不一定遵守本规范。以简要的方式写明改动的内容即可。**~~

对于提交时需要填写的 commit 信息，请遵守以下几点基本要求：

1. commit 摘要请简要描述这一次 commit 改动的内容。注意 commit 摘要的长度不要超过 50 字符，超出的部分会自动置于正文中。
2. 如果需要进一步描述本次 commit 内容，请在正文中详细说明。

对于 commit 摘要，推荐按照如下格式书写：

```text
<修改类型>(<文件名>): <修改的内容>
```

修改类型分为如下几类：

- `feat`：用于添加内容的情况。
- `fix`：用于修正现有内容错误的情况。
- `refactor`：用于对一个页面进行重构（较大规模的更改）的情况。
- `revert`：用于回退之前更改的情况。

## Pull Request 信息格式规范

~~**事实上，我们提交 Pull Request 时也不一定遵守本规范。以简要的方式写明改动的内容即可。**~~

对于 Pull Request，请遵守以下几点要求：

1. 标题请写明本次 PR 的目的（做了 **什么** 工作，修复了 **什么** 问题）。
2. 内容请简要叙述修改的内容。

对于 Pull Request 的标题，推荐使用如下格式书写：

```plain
<修改类型>(<文件名>): <修改的内容> (<对应 issue 的编号>)
```

修改类型分为如下几类：

- `feat`：用于添加内容的情况。
- `fix`：用于修正现有内容错误的情况。
- `refactor`：用于对一个页面进行重构（较大规模的更改）的情况。
- `revert`：用于回退之前更改的情况。

示例：

- `fix(ds/persistent-seg): 修改代码注释使描述更清晰`
- `fix: tools/judger/index 不在目录中 (#3709)`
- `feat(math/poly/fft): better proof`
- `refactor(ds/stack): 整理页面内容`

## markdown 样式

建议使用 [markdownlint](https://github.com/DavidAnson/markdownlint) 之类的静态检查器对文档进行语法检查，以确保内容被正确解析。

建议中英文混排时添加空格以增加可读性。其余样式可参考该 [指南](https://github.com/sparanoid/chinese-copywriting-guidelines)

## 图片样式

在 markdown 中插入图片的格式为：

```
![标签文字](图片URL或路径)
```

如有图片插入需求，则在对应目录底下新建 `pics` 文件夹，用于存放对应的图片，图片标签文字则自行起对应标题，图片命名为 `对应引用的md文件名-图x-图片标签` x为对应的图片编号，例如 `![升学去向图](./pics/sociology_and_history-图1.jpg)` 如此格式。

