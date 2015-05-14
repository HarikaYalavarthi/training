* Use debounce key with the ngModelOptions directive
* Duration is specified in milli-seconds
  
  ```
  ng-model-options="{ debounce: 500 }"
  ng-model-options="{ updateOn: 'default blur', debounce: { default: 500, blur: 0 } }"
  ```
* When these attributes are added to an element, they will be applied to all the child elements and controls that inherit from it unless they are overridden

<p data-height="266" data-theme-id="14134" data-slug-hash="vONXBv" data-default-tab="result" data-user="ajit-kumar-azad" class='codepen'>See the Pen <a href='http://codepen.io/ajit-kumar-azad/pen/vONXBv/'>vONXBv</a> by Ajit Kumar (<a href='http://codepen.io/ajit-kumar-azad'>@ajit-kumar-azad</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>
