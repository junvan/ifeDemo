
### Day03
#### 

参考闫琪同学的

|属性 |描述| 常见属性值/单位 |
|:--:|:--:|:--:|
|font-family|设置字体|例：Arial,sans-serif |
|font-size |设置字体大小| px、em、rem|
| font-style|设置字体样式|normal、italic、oblique|
|font-weight|设置字体粗细|normal、bold、lighter、bolder、100~900|
|font-variant|定义元素的文本是否为小型的大写字母|normal、small-caps|
|font|字体简写|`font-style font-variant font-weight font-stretch font-size / line-height font-family`|
|text-transform|文本转换|none、uppercase、lowercase、capitalize、full-width|
|text-decoration|文本装饰|none、underline、overline、line-through|
|text-shadow|文字阴影|例：4px 4px 5px red；水平偏移 垂直偏移 模糊半径 阴影颜色   |
|text-align|文本对齐|left、right、center、justify|
|line-height|行高|px、数字|
|letter-spacing|字母间距|px|
|word-spacing|字间距|px|
|text-indent|文本缩进|px|
|text-overflow|定义内联内容溢出其块容器是否截断或者添加(...)及自定义字符|clip  ellipsis
|white-space|设置元素中空白的处理方式|normal  pre  nowrap  pre-wrap  pre-line|
|word-break|定义元素内容文本的字间与字符间的换行行为|normal  keep-all  break-all  break-word|
|word-wrap|设置或检索当内容超过指定容器的边界时是否断行|normal  break-word |


下面的表格总结了 white-space 属性的行为：

|值	|空白符|	换行符|	自动换行|
|:--:|:--:|:--:|:--:|
|pre-line|	合并|	保留|	允许|
|normal	|合并|	忽略|	允许|
|nowrap	|合并|	忽略|	不允许|
|pre|	保留|	保留|	不允许|
|pre-wrap|	保留|	保留|	允许|


##### CSS3 选择器
|选择器	|例子	|例子描述|
|:--:|:--:|:--:|
|.class|	.intro|	选择 class="intro" 的所有元素。
|#id|	#firstname|	选择 id="firstname" 的所有元素。
|*|	*	|选择所有元素。
|element	|p|	选择所有 `<p>` 元素。
|element,element|	div,p|	选择所有 `<div>` 元素和所有 `<p>` 元素。
|element element|	div p|	选择 `<div>` 元素内部的所有 `<p>` 元素。
|element>element|	div>p|	选择父元素为 `<div>` 元素的所有 `<p>` 元素。
|element+element|	div+p|	选择紧接在 `<div>` 元素之后的所有 `<p>` 元素。
|[attribute]|	[target]|	选择带有 target 属性所有元素。
|[attribute=value]|	`[target=_blank]`	|选择 target="_blank" 的所有元素。
|[attribute~=value]|	[title~=flower]	|选择 title 属性包含单词 "flower" 的所有元素。
|`[attribute&#124=value]`|	`[lang&#124=en]`|	选择 lang 属性值以 "en" 开头的所有元素。
|:link|	a:link|	选择所有未被访问的链接。
|:visited	|a:visited|	选择所有已被访问的链接。
|:active|	a:active|	选择活动链接。
|:hover|	a:hover	|选择鼠标指针位于其上的链接。
|:focus|	input:focus|	选择获得焦点的 input 元素。
|:first-letter|	p:first-letter|	选择每个 `<p>` 元素的首字母。
|:first-line|	p:first-line|	选择每个 `<p>` 元素的首行。
|:first-child|	p:first-child|	选择属于父元素的第一个子元素的每个 `<p>` 元素。
|:before|	p:before|	在每个 `<p>` 元素的内容之前插入内容。
|:after|	p:after|	在每个 `<p>` 元素的内容之后插入内容。
|:lang(language)|	p:lang(it)|	选择带有以 "it" 开头的 lang 属性值的每个 `<p>` 元素。
|element1~element2|	p~ul|	选择前面有 <p> 元素的每个 <ul> 元素。
|[attribute^=value]|	a[src^="https"]|	选择其 src 属性值以 "https" 开头的每个 <a> 元素。
|[attribute$=value]	|a[src$=".pdf"]|	选择其 src 属性以 ".pdf" 结尾的所有 <a> 元素。
|`[attribute*=value]`|	`a[src*="abc"]`|	选择其 src 属性中包含 "abc" 子串的每个 <a> 元素。
|:first-of-type|	p:first-of-type	|选择属于其父元素的首个 `<p>` 元素的每个 `<p>` 元素。
|:last-of-type|	p:last-of-type|	选择属于其父元素的最后 `<p>` 元素的每个 `<p>` 元素。
|:only-of-type|	p:only-of-type|	选择属于其父元素唯一的 `<p>` 元素的每个 `<p>` 元素。
|:only-child|	p:only-child|	选择属于其父元素的唯一子元素的每个 `<p>` 元素。
|:nth-child(n)|	p:nth-child(2)|	选择属于其父元素的第二个子元素的每个 `<p>` 元素。
|:nth-last-child(n)|	p:nth-last-child(2)	|同上，从最后一个子元素开始计数。
|:nth-of-type(n)|	p:nth-of-type(2)|	选择属于其父元素第二个 `<p>` 元素的每个 `<p>` 元素。
|:nth-last-of-type(n)|	p:nth-last-of-type(2)|	同上，但是从最后一个子元素开始计数。
|:last-child|	p:last-child|	选择属于其父元素最后一个子元素每个 `<p>` 元素。
|:root|	:root	|选择文档的根元素。
|:empty	|p:empty	|选择没有子元素的每个 `<p>` 元素（包括文本节点）。
|:target|	#news:target|	选择当前活动的 #news 元素。
|:enabled|	input:enabled|	选择每个启用的 `<input>` 元素。
|:disabled|	input:disabled	|选择每个禁用的 `<input>` 元素
|:checked|	input:checked	|选择每个被选中的 `<input>` 元素。
|:not(selector)	|:not(p)|	选择非 `<p>` 元素的每个元素。
|::selection|	::selection|	选择被用户选取的元素部分。

##### 尺寸
|单位	|描述|
|:--:|:--:|
|%	|百分比
|in	|英寸
|cm	|厘米
|mm	|毫米
|em	|1em 等于当前的字体尺寸。2em 等于当前字体尺寸的两倍。例如，如果某元素以 12pt 显示，那么 2em 是24pt。在 CSS 中，em 是非常有用的单位，因为它可以自动适应用户所使用的字体。
|ex	|一个 ex 是一个字体的 x-height。 (x-height 通常是字体尺寸的一半。)
|pt	|磅 (1 pt 等于 1/72 英寸)
|pc	|12 点活字 (1 pc 等于 12 点)
|px|	像素 (计算机屏幕上的一个点)

##### css颜色
可以使用Color Name(颜色名称), HEX, RGB, RGBA, HSL, HSLA, transparent来指定color