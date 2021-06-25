# 一、认识flex

不需要浮动，不需要清除浮动，自适应平均分配间距

``` css
.div-parent{
	display: flex;
	width: 80%;
	height: 300px;
	background-color: pink;
	justify-content: space-around;
 }

.span-child{	
	/* width: 150px;  */
	felx: 1; 
	height: 100px;
	background-color: purple;
	margin-right: 2px;
}
```





# 二、布局原理

### 1、任何容器都可以指定为flex布局

- 当父盒子设为flex布局后，子元素的float、clear和vertical-align属性将失效
- 伸缩布局 = 弹性布局 = 伸缩盒布局 = 弹性盒布局 = flex布局
- 设为flex布局的元素称为“flex容器（flex-container）”，其所有子元素自动成为容器成员，称为“flex项目（flex-item)"
- 子容器可以横向也可以纵向排列

总结原理：通过给父盒子添加flex属性，来控制子盒子的位置和排列方式。



# 三、flex布局父项常见属性

### 1、常见父属性

- flex-direction : 设置主轴的方向
- justify-content： 设置主轴上子元素的排列方式
- flex-wrap：设置子元素是否换行
- align-items： 设置侧轴上子元素的排列方式（单行）
- align-content： 设置侧轴上子元素的排列方式（多行）
- flex-flow：复合属性，相当于同时设置flex-direction和flex-wrap

##### 1.1 flex-direction

该属性用以设置主轴方向

- row 从左至右（默认）
- row-reverse 从右至左
- column 从上至下
- column-reverse 从下至上

##### 1.2 justify-content

设置主轴上子元素的排列方式

- flex-start 
- flex-end
- center
- space-around 子元素平分剩余空间
- space-between 子元素先两侧贴边，再平分剩余空间

##### 1.3 flex-wrap

设置子元素是否换行

- nowrap 不换行（默认）
- wrap 换行

##### 1.4 align-items

设置子元素在侧轴方向的排列方式（单行）

- flex-start
- flex-end
- center
- stretch

##### 1.5 align-content

设置子元素在侧轴方向的排列方式（多行）

- flex-start
- flex-end
- center
- stretch
- space-around
- space-between

##### 1.6 flex-flow

复合属性，相当于同时设置flex-direction和flex-wrap，举例：

``` css
div{
    display: flex;
    flex-wrap: center wrap
}
```



# 四、flex布局子项常见属性

##### 1、flex

子项目占用的分数，使用方法：

flex: 1;  flex: 0;  flex: -1; 等等

##### 2、 order

设定子项目的排列方式，**默认为0**，值越小，优先级越高（可以改变盒子排列顺序） -1 0 1 等。

##### 3、align-self

单独控制子项自己在侧轴的排列方式（可以指定移动哪个盒子）



![flex常用属性](.\f.png)









































