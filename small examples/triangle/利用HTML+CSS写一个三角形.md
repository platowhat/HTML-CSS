写之前，首先要了解其中的原理

html代码只需创建两个名为triangle、triangle-left的div盒子即可，
代码：

```
<body>
	<div id="triangle"></div><br /><br /><br />
	<div id="triangle-left"></div>
	
</body>
```

在triangle.html文件中，下面代码及其实现后的效果图如下：

```
#triangle{
	margin-top:50px;
	width: 100px;
	height: 100px;
	border-top:100px solid red;
	border-right:100px solid blue;
	border-bottom:100px solid green;
	border-left:100px solid orange;
}
```

图：![image](https://github.com/kivet-h/HTML-CSS/raw/master/images/triangle01.jpg)


实现出现三角形的效果，可以将div盒子宽高都设为0px，上面图就会变成四个三角形组成的一个正方形，再通过设置边框宽度以及颜色等，就能实现一个三角形
代码：

```
#triangle-left {
    width: 0px; 
    height: 0px; 
    border-top: 50px solid transparent;
    border-right: 100px solid red;
    border-bottom: 50px solid transparent;
}
```

三角形效果图：![image](https://github.com/kivet-h/HTML-CSS/raw/master/images/triangle02.png)
