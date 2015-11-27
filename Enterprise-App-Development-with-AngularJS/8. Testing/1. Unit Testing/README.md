* Unit testing refers to the practice of testing certain functions and areas – or units – of our code. This gives us the ability to verify that our functions work as expected. 
* This helps us to identify failures in our algorithms and/or logic to help improve the quality of the code that composes a certain function. As More and more tests are written, ending up creation of suite of tests that can run at any time during development to continually verify the quality of work.
* A second advantage to approaching development from a unit testing perspective is that likely writing code that is easy to test.
* A third advantage for writing solid unit tests and well-tested code is that future changes can be prevented from breaking functionality. 
* Dependency injection in ANgular JS built-in, which makes testing components much easier, because component's dependencies can be passed and stub or mock them.

### Karma
* Karma is a JavaScript command line tool that can be used to spawn a web server which loads application's source code and executes tests. 
* Karma can be configured to run against a number of browsers, which is useful for being confident that application works on all browsers need to supported. 
* Karma is executed on the command line and will display the results of tests on the command line once they have run in the browser.

### Jasmine

* Jasmine is a behavior driven development framework for JavaScript that has become the most popular choice for testing Angular applications. 
* Jasmine provides functions to help with structuring tests and also making assertions. 
* As tests grow, keeping them well structured and documented is vital, and Jasmine helps achieve this.

```script
describe("sorting the list of users", function() {
  // individual tests go here
});
```
### angular-mocks

* Angular also provides the ngMock module, which provides mocking for tests. 
* One of the most useful parts of ngMock is $httpBackend, which lets us mock XHR requests in tests, and return sample data instead.
