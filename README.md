- window.devicePixelRatio = 物理像素 / dips (设备独立像素)  

- img 一定要设置 width 和 vertical
```css
img {
  vertical-align: middle;
  width: 100%;
}
```

- 当包含 input 的父容器设置 transform: translate(-50%, -50%) 时, input 有可能无法弹出输入法;
```css
div.parent {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```
当前解决办法: 改用 flex 布局来设置垂直水平居中

- 在调用微信的 JS-SDK 时, 一定要设置 link 属性, 否则 JS-SDK 会不生效

- a input button 标签在移动端需要设置触摸高亮隐藏
```css
a, input, button {
  -webkit-tap-highlight-color:rgba(0,0,0,0);
}
```
