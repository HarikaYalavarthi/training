* :: is considered one-time binding
* One-time expressions will stop recalculating once if the expression result is a non-undefined value

```html
<div ng-controller="EventController">
	<button ng-click="clickMe($event)">Click Me</button>
	<p id="one-time-binding-example">One time binding: {{::name}}</p>
	<p id="normal-binding-example">Normal binding: {{name}}</p>
</div>
```
