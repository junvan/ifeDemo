###Day02：
#### 0、实例解析
```
<!DOCTYPE html> --- 声明为 HTML5 文档
<html lang="en"> --- HTML 页面的根元素
<head> --- 包含了文档的元（meta）数据
    <meta charset="UTF-8">
    <title></title> --- 描述了文档的标题
</head>
<body> --- 包含了可见的页面内容
</body>
</html>
```
####1、 HTML是什么，HTML5是什么
```
HTML: 超文本标记语言（HyperText Markup Language）
HTML5: HTML5 是 HTML 最新的修订版本，是下一代 HTML 标准。
HTML5 中的一些有趣的新特性：

1. 用于绘画的 canvas 元素
2. 用于媒介回放的 video 和 audio 元素
3. 对本地离线存储的更好的支持
4. 新的特殊内容元素，比如 article、footer、header、nav、section
5. 新的表单控件，比如 calendar、date、time、email、url、search
```
####2、 HTML元素标签、属性都是什么概念？
```
HTML 标记标签通常被称为 HTML 标签 (HTML tag)。

1. HTML 标签是由尖括号包围的关键词，比如 <html>
2. HTML 标签通常是成对出现的，比如 <b> 和 </b>
3. 标签对中的第一个标签是开始标签，第二个标签是结束标签
4. 开始和结束标签也被称为开放标签和闭合标签

HTML 属性
1. HTML 元素可以设置属性
2. 属性可以在元素中添加附加信息
3. 属性一般描述于开始标签
4. 属性总是以名称/值对的形式出现，比如：name="value"。
```

####3、 文档类型是什么概念，起什么作用？
```
DOCTYPE是document type（文档类型）的简写
1.<!DOCTYPE> 声明必须是 HTML 文档的第一行，位于 <html> 标签之前。
<!DOCTYPE> 声明不是 HTML 标签；它是指示 web 浏览器关于页面使用哪个 HTML 版本进行编写的指令。
2.在 HTML 4.01 中，<!DOCTYPE> 声明引用 DTD，因为 HTML 4.01 基于 SGML。DTD 规定了标记语言的规则，这样浏览器才能正确地呈现内容。HTML5 不基于 SGML，所以不需要引用 DTD。
3.请始终向 HTML 文档添加 <!DOCTYPE> 声明，这样浏览器才能获知文档类型。
4.HTML 4.01 与 HTML5 之间的差异在 HTML 4.01 中有三种 <!DOCTYPE> 声明。在 HTML5 中只有一种：<!DOCTYPE html>
5.不加这一行，就表示页面采用浏览器本身的解析标准，这样会造成页面在不同的浏览器（IE、火狐等）可能出现不同的显示效果。
```
####4、 meta标签都用来做什么的？
```
<meta>为页面提供了元信息，放在文档的顶部。它可以通过属性定义元信息，包括定义字符集，定义对页面的描述，针对搜索引擎的关键词等等。
```
####5、 Web语义化是什么，是为了解决什么问题
```
用正确的标签做正确的事情。
html语义化让页面的内容结构化，结构更清晰，便于对浏览器、搜索引擎解析;
即使在没有样式CSS情况下也以一种文档格式显示，并且是容易阅读的;
搜索引擎的爬虫也依赖于HTML标记来确定上下文和各个关键字的权重，利于seo;
使阅读源代码的人对网站更容易将网站分块，便于阅读维护理解。
```
####6、 链接是什么概念，对应什么标签？
```
HTML使用标签 <a>来设置超文本链接。
超链接可以是一个字，一个词，或者一组词，也可以是一幅图像，您可以点击这些内容来跳转到新的文档或者当前文档中的某个部分。
当您把鼠标指针移动到网页中的某个链接上时，箭头会变为一只小手。
在标签<a> 中使用了href属性来描述链接的地址。
默认情况下，链接将以以下形式出现在浏览器中：

1. 一个未访问过的链接显示为蓝色字体并带有下划线。
2. 访问过的链接显示为紫色并带有下划线。
3. 点击链接时，链接显示为红色并带有下划线
```
####7、 常用标签都有哪些，都适合用在什么场景
|标签 | 描述 |
| :--- | :---: |
| `<h1> to <h6>` |	定义 HTML 标题。
| `<p>` |	定义段落。
| `<hr>` |	定义水平线。
| `<!--...-->` |	定义注释。
| `<img>` |	定义图像。
| `<ul>` |	定义无序列表。
| `<ol>` |	定义有序列表。
| `<li>` |	定义列表的项目。
| `<div>` |	定义一个元素块。
| `<span>` |	组合文档中的行内元素。
####8、 表单标签都有哪些，对应着什么功能，都有哪些属性
| 表单标签 |	描述	 | 属性 | 
| :---: | :---: | :---: | 
| `<form>` | 定义表单 | action, autocomplete, method, etc. |
| `<input>` |	定义输入域 |	autofocus, type, min, etc.	input
| `<textarea>` |	定义textarea |	autofocus, cols, form, required, etc.	textarea
| `<label>` |	定义表单控件的名称 |	for, form	label
| `<fieldset>` |	定义fieldset	 | disabled, form , name	fieldset
| `<legend>` |	为以下元素定义标题：`<fieldset>`、`<figure>`、`<details>` |	支持html5的事件和全局属性	legend
| `<select>` |	标签创建下拉列表 |	data, form , name, 'multiple', etc.	select
| `<optgroup>` |	定义选项组 |	lable, disabled	optgroup
| `<option>` |	定义下拉列表中的选项 |	lable, disabled， selected, value	option
| `<button>` |	定义按钮 |	name, disabled， autofocus, etc.	button

####9、 ol, ul, li, dl, dd, dt等这些标签都适合用在什么地方，举个例子
```
ol 为有序列表,即为一个需要排序的列表内容进行排列;
ul 为无序列表,即为一个需要列表但不需要排顺序的内容排列;
li 为列表的内容;
dl 为定义列表;
dt 为定义列表内的标题或项目名称;
dd 为定义定义列表中项目的描述。
```