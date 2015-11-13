Unit testing refers to the practice of testing certain functions and areas – or units – of our code. This gives us the ability to verify that our functions work as expected. That is to say that for any function and given a set of inputs, we can determine if the function is returning the proper values and will gracefully handle failures during the course of execution should invalid input be provided.

Ultimately, this helps us to identify failures in our algorithms and/or logic to help improve the quality of the code that composes a certain function. As you begin to write more and more tests, you end up creating a suite of tests that you can run at any time during development to continually verify the quality of your work.

A second advantage to approaching development from a unit testing perspective is that you'll likely be writing code that is easy to test. Since unit testing requires that your code be easily testable, it means that your code must support this particular type of evaluation. As such, you're more likely to have a higher number of smaller, more focused functions that provide a single operation on a set of data rather than large functions performing a number of different operations.

A third advantage for writing solid unit tests and well-tested code is that you can prevent future changes from breaking functionality. Since you're testing your code as you introduce your functionality, you're going to begin developing a suite of test cases that can be run each time you work on your logic. When a failure happens, you know that you have something to address.

Dependency injection in ANgular JS built-in, which makes testing components much easier, because you can pass in a component's dependencies and stub or mock them as you wish.Components that have their dependencies injected allow them to be easily mocked on a test by test basis, without having to mess with any global variables that could inadvertently affect another test.

### Karma
Karma is a JavaScript command line tool that can be used to spawn a web server which loads your application's source code and executes your tests. You can configure Karma to run against a number of browsers, which is useful for being confident that your application works on all browsers you need to support. Karma is executed on the command line and will display the results of your tests on the command line once they have run in the browser.
Karma is a NodeJS application, and should be installed through npm. Full installation instructions are available on the Karma website.
### Jasmine

Jasmine is a behavior driven development framework for JavaScript that has become the most popular choice for testing Angular applications. Jasmine provides functions to help with structuring your tests and also making assertions. As your tests grow, keeping them well structured and documented is vital, and Jasmine helps achieve this.

In Jasmine we use the describe function to group our tests together:
```script
describe("sorting the list of users", function() {
  // individual tests go here
});
```
### angular-mocks

Angular also provides the ngMock module, which provides mocking for your tests. This is used to inject and mock Angular services within unit tests. In addition, it is able to extend other modules so they are synchronous. Having tests synchronous keeps them much cleaner and easier to work with. One of the most useful parts of ngMock is $httpBackend, which lets us mock XHR requests in tests, and return sample data instead.
