### IDE编辑器
> 推荐[WebStorm](https://www.jetbrains.com/webstorm/)和[Sublime Text](https://www.sublimetext.com/)

### WebStorm
&emsp;&emsp;我之前一直在用。我觉得如果你需要快速开发项目，或者嫌编辑器配置麻烦，那么推荐WebStorm。它集成很多丰富的功能，包括代码自动补全，鼠标悬停显示变量出处，命令行操作，提供本地静态页面http访问等等，几乎涵盖了你需要的所有功能。但正因此编辑器会经常卡死，崩溃，响应慢。由于它是收费软件需要破解，而且还经常崩溃，后来我才转战sublime。

- 这里我贴一个[WebStorm2016 1.3版本的破解](http://www.jianshu.com/p/c5f7ab33add0)教程；
- webstorm所有的快捷键都可以在<kbd>File->Settings->Keymap</kbd>里面查看；
- 在<kbd>File->Settings->plugins</kbd>安装插件。如：让WebStorm支持Markdown格式，我们搜索“markdown support”点击安装插件，重启WebStorm即可。值得一提是，WebStorm的Markdown自带预览功能很好用。
- 还有两个好用的功能是sublime上面没有的，一个是右键点击项目根目录选择<kbd>Local History->Show History</kbd>可以查看项目修改的历史情况，可以返回修改历史上的节点哦，另一个是，右键点击单个文件选择<kbd>Compare With</kbd>，在弹窗里选择一个不同版本的同一个文件，可以进行对比对比，向左合并或向右合并。这个太强大了，直接省去了再装一个[Beyond Compare](http://www.beyondcompare.cc/xiazai.html)软件。
- 如果项目是协作开发并且用git做版本控制了，还有个更牛B的功能，在文件编辑区域右键点击行号，选择<kbd>Annotate</kbd>可以看到此处是谁写的代码，你写了bug，躲也躲不掉。哈哈……
- 当然你辛苦设置好WebStorm配置可以在本地查看，windows系统默认放置<kbd>C:\Users\admin\.WebStorm2016.1</kbd>，你可以拷贝到其他电脑上继续使用。记住千万不要用特殊手段关闭WebStorm，比如：关闭进程，突然断电导致电脑关机都可能导致webstorm异常不能启动。
#### WebStorm 相关
- [官网](https://www.jetbrains.com/webstorm/)
- [WebStorm主题](http://www.webstormthemes.com/)
- [IDEA系列主题](http://www.riaway.com/)
- [WebStorm插件](https://plugins.jetbrains.com/webstorm)
- [webstorm 入门指南](http://book.apebook.org/minghe/webstorm/index.html)
- [webstorm快捷键](http://www.jianshu.com/p/7229aff1ae74)

### Sublime Text
&emsp;&emsp;界面非常简洁，是一个轻量级而功能强大的编辑器。它也是收费软件，但是相比WebStorm要好破解一些。[sublime破解](http://www.jianshu.com/p/04e1b65dd2c0)，根据你安装的插件sublime才变得功能更加丰富。在安装各种插件之前你需要先装插件管理器[Package Control](https://packagecontrol.io/installation)

- **安装插件：**Ctrl+Shift+P，输入install，等待几秒后出现插件列表，输插件名再回车就能自动安装。
我本地安装的插件列表：
> A File Icon————好看的文件图标
> AdvancedNewFile————快速新建文件<br>
> Alignment————用于代码对齐<br>
> AutoFileName————自动补全文件(目录)名<br>
> Better Less————格式化less文件<br>
> Compare Side-By-Side————Sublime版本的BeyongCompare<br>
> DocBlockr————代码块注释<br>
> Emmet————快速编写HTML和CSS代码，默认快捷键 Tab<br>
> Git————集成git管理功能<br>
> WakaTime————第三方可视化监控平台，可统计操作sublime的各种数据
> Gitignore————一键生成git忽略文件模板<br>
> jQuery————快速生成jquery代码块<br>
> JsFormat————JavaScript代码格式化<br>
> JSON Key-Value————json代码高亮显示<br>
> LESS————高亮显示less语句<br>
> MarkdownEditing————编写的 markdown文件<br>
> Package Control————插件管理器<br>
> PackageResourceViewer———在浏览器中预览markdown文件<br>
> Theme - Soda————[soda主题](http://buymeasoda.github.io/soda-theme/)<br>
> HTML-CSS-JS Prettify————快速格式化html,css,js文件<br>
> 另外几款精美的主题：[Material](http://equinsuocha.io/material-theme/#/default)，[Seti_UI](https://packagecontrol.io/packages/Seti_UI)，[Boxy Theme](https://packagecontrol.io/packages/Boxy%20Theme)（插件不是越多越好哦，装多了快捷键就会重合，反而不方便）
- **删除插件：** Ctrl+Shift+P，输入remove package，选择插件再回车。
- **调用插件：** 先调出执行面板Ctrl+Shift+P，输入关键字，如：输入git，会出现git相关的操作命令
- **基本设置：**
```
{
    //关闭自动保存
    "atomic_save": false,
    //颜色主题
    "color_scheme": "Packages/Color Scheme - Default/Solarized (Dark).tmTheme",
    //字体设置
    "font_face": "YaHei Consolas Hybrid",  
    //字号大小  
    "font_size": 14,
    //打开当前行背景颜色
    "highlight_line": true,
    //禁用vi模式编辑包
    "ignored_packages":
    [
        "Vintage"
    ],
    //显示行号右侧的代码段闭合展开三角号
    "fade_fold_buttons": false,
    //使用 unix 风格的换行符
    "default_line_ending": "unix",
    // 侧边栏文件夹显示加粗，区别于文件
    "bold_folder_labels": true,
    //显示滚动条
    "overlay_scroll_bars": "enabled",
    //当前页失去焦点自动保存
    "save_on_focus_lost": true,
    // Tab转空格
    "translate_tabs_to_spaces": true,
    // 自动换行
    "word_wrap": true,
    //主题风格
    "theme": "Material-Theme.sublime-theme"(或"Seti.sublime-theme")
}
```

#### Sublime相关
- [官网](https://www.sublimetext.com/)
- [扩展管理器](https://packagecontrol.io/)
- [Sublime主题](https://juejin.im/entry/599a1bed6fb9a0248070d4b1)
- [Sublime设置](https://www.jeffjade.com/2015/12/15/2015-04-17-toss-sublime-text/)
- [Sublime快捷键](http://jinfang.life/posts/e4aa08c5/)