### task01_01：控制div属性

【平均用时 0.2 天】
[【我的代码】]()
[【效果预览】]()

### 任务目的
通过不同的按钮，来给div改变style

### 任务描述
- 功能的实现是由两个JS函数构成的
- 第一个是changeStyle函数，它的作用是连接定义好的属性和button；
- 第二个函数是一个for循环包裹着click事件。

### 任务注意事项
- window.onload在启动页面时就要把各个按钮配置好，所以它下面需要var很多变量；
- 第二步是遍历每一个oBtn[i],使前四个按钮对号入座，第五个按钮为diaplay:none;
- this指向的是调用它的函数--oBtn[i]；
- 调用changeStyle，连接属性和button。

