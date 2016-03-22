# zhu
测试用例
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>响应式设计</title> 
	<style type="text/css">
			*{
	margin:0;
	padding: 0;
}
ul,ol{
	list-style: none;
}
a{
	text-decoration: none;
}

.body{
  box-sizing: border-box;
}
.same{
	border: solid 1px #999;
	background: #eee;
	 margin-top: 20px;
	 margin-left: 20px;
	 float: left;
	 height: 50px;
}
.row:before,
.row:after{
				content: "";
				display: table;
				clear: both;
			}
/*屏幕宽度大于769px时*/
@media all and (min-width: 769px){
				.col-md-1{ width: calc(8.33% - 20px);}
				.col-md-2{ width: calc(16.4% - 20px);}
				.col-md-3{ width: calc(25.0% - 20px);}
				.col-md-4{ width: calc(33% - 20px);}
				.col-md-6{ width: calc(49% - 20px);}
			}

/* 屏幕宽度小于769px时*/
@media all and (max-width: 768px){
	  			.col-sd-2{width: calc(16.0% - 20px);}
	  			.col-sd-3{width: calc(24% - 20px);}
	  			.col-sd-6{width: calc(49% - 20px);}
	  			.col-sd-8{width: calc(64% - 20px);}
	  			.col-sd-12{width: calc(98.5% - 20px);}

	</style>
</head>
<body>
<div clas="body">
<div class="row">
		<div class="same col-md-4 col-sd-6"> </div>
		<div class="same col-md-4 col-sd-6"> </div>
		<div class="same col-md-4 col-sd-12"> </div>
</div>

<div class="row">
		<div class="same col-md-3 col-sd-3 "> </div>
		<div class="same col-md-6 col-sd-6"> </div>
		<div class="same col-md-3 col-sd-3"> </div>
</div>

<div class="row">
		<div class="same col-md-1 col-sd-2"> </div>
		<div class="same col-md-1 col-sd-2"> </div>
		<div class="same col-md-2 col-sd-8"> </div>
		<div class="same col-md-2 col-sd-3"> </div>
		<div class="same col-md-6 col-sd-3"> </div>

</div>

</div>
</body>
</html>
