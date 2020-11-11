# 标签属性

1、标签有标签名、标签属性和文本内容三部分组成（注意：单标签没有文本内容）

2、标签属性是对标签的一种描述方式。

3、标签属性分通用属性、自有属性、用户自定义属性。

4、通用属性：所有标签都具有的属性叫作通用属性

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

- 表格是有行、列组成。

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
  textarea类：
  select类：
  button类：
  ```

  

- 

