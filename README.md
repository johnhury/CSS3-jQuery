CSS3+jQuery������ͼƬ��ͣЧ�����ܹ��ж��������ķ������ֿ��԰�����ķ�����֣�Ҳ���Դӷ�������֣����趨�ӳ�ֵ��

ʹ�÷�����
1����head����������ʽ���ļ�lrtk.css, style.css
2������jquery.min.js��modernizr.custom.97074.js, jquery.hoverdir.js(������)
3������HTML <div class="container">...</div>
<li>
	<a href="http://www.lanrentuku.com/">
		<img src="images/12.jpg" />
		<!-- ���� -->
		<div><span>Seahorse by Trevor Basset</span></div>
	</a>
</li>
4������javascript����

$(function() {

	$(' #da-thumbs > li ').each( function() { $(this).hoverdir({
		hoverDelay : 50, // �����ӳ�
		inverse : true // �Ƿ񷴷������
	}); } );

});

�ɵ����趨ĳ��liԪ��
$('li').hoverdir({
	hoverDelay : 50, // �����ӳ�
	inverse : true // �Ƿ񷴷������
});
