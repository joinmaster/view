<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>小队长，登录一下吧</title>
</head>
<body>
	<nav class="container">
		<h1>登录一下，方便联系</h1>
	</nav>
	<main class="container">
		<div >
			<form action="<?php echo $_SERVER['PHP_SELF']; ?>" method="post">
			  <div class="form-group">
			    <label for="userphone">手机号</label>
			    <div class="code-father">
			    	<input type="tel" class="form-control" id="userphone" name="userphone" aria-describedby="phoneHelp" placeholder="填写手机号">
			    	<input type="button" class="code-box" id="code-box" onclick="sendemail()" value="获取验证码">
			    </div>
			    
			    <small id="phoneHelp" class="form-text text-muted">我们会保障您的隐私安全</small>
			  </div>

			  <div class="form-group">
			  	<label for="usercode">验证码</label>
					<input type="text" class="form-control" id="usercode" name="usercode" placeholder="填写验证码">
			  </div>
        
			  <button type="submit" class="btn btn-primary btn-lg btn-block">登录</button>
			</form>
		</div>
	</main>
	<script src="static/assets/vendors/jquery/jquery-1.12.1.js"></script>
	<script>
		var countdown=60; 
		function sendemail(){
		    var obj = $("#code-box");
		    settime(obj);
		    
		    }
		function settime(obj) { //发送验证码倒计时
		    if (countdown == 0) { 
		        obj.attr('disabled',false); 
		        obj.val("获取验证码");
		        countdown = 60; 
		        return;
		    } else { 
		        obj.attr('disabled',true);
		        obj.val("重新发送(" + countdown + ")");
		        countdown--; 
		    } 
		setTimeout(function() { 
		    settime(obj) }
		    ,1000) 
		}
	</script>
</body>
</html>
