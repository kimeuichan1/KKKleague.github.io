# KKKleague.github.io
스탯계산기
<!DOCTYPE html>
<html>
<body>

<h1>KKK리그 스탯계산기</h1>

<label for="방문">방문 수:</label><br>
<input type="number" id="방문" name="방문"><br>
<label for="게시글">게시글 수:</label><br>
<input type="number" id="게시글" name="게시글"><br>
<label for="댓글">댓글 수:</label><br>
<input type="number" id="댓글" name="댓글"><br>

<button onclick="계산()">계산하기</button>

<p id="결과"></p>

<script>
function 계산() {
  var 방문 = document.getElementById("방문").value;
  var 게시글 = document.getElementById("게시글").value;
  var 댓글 = document.getElementById("댓글").value;

  var 스탯 = (방문 / 50) + (게시글 / 20) + (댓글 / 100);

  document.getElementById("결과").innerHTML = "계산된 스탯은 " + 스탯 + "입니다.";
}
</script>

</body>
</html>
