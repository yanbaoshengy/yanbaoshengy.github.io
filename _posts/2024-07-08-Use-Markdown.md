layout: post
title: 使用Markdown语法编写博客内容
date: 2024-07-08
Author: 阎子君
categories: Markdown
tags: [Github, Markdown]
comments: true
--- 

<!-- more -->

**Markdown是一种轻量级标记语言，排版语法简洁，让人们更多地关注内容本身而非排版。它使用易读易写的纯文本格式编写文档，可与HTML混编，可导出 HTML、PDF 以及本身的 .md 格式的文件。**

## Markdown 文章开头（适用于本人发布个人博客）

	---
	layout: post
	title: 使用Markdown语法编写博客内容
	date: 2024-07-08
	Author: 阎子君
	categories: Markdown
	tags: [Github, Markdown]
	comments: true
	---

## Markdown 标题语法

# 一级标题

    # 一级标题

## 二级标题

    ## 二级标题

### 三级标题

    ### 三级标题

一级标题
===============

    在文本下方添加任意数量的 == 号来标识一级标题

二级标题
---------------

	在文本下方添加任意数量的 -- 号来标识二级标题

**注意：不同的 Markdown 应用程序处理 # 和标题之间的空格方式并不一致。为了兼容考虑，请用一个空格在 # 和标题之间进行分隔。**

	# Here's a Heading  正确
	#Here's a Heading   错误




## Markdown 段落语法

**要创建段落，请使用空白行将一行或多行文本进行分隔。**

	例如下：
	I really like using Markdown.
	使用空白行将一行或多行文本进行分隔
	I think I'll use it to format all of my documents from now on.
	效果如下：

I really like using Markdown.

I think I'll use it to format all of my documents from now on.

**注意：不要用空格（spaces）或制表符（ tabs）缩进段落。**

## Markdown 换行语法

**在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行。**

	例如下：
	This is the first line.  
	And this is the second line.
	效果如下：

This is the first line.   
And this is the second line.

## Markdown 强调语法 

**通过将文本设置为粗体或斜体来强调其重要性。**

### 粗体

	要加粗文本，请在单词或短语的前后各添加两个星号（asterisks）或下划线（underscores）。如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号（asterisks）。

I just love **bold text**.

	I just love **bold text**.

I just love __bold text__.

	I just love __bold text__.

Love**is**bold

	Love**is**bold

### 斜体

	要用斜体显示文本，请在单词或短语前后添加一个星号（asterisk）或下划线（underscore）。要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不要带空格。

Italicized text is the *cat's meow*.

	Italicized text is the *cat's meow*.

Italicized text is the _cat's meow_.

	Italicized text is the _cat's meow_.

A*cat*meow

	A*cat*meow

### 粗体和斜体

	要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加三个星号或下划线。要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个星号，中间不要带空格。

This text is ***really important***.

	This text is ***really important***.

This text is ___really important___.

	This text is ___really important___.

This text is __*really important*__.

	This text is __*really important*__.

This text is **_really important_**.

	This text is **_really important_**.

This is really***very***important text.

	This is really***very***important text.

## Markdown 引用语法

**要创建块引用，请在段落前添加一个  >  符号。**

	> Dorothy followed her through many of the beautiful rooms in her castle.

> Dorothy followed her through many of the beautiful rooms in her castle.

### 多个段落的块引用

**块引用可以包含多个段落。为段落之间的空白行添加一个  >  符号。**

	> Dorothy followed her through many of the beautiful rooms in her castle.
	>
	> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 嵌套块引用

**块引用可以嵌套。在要嵌套的段落前添加一个 >> 符号。**

	> Dorothy followed her through many of the beautiful rooms in her castle.
	>
	>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 带有其它元素的块引用

**块引用可以包含其他 Markdown 格式的元素。并非所有元素都可以使用，你需要进行实验以查看哪些元素有效。**

	> #### The quarterly results look great!
	>
	> - Revenue was off the chart.
	> - Profits were higher than ever.
	>
	>  *Everything* is going according to **plan**.

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

## Markdown 列表语法

### 有序列表

**要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。**

	1. First item
	2. Second item
	3. Third item
	4. Fourth item
	或
	1. First item
	1. Second item
	1. Third item
	1. Fourth item
	或
	1. First item
	8. Second item
	3. Third item
	5. Fourth item
	输出效果都为：

