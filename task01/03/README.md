## task01_03：网页换肤

【平均用时 0.2 天】
[【我的代码】](https://github.com/wangsiyuan233/MyDemo/blob/master/task01/03/task01_03.html)
[【效果预览】](https://wangsiyuan233.cn/MyDemo/task01/03/task01_03.html)

### 任务目的
将输入的内容拿出来做成弹窗。

### 任务描述
- 需要一个window.onload函数和弹窗函数;
- `button[i].onclick = function(){myFn(input[0],input[1])}`, `onclick`将两个函数连接。

### 任务注意事项
- 由于只取`input`里面的两个值，所以不用在开始的时候遍历`input`;
- 弹窗函数`alert`出来的是 `a.value` 而不是 `a`;
- `var button = document.getElementsByTagName('button')[0]`取button时也是[0]。




