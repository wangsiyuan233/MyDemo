## task05_01：select控件

【平均用时 0.2 天】
[【我的代码】](https://github.com/wangsiyuan233/MyDemo/blob/master/task05/01/task05_01.html)
[【效果预览】](https://wangsiyuan233.cn/MyDemo/task05/01/task05_01.html)

### 任务目的
- 选中的`li`元素出现在`span`元素上：`li[i].onclick = function(){span.innerHTML = this.innerHTML}`

### 任务描述
啊，实现了一个我想要的效果，开心

### 任务注意事项
- `getElementsByTagName`即使只有一个标签，也要指明是第零个；
- `(event||window.event).cancelBubble = true`阻止冒泡；

