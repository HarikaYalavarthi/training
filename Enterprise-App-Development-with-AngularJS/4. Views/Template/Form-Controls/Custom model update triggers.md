* By default, any change to the content will trigger a model update and form validation
* We can override this behavior using the ngModelOptions directive to bind only to specified list of events. E.g. ng-model-options="{ updateOn: 'blur' }"
* We can set several events using a space delimited list. E.g. ng-model-options="{ updateOn: 'mousedown blur' }"
* We can use the default behaviour by using default as one of the events in the list

<p data-height="266" data-theme-id="14134" data-slug-hash="gpaMVJ" data-default-tab="result" data-user="ajit-kumar-azad" class='codepen'>See the Pen <a href='http://codepen.io/ajit-kumar-azad/pen/gpaMVJ/'>gpaMVJ</a> by Ajit Kumar (<a href='http://codepen.io/ajit-kumar-azad'>@ajit-kumar-azad</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>
