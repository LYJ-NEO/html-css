---
title : Boostrap - 按钮
---

### Boostrap按钮样式

任何带有class .btn 的元素都会继承圆角灰色按钮的默认外观。但是 Bootstrap 提供了一些选项来定义按钮的样式，具体如下表所示。
可用于\<a\>、\<button\>或\<input\>元素。

|类|描述|
|------|------|
|.btn|为按钮添加基本样式|
|.btn-default|默认/标准按钮|
|.btn-primary|原始按钮样式（未被操作）|
|.btn-success|表示成功的动作|	
|.btn-info|该样式可用于要弹出信息的按钮|
|.btn-warning|表示需要谨慎操作的按钮|	
|.btn-danger|表示一个危险动作的按钮操作|
|.btn-link|让按钮看起来像个链接 (仍然保留按钮行为)|
|.btn-lg|制作一个大按钮|
|.btn-sm|制作一个小按钮|
|.btn-xs|制作一个超小按钮|
|.btn-block|块级按钮(拉伸至父元素100%的宽度)|	
|.active|按钮被点击|	
|.disabled|禁用按钮|	

~~~html
<!-- 标准的按钮 -->
<button type="button" class="btn btn-default">默认按钮</button>
<!-- 提供额外的视觉效果，标识一组按钮中的原始动作 -->
<button type="button" class="btn btn-primary">原始按钮</button>
<!-- 表示一个成功的或积极的动作 -->
<button type="button" class="btn btn-success">成功按钮</button>
<!-- 信息警告消息的上下文按钮 -->
<button type="button" class="btn btn-info">信息按钮</button>
<!-- 表示应谨慎采取的动作 -->
<button type="button" class="btn btn-warning">警告按钮</button>
<!-- 表示一个危险的或潜在的负面动作 -->
<button type="button" class="btn btn-danger">危险按钮</button>
<!-- 并不强调是一个按钮，看起来像一个链接，但同时保持按钮的行为 -->
<button type="button" class="btn btn-link">链接按钮</button>
~~~

### 按钮大小

下表列出了获得各种大小按钮的class：

|类|描述|
|.btn-lg|这会让按钮看起来比较大。|
|.btn-sm|这会让按钮看起来比较小。|
|.btn-xs|这会让按钮看起来特别小。|
|.btn-block|这会创建块级的按钮，会横跨父元素的全部宽度。|

~~~html
<div class="col-xs-6 col-sm-6 col-md-6 col-lg-6">
            <p>
            <button type="button" class="btn btn-primary btn-lg">大的原始按钮</button>
            <button type="button" class="btn btn-default btn-lg">大的按钮</button>
            </p>
            <p>
            <button type="button" class="btn btn-primary">默认大小的原始按钮</button>
            <button type="button" class="btn btn-default">默认大小的按钮</button>
            </p>
            <p>
            <button type="button" class="btn btn-primary btn-sm">小的原始按钮</button>
            <button type="button" class="btn btn-default btn-sm">小的按钮</button>
            </p>
            <p>
            <button type="button" class="btn btn-primary btn-xs">特别小的原始按钮</button>
            <button type="button" class="btn btn-default btn-xs">特别小的按钮</button>
            </p>
            <p>
            <button type="button" class="btn btn-primary btn-lg btn-block">块级的原始按钮</button>
            <button type="button" class="btn btn-default btn-lg btn-block">块级的按钮</button>
            </p>
</div>
~~~

### 按钮状态

Bootstrap 提供了激活、禁用等按钮状态的 class。

* 激活状态

按钮元素	添加 .active class 来显示它是激活的。
锚元素	添加 .active class 到 <a> 按钮来显示它是激活的。

~~~html
<p>
  <button type="button" class="btn btn-default btn-lg ">默认按钮</button>
  <button type="button" class="btn btn-default btn-lg active">激活按钮</button>
</p>
<p>
  <button type="button" class="btn btn-primary btn-lg ">原始按钮</button>
  <button type="button" class="btn btn-primary btn-lg active">激活的原始按钮</button>
</p>
~~~

* 禁用状态

按钮元素 添加 disabled 属性 到 <button> 按钮。
锚元素	添加 disabled class 到 <a> 按钮。

~~~html
<p>
  <button type="button" class="btn btn-default btn-lg">默认按钮</button>
  <button type="button" class="btn btn-default btn-lg" disabled="disabled">禁用按钮</button>
</p>
<p>
  <button type="button" class="btn btn-primary btn-lg ">原始按钮</button>
  <button type="button" class="btn btn-primary btn-lg" disabled="disabled">禁用的原始按钮</button>
</p>
<p>
  <a href="#" class="btn btn-default btn-lg" role="button">链接</a>
  <a href="#" class="btn btn-default btn-lg disabled" role="button">禁用链接</a>
</p>
<p>
  <a href="#" class="btn btn-primary btn-lg" role="button">原始链接</a>
  <a href="#" class="btn btn-primary btn-lg disabled" role="button">禁用的原始链接</a>
</p>
~~~

### 按钮组、下拉菜单按钮组、分割按钮

* 在div中直接使用.btn-group可以创建按钮组。

~~~html
<div class="btn-group">
  <button type="button" class="btn btn-primary">Apple</button>
  <button type="button" class="btn btn-primary">Samsung</button>
  <button type="button" class="btn btn-primary">Sony</button>
</div>
~~~

*  可以通过 .btn-group-justified 类来设置自适应大小的按钮组



