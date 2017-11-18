# project1
web
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<script src="http://cdn.static.runoob.com/libs/angular.js/1.4.6/angular.min.js"></script>
<style>
ul {
    list-style-type: none;
    margin: 2;
    padding: 0;
    overflow: hidden;
    background-color: #333;
}

li {
    float: left;
}

li a {
    display: block;
    color: white;
    text-align: center;
    padding: 10px 14px;
    text-decoration: none;
}

li a:hover {
    background-color: #111;
}
.active {
    background-color: #4CAF50;
	a-color: #333;
}
</style>
</head>
<body>
 <ul>
  <li><a href="#home">邮箱</a></li>
  <li><a href="#news">联系人</a></li>
  <li><a href="#contact">日历</a></li>
  <li><a href="#about">任务</a></li>
  <li><a href="#about">公文包</a></li> 
  <li><a href="#about">首选项</a></li>
  <li><a href="#about">常见问题</a></li>
  <li><a class="active" href="#about">写信</a></li>
</ul>
<form ng-app="" name="myForm">
    <button ng-click="reciver()">收件人：</button>
    <input type="email" name="myAddress" ng-model="text">
    <span ng-show="myForm.myAddress.$error.email">不是一个合法的邮箱地址</span>
</form>
 
</body>
</html>
