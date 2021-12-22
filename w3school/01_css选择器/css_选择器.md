## css选择器
用于查找或选择要设置样式的HTML元素。


## css选择器的五种类型
- 简单选择器：根据名称、id、类来选取元素
- 组合器选择器：根据他们之间的特定关系来选取元素。
- 伪类选择器：根据特定状态选取元素。
- 伪元素选择器：选取元素的一部分并设置其样式。
- 属性选择器：根据属性或属性值来选取元素。


## 简单选择器语法
##### 1.css 元素选择器
根据标签名字选择
```css
p {
  text-align: center;
  color: red;
}
```

#### 2. css id选择器
根据元素的id属性选择。

<font color=red>注意：id名称不能以数字开头。</font>
```css
#para1 {
  text-align: center;
  color: red;
}
```

#### 3. css 类选择器
根据元素的class属性选择。
```css
.center {
  text-align: center;
  color: red;
}
```
<font color=red>注意：class的值不能以数字开头。</font>

还有一些组合用法。
比如同时指定标签和class，比如指定p标签中class为center的元素。
```css
p.center {
  text-align: center;
  color: red;
}
```

#### 4. css 通用选择器
通用选择器用'*'表示，意为选择页面上所有的HTML元素。
```css
* {
  text-align: center;
  color: blue;
}
```

#### 5. css 分组选择器
一般用于，多个类型的元素需要同一种css样式时。

正常写法如下：
```css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}

```

使用分组选择器写法如下：
```css
h1, h2, p {
  text-align: center;
  color: red;
}
```

