* Basic syntax:
  
  ```{{expression | filter}}```
  
  E.g. {{ 12 | currency }}
* Filters can be chained:
  
  ```{{expression | filter1 | filter2 | ...}}```
  
  E.g. {{ 12.25 | number | currency }}
* Filters can have, optional, parameters:

  ```{{expression | filter:argument1:argument2:...}}```
  
  E.g. {{ 12 | number:2 }}
