---
title: "learn markdown"
date: 2019-08-29T15:47:30
categories:
  - blog
tags:
  - learn
  - update
---
# 总结
markdown特别方便，很快捷，以后会经常使用，但是有这么几个问题：
1. 链接有问题，如果直接使用`<http://wwww.***.com>`，会出不了链接，并且，影响整个页面的布局；所以，推荐使用`[链接名称](链接地址) `，比如[菜鸟教程](https://www.runoob.com)；还有一些html标签，也需要放在``里面，才能保证页面解析不出错；
2. 使用`$$ latex公式 $$`，在PC端解析不出来，在某些特定的markdown网站 [mdeditor](https://www.mdeditor.com/)才可以解析出来；
3. 写markdown时，空格，很重要；经常是空格搭配特定格式/字符，才能生效；
4. 流程图的解析也有问题，等用到的时候再去研究。


# 1、Markdown标题

###### 六级标题
##### 五级标题
#### 四级标题
### 三级标题
## 二级标题
# 一级标题

# 2、Markdown段落
### 换行
Markdown 段落没有特殊的格式，直接编写文字就好，段落的换行是使用两个以上空格加上回车。  
(上面就是使用`两个空格+回车`进行换行的)当然也可以在段落后面使用一个空行来表示重新开始一个段落。

上面就是使用了`一个空行`，来进行换行的。

### 字体
*斜体文本*
_斜体文本_
**粗体文本**  
__粗体文本__
***粗斜体文本***
___粗斜体文本___

上标：X<sub>2</sub>，下标：O<sup>2</sup>

### 分割线
你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：
***
* * *
*****
- - -
----------
### 删除线
如果段落上的文字要添加删除线，只需要在文字的两端加上两个波浪线 ~~ 即可，实例如下：  
baiyunfei429  
~~baiyunfei429~~

### 下划线
下划线可以通过 HTML 的 `<u>` 标签来实现：  
<u>带下划线文本</u>

### 脚注
脚注是对文本的补充说明。
Markdown 脚注的格式如下:  
[^要注明的文本]  

创建脚注格式类似这样 [^RUNOOB]。  
[^RUNOOB]: 菜鸟教程 -- 学的不仅是技术，更是梦想！！！


# 3、Markdown列表
Markdown 支持有序列表和无序列表。  
无序列表使用星号(*)、加号(+)或是减号(-)作为列表标记：  
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项

有序列表使用数字并加上 . 号(PS:.后面有个一个空格)来表示，如：
1. 第一项
2. 第二项
3. 第三项

列表嵌套,只需在子列表中的选项添加`四个空格`即可：

1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第一个元素

# 4、Markdown区块
Markdown 区块引用是在段落开头使用 > 符号 ，然后后面紧跟一个空格符号：

> 区块引用  
> 菜鸟教程  
> 学的不仅是技术更是梦想

另外，区块是可以嵌套的，一个 > 符号是最外层，两个 > 符号是第一层嵌套，以此类推退：

> 最外层
> > 第一层嵌套
> > > 第二层嵌套

区块中使用列表,实例如下：

> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项

列表中使用区块
如果要在列表项目内放进区块，那么就需要在 > 前添加四个空格的缩进。实例如下：

* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
* 第二项


#### GFM task list
3-1，3-2，3-3，4-1，4-2都加了4个空格，仍在没有变成子选项，额。。。。感觉也有问题
- [x] GFM task list 1
- [x] GFM task list 2
- [ ] GFM task list 3
    - [ ] GFM task list 3-1
    - [ ] GFM task list 3-2
    - [ ] GFM task list 3-3
- [ ] GFM task list 4
    - [ ] GFM task list 4-1
    - [ ] GFM task list 4-2

- [x] todo1  
- [ ] todo2  
- [ ] todo3  

# 5、Markdown代码
如果是段落上的一个函数或片段的代码可以用反引号把它包起来（`），例如：

`printf()` 函数

代码区块
代码区块使用 4 个空格或者一个制表符（Tab 键）。

实例如下：  
  
    $(document).ready(function () {
        alert('RUNOOB');
    });

也可以用 ``` 包裹一段代码，并指定一种语言（也可以不指定)示例如下:


```javascript
$(document).ready(function () {
    alert('RUNOOB');
});

var a = 1, b = 1;
var sum = a + b;
console.log(sum);
```

# 6、Markdown链接
链接使用方法如下：

[链接名称](链接地址)  
或者  
`<链接地址>`(这种方式，貌似不怎么好使，在PC端显示有问题，而且影响其他的显示)

这是一个链接 [菜鸟教程](https://www.runoob.com)  
直接使用链接地址: 
`<https://www.runoob.com>`

### 高级链接  
链接也可以用变量来代替，文档末尾附带变量地址：    
这个链接用 1 作为网址变量 [Google][1]    
这个链接用 runoob 作为网址变量 [Runoob][runoob]    
然后在文档的结尾为变量赋值（网址）  

  [1]: http://www.google.com/
  [runoob]: http://www.runoob.com/

# 7、Markdown图片
Markdown 图片语法格式如下：

![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")
开头一个感叹号 !  
接着一个方括号，里面放上图片的替代文字  
接着一个普通括号，里面放上图片的网址，  
最后还可以用引号包住并加上选择性的 'title' 属性的文字。

使用实例：

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")

当然，你也可以像网址那样对图片网址使用变量:

这个链接用 2 作为网址变量 [RUNOOB][2].
然后在文档的结尾位变量赋值（网址）

[2]: http://static.runoob.com/images/runoob-logo.png

Markdown 还没有办法指定图片的高度与宽度，如果你需要的话，你可以使用普通的 `<img>` 标签。

<img src="http://static.runoob.com/images/runoob-logo.png" width="50%">

# 8、Markdown 表格
Markdown 制作表格使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。

语法格式如下：
(而且，表格的显示，怪怪的，不好看)
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |

对齐方式

我们可以设置表格的对齐方式：

-: 设置内容和标题栏居右对齐。  
:- 设置内容和标题栏居左对齐。  
:-: 设置内容和标题栏居中对齐。  
实例如下：

| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |


# 9、Markdown 高级技巧
### 支持的 HTML 元素
不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。

目前支持的 HTML 元素有：`<kbd> <b> <i> <em> <sup> <sub> <br>`等 ，如：

使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑

### 转义
Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符：

**文本加粗** 
\*\* 正常显示星号 \*\*

Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：  
\   反斜线  `   反引号  *   星号  _   下划线  {}  花括号  []  方括号  
()  小括号  #   井字号  +   加号  -   减号  .   英文句点  !   感叹号

### 公式
当你需要在编辑器中插入数学公式时，可以使用两个美元符 $$ 包裹 TeX 或 LaTeX 格式的数学公式来实现。提交后，问答和文章页会根据需要加载 Mathjax 对数学公式进行渲染。如：

$$  
\begin{array}
\overline{a+b+c} \\
\underline{a+b+c} \\
\overleftarrow{a+b} \\
\underleftarrow{a+b} \\
\underleftrightarrow{a+b} \\
\vec x = \vec{AB} \\
\overbrace {a+b}^\text{a,b} \\
a+\rlap{\overbrace{\phantom{b+c+d}}^m}b+\underbrace{c+d+e}_n+f
\end{array}  
$$ 

\\[
(a+b) \times c = a\times c + b \times c \\
\\]

但是，没有把latex公式解析。。。。。额

