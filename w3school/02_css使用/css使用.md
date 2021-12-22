## 3种使用css的方法
- 外部css
- 内部css
- 行内css

## 外部css
外部css是指通过外部样式表(css文件)，只修改一个文件即可修改整个网站的外观。
每张HTML页面必须在head部分的link元素中进行定义。
```html
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

mystyle.css
```css
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```
<font color=red>注意：在css中，值和单位之间不能有空格！</font>

## 内部css
如果一张HTML页面拥有唯一的样式，那么可以使用内部样式表。
内部样式表是在head部分style元素中定义的。

例如：
```html
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
} 
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

## 行内css
行内样式，也称为内联样式。
一般用于单个元素应用唯一的样式。
```html
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```
<font color="yellow">提示：行内样式会将内容和呈现混合在一起。请谨慎使用。</font>

## 多个样式表
如果不同的样式表为同一个选择器（元素）定义了一些属性，则将使用最后读取的样式表中的值。


## 层叠顺序
当某个HTML元素指定了多个样式时，会使用哪种样式呢？
页面中所有样式将按照以下规则"层叠"为新的虚拟样式表，优先级从高到低，如下：
1. 内行样式（内联样式），也就是写在html元素中的style。
2. 外部和内部样式表（head标签部分），如果内容有冲突，后引用的会覆盖先引用的。
3. 浏览器默认样式。
