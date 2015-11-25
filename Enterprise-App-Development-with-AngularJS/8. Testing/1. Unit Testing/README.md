Unit testing refers to the practice of testing certain functions and areas – or units – of our code. This gives us the ability to verify that our functions work as expected. That is to say that for any function and given a set of inputs, can be determined if the function is returning the proper values and will gracefully handle failures during the course of execution should invalid input be provided.

Ultimately, this helps us to identify failures in our algorithms and/or logic to help improve the quality of the code that composes a certain function. As More and more tests are written, ending up creation of suite of tests that can run at any time during development to continually verify the quality of work.

A second advantage to approaching development from a unit testing perspective is that likely writing code that is easy to test. Since unit testing requires that code can be easily testable, it means that code must support this particular type of evaluation. As such, more likely to have a higher number of smaller, more focused functions that provide a single operation on a set of data rather than large functions performing a number of different operations.

A third advantage for writing solid unit tests and well-tested code is that future changes can be prevented from breaking functionality. Since testing code as introduction of functionality, going to begin developing a suite of test cases that can be run each time you work on logic. When a failure happens, there will be something to address.

Dependency injection in ANgular JS built-in, which makes testing components much easier, because component's dependencies can be passed and stub or mock them.Components that have their dependencies injected allow them to be easily mocked on a test by test basis, without having to mess with any global variables that could inadvertently affect another test.

### Karma
Karma is a JavaScript command line tool that can be used to spawn a web server which loads application's source code and executes tests. Karma can be configured to run against a number of browsers, which is useful for being confident that application works on all browsers need to supported. Karma is executed on the command line and will display the results of tests on the command line once they have run in the browser.
Karma is a NodeJS application, and should be installed through npm. Full installation instructions are available on the Karma website.
### Jasmine

Jasmine is a behavior driven development framework for JavaScript that has become the most popular choice for testing Angular applications. Jasmine provides functions to help with structuring tests and also making assertions. As tests grow, keeping them well structured and documented is vital, and Jasmine helps achieve this.

In Jasmine describe function to group our tests together should be used:
```script
describe("sorting the list of users", function() {
  // individual tests go here
});
```
### angular-mocks

Angular also provides the ngMock module, which provides mocking for tests. This is used to inject and mock Angular services within unit tests. In addition, it is able to extend other modules so they are synchronous. Having tests synchronous keeps them much cleaner and easier to work with. One of the most useful parts of ngMock is $httpBackend, which lets us mock XHR requests in tests, and return sample data instead.
