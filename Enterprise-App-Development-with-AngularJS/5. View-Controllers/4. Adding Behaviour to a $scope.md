* We add behavior:
  - To react to events or 
  - To execute computation in the view
* We add behavior to the scope by attaching methods to the $scope object
* These methods are then available to be called from the template/view

```js
var myApp = angular.module('myApp',[]);

myApp.controller('DoubleController', ['$scope', function($scope) {
  $scope.double = function(value) { return value * 2; };
}]);
```

```html
<div ng-controller="DoubleController">
  Two times <input ng-model="num"> equals {{ double(num) }}
</div>
```
