* $http.get
* $http.head
* $http.post
* $http.put
* $http.delete
* $http.jsonp
* $http.patch

```js
// Simple GET request example
$http.get('/someUrl').
	success(function(data, status, headers, config) {
		// this callback will be called asynchronously
		// when the response is available
	}).
	error(function(data, status, headers, config) {
		// called asynchronously if an error occurs
		// or server returns response with and error status
	});
```
