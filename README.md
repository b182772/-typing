<!DOCTYPE html>
<html long="ja">
<head>
<meta charset="utf-8">
<title>フラッシュタイピング練習</title>
</head>
<body>
<form method="post">
<input type="text" id="name"></p>
</form>
<script>
function getRndStr(){
  var str = document.getElementById("name").value;
  var len = 2;
  var result = "";
  for(var i=0;i<len;i++){
    result += str.charAt(Math.floor(Math.random() * str.length));
  }
  return result;
}
function test(){
  document.getElementById("area1").innerHTML = getRndStr();
}
</script>
<input type="button" value=" ボタン " onclick="test();" style="width:100px;margin:5px;">
<div id="area1" class="result" style="position: absolute; left: 300px; top: 150px; font-size:100pt;"  </div>
</body>
</html>
