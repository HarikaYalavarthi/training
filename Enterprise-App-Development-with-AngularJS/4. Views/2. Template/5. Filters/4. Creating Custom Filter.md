* Register a new filter factory function with your module
  - This factory function should return a new filter function which takes the input value as the first argument
   - Any filter arguments are passed in as additional arguments to the filter function
* The filter function should be stateless and idempotent
