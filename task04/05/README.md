## task04_05：一键读取css属性

【平均用时 0.1 天】
[【我的代码】](https://github.com/wangsiyuan233/MyDemo/blob/master/task04/05/task04_05.html)
[【效果预览】](https://wangsiyuan233.cn/MyDemo/task04/05/task04_05.html)

### 任务目的
- 读取不同的属性值

### 任务描述
- 第一函数用来规定传参办法，第二个函数调用第一个函数

### 任务注意事项
- 我们使用`element.style`也可以获取元素的CSS样式声明对象，但是其与`getComputedStyle`方法还有有一些差异的。
1、只读与可写
正如上面提到的`getComputedStyle`方法是只读的，只能获取样式，不能设置；而`element.style`能读能写，能屈能伸。
2、获取的对象范围
`getComputedStyle`方法获取的是最终应用在元素上的所有CSS属性对象（即使没有CSS代码，也会把默认的祖宗八代都显示出来）；而`element.style`只能获取元素`style`属性中的`CSS`样式。因此对于一个光秃秃的元素`<p>`，`getComputedStyle`方法返回对象中`length`属性值（如果有）就是190+(据我测试FF:192, IE9:195, Chrome:253, 不同环境结果可能有差异), 而`element.style`就是0。
- `currentStyle`是IE浏览器自娱自乐的一个属性，其与`element.style`可以说是近亲，至少在使用形式上类似，`element.currentStyle`，差别在于`element.currentStyle`返回的是元素当前应用的最终CSS属性值（包括外链CSS文件，页面中嵌入的`<style>`属性等）。

因此，从作用上将，`getComputedStyle`方法与`currentStyle`属性走的很近，形式上则`style`与`currentStyle`走的近。不过，`currentStyle`属性貌似不支持伪类样式获取，这是与`getComputedStyle`方法的差异，也是jQuery `css()`方法无法体现的一点。








