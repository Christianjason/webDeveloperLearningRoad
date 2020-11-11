Html知识点回顾

- 熟悉HTML文件结构，并联系标准标签的使用

```html
<!doctype html>
<html>
		<head>
				<meta http-equiv="content-type" content="text/html"; charset="utf-8" />
				<meta name="keyword" content="..." />
				<meta name="description" content="..." />
				<link rel="shortcut icon" href="图标的路径 + 文件名" type="image/x-icon" />
				<title>...</title>
				<link rel="stylesheet" href="外部样式文件名（需要带路径，能够访问）" />
				<style type="text/css">
						样式设置
				</style>
		</head>
	
		<body>
				<!--网页主体内容（根据需求）-->
		</body>
  
  	<script language="javascript" type="text/javescript">
    		脚本代码
    </script>
</html>
```

- 熟悉W3C规范，熟悉语义化标签，整理每一个标签对应的语义环境

```html
w3c标准由结构（HTML）、表现（css）、行为（javascript逻辑）三部分组成。
W3C常见的标准与规范列举：
	1）定义语言编码
			<meta http-equiv="content-type" content="text/html"; charset="utf-8" />
			或
			<meta charset="utf-8" />
	2）JavaScript定义（需要制定语言（javascript）以及类型（text/javascript）
			<script language="javascript" type="text/javescript">
    			脚本代码
    	</script>
	3）CSS定义（指定type属性）
			<style type="text/css">
						样式设置
			</style>
			为了保证各个浏览器的兼容性，在写CSS的时候需要带上计量单位。
	4）不要在注释内容中使用“--”
			注释的书写方式：<!--==注释内容==-->
	5）所有标签的元素及属性名称都必须用小写
	6）所有的属性值必须用双引号包含
	7）如果文档要输出<, > 和 &等，请使用实体转义符
      <p>&gt...</p>
    	<p>&lt...;&amp;..</p>
  8）要给所有的属性赋值，不赋值则默认认为值是属性名本身
    	<img src="..." alt="xx" />
    	<input type="text" readonly />
    	<!--readonly没有赋值，则将readonly本身赋值给readonly属性-->
  9）所有的标签都必须要有一个相应的结束标记（即标签必须要闭合）
  		<p> </p>
    	<hr />
    	<br />
	10）所有的标签必须合理嵌套，不能出现嵌套交叉
  		行级标签只能套行级标签
    	块级标签可以套块级、行级标签，但是也有例外。
    	<div><p><div></div></p> 不能存在这种交叉嵌套
  11）图片要添加有意义的alt属性
    	增加用户体验效果
  12）在form表单中添加lable标签，以增加用户友好度。
```

- 练习并测试html标签的嵌套规则

```
行级标签只能套行级标签
块级标签可以套块级、行级标签，但是也有例外。
```

- 用html实现静态页面

