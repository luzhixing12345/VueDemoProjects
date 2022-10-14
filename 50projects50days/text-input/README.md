# 输入字段文本动画

效果展示

![input-text](https://raw.githubusercontent.com/learner-lu/picbed/master/input-text.gif)

基本实现参考 : https://www.bilibili.com/video/BV1UT41157KF

按钮样式参考 : https://codepen.io/yuhomyan/pen/OJMejWJ (btn-16)

> 16种很漂亮的按钮样式,CSS动画效果

背景配色:

```css
background-image: linear-gradient(to right, #f6d365 0%, #fda085 100%);
```

输入框样式:

- 复制[CSS文件](../../CSS-style/input/text-input.css)内全部代码
- 应用到一个input标签

  ```html
  <div class="inputBox">
        <input type="text" required="required">
        <span>First Name</span>
  </div>
  ```

按钮样式:

- 复制[CSS文件](../../CSS-style/button/text-input.css)内全部代码
- 应用到一个按钮

  ```html
  <button class="custom-btn btn-style">Submit</button>
  ```

  注意检查 `custom-btn` `btn-style` 是否存在冲突
