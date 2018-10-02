# showHide-component
css3 &amp; jquery 显示隐藏 动画效果 插件
### 兼容主流浏览器chrome和IE9+等，同时兼容IE6 7 8
### 目前支持: 
淡入淡出 (fade)
上滑动收起，下滑动展开(slideUpDown)
左滑动收起，右滑动展开(slideLeftRight)
淡出上滑动收起，淡入下滑动展开(fadeSlideUpDown)
淡出左滑动收起，淡入右滑动展开(fadeSlideLeftRight)

## 使用前提
导入transition.css （注意自定义样式不要和transition.css的样式名冲突）
```
<link rel="stylesheet" href="../css/transition.css">
```

依次导入
  jquery.js
  transition.js
  showHide.js
```
<script src="../js/jquery-3.3.1.js"></script>
<script src="../js/transition.js"></script>
<script src="../js/showHide.js"></script>
 ```
 
 ## 使用方式
 ```
// 插件的初始化方式
$box.showHide({
  css3: false,
  js: false,
  animation: "slideUpDown"           
});
btnShow.on("click", function () {
  // 插件的展示调用
  $box.showHide("show");
});
btnHide.on("click", function () {
  // 插件的隐藏调用
  $box.showHide("hide");
});
// 插件的显示前，显示后，隐藏前，隐藏后的回调函数
$box.on("show shown hide hidden", function (e) {
  console.log(e.type);
});        
```
 
 
