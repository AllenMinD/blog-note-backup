<h1>Flexbox布局</h1>  

**目录**  
1. [Flexbox语法](#chapter1)  
2. [Flexbox应用实例](#chapter2)  


<h3 id="chapter1">一、Flexbox语法</h3>  
具体参考阮一峰老师的介绍：[戳我](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html)  

我来小结一下Flexbox有哪些属性，方便速查：  
（在“ | ”左右的值表示属性的可选值，在“ || ”左右的表示的是两个属性）  

  + 以下6个属性设置到【容器】上：  
    - `flex-direction`: row | row-reverse | column | column-reverse;  // 主轴的方向
    - `flex-wrap`: nowrap |  wrap |  wrap=reverse;  //  是否"换行"
    - `flex-flow`: (flex-direction) || (flex-wrap);  // flex-direction和flex-wrap的合体简写
    - `justify-content`: flex-start | flex-end | center | space-between | space-around;  // 主轴上的对齐方式
    - `align-items`: flex-start |  flex-end | center| baseline | stretch;  // 交叉轴上的对齐方式
    - `align-content`: flex-start | flex-end | center | space-between | space-around | stretch;  // 定义了多根轴线时的对齐方式  

  + 以下6个属性设置到【项目】上：  
    - `order`: (integer);  // 项目的排列顺序。默认为0，数值越小越靠前。
	- `flex-grow`: (number);  // 放大比例。默认为0，即如果存在剩余空间，也不放大
	- `flex-shrink`: (number);  // 缩小比例。默认为1，即如果空间不足，就等比例缩小
	- `flex-basis`: (length) | auto;  // 在分配多余空间之前，项目占据的主轴空间（main size）
	- `flex`: none | [(flex-grow) || (flex-shrink) || (flex-basis)];  // 默认是0 1 auto (后两个属性可选)
	- `align-self`: auto | flex-start | flex-end | center |  baseline | stretch;  // 允许单个项目与其他项目不一样的对齐方式
  


<h3 id="chapter2">二、Flexbox实例应用</h3>  
关于Flexbox的实例应用具体还是看阮一峰老师的介绍：[再戳我](http://www.ruanyifeng.com/blog/2015/07/flex-examples.html)  

我继续来小结一下关于Flexbox的实例应用，方便速查（点进去就是例子，按F12看代码）：  

  + [骰子布局](https://allenmind.github.io/flexbox-exmaple/LearnFlexbox2.html)
  + [网格布局](https://allenmind.github.io/flexbox-exmaple/LearnFlexbox3-1.html)
  + [圣杯布局](https://allenmind.github.io/flexbox-exmaple/LearnFlexbox3-2.html)
  + [输入框（表单）布局](https://allenmind.github.io/flexbox-exmaple/LearnFlexbox3-3.html)
  + [悬挂式布局（左边头像，右边名字和内容）](https://allenmind.github.io/flexbox-exmaple/LearnFlexbox3-4.html)
  + [固定页脚到视口底部](https://allenmind.github.io/flexbox-exmaple/LearnFlexbox3-5.html)