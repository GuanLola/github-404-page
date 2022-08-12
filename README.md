<div align="center">
  <h1>Github-404-page</h1>
  <p>仿github404页面, 实现图片层次轴动特效</p>
  <a>
    <img src="https://img.shields.io/badge/license-MIT-green" alt="license">
  </a>
</div>

[简体中文](./README.md)

> error页面，404。

## 目录

1. [html](./_error.html)
2. [css](./static/css/_error.css)
3. [js](./static//js/_error.js)
4. [imgs](./static/imgs)

## 简介

仿github404页面, 实现图片层次轴动特效.

### 版本

1.0


代码示例

```javascript
// window.plaxify
var layers = document.querySelectorAll('.js-plaxify')
		
for (var layer, i = 0; layer = layers[i]; i++) {
  window.plaxify(layer, {
      xRange: layer.getAttribute('data-xrange'),
      yRange: layer.getAttribute('data-yrange')
  })
}
```

# 文件

## CSS 相关

CSS定位

## js相关

一个plaxify.js库

## images相关

github-404页面相关资源图片


# 示例效果

废话少说，先看效果如图所示:

![res.gif](./static/result-imgs/res.gif)

# 重要代码

plaxify.js是整个页面的核心，它封装了移动功能，函数使用说明如下：

```
// HTMLDomElement 需要这个效果的dom元素
window.plaxify(HTMLDomElement, {
  xRange: Number, // x轴移动的最大范围
  yRange: Number, // y轴移动的最大范围
  invert: Boolean // 是否与鼠标移动方向相反
})
```