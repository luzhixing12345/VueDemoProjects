# 鼠标输入方格

## CSS

- overflow

  ```css
  overflow: hidden;
  ```

  当一个元素的内容太大而无法适应

  <https://developer.mozilla.org/zh-CN/docs/Web/CSS/overflow>

- margin

  元素周围创建空间,在任何定义的边界之外

  - 4个值为 上 右 下 左
  - 3个值为 上 左右 下
  - 2个值为 上下 左右
  - 1个值为 四边距离

  auto为水平居中

  ```css
  margin : 0 auto // 上下边界0,水平距离相同
  ```

  inherit : 继承父元素的margin

- 计算元素的宽度和高度

  https://developer.mozilla.org/zh-CN/docs/Web/CSS/box-sizing

  ```css
  * {
    box-sizing: border-box;
  }
  ```

  > 一般来说都设置这一项,便于计算