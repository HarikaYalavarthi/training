
The ngStyle directive allows you to set CSS style on an HTML element conditionally.

####Usage:

as attribute:

`<ANY
	ng-style="expression">
...
</ANY>`


as CSS class:

`<ANY class="ng-style: expression;"> ... </ANY> `

####Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngStyle|expression|Expression which evals to an object whose keys are CSS style names and values for those CSS Keys.Since some CSS style names are not valid keys for an object,they must be quoted.See the 'background-color' style in the example below.|


<p data-height="268" data-theme-id="0" data-slug-hash="ojmZZd" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/ojmZZd/'>ojmZZd</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

####Explanation:

In the above example we have declared 'myStyle' in ng-style and every time we click on the 'set color' or 'set background' or 'clear' button we are changing the value of 'my-style' which id being reflected on the 'Sample Text'. 
