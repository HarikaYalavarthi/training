* Expression Sandboxing
* Design your template properly
  - Do not mix client and server templates
  - Do not use user input to generate templates dynamically
  - Do not run user input through $scope.$eval
* JSON Vulnerability
  - Retrieve JSON with POST request
  - Prefix response with “)]}’,\n”
* XSRF (Cros-site Request Forgery)
  - Server must set XSRF-TOKEN session cookie
  - Use X-XSRF-TOKEN in HTTP header to establish valid requestor
