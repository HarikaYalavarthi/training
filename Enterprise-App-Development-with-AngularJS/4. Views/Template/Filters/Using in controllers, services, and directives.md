* inject a dependency with the name <filterName>Filter to your controller/service/directive

E.g. using the dependency `numberFilter` will inject the number filter

```js
angular.module('FilterInControllerModule', []).
controller('FilterController', ['filterFilter', function(filterFilter) {
  this.array = [
    {name: 'Tobias'},
    {name: 'Jeff'},
    {name: 'Brian'},
    {name: 'Igor'},
    {name: 'James'},
    {name: 'Brad'}
  ];
  this.filteredArray = filterFilter(this.array, 'a');
}]);
```
