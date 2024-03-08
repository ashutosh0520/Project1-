<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<script src="https://cdn.tailwindcss.com"></script>
<title>JavaScript Operators Practice</title>
<style>
  body {
    font-family: 'Popins', Tahoma, Geneva, Verdana, sans-serif;
    background-color: rgb(253, 252, 193);
   text-align: center;
    padding: 50px;
  }
  h1 {
    color: #db5353;
  
  }
  p {
    margin: 20px 0;
  }
  input[type="number"] {
    padding: 10px;
    margin: 10px;
    border: 2px solid #0c0000;
    border-radius: 5px;
  
  }
  button {
    padding: 10px 20px;
    background-color: #13a9c7;
    color: rgb(11, 119, 168);
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  button:hover {
    background-color: #95f8fa;
  }
  #result {
    margin-top: 20px;
  }
</style>
</head>
<body>
<h1>Practice JavaScript Operators</h1>
<p>Enter two numbers:</p>
<input type="number" id="num1" placeholder="Number 1">
<input type="number" id="num2" placeholder="Number 2">
<button onclick="performOperations()">Calculate</button>
<p id="result"></p>

<script>
function performOperations() {
  var num1 = document.getElementById('num1').value;
  var num2 = document.getElementById('num2').value;
 
  num1 = Number(num1);
  num2 = Number(num2);
 
  var add = num1 + num2;
  var subtract = num1 - num2;
  var multiply = num1 * num2;
  var divide = num1 / num2;
 
  document.getElementById('result').innerHTML = 'Addition: ' + add + '<br>' +
                                                'Subtraction: ' + subtract + '<br>' +
                                                'Multiplication: ' + multiply + '<br>' +
                                                'Division: ' + divide;
}
</script>
</body>
</html>
