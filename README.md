CSS3+jQuery鼠标跟随图片悬停效果，能够判断鼠标移入的方向，遮罩可以按移入的方向出现，也可以从反方向出现，可设定延迟值。

使用方法：
1、在head区域引入样式表文件lrtk.css, style.css
2、引入jquery.min.js和modernizr.custom.97074.js, jquery.hoverdir.js(函数库)
3、引入HTML <div class="container">...</div>
<li>
	<a href="http://www.lanrentuku.com/">
		<img src="images/12.jpg" />
		<!-- 标语 -->
		<div><span>Seahorse by Trevor Basset</span></div>
	</a>
</li>
4、引入javascript代码

$(function() {

	$(' #da-thumbs > li ').each( function() { $(this).hoverdir({
		hoverDelay : 50, // 控制延迟
		inverse : true // 是否反方向出现
	}); } );

});

可单独设定某个li元素
$('li').hoverdir({
	hoverDelay : 50, // 控制延迟
	inverse : true // 是否反方向出现
});
