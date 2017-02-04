1 window.devicePixelRatio = 物理像素 / dips (设备独立像素)  
2 img 一定要设置 width 和 vertical
```css
img {
  vertical-align: middle;
  width: 100%;
}
```

3 当包含 input 的父容器设置 transform: translate(-50%, -50%) 时, input 有可能无法弹出输入法;
```css
div.parent {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```
当前解决办法: 改用 flex 布局来设置垂直水平居中

4 在调用微信的 JS-SDK 时, 一定要设置 link 属性, 否则 JS-SDK 会不生效
