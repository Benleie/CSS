## flex-box-demo Flex 布局示例

> 感谢阮一峰老师的教程 http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html

本示例将教程上所有的布局都简单的实现了一遍，预览地址：http://static.vgee.cn/static/index.html

## inline
+ inline元素无法设置`width, height, margin-top, margin-bottom`,inline-block元素则可以
	+ img,input

## common css
+ 某元素使用`margin:0 auto;`无效
	+ 该元素没有指定width
	+ 该元素display属性不为block, inline-block也不行
	+ 该元素有浮动？