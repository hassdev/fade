<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8" />
<title>js test 003</title>
<link rel="stylesheet" href="reset.css" />
<style>
html, body {
	overflow: hidden;
	padding-right: 17px;
}

html {
	opacity: 0;
	-webkit-transition: opacity 2s;
	transition: opacity 2s;
	height: 0%;
	/*border: solid 1px green;*/
}

body {
	height: 0%;
	/*border: solid 1px orange;*/
}

.show {
	overflow: visible;
}

button {
	width: 10%;
	margin: 5px 0;
}
</style>
</head>

<body>
	<p>数値を入力してください。</p>
	<form>
		横幅：<input type="text" id="inpt1" value="" /><br>
		縦幅：<input type="text" id="inpt2" value="" /><br>
		<button id="fly">計算</button>
	</form>

	<p>this is a paragraph</p><br>

	<p>this is another paragraph</p><br>

	<p>this is another paragraph</p><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>
	<p>this is another paragraph</p><br><br>

	<script>
		//var a = "";
		//alert(a.indexOf("@"));

		//the function "indexOf" returns the position of first occurence of a specified value in a string.
		//関数 "indexOf" は引数に入力した値を文字列から検索して検索した文字列の位置を数字で返す。

		document.getElementById("fly").onclick = test;

		function test() {
			var x = document.getElementById("inpt1").value;
			var y = document.getElementById("inpt2").value;
			if(x === "" || y === "" || isNaN(x) || isNaN(y)) {
				alert("数値を入力してください。");
			}
			else {
				var z = x * y;
				alert(z);
			}
		}
	</script>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
<script>
	$(document).ready(function() {
		var x = function pop() {
			$("html, body").addClass("show").css("padding-right", "0px");
		}

		setTimeout(function() {
			$("html").css("opacity", 1).css("height", "100%");
			$("body").animate({height: "100%"}, 1000, x);
		}, 300);
	});
</script>
</body>
</html>
