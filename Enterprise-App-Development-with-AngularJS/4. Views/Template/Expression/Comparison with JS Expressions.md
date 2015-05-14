* Context
  - JavaScript expressions are evaluated against the global window. In Angular, expressions are evaluated against a scope object.
* Forgiving
  - In JavaScript, trying to evaluate undefined properties generates ReferenceError or TypeError. In Angular, expression evaluation is forgiving to undefined and null
* No control flow statements
  - Apart from a ? b : c ternary op, we cannot use the following in an Angular expression: conditionals, loops, or exceptions. Use controllers, instead.
* No function declarations
  - cannot declare functions in an Angular expression, even inside ng-init directive
* No RegEx creation with literal notation
  - cannot create regular expressions in an Angular expression. Use controller or filter, instead.
* No comma and void parameters
  - cannot use , or void in an Angular expression
* Filters 
  - can use filters within expressions to format data before displaying it
