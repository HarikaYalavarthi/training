

```
<div ng-app="MyModule" ng-controller="PayController as pay">
	<span>Go ahead and pay {{pay.pymt.whom}} INR {{pay.pymt.amt}}.</span>
    <button class="btn" ng-click="pay.pay()">Pay</button>
    <p></p>
    <b>{{pay.pymt.status}}</p>
</div>
```
