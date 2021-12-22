## css背景属性用于定义元素的背景效果

#### css背景属性
- background-color
- background-image
- background-repeat
- background-attachment
- background-position

## background-color
用于指定元素的背景色。
```css
body {
  background-color: lightblue;
}
```

也可以指定任何元素的背景色。
```css
h1 {
  background-color: green;
}

div {
  background-color: lightblue;
}

p {
  background-color: yellow;
}
```

opacity属性指定元素的透明度。取值范围0~1。值越低越透明。
```css
div {
  background-color: green;
  opacity: 0.3;
}
```
<font color="red">注意：使用opacity属性为元素指定透明度时，其所有子元素都继承相同的透明度。
这可能会使完全透明的元素内的文字难以阅读。</font>

###### 使用RGBA的透明度
如果不希望对子元素应用不透明度，可以使用RGBA颜色值，这里的alpha仅对应用元素的背景色有效。


## background-image
用于指定图片作为元素的背景图像。
默认情况下，图像会重复，以覆盖整个元素。
```css
body {
  background-image: url("paper.gif");
}
```
<font color="red">注意：如果元素的背景图片颜色和文本的颜色反差较小，将不利于阅读，用户体验很差。</font>


## background-repeat
默认情况下，background-image属性在水平和垂直方向上都会重复图像。

设置水平方向重复：
```css
body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-x;
}
```

<p>若想垂直方向重复，将background-repeat设置为repeat-y。</p>
<p>若是不想重复，将background-repeat设置为no-repeat。</p>

## background-position
用于指定背景图像的位置。
例如，吧背景图片放在右上角：
```css
body {
  background-image: url("tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
```


## background-attachment
指定背景图像是应该滚动还是固定的。

若是固定的，则不会随页面的其余部分一起滚动。
```css
body {
  background-image: url("tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
}
```

若想让其滚动
```css
body {
  background-image: url("tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: scroll;
}
```

## background简写属性
为了减少代码量，css支持简写属性。
比如正常编写属性如下：
```css
body {
  background-color: #ffffff;
  background-image: url("tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
```

可以简化为：
```css
body {
  background: #ffffff url("tree.png") no-repeat right top;
}
```

简写属性时，属性值的顺序为：
1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position

<font color="red">注意：将属性值依次写入，若属性值为空可以不写，一定要保证顺序。</font>
