
# 命名约定

推荐遵从 [CSS Guidelines](http://cssguidelin.es/#naming-conventions) 的建议。

良好的命名对保持整体代码的一致性和可读性非常重要，在 Sass 中可以命名的地方如下：

- 变量；
- 函数；
- 混合宏。

由于 Sass 占位符遵循和类名相同的命名模式，因此被视为常规的 CSS 选择器，也就在这个列表中故意忽略掉了。

就变量、函数和混合宏的命名而言，我们坚持一些很 *CSS-y* 的风格：**小写连字符分隔**，有意义的命名。

{% include snippets/naming/01/index.html %}

## 常量 **【_执行_】**

对于众多编程语言，我建议使用全大写方式书写常量。这不仅是一个由来已久的编程习惯，而且可以很好的与小写连字符变量加以区别。

{% include snippets/naming/02/index.html %}

如果你在 Sass 中使用常量，请参考这篇文章：[如何在 Sass 中使用常量](http://www.sitepoint.com/dealing-constants-sass/).

## 命名空间 **【_推荐_】**

如果你打算分发你的 Sass 代码，比如一个库、框架、栅格系统或者其他的什么，为了防止与其他人的代码发生冲突，你就可能会考虑使用命名空间包裹你所有的变量、函数、混合宏和占位符。

举例来说，如果你参加了一个名为 *Sassy Unicorn* 的项目 —— 这意味着你可以向其贡献代码，你可能会考虑使用 `su-` 作为一个命名空间。这确实非常独特，既不会引发命名冲突，又足够短小而没有书写困难。

{% include snippets/naming/03/index.html %}

关于 CSS 的全局命名，[Kaelig](http://kaelig.fr) 写过 [一篇非常具有思考价值的文章](http://blog.kaelig.fr/post/44554267597/please-respect-the-global-css-namespace)。

<div class="note">
  <p>需要注意的是，自动命名空间功能绝对是即将到来的Sass4.0中重构的<code>@import</code>的一个设计目标。随着即将取得结果，将会越来越少的需要手动命名，最终，手动命名库名实际上会越来越难用。</p>
</div>
