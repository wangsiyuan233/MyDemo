## task01_01：控制div属性

【平均用时 0.2 天】
【难度：❀ ❀】
[【我的代码】](https://github.com/wangsiyuan233/MyDemo/blob/master/task01/01/task01_01.html)
[【效果预览】](https://wangsiyuan233.cn/MyDemo/task01/01/task01_01.html)

### 任务目的
通过不同的按钮，来给`div`改变`style`

### 任务描述
- 功能的实现是由两个JS函数构成的
- 第一个是`changeStyle`函数，它的作用是连接定义好的属性和`button`；
- 第二个函数是一个`for`循环包裹着`click`事件。

### 任务注意事项
- `window.onload`在启动页面时就要把各个按钮配置好，所以它下面需要`var`很多变量；
- 第二步是遍历每一个`oBtn[i]`,使前四个按钮对号入座，第五个按钮为`diaplay:none`;
- `this`指向的是调用它的函数--`oBtn[i]`；
- 调用`changeStyle`，连接属性和`button`。

