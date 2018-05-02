## task02_03：数组求和

【平均用时 0.03 天】
[【我的代码】](https://github.com/wangsiyuan233/MyDemo/blob/master/task02/03/task02_03.html)
[【效果预览】](https://wangsiyuan233.cn/MyDemo/task02/03/task02_03.html)

### 任务目的
数组求和

### 任务描述
- 分别把 input/bottun/strong的值取出来
- 利用onkeyup控制符合标准的输入
- `sum += parseInt(oInput[i])`

### 任务注意事项
- `input` 里面的 `value` 值是输入框里面的默认值；`<input type="text" value="1,2,3,4,5,6,7" />`
- 不让输入全角符号和英文字母，但是竟然可以输入中文，这个bug咋修复呢？
- `strong.innerHTML = sum` (标签提取物.innerHTML)
- `parseInt()` 函数可解析一个字符串，并返回一个整数。
- `var i in oInput`与`var i = 0; i < input.length; i++`






