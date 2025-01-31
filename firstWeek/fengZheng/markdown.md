# markdowan基础学习篇
## 1.标题
在下一行使用“=”可标记上一行为一级标题；使用“-”可标记上一行为二级标题；在段落前加上1-6个“#”并空格，可标记该行为1-6级标题。

## 2.段落
1.在段落末尾添加“两个空格”并回车，可实现段落换行；  
2.在两个段落中间空一行，也可实现分段；

3.如上。

### 2.1 字体
可使用的字体如下：  
*斜体文本*  
_斜体文本_  
**粗体文本**  
__粗体文本__  
***粗斜体文本***  
___粗斜体文本___  

### 2.2 分割线
可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：  
***

* * *

*****

- - -

----------

### 2.3 删除线
只需要在文字的两端加上两个波浪线 ~~ 即可，如下：  
~~BAIDU.COM~~

### 2.4 下划线
通过 HTML 的 u 标签来实现:  
<u>带下划线文本</u>

### 2.5 脚注
[^要注明的文本] 示例如下：  
创建脚注格式类似这样 [^RUNOOB]。

[^RUNOOB]: 学的不仅是技术，更是梦想！！！

## 3.列表Markdown Preview Enhanced
Markdown 支持有序列表和无序列表。
### 3.1 无序列表
无序列表使用星号(*)、加号(+)或是减号(-)作为列表标记，这些标记后面要添加一个空格，然后再填写内容：
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项

### 3.2 有序列表
有序列表使用数字并加上 . 号来表示，如：
1. 第一项
2. 第二项
3. 第三项

### 3.3 列表嵌套
列表嵌套只需在子列表中的选项前面添加四个空格即可：
1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素

## 4.区块
Markdown 区块引用是在段落开头使用 > 符号 ，然后后面紧跟一个空格符号：
> 区块引用  
> 菜鸟教程  
> 学的不仅是技术更是梦想

### 4.1 区块嵌套
区块是可以嵌套的，一个 > 符号是最外层，两个 > 符号是第一层嵌套，以此类推：
> 最外层
> > 第一层嵌套
> > > 第二层嵌套

### 4.2 区块中使用列表
> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项

### 4.3 列表中使用区块
如果要在列表项目内放进区块，那么就需要在 > 前添加四个空格的缩进。
* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
* 第二项

## 5.代码
如果是段落上的一个函数或片段的代码可以用反引号把它包起来，例如：`printf()` 函数

### 5.1 代码区块
代码区块使用 4 个空格或者一个制表符（Tab 键）。  
    <javascript  
    echo 'RUNOOB';  
    function test(){  
      return 这是一个代码块  
    }

### 5.2 代码区块2
在代码上下行用```标记，注意`符号是tab键上面那个，要实现语法高亮，则在```后面加上编程语言的名称  
```javascript
function test(){
  return 这是一个代码块
}
```

## 6.链接
### 6.1 方法  
[链接名称](链接地址)  
或者  
<链接地址>

例如:   
跳转[百度](https://www.baidu.com)  
百度：<https://www.baidu.com>

### 6.2 高级链接
可以通过变量来设置一个链接，变量赋值在文档末尾进行：  
这个链接用 1 作为网址变量 [Google][1]
这个链接用 runoob 作为网址变量 [Runoob][runoob]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [runoob]: http://www.runoob.com/

## 7.图片
### 7.1 语法格式
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")  
例如：  
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)  
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")

### 7.2 高级图片
也可以像网址那样对图片网址使用变量:  
这个链接用 1 作为网址变量 [RUNOOB][1].
然后在文档的结尾为变量赋值（网址）

[1]: http://static.runoob.com/images/runoob-logo.png

### 7.3 指定图片大小
Markdown 还没有办法指定图片的高度与宽度，如果你需要的话，你可以使用普通的 img 标签。  
<img src="http://static.runoob.com/images/runoob-logo.png" width="50%">

## 8.表格
### 8.1 使用方式
Markdown 制作表格使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。语法格式如下：
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |

### 8.2 对齐方式
+ -: 设置内容和标题栏居右对齐。
+ :- 设置内容和标题栏居左对齐。
+ :-: 设置内容和标题栏居中对齐。
例如：<sup>必须空一行才能建表</sup>

| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元 | 单元 | 单元格 |
| 单元 | 单元 | 单元格 |


## 9.高级技巧
### 9.1 支持HTML元素
不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。  
目前支持的 HTML 元素有：kbd、b、i、em、sup、sub、br等 ，如  
使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑

### 9.2 转义
Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠“\”转义特殊字符：  
**文本加粗**   
\*\* 正常显示星号 \*\*  
Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：  
“\”   反斜线  
“`”   反引号  
“*”   星号  
“_”   下划线  
“{}”  花括号  
“[]”  方括号  
“()”  小括号
“#”   井字号  
“+”   加号  
“-”   减号  
“.”   英文句点  
“!”   感叹号  

### 9.3 公式
默认下的分隔符：  
\$...$ 或者 \(...\) 中的数学表达式将会在行内显示。  
\$\$...$$ 或者 \[...\] 或者 ```math 中的数学表达式将会在块内显示。  
$$
\begin{Bmatrix}
   a & b \\
   c & d
\end{Bmatrix}
$$
$$
\begin{CD}
   A @>a>> B \\
@VbVV @AAcA \\
   C @= D
\end{CD}
$$