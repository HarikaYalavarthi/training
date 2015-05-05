Use it if you want to eval() an Angular expression yourself

```js
$scope.expr = '3*10|currency';
```

```
<div ng-controller="ExampleController" class="expressions">
  Expression:
  <input type='text' ng-model="expr" size="80"/>
  <button ng-click="addExp(expr)">Evaluate</button>
  <ul>
   <li ng-repeat="expr in exprs track by $index">
     [ <a href="" ng-click="removeExp($index)">X</a> ]
     <tt>{{expr}}</tt> => <span ng-bind="$parent.$eval(expr)"></span>
    </li>
  </ul>
</div>
```
