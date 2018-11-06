
# 响应式设计和断点

## 命名断点 **【_执行_】**

**断点不应该用设备来命名，而应使用更通用的方式。**特别是，现在有一些手机比平板更大，而有一些平板比电脑更大……

{% include snippets/rwd/01/index.html %}

就此来说，任何不与特定设备关联而表达清晰的[命名约定](http://css-tricks.com/naming-media-queries/)，都会因其广泛的通用性获得认可。

{% include snippets/rwd/02/index.html %}

<div class="note">
  <p>上面的示例使用了嵌套的 map，但这并不是强制或绝对的，你完全可以使用字符串来代替（比如 <code>'(min-width: 800px)'</code>）。</p>
</div>

## 断点管理器 **【_参考_】**

一旦用自己钟意的方式命名完断点，就需要有一种方式在实际的媒体查询中使用它。有太多方法可以做这件事，推荐使用 `map-get()` 函数读取断点地图的方法。这套系统简洁而高效。

{% include snippets/rwd/03/index.html %}

<div class="note">
  <p>更多有关 Sass 中媒体查询的信息，请参考 <a href="http://www.sitepoint.com/managing-responsive-breakpoints-sass/">SitePoint</a> 和 <a href="http://css-tricks.com/approaches-media-queries-sass/">CSS-Tricks</a> 中优秀的实践文章。</p>
</div>

## 媒体查询用法 **【_推荐_】**

媒体查询紧贴选择器

{% include snippets/rwd/04/index.html %}

生成结果：

{% include snippets/rwd/05/index.html %}
