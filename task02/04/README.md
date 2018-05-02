## task02_04：弹层

【平均用时 0.03 天】
[【我的代码】](https://github.com/wangsiyuan233/MyDemo/blob/master/task02/04/task02_04.html)
[【效果预览】](https://wangsiyuan233.cn/MyDemo/task02/04/task02_04.html)

### 任务目的
点击按钮弹层

### 任务描述
- 创建一个大的透明层，点击按钮时候激活；点击x时候关闭；

### 任务注意事项
- 重点在于html里的三个div;第一个是 全屏50%透明度的 overlay;第二个是 中间提示框 win;第三个是 button 按钮；
- 【overlay 大透明遮罩一定要在 win 之前】，其他顺序随意。
- 还是不能够点击其他位置退出弹层，需要用到JQ的.one来实现这一个功能
- `document.getElementsByTagName("button")[0]`因为是TagName,所以要取第一个值。








