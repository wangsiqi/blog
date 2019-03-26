---
layout:     post
title:      Markdown基本语法
subtitle:   Markdown
date:       2019-03-25 16:28:26 +0800
author:     wangsiqi
header-img: img/post-bg-github-cup.jpg
catalog: true
tags:                              
    - Markdown
---

> <span style="font-size:18px">Markdown 是一个 Web 上使用的文本到HTML的转换工具，可以通过简单、易读易写的文本格式生成结构化的HTML文档。</span>

### 1、标题
 <span style="font-size:16px">Atx 形式则是在行首插入 1 到 6 个 # ，对应到标题 1 到 6 阶，例如：</span>

```
# 一级标题 H1
## 二级标题 H2
### 三级标题 H3
#### 四级标题 H4
##### 五级标题 H5
###### 六级标题 H6
```
 <span style="font-size:16px">效果如下：</span>
# 一级标题 H1
## 二级标题 H2
### 三级标题 H3
#### 四级标题 H4
##### 五级标题 H5
###### 六级标题 H6




### 2、分级标题
 <span style="font-size:16px">类 Setext 形式是用底线的形式，利用 = （最高阶标题）和 - （第二阶标题），例如：</span>
```

一级标题
===============================
二级标题
-------------------------------
```

 <span style="font-size:16px">效果如下：</span>

一级标题
================================

二级标题
-------------------------------


### 3.区块引用
<span style="font-size:16px">Markdown 标记区块引用是使用类似 email 中用 > 的引用方式</span>

```
/***第一种方式,每行都在最前面加上***/
> 宁愿做一朵篱下的野花，
> 不愿做一朵受恩惠的蔷薇。
> 与其逢迎献媚，
> 偷取别人的欢心，
> 毋宁被众人所鄙弃

/** 第二种方式，只在整个段落的第一行最前面加上 > **/
> 宁愿做一朵篱下的野花，
 不愿做一朵受恩惠的蔷薇。
 与其逢迎献媚，
 偷取别人的欢心，
 毋宁被众人所鄙弃

 /*** 第三种方式，区块引用可以嵌套（引用内的引用），只要根据层次加上不同数量的 > ***/

> 宁愿做一朵篱下的野花，
>> 不愿做一朵受恩惠的蔷薇。
>> 与其逢迎献媚，
> 偷取别人的欢心，
> 毋宁被众人所鄙弃
```

 <span style="font-size:16px">第一种方式和第二种方式效果一样：</span>

> 宁愿做一朵篱下的野花，
 不愿做一朵受恩惠的蔷薇。
 与其逢迎献媚，
 偷取别人的欢心，
 毋宁被众人所鄙弃

 <span style="font-size:16px">第三种方式效果如下：</span>

> 宁愿做一朵篱下的野花，
> 不愿做一朵受恩惠的蔷薇。
>> 与其逢迎献媚，
>> 偷取别人的欢心，
>> 毋宁被众人所鄙弃

### 4、列表
<span style="font-size:16px">Markdown 支持有序列表和无序列表。</span>
```
/***无序列表使用星号、加号或是减号作为列表标记,支持HTML无序列表代码***/

*   北京
*   上海
*   成都

+   北京
+   上海
+   成都

-   北京
-   上海
-   成都

<ul>
    <li>北京</li>
    <li>上海</li>
    <li>成都</li>
</ul>


/***有序列表则使用数字接着一个英文句点,支持HTML有序列表代码***/

1.  北京
2.  上海
3.  成都

<ol>
    <li>北京</li>
    <li>上海</li>
    <li>成都</li>
</ol>

```

<span style="font-size:16px">效果如下：</span>
<ul>
    <li>北京</li>
    <li>上海</li>
    <li>成都</li>
</ul>

<ol>
    <li>北京</li>
    <li>上海</li>
    <li>成都</li>
</ol>

### 4、代码区块
<span style="font-size:16px">和程序相关的写作或是标签语言原始码通常会有已经排版好的代码区块，通常这些区块我们并不希望它以一般段落文件的方式去排版，而是照原来的样子显示，Markdown 会用 `<pre>` 和 `<code>` 标签来把代码区块包起来。</span>

<span style="font-size:16px">只要简单地缩进 4 个空格或是 1 个制表符,或者把文本用 ` ``` ` 包裹起来。</span>

    /*** ```包裹 ***/
    ```
        <div>
            <div></div>
            <div></div>
            <div></div>
        </div>
    ```
    /*** 制表符 ***/
        <div>
            <div></div>
            <div></div>
            <div></div>
        </div>    

     /*** 4个空格 ***/    
        <div>
           <div></div>
            <div></div>
            <div></div>
        </div>

<span style="font-size:16px">效果如下:</span>

    <div>
        <div></div>
        <div></div>
        <div></div>
    </div>


### 5、分隔线
<span style="font-size:16px">你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线</span>

    * * *

    ***

    *****

    - - -

    ---------------------------------------
<span style="font-size:16px">效果如下:</span>
* * *

***

*****

- - -

---------------------------------------

### 6、链接
<span style="font-size:16px">Markdown支持两种形式的链接语法：行内式和参考试两种形式。</span>

    /***行内式***/

    [GitHub文本](http://github.com)



    /***参考试***/

    [1]:http://github.com
    [GitHub]:http://github.com

    [GitHub文本][1]      //下标为1的链接 文本为GitHub文本
    [GitHub文本][GitHub] //key为GitHub的链接 文本为GitHub文本



<span style="font-size:16px">行内式效果：</span>

[GitHub文本](http://github.com)

<span style="font-size:16px">参考试效果：</span>

[1]:http://github.com
[GitHub文本][1]

### 7、图片


```
/***行内式***/
![alt](url "title")

![小猪佩奇](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1553581173756&di=4c4d833fa1de4a9176b12b5a2fdb07c9&imgtype=0&src=http%3A%2F%2Fpic1.win4000.com%2Fpic%2F7%2Fd2%2Ff2c2a37a72.jpg "小猪佩奇")



/***参考式***/
![alt][key]
[key]: url "title"

![小猪佩奇][1]
[1]: https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1553581173756&di=4c4d833fa1de4a9176b12b5a2fdb07c9&imgtype=0&src=http%3A%2F%2Fpic1.win4000.com%2Fpic%2F7%2Fd2%2Ff2c2a37a72.jpg "小猪佩奇"

```

<span style="font-size:16px">行内式效果：</span>

![小猪佩奇](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1553581173756&di=4c4d833fa1de4a9176b12b5a2fdb07c9&imgtype=0&src=http%3A%2F%2Fpic1.win4000.com%2Fpic%2F7%2Fd2%2Ff2c2a37a72.jpg "小猪佩奇")


<span style="font-size:16px">参考试效果：</span>

![小猪佩奇][2]

[2]: https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1553581173756&di=4c4d833fa1de4a9176b12b5a2fdb07c9&imgtype=0&src=http%3A%2F%2Fpic1.win4000.com%2Fpic%2F7%2Fd2%2Ff2c2a37a72.jpg "小猪佩奇"
