# My typora theme

## 缘起

> 大约两年前第一次知道**Typora**这个使用Markdown语法书写笔记的软件。一年前开始真正使用 Typora，也正是这时才知道 Typora 可以通过更换主题改变笔记的排版样式，遂开始网罗各种**Typora主题**。一次逛知乎偶然地发现了@张晋大佬基于`urise polar`和`pie`修改的主题，这才发现原来也可以给自己定制主题啊，就想着自己也要写个 Typora 主题。
>
> 但无奈的是自己是一个渣渣，记得当时连为什么有些主题会带一个同名文件夹而有些主题只有一个`.css`文件都不知道，也看不太懂`.css`代码。这一年里因为写公众号推文需要用**Markdown Nice**而简单地学习了一些CSS语法，Typora也使用的更频繁了，所以写一个自己的 Typora 主题的想法又开始在心中萌发。
>
> 感谢前辈们提供的主题样式，让我可以在他们的主体框架下对样式进行修改。本主题主要基于**@张晋**的 Typora 主题和`urise polar`主题进行修改，并且也参考了其他的主题和部分的Markdown Nice主题，一并表示感谢。

## 主题安装

1. 打开 Typora，点击【文件】菜单，找到【偏好设置】。在偏好设置中点击【外观】，右侧页面点击【打开主题文件夹】，即弹出 Typora 的主题文件夹；
2. 下载本主题，并将主题下的`xiaoya.css`文件和`xiaoya`文件夹放到Typora 的主题文件夹下
3. 重新打开 Typora，即可在【主题】菜单下找到名为`xiaoya`的主题

## 主题介绍

### 主题色

目前该主题拥有两种主题色：**雅紫**和**月青**，默认主题色为雅紫。

如果你想使用月青作为主题色可以打开`xiaoya.css`文件，在`:root{}`找到**主题色月青**，将以下的颜色定义代码取消注释（大约是代码第31行到53行），并将**主题色雅紫**注释起来（大约是代码第6行到底28行）

#### 雅紫

![shadow](https://s2.loli.net/2022/01/25/xGrseiazKnNBuv9.png)

#### 月青

![shadow](https://s2.loli.net/2022/01/25/QNKVPTpbuDHy8Sc.png)

### 启动界面

参考`urise polar`主题，在打开空白`.md`文件Typora显示一张图片作为背景

![shadow](https://s2.loli.net/2022/01/24/n4McZTShwfELudi.png)

### 字体

>  主题的正文字体大小为16px，除以下特别的声明外主题的所有英文字体为HelveticaNeue，中文字体为苹方字体；
>
> 二三四五六级标题使用的英文字体为Times New Roman，中文字体为宋体；
>
> 引用的英文字体为HelveticaNeue，中文字体为楷体；
>
> 行内代码英文字体为lmmono10，中文字体为宋体；
>
> 代码块英文字体为Roboto Mono，中文字体为宋体；
>
> 链接字体为方正喵鸣体

## 效果展示

### 标题

![shadow](https://s2.loli.net/2022/01/25/t1Bq7G5H83Ulxed.png)

### 引用及列表

![shadow](https://s2.loli.net/2022/01/25/26jQwSJlAgZME1Y.png)

### 表格及任务列表

![shadow](https://s2.loli.net/2022/01/25/gYlienSLKp8vPOz.png)

### 文字样式代码块等

![shadow](https://s2.loli.net/2022/01/25/NQeKp6GyrPXtbzj.png)

### 公式

![shadow](https://s2.loli.net/2022/01/25/FVA9rs4nZpSIOkj.png)

### 图片

> 本主题提供三种图片样式

第一种是无任何装饰的普通图片

![](https://s2.loli.net/2022/01/25/sOaxFJpVoD6BjIM.png)

第二种是带有圆角和阴影的图片，使用方法是在`[ ]`中写入**shadow**，即`![shadow](url)`

![](https://s2.loli.net/2022/01/25/p7jteU9DVPGQIRF.png)

第三种是带有边框的图片，使用方法是在`[ ]`中写入**frame**，即`![frame](url)`

![](https://s2.loli.net/2022/01/25/EHY31Uc7n2tgOfR.png)

## 注

1. 我在css文件下放入了一段插入一张图片作为笔记页面背景的代码，如果想使用这个效果，可以在`#write{}`中取消以下代码的注释。

```css
#write {
    /* background-image: url("./xiaoya/Pio.png");
    background-repeat: no-repeat;
    background-size: 30%;
    background-position: 20% bottom;
    background-attachment: fixed;  */
  }
```

代码的位置大约在142行到146行，效果如下

![shadow](https://s2.loli.net/2022/01/25/sG9WSz1xjdQFyhl.png)

2. 月青主题色与雅紫主题色相比改变了一个引用样式

![shadow](https://s2.loli.net/2022/01/25/ecrGgpIA6RqjdWC.png)

如果想使用我定制好的月青引用样式请将大约第380行到第388行代码`blockquote {...}`注释起来，并将大约第391行到第409行代码`blockquote p:first-of-type::before{...} 及 blockquote {...}`取消注释

## 最后

如果你觉得来回切换**雅紫**和**月青**主题色太麻烦，我也分别给出了单主题的css文件。其中雅紫主题文件为`elegant-purple.css`，月青主题文件为`cyan-moon.css`。**xiaoya文件夹**是必要的，里面包含了字体背景图片等文件

---

## 更新

2022.01.18

- 构思主题样式，将主题命名为xiaoya，确定主题色为紫色，并将主题色命名为雅紫
- 确定主体文字大小为16px，中文字体使用苹方字体，英文字体使用Helvetica Neue

2022.01.21

- 完成层级标题及引用样式的css部分

2022.01.22

- 完成列表、表格、分割线、加粗、删除线、高亮、任务列表、脚注、行内代码、代码块、公式、链接、图片等样式的css部分
- 更改二级标题到六级标题的英文字体为Times New Roman，中文字体为宋体
- 更改引用块中文字体为楷体
- 更改行内代码中文字体为宋体，英文字体为lmmono 10
- 更改链接中文字体为方正喵鸣体

2022.01.23

- 增加当打开空白文件使用一张图片作为整个typora页面背景的效果
- 修改二级标题样式
- 调换三级标题与四级标题样式
- 主题css文件中加入一段页面图片背景代码（默认隐藏）
- 选用materials-ocean主题作为代码块高亮主题

2022.01.24

- 新增一套青色主题色，将主题色命名为月青
- 为月青主题色定制一个新的引用样式
- 微调月青主题色的三级标题

2022.01.25

- 修复目录中层级标题对齐的问题
- 加深月青主题色鼠标选中文本的颜色
- 将xiaoya主题中的雅紫主题色和月青主题色分离成独立的主题，雅紫主题文件名为elegant-purple，月青主题文件名为cyan-moon

