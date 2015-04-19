# valuable-css(不熟悉但有用的css)
=================
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
```css
background-clip:border-box|padding-box|content-box;//syntax
```
> ##### code to test the result
>> /* div style */
>>
>>>		width:300px;
>>>		height:300px;
>>>		padding:50px;
>>>		background-color:yellow;
>>>		background-clip:border-box;
>>>		border:5px dashed #92b901;