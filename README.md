# CSS3-Transform-3D

正确来讲应该是 transform： translate3d()　rotate3d()　scale3d()

####创建舞台场景(-webkit-)

  perspective:　800px;
  
  perspective-origin:　50%　50%;　(默认)
  
  transform-style:preserve-3d;
  
  transform-origin: 50%　50%　0;
  
 [transform-style:preserve-3d;](https://developer.mozilla.org/zh-CN/docs/Web/CSS/transform-style)     子元素
  位于3D场景内（非继承）
  
####变换元素(-webkit-)

   
    transform-origin: x　y　z;
    
    backface-visibility: visible　|　hidden; 默认显示
    
    transform：translate3d(px,px,px)　rotate3d(deg,deg,deg)　scale3d(1,1,1,)；之间用空格分开
    
#####transform-origin的取值

    1.px
    2.%
    3.绕X轴：top  center bottom
    4.绕Y轴：left center right
    
#####通常情况不同变换元素由不同容器单独存放，通常会在变换之前，加上transform-translate-3d(0,0,0,)触发GPU加速

###正负值----方向

　　translateX　　　　　　　　　　－＋(左负-右正)　　
    
　　translateY　　　　　　　　　　－＋(上负-下正)　　　　　　　　　　　　
    
　　translateZ　　　　　　　　　　物体正面方向为正，背面方向为负　　
    
　　rotateX　　　　　　　　　　　 上边向屏幕内滚为正，从侧面看顺时针旋转为正　　[demoX](https://herohql521.github.io/CSS3-Transform-3D/rotateX.html)
    
　　rotateY　　　　　　　　　　　 右边向屏幕内滚为正，从俯视图看逆时针为正　　[demoY](https://herohql521.github.io/CSS3-Transform-3D/rotateY.html)　　　

　　rotateZ　　　　　　　　　　　顺时针为正　　[demoZ](https://herohql521.github.io/CSS3-Transform-3D/rotateZ.html)　　

    
    
