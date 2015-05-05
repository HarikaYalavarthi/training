$q service helps run functions asynchronously, and use their return values (or exceptions) when they are done processing


* Promise dictates the following for async requests:
* Async request return a promise instead of a return value
* The Promise has a then function, which has two arguments
  - a function to handle “resolved” or “success” event
  - a function to handle the “rejected” or “failure” event
* It is guaranteed that one of the two callbacks will be called, as soon as the result is available
