<!DOCTYPE html>
<html>
<head>
  <title>Access Page</title>
</head>
<body>

<h2>Enter Access Values</h2>

<input type="text" id="value1" placeholder="First value">
<input type="text" id="value2" placeholder="Second value">
<button onclick="checkAccess()">Submit</button>

<p id="result"></p>

<script>
function checkAccess() {
  const v1 = document.getElementById("value1").value;
  const v2 = document.getElementById("value2").value;

  if (v1 === "alpha" && v2 === "beta") {
    window.location.href = "secret1.html";
  } else if (v1 === "gamma" && v2 === "delta") {
    window.location.href = "secret2.html";
  } else {
    document.getElementById("result").innerText = "Access denied";
  }
}
</script>

</body>
</html>
