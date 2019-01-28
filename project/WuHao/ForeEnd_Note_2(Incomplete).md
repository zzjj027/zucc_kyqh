#基本的HTML标签
---
###**1.HTML标题**
> 通过 **&lt;h1&gt; ~ &lt;h6&gt;** 标签定义,h1字体最大
> > 标题标签仅用于标题，用于加粗是不好的习惯,
> <pre>
> &lt;h1&gt;This is a heading&lt;/h1&gt;
> &lt;h2&gt;This is a heading&lt;/h2&gt;
> &lt;h3&gt;This is a heading&lt;/h3&gt;
> </pre>

###**2.HTML 段落**
> 通过 **&lt;p&gt;** 标签进行定义
> <pre>
> &lt;p&gt;This is a paragraph.&lt;/p&gt;
> </pre>

###**3.HTML 链接**
> 通过 **&lt;a&gt;** 标签进行定义
> <pre>
> &lt;a href="http://www.w3school.com.cn"&gt;This is a link&lt;/a&gt;
> </pre>
> > 在 href 属性中指定链接的地址。

###**4.HTML 图像**
> 通过 **&lt;img&gt;** 标签进行定义
> <pre>
> &lt;img src="w3school.jpg" width="104" height="142" /&gt;
> </pre>
> >图像的名称和尺寸是以属性的形式提供的。

---
#HTML元素
HTML 文档是由 HTML 元素定义的, HTML 元素指的是从开始标签（start tag）到结束标签（end tag）的所有代码。
> 开始标签常被称为开放标签（opening tag），结束标签常称为闭合标签（closing tag）。
> 
---
> HTML 元素以开始标签起始
> HTML 元素以结束标签终止
> 元素的内容是开始标签与结束标签之间的内容
> 某些 HTML 元素具有空内容（empty content）
> 空元素在开始标签中进行关闭（以开始标签的结束而结束）
> 大多数 HTML 元素可拥有属性

> **&lt;p&gt; 元素：**
>定义 HTML 文档中的一个段落。
>
> **&lt;body&gt; 元素：**
> <pre>
> &lt;body&gt;
> &lt;p&gt;This is my first paragraph.&lt;/p&gt;
> &lt;/body&gt;
> </pre>
> <body> 元素定义了 HTML 文档的主体。
>
> **&lt;html&gt; 元素：**
> <pre>
> &lt;html&gt;
> &lt;body&gt;
> &lt;p&gt;This is my first paragraph.&lt;/p&gt;
> &lt;/body&gt;
> &lt;/html&gt;
> </pre>
> <html> 元素定义了整个 HTML 文档。
> 
> **空元素**
> 
> 没有内容的 HTML 元素被称为空元素。**空元素是在开始标签中关闭的**。
> &lt;br&gt; 就是没有关闭标签的空元素.正确关闭：**&lt;br/&gt;**
> 
---

#HTML 属性
---
> HTML 标签可以拥有属性。属性提供了有关 HTML 元素的更多的信息。
> 属性总是以 **名称/值对** 的形式出现，比如：name="value"。
> 属性总是在 HTML 元素的**开始标签**中规定。
> <pre> 
> &lt;a href="http://www.w3school.com.cn"&gt;This is a link&lt;/a&gt;
> </pre>
> 
> HTML 链接由 &lt;a&gt;标签定义。链接的地址在 href 属性中指定：
>> **HTML 提示：使用小写属性**
>> **始终为属性值加引号** ，大多数情况下是双引号，在属性值本身为双引号的情况下使用单引号

>> **HTML 属性参考手册**
>> [http://www.w3school.com.cn/tags/index.asp](http://www.w3school.com.cn/tags/index.asp)

