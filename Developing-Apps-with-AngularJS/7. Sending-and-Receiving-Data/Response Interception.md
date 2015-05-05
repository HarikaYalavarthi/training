```js
myModule.factory(‘myInterceptor’, function($q, notifyService, errorLog) {
	return function(promise) {
		return promise.then(function(response) {
			return response;
}, function(response) {
	errorLog($response);
	return $q.reject(response);
});
}
});

$httpProvider.responseInterceptors.push(‘myInterceptor’);
```
