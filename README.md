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

### 版本迁移

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