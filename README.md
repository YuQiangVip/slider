# slider
Sliding verification (compatible with mobile terminals)
<br/>
js/css引入
<br/>
<link rel="stylesheet" href="css/jquery.slider.css" /><br/>
<script type="text/javascript" src="js/jquery.min.js"></script><br/>
<script type="text/javascript" src="js/jquery.slider.min.js"></script><br/>
<br/>
html模板<br/>
<div class="container"><br/>
  <div class="demo"><br/>
    <div class="btns"><br/>
	  <button id="reset1">还原</button><br/>
    </div> <br/>
    <div id="slider1" class="slider"></div><br/>
    <div class="result">验证结果：<span id="result1"></span><br/>
    </div><br/>
  </div><br/>
</div><br/>
<br/>
script配置<br/>
<script><br/>
	$("#slider1").slider({<br/>
		callback: function (result) {<br/>
			$("#result1").text(result);<br/>
		}<br/>
	});<br/>
	// 还原<br/>
	$("#reset1").click(function () {<br/>
		$("#slider1").slider("restore");<br/>
	});<br/>
</script>
