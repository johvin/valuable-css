# valuable-css(不熟悉但有用的css)
*本文记录了本人在日常code中使用频率较低，但却很有用的一些css*<br>

### background属性
*background属性可以设置所有背景属性。*<br>
*可以设置的属性如下：*<br>
* background-color
* background-position
* background-size
* background-repeat
* background-origin
* background-clip
* background-attachment
* background-image

#### background-clip
*规定背景的绘制区域*<br>

**css syntax:**
```css
background-clip:border-box|padding-box|content-box;
```

code to test the effect
```css
div
{
	width:300px;
	height:300px;
	padding:50px;
	background-color:yellow;
	background-clip:border-box;
	border:5px dashed #92b901;
}
```

> ##### code to test the effect
>> /* div style */
>>>		width:300px;
>>>		height:300px;
>>>		padding:50px;
>>>		background-color:yellow;
>>>		background-clip:border-box;
>>>		border:5px dashed #92b901;

#### background-origin
*规定背景图片的定位区域。*
*背景图片可以放置于`content-box`、`padding-box`或`border-box`区域。*<br>

**css syntax:**
```css
background-clip:border-box|padding-box|content-box;//与background-clip语法一致
```
[![bgOrigin]](http://www.w3school.com.cn/tiy/t.asp?f=css3_background-origin)
[bgOrigin]:http://www.w3school.com.cn/i/background-origin.gif "background-origin区域示意图"


**code to test the effect**
```css
div
{
	border:10px dotted black;
	padding:35px;
	background-image:url('/i/bg_flower.gif');
	background-repeat:no-repeat;
	background-position:left;
}
#div1
{
	background-clip:border-box;
	background-origin:border-box;
}
#div2
{
	background-origin:content-box;
}
```

#### background-size
*规定背景图像的尺寸*<br>

**javascript syntax:**
```javascript
object.style.backgroundSize = '60px 80px'
or
object.style['background-size'] = "auto 80px"
```

**css syntax:**
```css
background-size: length | percentage | cover | contain
```
[水平复制4次效果][bgSize]
[bgSize]: http://www.w3school.com.cn/tiy/t.asp?f=css3_background-size3 "拉伸背景图像，对背景图像水平复制四次"
