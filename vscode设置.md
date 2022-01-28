# 编程萌新必备VSCode入门指南
> 课程内容来自B站 慕课网官方账号  
> (慕课网<https://www.imooc.com>)  
> <https://www.bilibili.com/video/BV1hw41197Ms?p=5>

## 快捷键

* CTRL + c 复制 
* CTRL + v 粘贴
* CTRL + x 剪切
* CTRL + f 查找
* CTRL + h 替换
* CTRL + / 行注释
* shift + alt + a 块注释
* CTRL + shift + enter 上方插入一行
> 上方插入一行 在我的`vscode`里的`markdown`中不管用
* CTRL + shift + f 文件夹查找
* CTRL + enter 下方插入一行
* shift + alt + f 格式化代码

## `git`是什么

* `git` 是一个开源发分布式版本控制系统
* 可以有效、高速地处理很小到非常大的项目版本管理

### git工作流

![git工作流](Screenshot/2022-01-14-16-50-05.png)

* `workspace` 正常电脑的工作区
:   直接进行标记的代码
* `repository` 本地仓库
:   本地的提交
* `remote` 远程仓库
:   盛放最终代码

1. 先要pull代码
2. 从远程仓库clone
3. 进行检出checkout
4. 本地编写代码，先添加add
5. 再提交commit
6. 没问题后push到远程仓库

### `git`下载与安装

+ 搜索git或访问<https://git-scm.com/>下载安装

### 注册`GitHub`

+ `github`是一个面向开源及私有软件项目的托管平台

# markdown中不常用操作 {#index}

## 注脚

使用 Markdown[^1]可以效率的书写文档, 直接转换成 HTML[^2]

## 超链接

### 行内式

语法说明：

- []里写链接文字,()里写链接地址, ()中的""中可以为链接指定title属性，title属性可加可不加。   
- title属性的效果是鼠标悬停在链接上会出现指定的 title文字,链接地址与title前有一个空格。

代码：
~~~
欢迎阅读 [择势勤](https://www.jianshu.com/u/16d77399d3a7 "择势勤")
~~~

显示效果：

欢迎阅读 [择势勤](https://www.jianshu.com/u/16d77399d3a7 "择势勤")

### 参考式

> 参考式超链接一般用在学术论文上面，或者另一种情况，如果某一个链接在文章中多处使用，那么使用引用 的方式创建链接将非常好，它可以让你对链接进行统一的管理。

语法说明：

- 参考式链接分为两部分
    1. 文中的写法 [链接文字][链接标记] 
    2. 在文本的任意位置添加[链接标记]:链接地址。
    

- 如果链接文字本身可以做为链接标记，你也可以写成[链接文字][]
[链接文字]：链接地址的形式，见代码的最后一行。

代码：
~~~
我经常去的几个网站[Google][1]、[Leanote][2]。
[1]:http://www.google.com 
[2]:http://www.leanote.com
~~~
显示效果： 

我经常去的几个网站[Google][1]、[Leanote][2]。  

[1]:http://www.google.com 
[2]:http://www.leanote.com

### 锚点（页内超链接）
> 网页中，锚点其实就是页内超链接，也就是链接本文档内部的某些元素，实现当前页面中的跳转。

比如我这里写下一个锚点，点击回到目录，就能跳转到目录。 在目录中点击这一节，就能跳过来。还有下一节的注脚。这些根本上都是用锚点来实现的.**只支持在标题后插入锚点，其它地方无效。**

代码：

~~~
 # 2markdown中不常用的操作 {#index}
 文本
 文本
跳转到[markdown中不常用的操作](#index)
~~~

显示效果： 

跳转到[markdown中不常用的操作](#index)












[^1]:Markdown是一种纯文本标记语言

[^2]:HyperText Markup Language 超文本标记语言