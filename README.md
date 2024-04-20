<!DOCTYPE html>
<html>
<body>

<h1>Hello, I'm Grim!</h1>

<p>Testing a few things out...</p>

<h1>Chess Board</h1>

<!-- Your chess board here -->

<p>Enter your move:</p>
<input type="text" id="move" name="move">
<button onclick="createLink()">Submit</button>

<p id="link"></p>

<script>
function createLink() {
  var move = document.getElementById("move").value;
  var link = "http://localhost:8080/api/chess/play?move=" + move;
  document.getElementById("link").innerHTML = '<a href="' + link + '">Make a move</a>';
}
</script>

</body>
</html>
