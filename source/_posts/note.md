# 地图定位
```
地图的class big-map__content
设置的js操作的class js-game-big-map

```

使用插件

better-scroll
解决移动端（支持pc 的各种场景需求的插件，基于原生的js实现的，轻量级的js lib
https://better-scroll.github.io/docs-v1/doc/zh-hans/#better-scroll%20%E6%98%AF%E4%BB%80%E4%B9%88
滚动绑定在外层元素 wrapper 中，滚动的部分是content元素，bscroll只处理容器的第一个子元素
外层元素设置固定大小
子元素可以超过固定大小后，可在其内部滚动
##### 属性
- startX
number
默认0
横轴的初始化位置

- startY
number
默认0
纵轴初始化位置

- scrollX
boolean
默认false
设置为true 可横向滚动
注意：当设置 eventPassthrough 为 'horizontal' 的时候，该配置无效

- scrollY
boolean
默认true
纵向滚动
当设置 eventPassthrough 为 'vertical' 的时候，该配置无效

- freeScroll
boolean
false
设置成true时，支持横向和纵向同时滚动
当设置 eventPassthrough 不为空的时候，该配置无效。




