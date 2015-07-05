# CANVAS_learn
##入门
###创建canvas
`<canvas id="c" width="1024" height="768"></canvas>`
不建议用CSS设置
```
var canvas = document.getElementById('c');
var context = canvas.getContext('2d');
// 使用context绘制
```

###绘制直线、多边形和七巧板
####直线，多边形
```
context.moveTo(100, 100);
context.lineTo(700, 700);
context.lineWidth = 5;
context.strokeStyle= "#ff0000";
context.stroke();

context.fillStyle = "#00ff00";
context.fill();

// 画多个直线或者多边形
context.beginPath();
context.closePath();
```
####弧和园
```
context.arc(
    centerx, centery, radius,
    startingAngle, endingAngle,
    anticlockwise = false
)
```

####实战
电子时钟[http://lishengzxc.github.io/CANVAS_learn/clock/](http://lishengzxc.github.io/CANVAS_learn/clock/)

###线条的属性
 - lineCap
 - butt
 - round
 - square
