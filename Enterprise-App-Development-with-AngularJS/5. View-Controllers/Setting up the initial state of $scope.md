* Set up the initial state of a scope by attaching properties to the $scope object
* The properties contain the view model
* All the $scope properties will be available to the template at the point in the DOM where the Controller is registered

```js
var myApp = angular.module('myApp',[]);

myApp.controller('GreetingController', ['$scope', function($scope) {
  $scope.greeting = 'Hola!';
}]);
```

```html
<div ng-controller="GreetingController">
  {{ greeting }}
</div>
```
