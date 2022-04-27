<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="stylesheet" type="text/css" href="onlineattendance.css">
	<link rel="icon" type="image/x-icon" href="hindusthan.jpg">
	<title>Attendance sheet</title>
</head>

<style type="text/css">
	*
{
	padding: 0;
	margin: 0;
	font-family: sans-serif;
}
.form
{
	height: 100%;
	width: 100%;
	background-image: linear-gradient(rgba(0, 0, 0, 0.4),rgba(0, 0, 0, 0.4)),url(hindusthanbackground.jpg);
	background-position: center;
	background-size: cover;
	position: absolute;
}
.form-box
{
	width: 380px;
	height: 480px;
	position: relative;
	margin: 6% auto;
	background: #fff;
	padding: 5px;
	border-radius: 30px;
	overflow: hidden;
}
.button-box
{
	width: 220px;
	margin: 35px auto;
	position: relative;
	box-shadow: 0 0 20px 9px #ff61241f;
	border-radius: 30px;
}
.toggle-btn
{
	padding: 10px 30px;
	cursor: pointer;
	background: transparent;
	border: 0;
	outline: none;
	position: relative;
}
#btn
{
	top: 0;
	left: 0;
	position: absolute;
	width: 110px;
	height: 100%;
	background: linear-gradient(to right, #5A5BF3,#01E7D9);
	border-radius: 30px;
	transition: .5s;
}
.input-group
{
	top: 180px;
	position: absolute;
	width: 280px;
	transition: .5s;
}
.input-field
{
	width: 100%;
	padding: 10px 0;
	margin: 5px 0;
	border-left: 0;
	border-right: 0;
	border-top: 0;
	border-bottom: 1px solid #999;
	outline: none;
	background: transparent;
}
.submit-btn
{
	width: 100%;
	padding: 10px 30px;
	cursor: pointer;
	display: block;
	margin: auto;
	background: linear-gradient(to right, #5A5BF3,#01E7D9);
	border: 0;
	outline: none;
	border-radius: 30px;
	position: relative;
	top: 15px;
}
.forgot
{
	margin: 30px 10px 30px 0;
	color: blue;
	font-size: 15px;
	bottom: -80px;
	position: absolute;	
	text-decoration: none;
}
.forgot:hover
{
	color: violet;
}
#admin
{
	left: 50px;

}
#student
{
	left: 450px;	
}
</style>

<body>

<div class="form">
	<div class="form-box">
		<div class="button-box">
			<div id="btn"></div>
			<button type="button" class="toggle-btn" onclick="admin()">Admin</button>
			<button type="button" class="toggle-btn" onclick="student()">Student</button>
		</div>
		  <form id="admin" class="input-group">
			<input type="text" class="input-field" placeholder="Email" required/>
			<input type="text" class="input-field" placeholder="Password" required/>
			<button type="submit" class="submit-btn">Login</button>
			<a href="#" class="forgot">Forgot Password?</a>
		  </form>
		  <form id="student" class="input-group">
			<input type="text" class="input-field" placeholder="Roll number" required/>
			<input type="date" class="input-field" placeholder="email id" required/>
			<!-- <input type="checkbox" class="check-box"><span>I agree to the terms and conditions</span> -->
			<button type="submit" class="submit-btn">Login</button>
		  </form>
	</div>
</div>

<script type="text/javascript">
	var x = document.getElementById("admin");
	var y = document.getElementById("student");
	var z = document.getElementById("btn");

	function student()
	{
		x.style.left = "-400px";
		y.style.left = "50px";
		z.style.left = "110px";
	}
	function admin()
	{
		x.style.left = "50px";
		y.style.left = "450px";
		z.style.left = "0px";
	}
</script>

</body>
</html>
