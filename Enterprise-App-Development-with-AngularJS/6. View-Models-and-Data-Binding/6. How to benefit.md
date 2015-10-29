* If the expression will not change once set, it is a candidate for one-time binding
* When interpolating text or attributes
  
  ```html
  <div name="attr: {{::color}}">text: {{::name}}</div>
  ```
* When using a directive with bidirectional binding and the parameters will not change

  ```js
  someModule.directive('someDirective', function() {
  	return {
  		scope: {
  			name: '=',
  			color: '@'
  		},
  		template: '{{name}}: {{color}}'
  	};
  });
  ```

* When using a directive that takes an expression

  ```html
  <ul>
  	<li ng-repeat="item in ::items">{{item.name}};</li>
  </ul>
  ```
