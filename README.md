# slider
Sliding verification (compatible with mobile terminals)
js/css引入<br/>
\<link rel="stylesheet" href="css/jquery.slider.css" /\>
<script type="text/javascript" src="js/jquery.min.js"></script><br/>
<script type="text/javascript" src="js/jquery.slider.min.js"></script><br/>
html模板<br/>
\<div class="container"\><br/>
&nbsp;&nbsp;\<div class="demo"\><br/>
&nbsp;&nbsp;&nbsp;&nbsp;\<div class="btns"\\><br/>
&nbsp;&nbsp;&nbsp;&nbsp;\<button id="reset1"\>还原\</button\><br/>
&nbsp;&nbsp;&nbsp;&nbsp;\</div\> <br/>
&nbsp;&nbsp;&nbsp;&nbsp;\<div id="slider1" class="slider"\>\</div\><br/>
&nbsp;&nbsp;&nbsp;&nbsp;\<div class="result"\>验证结果：\<span id="result1"\>\</span\><br/>
&nbsp;&nbsp;&nbsp;&nbsp;\</div\><br/>
&nbsp;&nbsp;\</div\><br/>
\</div\><br/>
<br/>
script配置<br/>
\<script\><br/>
&nbsp;&nbsp;\$("#slider1").slider({<br/>
&nbsp;&nbsp;&nbsp;&nbsp;callback: function (result) {<br/>
&nbsp;&nbsp;&nbsp;&nbsp;$("#result1").text(result);<br/>
&nbsp;&nbsp;}<br/>
&nbsp;&nbsp;});<br/>
&nbsp;&nbsp;// 还原<br/>
&nbsp;&nbsp;$("#reset1").click(function () {<br/>
&nbsp;&nbsp;&nbsp;&nbsp;$("#slider1").slider("restore");<br/>
&nbsp;&nbsp;});<br/>
\</script\>
<br />
<br />
<p>
可选参数
$("#slider2").slider({
  width: 340, // width
  height: 40, // height
  sliderBg:"rgb(134, 134, 131)",// 滑块背景颜色
  color:"#fff",// 文字颜色
  fontSize: 14, // 文字大小
  bgColor: "#33CC00", // 背景颜色
  textMsg: "按住滑块，拖拽验证", // 提示文字
  successMsg: "验证通过了哦", // 验证成功提示文字
  successColor: "red", // 滑块验证成功提示文字颜色
  time: 400, // 返回时间
  callback: function(result) { // 回调函数，true(成功),false(失败)
    $("#result2").text(result);
  }
});
</p>
