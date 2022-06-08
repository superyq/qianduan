<h1>css样式笔记</h1>

## a标签样式

```
a:link {} 超链接的初始状态
a:visited {} 超链接被访问状态
a:hover {} 鼠标悬停状态
a:active {} 激活状态
link->visited->hover->active
```

## 文本属性

```
font-size: 16px 字体大小
font-family:   字体
color: red 字体颜色
font-weight: bolder 更加粗
            normal 正常
            bold 加粗
font-style: italic 倾斜
            oblique 倾斜字
            normal 正常
text-align: left 水平靠左
line-height: 行高
text-indent: 首行缩进
text-decoration: underline下划线/overline上划线/line-through删除线。文本修饰
letter-spacing: 字间距
text-transform: capitalize单词首字母大写，lowercase单词全部小写,uppercase单词全部大写
```

## 背景属性

```
background-color: 背景颜色
background-image: 背景图片
backgorund-repeat: 背景平铺模式
backgorund-position: 背景图片定位
background-attachment:fixed固定，scroll滚动 背景图片固定
backgorund-size: cover盒子铺满但图片可能展示不全，contain图片展示全盒子可能铺不满
```

## 浮动属性

```
float: 浮动属性
clear:both/left/right/none 清除浮动
```

## 边框属性

```
border: 1px solid red;
            solid,double,dashed,dotted
```

## 列表属性

```
list-style-type: circle空心圆,disc实心圆，square实心方块
list-style-image: url("")
list-style-position: inside，列表里面
```

## 盒子模型

```
外边距，边框，内边距，内容
```

## 溢出属性

```
overflow: visible溢出显示在元素外，hidden隐藏，scroll滚动，auto,inherit继承父级overflow属性

white-space: normal/nowrap/pre/pre-wrap/pre-line/inherit 如何处理元素内的空白

text-overflow: ellipsis 省略号显示
```

## 定位属性

```
position: static默认，absolute绝对定位,relative相对定位，fixed固定定位，sticky粘性定位
```

## 小三角

```
width: 0px;
height: 0px;
border-top: 20px solid red;
border-left: 20px solid transparent;
border-bottom: 20px solid transparent;
border-right: 20px solid transparent;
```

## 精灵图/雪碧图

```
通过backgorund-position定位图片
```

## 宽高自适应

```
min-width,max-width,min-height,max-height
```

## 文本阴影

```
text-shadow: 2px 4px 10px red;

2px: 水平方向位移
4px: 垂直方向位移
10px: 模糊程度
red: 颜色
```

## 盒子阴影

```
box-shadow: 2px 4px 10px red;
```

## 圆角边框

```
border-radius: 10px;
```

## 字体引入

```
@font-face {
    font-family: <name>
    src: <source>
}
```

## 怪异盒模型

```
box-sizing: content-box标准盒模型，border-box怪异盒模型
```

## 弹性盒模型

```
display: flex;弹性盒模型

flex-wrap: wrap;换行
align-content: center;换行后的行间距

flex-direction: column垂直,row水平
justify-content: center主轴居中
align-items: center侧轴居中
```

## 多列布局/瀑布流

```
父级
column-count: 5;分成几列
column-gap: 30;列间距
column-rule: 2px solid red;列边框
column-fill: balance;列高度统一

子级
break-inside: avoid;禁止分裂
```

## 响应式布局

```
@media screen and (max-width:1024px) and (min-width: 768px) {

}
```

## px、em、rem

```
em: 相对单位，相对于父元素的字体大小
rem: 相对单位，相对于根元素(html)字体大小，div width: 10rem;

fontsize 计算

document.documentElement.style.fontSize = document.documentElement.clientWidth/750 * 100 + 'px'
fontsize = 当前设备的css宽度/物理分辨率(设计稿宽度) * 基准font-size
```

## vh、vw

```
100vh === 视口高度
100vw === 视口宽度
```

## 渐变

```
linear-gradient(90deg, red, yellow, green);线性渐变
radial-gradient(circle, red 10%, yellow 20%, green 30%);径向渐变
                circle渐变为最大圆形, ellipse根据形状渐变
reapting-linear-gradient(90deg, red, yellow, green);重复渐变
```

## 过度

```
transition: all 5s linear 3s
all 参与过度对象
5s  过度时间
3s  延迟时间
linear 过度动画类型
linear 匀速，ease 逐渐慢下来，ease-in 加速，ease-out 减速， ease-in-out 先加速后减速
```

## 动画

```
transform: translateX(100px) 水平移动,scale(1.2) 放大缩小, rotate(40deg) 旋转
```

## 声明动画

```
@keyframes aa {
    from {}
    to {}
    或
    0%
    10%
    100%
}

animation: aa 2s linear infinite(循环);
```

## 3d动画

```
父级
transform-style: preserve-3d; 3d舞台
perspective: 900px; 景深
```

## 网格布局

