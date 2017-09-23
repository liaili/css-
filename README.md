
*最近在看一本叫做《css揭秘》的书，认识了一些css的属性，这些小技巧可以解决很多开发的问题，所以我记录下来了，同时希望对别人有帮助。

## 一，半透明边框
*在css2.1中，背景色是延伸到边框所在的区域下层，所以如果边框的颜色和背景色是一样的，那就看不到边框的颜色了。
*解决方案：我们可以通过background-clip属性来改变背景色的显示区域。这个属性的默认值是border-box，背景色会延伸到边框下面；把值设置为padding-box，
背景色就只会延伸到内边距，不包含边框。以下是例子：   
`
border:10px solid rgba(255,255,255,0.5);    
background:white;   
background-clip: padding-box;
`
