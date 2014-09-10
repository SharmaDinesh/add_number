add_number
==========
 File Name : index.html

<!DOCTYPE html>
<html ng-app="myApp">

<head>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.0.8/angular.min.js"></script>
<script src="script.js"></script>
</head>


<body>
<h1>Hello {{name}} ! </h1>
Number 1  : <input  type="text" ng-model="num1" />

Number 2  : <input  type="text" ng-model="num2" />
<h5> Result : {{result}}</h5>
<input type="button"  value="add" ng-click="add(num1,num2)"/>
</body>

</html>


Script Name : script.js

var app = angular.module('myApp', []);

app.controller('MainCtrl', function($scope) {
$scope.add=function(num1,num2)
{
  $scope.result=num1+num2;

}

});

OutPut:

Adding Two Numbers 
Number 1 : 40
Number 2 : 20
Total:60





