# CSS 选择器

[css dinner](https://flukeout.github.io/)

[答案](https://gist.github.com/chrisman/fcb0a88459cd98239dbe6d2d200b02d1)

## 1. 通过标签选择: bento

![](image/1.gif)

## 2. 通过id: #fancy

```html
<div class="table">
    <plate id="fancy" />
    <plate />
    <bento />
</div>
```

![](image/2.gif)

## 3. 多级标签选择: plate apple

```html
<div class="table">
    <bento />
    <plate>
        <apple />
    </plate>
    <apple />
</div>
```

找到所有plate标签中的apple标签

![](image/3.gif)

## 4. 多级选择: #fancy pickle

```html
<div class="table">
    <bento>
        <orange />
    </bento>
    <plate id="fancy">
        <pickle />
    </plate>
    <plate>
        <pickle />
    </plate>
</div>
```

![](image/4.gif)

可以借助id选择器来定位

## 5. 通过类名(class)定位: .small

```html
<div class="table">
    <apple />
    <apple class="small" />
    <plate>
        <apple class="small" />
    </plate>
    <plate />
</div>
```

![](image/5.gif)

## 6. 标签和class组合: orange.small

![](image/6.gif)

## 7. 标签 class的多级组合: bento orange.small

![](image/7.gif)

## 8. 逗号同时选择多个: bento, plate

![](image/8.gif)

## 9. 选择所有: *

![](image/9.gif)

## 10. 标签和*组合: plate *

![](image/10.gif)

## 11. 选择第一个跟随的元素: plate + apple

![](image/11.gif)

![](image/12.jpg)

## 12. 选择跟在元素有后面的所有某元素: bento ~ pickle

![](image/12.gif)

A~B: 跟在A元素后面的所有B元素(兄弟关系)

## 13. 选择元素的直接子元素: plate > apple

![](image/13.gif)

> 第一个apple并不是直接子元素

## 14. 选择第一个元素: orange:first-child

![](image/14.gif)

![](image/14.jpg)

注意区分有无空格:

- plate:first-child 表示选择所有的第一个plate元素,指定是plate元素
- plate :first-child 表示选择plate中的第一个元素,未指定,第一个就行

## 15. 选择唯一子元素,要求父元素中只有这一个唯一的子元素: plate: only-child

![](image/15.gif)

![](image/15.jpg)

## 16. 选择最后一个元素: .small:last-child

![](image/16.gif)

## 17. 选择第n个元素: :nth-child(3)

> 索引从1开始

![](image/17.gif)

## 18. 选择倒数第n个元素: bento:nth-last-child(3)

![](image/18.gif)

## 19. 根据标签选择某种元素的第一个: apple:first-of-type

![](image/19.gif)

## 20. 特定规则选择: plate:nth-of-type(even)

> even 偶数 | odd 奇数

![](image/20.gif)

## 21. plate:nth-of-type(2n+3)

An+b 的次序不能改变

![](image/21.gif)

## 22. 选择在父类中唯一的元素: plate apple:only-of-type

![](image/22.gif)

## 23. 选择不同标签的最后一个元素: orange:last-of-type, apple:last-of-type

![](image/23.gif)

## 24. 选择空的: bento:empty

![](image/24.gif)

## 25. 选择不包含某种属性的: apple:not(.small)

![](image/25.gif)

## 26. 选择含有某种属性的: [for]

![](image/26.gif)

## 27. 选择属性与标签结合: plate[for]

![](image/27.gif)

## 28. 选择属性具有特定的值: [for='Vitaly']

![](image/28.gif)

## 29. 选择属性的开头值: [for^="Sa"]

![](image/29.gif)

## 30. 选择属性的结尾值: [for$="ato"]

![](image/30.gif)

## 31. 选择属性含有某些值: [for*="obb"]

![](image/31.gif)
