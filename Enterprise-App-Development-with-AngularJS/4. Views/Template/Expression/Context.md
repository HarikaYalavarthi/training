* Do not have access to global variables like window, document or location
  - Prevents accidental access to the global state
* Instead use services like $window and $location in functions called from expressions

```
<div class="example2" ng-controller="ExampleController">
  Name: <input ng-model="name" type="text"/>
  <button ng-click="greet()">Greet</button>
  <button ng-click="window.alert('Should not see me')">Won't greet</button>
</div>
```

```js
angular.module('expressionExample', [])
.controller('ExampleController', ['$window', '$scope', function($window, $scope) {
  $scope.name = 'World';

  $scope.greet = function() {
    $window.alert('Hello ' + $scope.name);
  };
}]);
```
