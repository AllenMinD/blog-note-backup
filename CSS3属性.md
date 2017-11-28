<h1>CSS3属性小结</h1>

**目录**  
1. [CSS3属性小结](#chapter1)  
2. [转换、过渡、动画](#chapter2)

[更全的参考](http://www.runoob.com/css3/css3-tutorial.html)

<h3 id="chapter1">一、CSS3属性小结</h3>

- [边框](http://www.w3school.com.cn/css3/css3_border.asp)
	+ border-radius：圆角框
	+ box-shadow：边框阴影（水平阴影、垂直阴影、模糊距离，以及阴影的颜色）
	+ border-image：边框图片
- [背景](http://www.w3school.com.cn/css3/css3_background.asp)
	+ background-size：背景图片大小
	+ background-origin：背景图片显示区域
- [文本](http://www.w3school.com.cn/css3/css3_text_effect.asp)
	+ text-shadow：文字阴影（水平阴影、垂直阴影、模糊距离，以及阴影的颜色）
	+ word-wrap：自动换行（break-word）
- [字体](http://www.w3school.com.cn/css3/css3_font.asp)
	+ @font-face：使用自定义字体
	+ 实例：
        <pre>
		@font-face
		{
		  font-family: myFirstFont;
		  src: url('Sansation_Bold.ttf'),
		       url('Sansation_Bold.eot'); /* IE9+ */
		  font-weight:bold;
		}
        </pre>
	+ 里面的属性（字体描述符）：
	  * font-family：字体的名称
	  * src：字体文件的 URL
	  * font-stretch：定义如何拉伸字体。默认是 "normal"。
	  * font-style：字体的样式。默认是 "normal"。 
	  * font-weight：字体的粗细。默认是 "normal"。
	  * unicode-range：定义字体支持的 UNICODE 字符范围。默认是 "U+0-10FFFF"。
- [转换](http://www.w3school.com.cn/css3/css3_2dtransform.asp)
	+ 转换是使元素改变形状、尺寸和位置的一种效果。
	+ transform：使元素应用 2D 或 3D 转换。
	+ transform-origin：允许你改变被转换元素的位置。
	+ transform-style：规定被嵌套元素如何在 3D 空间中显示。
	+ perspective:：规定 3D 元素的透视效果。
	+ perspective-origin：规定 3D 元素的底部位置。
	+ backface-visibility：定义元素在不面对屏幕时是否可见。
	+ [2D转换的方法](http://www.w3school.com.cn/css3/css3_2dtransform.asp)：
		* matrix(n,n,n,n,n,n)：定义 2D 转换，使用六个值的矩阵。
		* translate(x,y)：定义 2D 转换，沿着 X 和 Y 轴移动元素。
		* translateX(n)：定义 2D 转换，沿着 X 轴移动元素。
		* translateY(n)：定义 2D 转换，沿着 Y 轴移动元素。
		* scale(x,y)：定义 2D 缩放转换，改变元素的宽度和高度。
		* scaleX(n)：定义 2D 缩放转换，改变元素的宽度。
		* scaleY(n)：定义 2D 缩放转换，改变元素的高度。
		* rotate(angle)：定义 2D 旋转，在参数中规定角度。
		* skew(x-angle,y-angle)：定义 2D 倾斜转换，沿着 X 和 Y 轴。(可以用来画平行四边形)
		* skewX(angle)：定义 2D 倾斜转换，沿着 X 轴。
		* skewY(angle)：定义 2D 倾斜转换，沿着 Y 轴。
	+ [3D转换的方法](http://www.w3school.com.cn/css3/css3_3dtransform.asp)：
		* matrix3d(n,n,n,n,n,n,n,n,n,n,n,n,n,n,n,n)：定义 3D 转换，使用 16 个值的 4x4 矩阵。
		* translate3d(x,y,z)：定义 3D 转化。
		* translateX(x)：定义 3D 转化，仅使用用于 X 轴的值。
		* translateY(y)
		* translateZ(z)
		* scale3d(x,y,z)：定义 3D 缩放转换。
		* scaleX(x)：定义 3D 缩放转换，通过给定一个 X 轴的值。
		* scaleY(y)
		* scaleZ(z)
		* rotate3d(x,y,z,angle)：定义 3D 旋转。
		* rotateX(angle)：定义围绕 X 轴的 3D 旋转。
		* rotateY(angle)
		* rotateZ(angle)
		* perspective(n)：定义 3D 转换元素的透视视图。
	+ [过渡](http://www.w3school.com.cn/css3/css3_transition.asp)：
		- 实现了使元素从一种样式**逐渐**改变为另一种样式的效果。
		- 如需向多个样式添加过渡效果，请添加多个属性，由逗号隔开。
		- transition：简写属性，用于在一个属性中设置四个过渡属性。（下面为4个过度属性）
		- transition-property：规定应用过渡的 CSS 属性的名称。
		- transition-duration：定义过渡效果花费的时间。默认是 0。
		- transition-timing-function：规定过渡效果的时间曲线。默认是 "ease"（慢速开始，然后变快，然后慢速结束）。
		- transition-delay：	规定过渡效果何时开始（即延时）。默认是 0。   
	+ [动画](http://www.w3school.com.cn/css3/css3_animation.asp)：（这个真的很酷）
		- CSS3的动画可以看作是CSS3过渡的升级版。动画和过渡一样是使元素从一种样式**逐渐**改变为另一种样式的效果，但过渡只能在两种样式之间变换；而动画可以在多种样式之间变换，而且动画还可以规定在某一个时刻展现某一种样式。
		- @keyframes：定义动画（类似于函数）。定义格式大概是：`@keyframes 动画名 {...}`
		- animation：所有动画属性的简写属性，其中animation-name（动画名称）和animation-duration（动画时长）是必填的，除了 animation-play-state 属性。
		- animation-name：规定 @keyframes 动画的名称。
		- animation-duration：规定动画完成一个周期所花费的秒或毫秒。默认是 0。
		- animation-timing-function：规定动画的速度曲线。默认是 "ease"。
		- animation-delay：规定动画何时开始。默认是 0。
		- animation-iteration-count：规定动画被播放的次数。默认是 1。
		- animation-direction：规定动画是否在下一周期逆向地播放。默认是 "normal"。
		- animation-play-state：规定动画是否正在运行或暂停。默认是 "running"。
		- animation-fill-mode：规定对象动画时间之外的状态。
		- 例子：
			<pre>
			// 一般要把其他前缀写上, 如 @-moz-keyframes my first{...}
			@keyframes myfirst
			{
			  0%   {background: red;}
			  25%  {background: yellow;}
			  50%  {background: blue;}
			  100% {background: green;}
			}
			
			div {
			  animation:myfirst 5s;
			}
			</pre>
	+ [多列](http://www.w3school.com.cn/css3/css3_multiple_columns.asp)：
		- column-count：规定元素应该被分隔的列数。
		- column-gap：规定列之间的间隔。
		- column-rule：设置所有 column-rule-* 属性的简写属性（颜色、样式、宽度）。
	+ [用户界面](http://www.w3school.com.cn/css3/css3_user_interface.asp)
		- resize：规定是否可由用户调整元素尺寸
		- box-sizing：允许您以确切的方式定义适应某个区域的具体内容。
		- outline-offset：对轮廓进行偏移，并在超出边框边缘的位置绘制轮廓。
	+ [图片处理](http://www.runoob.com/css3/css3-images.html)
		- 响应式图片
		- 在图片上定位文本
		- 卡片式图片
		- 图片滤镜
		- 响应式图片相册
		- 图片Modal（模态、“蒙板”） 
	+ [按钮](http://www.runoob.com/css3/css3-buttons.html)
		- 按钮的各种样式
		- 按钮动画
	+ [分页的实现](http://www.runoob.com/css3/css3-pagination.html)
	+ [框大小](http://www.runoob.com/css3/css3-box-sizing.html)
	+ [弹性盒子Flex box](http://www.runoob.com/css3/css3-flexbox.html)
		- CSS3弹性盒子
		- 还可以看看我的一篇[总结](http://allenmind.cn/2017/11/09/Flexbox%E5%B8%83%E5%B1%80/)
	+ [多媒体查询@media](http://www.runoob.com/css3/css3-mediaqueries.html) 

<h3 id="chapter2">二、转换、过渡、动画</h3>

理清一下转换、过渡、动画的区别：

1. 首先是名字：
	- 转换：transform
	- 过渡：transition
	- 动画：animation
2. 然后是作用：
	- 转换（transform）是使元素改变形状、尺寸、位置、旋转的一种效果，分2D转换和3D转换。
	- 过渡（transition）是控制【元素在两种样式之间转换的】过程（控制这个过程进行的快慢、延时）。
	- 动画（animation）是控制【元素在多种样式之间转换的】过程。
3. 接着是用法：
	- 转换：`transform: 转换方法1 转换方法2 ...;` （多个转换方法之间用空格隔开）
	- 过渡：`transition: 属性1 过渡时间1, 属性2 多度时间2, ...;`
	- 动画：动画的话麻烦有点，要先【定义动画】，然后在animation属性指定这个【动画名称】和【播放时间】，具体如下：
		<pre>
		/* CSS3 动画 animation */
	    @keyframes ani {
	      0% {background: #ff3b42; color: yellow;}
	      25% {background: blue; color: yellow; transform: rotateY(180deg);}
	      50% {background: orange; color: blue; transform: translateX(300px);}
	      100% {background: yellow; color: blue; transform: rotate(180deg); width: 60px; height: 60px;}
	    }
	
	    div {
	      animation: ani 5s;
	      animation-iteration-count: 1;  /* 播放次数(infinite为无限次) */
	      animation-direction: alternate;  /* 下一周期逆向播放 */
	    }
		</pre>
4. 最后说下联系：
	- 转换（transform）可以用于过渡（transition）和动画（animation）当中。
	- 在目前看来，过渡和动画的本质是一样的：都是控制元素更换样式的过程。只不过过渡控制的是【元素在**2种**样式之间转换的】过程，而动画屌一点，可以控制【元素在**多种**样式之间转换的】过程，动画的功能比过渡更多。