1. First item
2. Second item
3. Third item
4. Fourth item

**嵌套使用**

	1. First item
	2. Second item
	3. Third item
		1. Indented item
		2. Indented item
	4. Fourth item

1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item

### 无序列表

**要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。**

    - First item
    - Second item
    - Third item
    - Fourth item
    或
    * First item
    * Second item
    * Third item
    * Fourth item
    或
    + First item
    + Second item
    + Third item
    + Fourth item
    输出效果都为

- First item
- Second item
- Third item
- Fourth item

**嵌套使用**

    - First item
    - Second item
    - Third item
        - Indented item
        - Indented item
    - Fourth item

- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item

### 在列表中嵌套其他元素

**要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：**

**段落**

    *   This is the first list item.
    *   Here's the second list item.
    
        I need to add another paragraph below the second list item.
    
    *   And here's the third list item.

*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.

**引用块**

    *   This is the first list item.
    *   Here's the second list item.
    
        > A blockquote would look great below the second list item.
    
    *   And here's the third list item.

*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great below the second list item.

*   And here's the third list item.

**代码块**

**代码块通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。**

    1.  Open the file.
    2.  Find the following code block on line 21:
    
            &lt;html>
              &lt;head>
                &lt;title>Test&lt;/title>
              &lt;/head>
    
    3.  Update the title to match the name of your website.

1.  Open the file.
2.  Find the following code block on line 21:

        &lt;html>
          &lt;head>
            &lt;title>Test&lt;/title>
          &lt;/head>

3.  Update the title to match the name of your website.

**图片**

    1.  Open the file containing the Linux mascot.
    2.  Marvel at its beauty.
    
        ![China-Number-1, the Linux mascot](images/China-Number-1.png)
    
    3.  Close the file.

1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

     ![China-Number-1, the Linux mascot](images/China/中华人民共和国国旗.png)

3.  Close the file.

**列表**

    1. First item
    2. Second item
    3. Third item
        - Indented item
        - Indented item
    4. Fourth item

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item

## Markdown 代码语法

**要将单词或短语表示为代码，请将其包裹在反引号 (`) 中。**

	At the command prompt, type `nano`.

At the command prompt, type `nano`.

**如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(``)中。**

	``Use `code` in your Markdown file.``

``Use `code` in your Markdown file.``

**要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。**

        &lt;html>
          &lt;head>
          &lt;/head>
        &lt;/html>
    
    &lt;html>
      &lt;head>
      &lt;/head>
    &lt;/html>

## Markdown 分隔线语法

	要创建分隔线，请在单独一行上使用三个或多个星号 (***)、破折号 (---) 或下划线 (___) ，并且不能包含其他内容。
	
	***
	
	---
	
	_________________

***

---

_________________

**为了兼容性，请在分隔线的前后均添加空白行。**

## Markdown 链接语法

    [超链接显示名](超链接地址 "超链接title")
    例如：
    [google](http://google.com/ "Google")

效果：
[google](http://google.com/ "Google")

**网址和Email地址**

    <地址>
    例如：
    <http://google.com/>
    <fake@example.com>

效果：
<http://google.com/>

<yanzijun@zijun.com>

**带格式化的链接 **

	强调 链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号。
	
	I love supporting the **[EFF](https://eff.org)**.
	This is the *[Markdown Guide](https://www.markdownguide.org)*.
	See the section on [`code`](#code).

I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).

## Markdown 图片语法

	要添加图像，请使用感叹号 (!), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。
	
	![替代文字](图片url "图片说明")
	<img src="/images/.../xxx.jpg(或png)"/>

### 链接图片

	给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。
	
	[![沙漠中的岩石图片](/assets/img/shiprock.jpg "Shiprock")](https://markdown.com.cn)


## Markdown 转义字符语法

	要显示原本用于格式化 Markdown 文档的字符，请在字符前面添加反斜杠字符 \ 。
	如果需要使用以上标记字符而不被Markdown理解为格式标记，需要用\转义：例如\\，效果为\。
	
	\* Without the backslash, this would be a bullet in an unordered list.

\* Without the backslash, this would be a bullet in an unordered list.

