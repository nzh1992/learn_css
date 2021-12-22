## css 颜色名
在css中，可以通过颜色名称来指定颜色。

## css 背景色
可以为HTML元素设置背景色。
```html
<h1 style="background-color:DodgerBlue;">China</h1>
<p style="background-color:Tomato;">China is a great country!</p>
```

## css 文本颜色
```html
<h1 style="color:Tomato;">China</h1>
<p style="color:DodgerBlue;">China is a great country!</p>
<p style="color:MediumSeaGreen;">China, officially the People's Republic of China...</p>
```

## css 边框颜色
```html
<h1 style="border:2px solid Tomato;">Hello World</h1>
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>
<h1 style="border:2px solid Violet;">Hello World</h1>
```

## css 颜色值
在css中，还可以使用RGB值、HEX值、HSL值、RGBA值或者HSLA值来指定颜色。
```html
<h1 style="background-color:rgb(255, 99, 71);">...</h1>
<h1 style="background-color:#ff6347;">...</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>

<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>
```

#### 什么是RGB？
RGB是一种色彩模式，也是工业界的一种颜色标准。
是通过红（R），绿（G），蓝（B）三个颜色通道的变化以及它们之间的叠加来得到公式各样的颜色的。
这个标准几乎包括了人类视力所能感知的所有颜色，是运用最广的颜色系统之一。

#### 什么是HEX？
将RGB值翻译成16进制来表达颜色。

#### 什么是HSL值？
HSL是一种将RGB色彩模型中的点在圆柱坐标系中的表示法。
HSL即色相(Hue)、饱和度(Saturation)、亮度(Lightness)的缩写。

#### 什么是RGBA？
由RGB色彩空间和Alpha通道组成。Alpha通道为图像的不透明度参数，其数值可以用0~1的小数，或者百分比表示。
0，表示完全透明，1，表示完全不透明。

#### 什么HSLA？
和RGBA同理。