# 标签属性

1、标签有标签名、标签属性和文本内容三部分组成（注意：单标签没有文本内容）

2、标签属性是对标签的一种描述方式。

3、标签属性分通用属性、自有属性、用户自定义属性。

4、通用属性：所有标签都具有的属性叫作通用属性（除br标签外）

```
id：用于给标签取一个唯一的名称。ID的名称是唯一的，不能重复的定义。
class：用来给标签取一个类名
style：用来设置该标签的行内样式。
title：鼠标移至标签的时候的提示文本，目的是起一个提示的作用
```

5、自定义标签属性：通常用于传值或用于图片的懒加载等方面

```
格式：data-* 
<img src="图片名" alt="xx" />
图片懒加载
<img data-src="图片名" alt="xxx" />  后续javascript根据界面位置获取相应的图片
用于传值
<p data-id="goodsid">...</p>
```

# 表格标签(table)

> 表格标签主要用于呈现格式化数据。

- 表格是有行、列组成（先行后列）。

```html
表格的格式
<table>
  <tr>	行1
    <th></th>
    <th></th>
    <th></th>
  </tr>
  <tr>
  	<td></td> 行1列1 
    <td></td> 行1列2
    <td></td>
    ...
  </tr>
	...
</table>

表头<th></th>会自动加粗与居中
```

- table属性

```
border:设置表格边框,默认单位是像素
width:设置表格宽度，默认单位是像素
cellspacing:设置单元格边框的间距
cellpadding:单元格中文本内容与边框的距离
align:表格的对齐方式 left（居左） center（居中）right（居右）；默认left
```

- 跨行/跨列属性

  > 主要用来绘制复杂的表格

  ```
  跨行合并：rowspan="xx"  合并单元格 删除其他的
  跨列合并：colspan="xx"   合并单元格。删除其他的
  ```

- 完整的表格

  > 完整表格的组成：caption（标题）、thead（表头）、tbody（表体）、tfoot（表尾）四部分组成

  ```
  table[]>comption{}+thead>tr>th*4+tbody>tr*4>td*4+tfoot>tr>td[rowspan=4]
  ```

- form表单标签是所有标签最核心标签之一。是用来实现前后端交互的一个重要标签

  ```
  常用属性：
  name：表单名称
  action：表单数据提交到地方（通常是一个后台文件名（.jsp/.php/.asp/.aspx/.py等），或者网址）。
  	如果是#，表示提交到当前文件。
  method：前端提交数据到后端的方法（方式主要有：get和post两种，默认get）
  ```

- 表单元素

  ```
  input类：
  根据不同的type属性，变化为多种状态输入方式
  主要用来完成输入，或发出指令。
  type值：text/password/radio/checkbox/file/button/image/submit/reset
  1)text：单行文本输入框。type=“text”可以不写，默认type就是text
  		属性：placeholder(提示)/name(命名，便于区分传送到后台的数据)/minlength(最小输入的字符个数)/maxlength(最多输入的字符个数)/disable(失效)/readonly(只读)
  				 value(设置缺省值)/pattern(用于正则匹配)
  2)password:密码框，属性与text一样
  3)radio:单选钮，通常用于两项以上。常用属性有：name(命名，这个是必须的)/value(值)/check(默认选中)/disable/readonly
  4)checkbox:复选框可以用来选择0项、1项或者多项。
  常用的属性有：name（必须要有）/value/checked/disable/readonly
  5)file:文件上传按钮
  6)button:普通按钮，通常用它去调用脚本代码，发送指令等。常用属性：value（按钮标题）/disable（失效）readonly（只读）
  7)image:图片按钮，用法与button一样。有一个特殊的属性(src，用于加载图片 替换了value)
  也有提交功能，与submit一样
  8)submit:提交按钮，用来见表单提交到后台
  属性：value/disable
  9)reset:重置按钮，将表单所有的组建输入的内容全部清空，还原为初始状态
  属性：value/disable
  textarea类：
  	文本域（也可以叫多行文本框），主要用于输入大批量的内容
  	常用的属性：name/id/cols/rowss/placeholder(提示)/maxlength/required(表示必须输入)/value(获取文本框里面的值)
  select类：
  	下拉列表框，用于单项选择
  	multiple属性表示可以多选，这个时候的下拉列表框变成了列表框
  	size:最多显示的行数
  button类：
  	普通按钮，具有提交功能。可以单独使用，可以不写到form里面。若写在form中，就有一个提交的功能。
  ```

  

- 

