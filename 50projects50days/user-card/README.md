# User-card

> <https://www.bilibili.com/video/BV1wT411J7Ah>

## section

<https://www.geeksforgeeks.org/html-section-tag/>

Section 标签定义文档的部分

## ul>li*3

vscode 快捷键设置,开启emmet

设置搜索emm,找到扩展中的Emmet

![20220713045052](https://raw.githubusercontent.com/learner-lu/picbed/master/20220713045052.png)

勾选两项,可以使用便捷缩写书写,见[vscode-emmet](https://code.visualstudio.com/docs/editor/emmet)

输入ul>li*3 之后使用 <kbd>Tab</kbd>  补齐

## [clip-path](https://developer.mozilla.org/en-US/docs/Web/CSS/clip-path)

创建一个剪辑区域，用于设置元素的哪一部分应该被显示。显示区域内的部分，而隐藏区域外的部分

### [circle](https://developer.mozilla.org/en-US/docs/Web/CSS/basic-shape/circle) 属性

## [position](https://developer.mozilla.org/zh-CN/docs/Web/CSS/position)

默认static,此时 top, right, bottom, left 和 z-index 属性无效

相对定位(relative)的元素并未脱离文档流，而绝对定位(absoluate)的元素则脱离了文档流

![20220713070529](https://raw.githubusercontent.com/learner-lu/picbed/master/20220713070529.png)

![20220713070537](https://raw.githubusercontent.com/learner-lu/picbed/master/20220713070537.png)

固定定位(fixed)在滚动后，它相对于 viewport 视口仍处于同一位置

sticky粘性定位元素在跨越特定阈值前为相对定位，之后为固定定位

[position（absolute、relative、static）](https://zhuanlan.zhihu.com/p/55666883)

### 一个应用场景

在写头像的图片的时候,我们先处理了avatar的css样式

```css
.container .card .content .avatar {
    position: relative;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    overflow: hidden;
    border : 10px solid rgba(0, 0, 0, 0.25);
}
```

现在的效果是

![20220713163343](https://raw.githubusercontent.com/learner-lu/picbed/master/20220713163343.png)

然后我们处理avatar的img的css

```css
.container .card .content .avatar img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
```

之后的效果就正常了

![20220713163420](https://raw.githubusercontent.com/learner-lu/picbed/master/20220713163420.png)

这是因为 `position : absoluate` 是相当于它的父级元素的定位

这样width height的100%就相当于avatar的宽高了

## [obejct-fit](https://developer.mozilla.org/zh-CN/docs/Web/CSS/object-fit)

cover : 被替换的内容在保持其宽高比的同时填充元素的整个内容框。如果对象的宽高比与内容框不相匹配，该对象将被剪裁以适应内容框

## [line-height](https://developer.mozilla.org/zh-CN/docs/Web/CSS/line-height)

多行元素的空间量
