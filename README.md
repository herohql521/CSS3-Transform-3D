# CSS3-Transform-3D

正确来讲应该是 transform： translate3d()　rotate3d()　scale3d()

####创建舞台场景(-webkit-)

  perspective:　800px;
  
  perspective-origin:　50%　50%;　(默认)
  
####变换元素(-webkit-)

    transform-style:preserve-3d;
    
    transform-origin: x　y　z;
    
    background-visibility: visibile　|　hidden; 默认显示
    
    transform：translate3d(px,px,px)　rotate3d(deg,deg,deg)　scale3d(1,1,1,)；之间用空格分开
    
#####transform-origin的取值

    1.px
    2.%
    3.绕X轴：top  center bottom
    4.绕Y轴：left center right
    
#####通常情况不同变换元素由不同容器单独存放，通常会在变换之前，加上transform-translate-3d(0,0,0,)触发GPU加速

    
    
