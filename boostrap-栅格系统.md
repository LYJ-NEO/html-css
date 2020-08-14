---
title : Boostrap-网格系统
---

## 什么是网格系统

平面设计中的网格系统使用一个二维框架来对齐和布置设计元素。将单个设计空间分解成网格，可以帮助将单个组件以吸引眼球的方式放置，创建用户流，
并使信息和视觉效果对受众更有吸引力和可访问性。

网格是一种辅助的坐标体系，类似笛卡尔坐标系那样。目的是为了更好设计和编排内容。

在平面设计中，网格是一种由一系列用于组织内容的相交的直线（垂直的、水平的）组成的结构（通常是二维的）。它广泛应用于打印设计中的设计布局和内容结构。在网页设计中，它是一种用于快速创建一致的布局和有效地使用 HTML 和 CSS 的方法。

### Boostrap的网格系统

Bootstrap包含了一个响应式的、移动设备优先的、不固定的网格系统，可以随着设备或视口大小的增加而适当地扩展到12列。它包含了用于简单的布局选项的预定义类，也包含了用于生成更多语义布局的功能强大的混合类。

* 响应式布局，简而言之就是一个网站能够兼容多个终端——而不是为每个终端做一个特定的版本。

说到响应式布局，就不得不提起CSS3中的Media Query（媒介查询），易用、强大、快捷。Media Query是制作响应式布局的一个利器，使用这个工具，可以非常方便快捷的制造出各种丰富的实用性强的界面。

响应式网格系统随着屏幕或视口（viewport）尺寸的增加，系统会自动分为最多12列。

* 视口ViewPort
  viewport是html中的meta标签，就是让移动设备显示的窗口宽度等于设备的真实宽度 width=device-width，可以正常浏览网页。

使用的方法：

<meta name="viewport" content="视口的属性" />
device-height：设备屏幕的输出高度
device-width ：设备屏幕的输出宽度
initial-scale：初始比例，页面加载时的默认比例1.0
user-scalable：指定用户是否可以对页面进行缩放yes允许/no不允许
minimum-scale：最小允许缩放的比率1.0
maximum-scale：最大允许缩放的比率1.0

<meta name=viewport content="width=device-width,initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0, user-scalable=no,minimal-ui">

### 网格系统（Grid System）的工作原理

网格系统通过一系列包含内容的行和列来创建页面布局。下面列出了Bootstrap网格系统是如何工作的：

* row行必须放置在 .container class 内，以便获得适当的对齐（alignment）和内边距（padding）。

* 使用行来创建列的水平组。

* 内容应该放置在列内，且唯有列可以是行的直接子元素

* 预定义的网格类，比如.row和.col-xs-4，可用于快速创建网格布局。LESS混合类可用于更多语义布局。

* 列通过内边距（padding）来创建列内容之间的间隙。该内边距是通过.rows上的外边距（margin）取负，表示第一列和最后一列的行偏移。

* 网格系统是通过指定您想要横跨的十二个可用的列来创建的。例如，要创建三个相等的列，则使用三个.col-xs-4。

boostrap网格基本结构：

~~~html
<div class="container">
   <div class="row">
      <div class="col-*-*"></div>
      <div class="col-*-*"></div>      
   </div>
   <div class="row">...</div>
</div>
<div class="container">....
~~~

