<!DOCTYPE html>
<html lang="en" dir="ltr">
	<head>
		<meta charset="utf-8">
		<title>BMI Calculator</title>
	</head>
	<style media="screen">
		body{
		margin: 0;
		padding: 0;
		text-align: center;
		font-family: sans-serif;
		background-color: darksalmon;
		min-height: 100vh;
		}
		div{
			background-color: rgb(16, 52, 70);
			width: 300px;
			padding: 60px;
			border-radius: 15px;
			margin:auto;
            margin-top: 6%;
		}
		h2{
			font-size: 30px;
			font-weight: 600;
			color: ghostwhite;
		}
		.text{
			text-align: left;
			margin-left: 3px;
			color: ghostwhite;
		}
			
			#info{
				font-size: 12px;
				font-family: inherit;
			}
	</style>
	<script type="text/javascript">
		function BMI() {
			var h=document.getElementById('h').value;
			var w=document.getElementById('w').value;
			var bmi=w/(h/100*h/100);
			var bmio=(bmi.toFixed(2));

			document.getElementById("result").innerHTML="Your BMI is " + bmio;
		}
	</script>
	<body>
		<div>
			<h2>BMI Calculator</h2>
			<p class="text">Height(in cm)</p>
			<input type="text" id="h">
			<p class="text">Weight(in kg)</p>
			<input type="text" id="w">
			<p id="result"></p>
			<button id="btn" onClick="BMI()">Calculate</button>
		</div>
	</body>
</html>
