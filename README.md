
## frontend-guidelines
> [前端开发环境的搭建，以及好用的开发工具的整理](https://cnyet.github.io/frontend-guidelines/)

#### 前言
&emsp;&emsp;每当我们进入一家新的公司或者换了新电脑，作为前端开发的我们，一定都会经历搭建开发环境，安装各种软件和工具等等诸如此类的预备工作，或许你还要面临各种软件的破解，解决软件升级后各种报错问题。还有些时候，我们可能还会遇到，之前用过一个很好的工具但是不记得叫什么名字或忘记在哪下载的了。麻烦的人类……<br>
&emsp;&emsp;对于要在一台新电脑上安装一套自己满意的开发环境，又没有完整的清单的你，继续往下看或许能帮到你。我在此整理了一套清单，一方面自己备份，一方面供同行们参考。
#### 安装开发工具和各种插件

##### IDE编辑器
> 推荐[WebStorm](https://www.jetbrains.com/webstorm/)和[Sublime Text](https://www.sublimetext.com/) ，[Atom](https://atom.io/)也很不错，界面风格挺清爽。

- **WebStorm** 我之前一直在用。我觉得如果你需要快速开发项目，或者嫌编辑器配置麻烦，那么推荐WebStorm。它集成很多丰富的功能，包括代码自动补全，鼠标悬停显示变量出处，命令行操作，提供本地静态页面http访问等等，几乎涵盖了你需要的所有功能。但正因此编辑器会经常卡死，崩溃，响应慢。由于它是收费软件需要破解，而且还经常崩溃，后来我才转战sublime。
1. 这里我贴一个[WebStorm2016 1.3版本的破解](http://www.jianshu.com/p/c5f7ab33add0)教程；
2. webstorm所有的快捷键都可以在<kbd>File->Settings->Keymap</kbd>里面查看；
3. 在<kbd>File->Settings->plugins</kbd>安装插件。如：让WebStorm支持Markdown格式，我们搜索“markdown support”点击安装插件，重启WebStorm即可。值得一提是，WebStorm的Markdown自带预览功能很好用。
4.  还有两个好用的功能是sublime上面没有的，一个是右键点击项目根目录选择<kbd>Local History->Show History</kbd>可以查看项目修改的历史情况，可以返回修改历史上的节点哦，另一个是，右键点击单个文件选择<kbd>Compare With</kbd>，在弹窗里选择一个不同版本的同一个文件，可以进行对比对比，向左合并或向右合并。这个太强大了，直接省去了再装一个[Beyond Compare](http://www.beyondcompare.cc/xiazai.html)软件。
5.  如果项目是协作开发并且用git做版本控制了，还有个更牛B的功能，在文件编辑区域右键点击行号，选择<kbd>Annotate</kbd>可以看到此处是谁写的代码，你写了bug，躲也躲不掉。哈哈……
6.  当然你辛苦设置好WebStorm配置可以在本地查看，windows系统默认放置<kbd>C:\Users\admin\.WebStorm2016.1</kbd>，你可以拷贝到其他电脑上继续使用。记住千万不要用特殊手段关闭WebStorm，比如：关闭进程，突然断电导致电脑关机都可能导致webstorm异常不能启动。

- **Sublime** 界面非常简洁，是一个轻量级而功能强大的编辑器。它也是收费软件，但是相比WebStorm要好破解一些。[sublime破解](http://www.jianshu.com/p/04e1b65dd2c0)，根据你安装的插件sublime才变得功能更加丰富。在安装各种插件之前你需要先装插件管理器[Package Control](https://packagecontrol.io/installation)
**安装插件：** Ctrl+Shift+P，输入install，等待几秒后出现插件列表，输插件名再回车就能自动安装。
**删除插件：** Ctrl+Shift+P，输入remove package，选择插件再回车。
我本地安装的插件列表：
> AdvancedNewFile————快速新建文件
> Alignment————用于代码对齐
> AutoFileName————自动补全文件(目录)名
> Better Less————格式化less文件
> Compare Side-By-Side————Sublime版本的BeyongCompare
> DocBlockr————代码块注释
> Emmet————快速编写HTML和CSS代码，默认快捷键 Tab
> Git————集成git管理功能
> Gitignore————一键生成git忽略文件模板
> jQuery————快速生成jquery代码块
> JsFormat————JavaScript代码格式化
> JSON Key-Value————json代码高亮显示
> LESS————高亮显示less语句
> MarkdownEditing————编写的 markdown文件
> Package Control————插件管理器
> PackageResourceViewer———在浏览器中预览markdown文件
> Theme - Soda————[soda主题](http://buymeasoda.github.io/soda-theme/)
> HTML-CSS-JS Prettify————快速格式化html,css,js文件
> 另外两款精美的主题：[Material](http://equinsuocha.io/material-theme/#/default)和[Seti_UI](https://packagecontrol.io/packages/Seti_UI)（我正在用）


