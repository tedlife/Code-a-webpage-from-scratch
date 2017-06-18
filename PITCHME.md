# 从头开始写一个作品集网页

---

## 项目起始文件（Start Files）

这个部分讲讲如何开始一个项目，一个起始项目文件，应该有些什么和注意的地方

---

### CSS Reset / CSS Normalize

起始文件应当包含 CSS Reset / CSS Normalize。参考下 [HTML5 Reset](https://github.com/murtaugh/HTML5-Reset/) 提供的 Reset 的写法，以及 [Normalize](http://necolas.github.io/normalize.css/) 提供的 Normalize 的写法。

---

### 响应式与移动优先（Mobile First）

项目起始需要选择的原则：Mobile First 还是 PC First。

---

如果是 Mobile First，那么 Media Queries 应当这样写：

```css
// Medium screen rules
@media screen and (min-width: 500px) {
	// rules here
}

// Large screen rules
@media screen and (min-width: 1140px) {
	// rules here
}
```

---

思考：如果是 PC First，那么 Media Queries 改怎样写？

---

响应式网站 `head` 中不要忘记加上这个 `meta`：

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

---

### 语义化及其意义

主要常用语义化标签有：`header`，`nav`，`main`，`footer`，`form`，`table`，`figure`。常用的语义化标签：`div`，`span`

---

语义化的意义是什么？为什么要用语义化元素标签？

* 搜索引擎友好（SEO）
* 代码易阅读且易维护
* 无障碍性（Accessibility）

---

### HTML5 空白模板

最流行的是这个：[html5 boilerplate](https://html5boilerplate.com/)，可以参考下

---

## 最基本的用户体验

用户体验是个涉及广泛的学科，这里只讨论我们写前端代码需要注意的最基本的用户体验

---

### 即时反馈

举最简单几个例子，都可以结合上次直播说说的 CSS 动画来做：

* 鼠标悬停在按钮上，按钮背景颜色等改变
* 提交表单，弹出提交成功的框

---

### 让用户知道自己在哪

网站设计与开发另一个重要的用户体验原则就是：让用户知道自己在哪。体现在我们这个项目里（没有导航），有下面几点：

* 做好 Logo 的指引首页的链接
* 写好 Head 里 `title`
* 网站标题 <h1> 等合理使用

---

其他网站开发中常用的：

* 面包屑导航
* 当前页面菜单项状态

---

## 做这个项目使用什么技术

* Flex / Grid
* Bootstrap 框架，推荐 [bootcss](http://www.bootcss.com/)，[bootwatch](http://bootswatch.com/)
* Float 等其它布局技巧
* 响应式图片，`picture` 标签

---

## 让你的项目更出色

* 使用命名规范 [BEM](http://getbem.com/)，简单，模块化，灵活
* 使用 CSS 预处理器 [SASS](http://sass-lang.com/)，如果你不习惯使用命令行来编译，可以使用软件 [Koala](http://koala-app.com/) 来将 SASS 文件编译成正常 CSS 文件
* 使用自动化任务管理器 [Gulp](http://gulpjs.com/)，需要先安装 node.js 环境


