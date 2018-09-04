# slider
Sliding verification (compatible with mobile terminals)

js/css引入
<link rel="stylesheet" href="css/jquery.slider.css" />
<script type="text/javascript" src="js/jquery.min.js"></script>
<script type="text/javascript" src="js/jquery.slider.min.js"></script>


html模板
<div class="container">
  <div class="demo">
    <div class="btns">
	  <button id="reset1">还原</button>
    </div> 
    <div id="slider1" class="slider"></div>
    <div class="result">验证结果：<span id="result1"></span>
    </div>
  </div>
</div>

script配置
<script>
	$("#slider1").slider({
		callback: function (result) {
			$("#result1").text(result);
		}
	});
	// 还原
	$("#reset1").click(function () {
		$("#slider1").slider("restore");
	});
</script>
