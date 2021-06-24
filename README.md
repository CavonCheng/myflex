# myflex
my notebook for learning flex css

# 一、初体验

不需要浮动，不需要清除浮动，自适应平均分配间距

```  .div-parent{```  

​	display: flex;

​	width: 80%;

​	height: 300px;

​	background-color: pink;

​	justify-content: space-around;

 ``` }``` 

.span-child{	

​	/* width: 150px;  */

​	felx: 1; 

​	height: 100px;

​	background-color: purple;

​	margin-right: 2px;

}



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
- align-content： 设置侧轴上子元素的排列方式（多行）
- align-items： 设置侧轴上子元素的排列方式（单行）
- flex-flow：符合属性，相当于同时flex-direction和flex-wrap



































