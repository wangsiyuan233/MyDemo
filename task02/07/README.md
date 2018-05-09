## task02_07：纯css实现tab切换

【平均用时 1.3 天】
【难度：❀ ❀ ❀】
[【我的代码】](https://github.com/wangsiyuan233/MyDemo/blob/master/task02/07/task02_07.html)
[【效果预览】](https://wangsiyuan233.cn/MyDemo/task02/07/task02_07.html)

## 任务目的
- [超级简陋可调试版本](http://js.jirengu.com/rejehasita/1/edit?html,css,output)
- 用于厘清关系。

## 任务描述
- 通过HTML及CSS实现设计稿
- 整个页面内容宽度固定，

## 任务注意事项
- 只需要完成HTML，CSS代码编写，不需要写JavaScript
- tab只需要实现样式，有能力余力的同学可以尝试实现不使用JavaScript的情况下，实现Tab切换
所有的下拉菜单（Select）均要求按照设计稿样式实现，下拉后的样式自定义，不需要实现下拉选择的功能，但样式要实现
- 在Chrome中完美实现与设计稿的除了文字以外的各项图片、字体、颜色、布局、内外边距等样式

****

## 任务总结
1. 重点：纯CSS实现tab切换

  `<input type="radio" name="pro-material" id="pro-1">`：巧用单选按钮，利用CSS3中`:checked`选择器实现切换功能

  `<label for="pro-1">`：for和`<input>`的id相同，显示单选按钮的文字

  `<div class="pro-table-1">`：没有checked时`display: none;`,checked时`display: block;`

  ```
  <li>
	    <input type="radio" name="pro-material" id="pro-1" checked>
	    <label for="pro-1">项目一</label>
	    <div class="pro-table-1">
	    	<table>...</table>
	    </div>
 </li>
```

2. 边框重叠部分不显示的效果实现方法：
  - 小div的底边框设为none
  - 小div显示在大div上面：小div`position: relative;`，大div`position: absolute;`

  ![](img_error/2017-05-09_170821.png)

**注意！**

1. `<input>`一定要有相同的name属性，否则不属于一个单选按钮，将出现以下错误：
![](img_error/2017-05-09_161822.png)

2. `<input>`一定要有`appearance: none;`或`display:none`的CSS样式，否则将出现以下错误：
![](img_error/2017-05-09_162729.png)

  若使用`appearance: none;`要注意浏览器的兼容性：

  ```
  appearance: none;
  -moz-appearance: none;
  -webkit-appearance: none;
  ```

3. `<li>`和`<label>`都要`float:left;`

  若`<li>`和`<label>`都没有`float:left;`，将出现以下错误：

  ![`<li>`和`<label>`都没有`float:left;`](img_error/2017-05-09_163941.png)

  若`<li>`没有`float:left;`，将出现以下错误：

  ![`<li>`没有`float:left;`](img_error/2017-05-09_163256.png)

  若`<label>`没有`float:left;`，将出现以下错误：

  ![`<label>`没有`float:left;`](img_error/2017-05-09_163832.png)

4. `<div class="pro-table-1">`要使用绝对定位，否则，将出现以下错误：
![](img_error/2017-05-09_164646.png)

  ![](img_error/2017-05-09_164549.png)










