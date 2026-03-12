<%@ page language="java" contentType="text/html; charset=UTF-8"
    pageEncoding="UTF-8"%>

<!DOCTYPE html>
<html>
<head>
<title>Student Mark List</title>

<script>
function calculateMarks() {

    let m1 = parseInt(document.getElementById("m1").value);
    let m2 = parseInt(document.getElementById("m2").value);
    let m3 = parseInt(document.getElementById("m3").value);
    let m4 = parseInt(document.getElementById("m4").value);
    let m5 = parseInt(document.getElementById("m5").value);

    let total = m1 + m2 + m3 + m4 + m5;
    let average = total / 5;

    document.getElementById("total").innerText = "Total Marks: " + total;
    document.getElementById("avg").innerText = "Average Marks: " + average;
}
</script>

</head>

<body>

<h2>Student Mark List</h2>

<table border="1">

<tr>
<td>Subject 1</td>
<td><input type="number" id="m1"></td>
</tr>

<tr>
<td>Subject 2</td>
<td><input type="number" id="m2"></td>
</tr>

<tr>
<td>Subject 3</td>
<td><input type="number" id="m3"></td>
</tr>

<tr>
<td>Subject 4</td>
<td><input type="number" id="m4"></td>
</tr>

<tr>
<td>Subject 5</td>
<td><input type="number" id="m5"></td>
</tr>

</table>

<br>

<button onclick="calculateMarks()">Calculate</button>

<p id="total"></p>
<p id="avg"></p>

</body>
</html>
