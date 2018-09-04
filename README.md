# slider
Sliding verification (compatible with mobile terminals)<br/>
js/css引入<br/>
\<link rel="stylesheet" href="css/jquery.slider.css" /\><br/>
<script type="text/javascript" src="js/jquery.min.js"></script><br/>
<script type="text/javascript" src="js/jquery.slider.min.js"></script><br/>
html模板<br/>
<div class="container"><br/>
&nbsp;&nbsp;<div class="demo"><br/>
&nbsp;&nbsp;&nbsp;&nbsp;<div class="btns"><br/>
&nbsp;&nbsp;&nbsp;&nbsp;<button id="reset1">还原</button><br/>
&nbsp;&nbsp;&nbsp;&nbsp;</div> <br/>
&nbsp;&nbsp;&nbsp;&nbsp;<div id="slider1" class="slider"></div><br/>
&nbsp;&nbsp;&nbsp;&nbsp;<div class="result">验证结果：<span id="result1"></span><br/>
&nbsp;&nbsp;&nbsp;&nbsp;</div><br/>
&nbsp;&nbsp;</div><br/>
</div><br/>
<br/>
script配置<br/>
<script><br/>
&nbsp;&nbsp;$("#slider1").slider({<br/>
&nbsp;&nbsp;&nbsp;&nbsp;callback: function (result) {<br/>
&nbsp;&nbsp;&nbsp;&nbsp;$("#result1").text(result);<br/>
&nbsp;&nbsp;}<br/>
&nbsp;&nbsp;});<br/>
&nbsp;&nbsp;// 还原<br/>
&nbsp;&nbsp;$("#reset1").click(function () {<br/>
&nbsp;&nbsp;&nbsp;&nbsp;$("#slider1").slider("restore");<br/>
&nbsp;&nbsp;});<br/>
</script>
