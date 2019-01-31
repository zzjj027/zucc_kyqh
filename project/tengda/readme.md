# PROJECT  
## Come From  
这里是滕达的project文件夹，存放看百度前端学院教程的成果  

## Daily  
### Day 1  
day1的内容我选择使用parcel来简单构建一个开发环境  
随后我按照parcel的文档写了一个quickstart详见qstart文件夹  
测试了一下简单的html格式和js格式  
最后把quickstart解析到了pj.tenderkun.com  

PS：parcel官方文档中有一句console.log('hello world')略有小错，我改成了双引号再加了一个分号。  

### Day 2  
今天找着mdn教程上打了一个简单的列表消息盒子样式。  
今天的学习成果：  
1、可以通过`info-box ul`类似的样式来为style为`.info-box`的各个子标签设置style  
2、通过 `document.querySelectorAll`函数可以获取所有指定的html元素  
3、javascript中的有关Attribute函数可以设置元素是否active  

### Day 3  
(文件存储在/定位MDNExample)
学习记录：  
1、style中的cursor规定显示的指针类型
(这里测试在markdown中插入图片的方法)  
![insertpng](../../img/cursorListFromTengda.png)  
(似乎在github的markdown里面写base64编码并不合适，但将转换python程序附在当前目录)  

2、  
`<label for="toggle">❔</label><input type="checkbox" id="toggle">`
可以像如上的方式用for来将label和input绑定来实现将label的点击事件同步到CheckBox中。  

3、  
`label[for="toggle"] `  
可以像如上的方式为含有指定for的元素赋予style  
`input[type="checkbox"]`  
type也是同理  

4、  
一个选择方式
`input[type=checkbox]:checked + aside`
上句的选择方式是 选择的checkbox相邻的aside元素

成果:  
实现了checkbox hack  
实现了一个不用JavaScript的可唤出侧边栏（太真实了，从来没想到过）  


### Day 4  
今天内容：弹性盒子
[找的辅助资料](https://www.cnblogs.com/cblx/p/8976309.html)  
[还有一个超好的资料](http://zh.learnlayout.com/display.html)  

笔记：  
1、![FlexBoxWrap](../../img/flex-wrapExample.png)  (勘误，这里应该是wrap，打错了QAQ)  
上图注释掉的`flex-wrap: wrap;`语句在这个example中有一个意想不到的效果  
当该语句不存在时  
![wrapType1](../../img/wrapType1.png)  
我们看到了预想中的效果，这里几个框自适应到了一行三个  
当该语句存在时  
![wrapType2](../../img/wrapType2.png)  
这里的框反而好像按列排列，这是因为当指定换行后，我们却没有指定框的左右长度，所以不会有例子1中的自适应的效果，几个框虽然是按照行排列，
但是每行只有1个，所以和列排列的样式相同。
2、  
可以将一个元素的display设置为none来使它隐藏，与visibility设置为hidden不同的是，display为none的元素不会占用位置。  
3、  
max-width属性可以适配小窗口而不会超出最大范围而显示一个滚动条  
4、  
```css
* {
  -webkit-box-sizing: border-box;
     -moz-box-sizing: border-box;
          box-sizing: border-box;
}
```
将上面的代码写入style可以保证所有的盒类元素都可以不用计算padding和border-width来写width和margin  
5、  
![Position](http://zh.learnlayout.com/position.html)
这是一个放着position的几个属性各是干嘛的。  
clear属性用来控制浮动（float），它的作用是使下面的dom元素可以清楚上面的dom元素的浮动效果（不受影响）。  
6、`overflow: auto;  `
将overflow设置成auto可以防止内部的浮动元素超出外部dom的范围。  
7、媒体查询  
```css
@media screen and (min-width:600px) {
  nav {
    float: left;
    width: 25%;
  }
  section {
    margin-left: 25%;
  }
}
@media screen and (max-width:599px) {
  nav li {
    display: inline;
  }
}
```  
上面的代码的作用是对于页面宽度在600及以上或者是600一下适用于不同的布局。  
7、针对移动设备还有一个知识点：  
`<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0">`  
这句话会将移动浏览器的viewport固定为设备的宽度

（下面试一下写一个markdown表格）

|属性值|作用|
|------|--|
|width|设置layout viewport  的宽度，为一个正整数，或字符串"width-device"|
|initial-scale|设置页面的初始缩放值，为一个数字，可以带小数|
|minimum-scale|允许用户的最小缩放值，为一个数字，可以带小数|
|maximum-scale	允许用户的最大缩放值，为一个数字，可以带小数|
|height|设置layout viewport  的高度，这个属性对我们并不重要，很少使用|
|user-scalable|是否允许用户进行缩放，值为"no"或"yes", no 代表不允许，yes代表允许|
