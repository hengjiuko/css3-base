                       学习CSS3的笔记
1.边框圆角效果：border-radius:5px 4px 3px 2p;/*四个半径分别是左上角、右上角、右下角和左下角，顺时针*/
2.边框阴影：box-shadow:X轴偏量 Y轴偏量 [阴影模糊半径] [阴影扩展半径] [阴影颜色] [投影方式]；
   投影方式:inset为内部阴影方式，省略为外部阴影方式（inset可以写在参数的第一个或最后一个）
3.border-image(为边框应用图片)：url(borderimg.png) 70 repeat 
   Round参数：理解为圆满的铺满
   Stretch参数：理解为拉伸
4.颜色之 RGBA
   语法：color:rgba(100,120,60,0.5)
 A指在RGB基础上控制alpha透明度的参数
5.css3渐变颜色
  css3 Gradient分为线性渐变（linear）和径向渐变(radial)
    linear-gradient(to bottom,#fff,#999)
                 /*渐变方向*/ /*表示颜色的起始点和结束点，可以有两至多个色值*/
6.css3文字与字体text-overflow与word-wrap
  text-overflow:clip    |    ellipsis
          /*表示剪切*/    /*表示显示省略标记*/
 想要实现溢出时产生省略号的效果，还须定义强制文本在一行内显示（white-space:nowrap）及溢出内容为隐藏（overflow:hidden），只有这样才能实现溢出文本显示省略号的效果，代码如下：
    text-overflow:ellipsis; 
    overflow:hidden; 
    white-space:nowrap;
       word-wrap也可以用来设置文本行为，当前行超过指定容器的边界时是否断开转行
  语法：word-wrap:normal     |    break-word
   /*表示控制连续文本换行*/  /*表示内容将在边界内换行*/
7.嵌入字体@font-face
    语法:  @font-face {
         font-family : 字体名称;
         src : 字体文件在服务器上的相对或绝对路径;
     }
    这样设置之后，就可以像使用普通字体一样在（font-*）中设置字体样式。

   比如：p {
          font-size :12px;
          font-family : "My Font";
          /*必须项，设置@font-face中font-family同样的值*/
       }
8.文本阴影text-shadow
   语法：text-shadow: X-Offset Y-Offset blur color;
   X-Offset：表示阴影的水平偏移距离，其值为正值时阴影向右偏移，反之向左偏移；      

   Y-Offset：是指阴影的垂直偏移距离，如果其值是正值时，阴影向下偏移，反之向上偏移；

   Blur：是指阴影的模糊程度，其值不能是负值，如果值越大，阴影越模糊，反之阴影越清晰，如果不需要阴影模糊可以将Blur值设置为0；
   Color：是指阴影的颜色，其可以使用rgba色。
9.与背景相关的样式
  1>background-origin:border-box | padding-box | content-box;
  设置背景图片的原始起始位置，参数分别表示背景图片是从边框，还是内边距（默认值），或者是内容区域开始显示。
  2>background-clip:border-box | padding-box | content-box | no-clip
  用来将背景图片做适当的裁剪以适应实际需要，参数分别表示从边框、或内填充，或者内容区域向外裁剪背景。no-clip表示不裁切，和参数border-box显示同样的效果。backgroud-clip默认值为border-box。
  3>background-size: auto | <长度值> | <百分比> | cover | contain
          用来设置背景图片的大小
   cover：将背景图片等比缩放以填满整个容器；
   contain：容纳，即将背景图片等比缩放至某一边紧贴容器边缘为止。
  4>multiple backgrounds
  语法缩写：background ： [background-color] | [background-image] | [background-position][/background-size] | [background-repeat] | [background-attachment] | [background-clip] | [background-origin],...


















