* Pre-bundled rule sets

  ```
  cat angular.js i18n/angular-locale_de-de.js > angular_de-de.js
  ```
* Including a locale script in index.html

  ```html
  <html ng-app>
  	<head>
  		...
  		<script src="angular.js"></script>
  		<script src="i18n/angular-locale_de-de.js"></script>
  		...
  	</head>
  </html>
  ```
