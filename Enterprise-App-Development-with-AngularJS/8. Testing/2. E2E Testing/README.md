####Prerequisites
* Protractor is a [Node.js](http://nodejs.org/) program.
* To run, Node.js should be installed. Download Protractor package will be downloaded using [npm](https://www.npmjs.org/), which comes with Node.js. Check the version of Node.js have been running `node --version`. It should be greater than v0.10.0.
* By default, Protractor uses the [Jasmine](http://jasmine.github.io/) test framework for its testing interface. This tutorial assumes some familiarity with Jasmine, and will use version 2.3.
* This tutorial will set up a test using a local standalone Selenium Server to control browsers. [Java Development Kit (JDK)](http://www.oracle.com/technetwork/java/javase/downloads/index.html) needed is installed to run the standalone Selenium Server. Check this by running `java -version` from the command line.

#####Setup
* Use npm to install Protractor globally with:

    npm install -g protractor

* This will install two command line tools, `protractor` and `webdriver-manager`. Try running `protractor --version` to make sure it's working.

* The `webdriver-manager` is a helper tool to easily get an instance of a Selenium Server running. Use it to download the necessary binaries with:

    webdriver-manager update

* Now start up a server with:

    webdriver-manager start

This will start up a Selenium Server and will output a bunch of info logs. Information can be seen about the status of the server at `http://localhost:4444/wd/hub`.

Steps of Processing
* Step 0 - write a test
Open a new command line or terminal window and create a clean folder for testing.Protractor needs two files to run, a **spec file** and a **configuration file**. 

```javascript
// spec.js
describe('Protractor Demo App', function() {
  it('should have a title', function() {
    browser.get('url');

    expect(browser.getTitle()).toEqual('title of you app');
  });
});
```

Now create the configuration file. Copy the following into conf.js:

```js
// conf.js
exports.config = {
  framework: 'jasmine',
  seleniumAddress: 'http://localhost:4444/wd/hub',
  specs: ['spec.js']
}
```

Now run the test with

    protractor conf.js

Chrome browser should be seen window open up and navigate to the Calculator, then close itself (this should be very fast!). The test output should be `1 tests, 1 assertion, 0 failures`. Congratulations, run first Protractor test!

* Step 1 - interacting with elements

Now let's modify the test to interact with elements on the page. Change spec.js to the following:

```js
// spec.js
describe('Protractor Demo App', function() {
  it('should add one and two', function() {
    browser.get('url');
    element(by.model('first')).sendKeys(1);
    element(by.model('second')).sendKeys(2);

    element(by.id('gobutton')).click();

    expect(element(by.binding('latest')).getText()).
        toEqual('5'); // This is wrong!
  });
});
```
Run the tests with

    protractor conf.js

* Step 2 - writing multiple scenarios

Let's put these two tests together and clean them up a bit. Change spec.js to the following:

```js
// spec.js
describe('Protractor Demo App', function() {
  var firstNumber = element(by.model('first'));
  var secondNumber = element(by.model('second'));
  var goButton = element(by.id('gobutton'));
  var latestResult = element(by.binding('latest'));

  beforeEach(function() {
    browser.get('url');
  });

  it('should have a title', function() {
    expect(browser.getTitle()).toEqual('Super Calculator');
  });

  it('should add one and two', function() {
    firstNumber.sendKeys(1);
    secondNumber.sendKeys(2);

    goButton.click();

    expect(latestResult.getText()).toEqual('3');
  });

  it('should add four and six', function() {
    // Fill this in.
    expect(latestResult.getText()).toEqual('10');
  });
});
```
* Step 3 - changing the configuration

Let's change the browser. Change conf.js to the following:

```js
// conf.js
exports.config = {
  framework: 'jasmine',
  seleniumAddress: 'http://localhost:4444/wd/hub',
  specs: ['spec.js'],
  capabilities: {
    browserName: 'firefox'
  }
}
```
