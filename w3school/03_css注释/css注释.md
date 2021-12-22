## css注释怎么写
以内部css为例，外部css也是同理。
```html
<style>
	/* 这是一条单行注释 */
	p {
		color: red;
	}
</style>
```

也可以在代码的任何位置添加注释
```html
<style>
	p {
		color: red; /* 把段落的颜色都改为红色 */
	}
</style>
```

而且注释可以横跨多行。
```css
/* 这是
一条多行的
注释 */ 

p {
  color: red;
}
```
