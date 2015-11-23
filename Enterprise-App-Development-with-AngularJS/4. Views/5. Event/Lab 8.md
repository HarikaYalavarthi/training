
You attach an event listener to an HTML element using one of the following AngularJS event listener <a class="x-grid-item"  href='/slidedeck/#1. Overview/2 Core-Concepts/5. Directive' target="_blank">directives</a>:
* ng-click
* ng-dbl-click
* ng-mousedown
* ng-mouseup
* ng-mouseenter
* ng-mouseleave
* ng-mousemove
* ng-mouseover
* ng-keydown
* ng-keyup
* ng-keypress
* ng-change

#####ng-click:

The ngClick directive allows you to specify custom behavior when an element is clicked.

######Usage:

as attribute:

`<ANY
	ng-click="expression">
...
</ANY>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngClick|expression|Expression to evaluate upon click.(Event object is available as $event)|


<p data-height="268" data-theme-id="0" data-slug-hash="WQLbrQ" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/WQLbrQ/'>WQLbrQ</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

####Explanation:

In the above example,every time you click on the “Increament” button the “ng-Click” event is getting fired and the count gets updated by '+1' which is seen in the output.

####ng-Dblclick:

The ngDblclick directive allows you to specify custom behavior on a dblclick event.

####Usage:

as attribute:

`<ANY
	ng-dblclick="expression">
...
</ANY>`


####Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngDblclick|expression|Expression to evaluate upon click.(Event object is available as $event)|


<p data-height="268" data-theme-id="0" data-slug-hash="zvyxdW" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/zvyxdW/'>zvyxdW</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

####Explanation:

In the above example,every time you double click on the “Increament” button the “ng-dblclick” event is getting fired and the count gets updated by '+1' which is seen in the output.


####ng-mousedown

The ngMousedown directive allows you to specify custom behavior on mousedown event.

####Usage:

as attribute:

`<ANY
	ng-mousedown="expression">
...
</ANY>`

####Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngMousedown|expression|Expression to evaluate upon mousedown.(Event object is available as $event)|


<p data-height="268" data-theme-id="0" data-slug-hash="MaZYGE" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/MaZYGE/'>MaZYGE</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

####Explanation:

In the above example,every time when the user depresses the mouse button. the “ng-mousedown” event is getting fired and the count gets updated by '+1' which is seen in the output.

####ng-mouseup

The ngMouseup directive allows you to specify custom behavior on mouseup event.

####Usage:

as attribute:

`<ANY
	ng-mouseup="expression">
...
</ANY>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngMouseup|expression|Expression to evaluate upon mouseup.(Event object is available as $event)|


<p data-height="268" data-theme-id="0" data-slug-hash="VvqYBO" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/VvqYBO/'>VvqYBO</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

In the above example,every time when the user releases the mouse button. the “ng-mouseup” event is getting fired and the count gets updated by '+1' which is seen in the output.

#####ng-mouseenter

The ngMouseenter directive allows you to specify custom behavior on mouseenter event.

#####Usage:

as attribute:

`<ANY
	ng-mouseenter="expression">
...
</ANY>`

#####Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngMouseenter|expression|Expression to evaluate upon mouseenter.(Event object is available as $event)|


<p data-height="268" data-theme-id="0" data-slug-hash="WQLbYp" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/WQLbYp/'>WQLbYp</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

The mouseenter event is fired when a pointing device (usually a mouse) is moved over the element.So the count gets updated by '+1' whenever mouse points in to the increament button which is seen in the output.

#####ng-mouseleave

The ngMouseleave directive allows you to specify custom behavior on mouseleave event.

######Usage:

as attribute:

`<ANY
	ng-mouseleave="expression">
...
</ANY>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngMouseleave|expression|Expression to evaluate upon mouseleave.(Event object is available as $event)|

######Example:

<p data-height="268" data-theme-id="0" data-slug-hash="rOoaPK" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/rOoaPK/'>rOoaPK</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

The mouseleave event is fired when a pointing device (usually a mouse) is moved off the element.So the count gets updated by '+1' whenever mouse points off to the increament button which is seen in the output.

#####ng-mousemove

The ngMousemove directive allows you to specify custom behavior on mousemove event.

######Usage:

as attribute:

`<ANY
	ng-mousemove="expression">
...
</ANY>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngMousemove|expression|Expression to evaluate upon mousemove.(Event object is available as $event)|

######Example:

<p data-height="268" data-theme-id="0" data-slug-hash="epbmoK" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/epbmoK/'>epbmoK</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

The mousemove event is fired when a pointing device (usually a mouse) is moved across the element.So the count gets updated by '+1' whenever mouse moves across the increament button which is seen in the output.

#####ng-mouseover

The ngMouseover directive allows you to specify custom behavior on mouseover event.

######Usage:

as attribute:

`<ANY
	ng-mouseover="expression">
...
</ANY>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngMouseover|expression|Expression to evaluate upon mouseover.(Event object is available as $event)|


######Example:

<p data-height="268" data-theme-id="0" data-slug-hash="BovygQ" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/BovygQ/'>BovygQ</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

The mouseover event is fired when a pointing device (usually a mouse) is moved onto the element.So the count gets updated by '+1' whenever mouse moves onto the increament button which is seen in the output.

#####ng-keydown

The ngKeydown directive allows you to specify custom behavior on keydown event.

######Usage:

as attribute:

`<ANY
	ng-mouseover="expression">
...
 </ANY>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngKeydown|expression|Expression to evaluate upon Keydown.(Event object is available as $event and can be interrogated for keyCode,altKey, etc.)|

######Example:

<p data-height="268" data-theme-id="0" data-slug-hash="PPXqYG" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/PPXqYG/'>PPXqYG</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

The keydown event is fired when a key is pressed down.So the count gets updated by '+1' whenever a  key is pressed or say a text in entered in the box.

#####ng-keyup

The ngKeyup directive allows you to specify custom behavior on keyup event.

######Usage:

as attribute:

`<ANY
	ng-Keyup="expression">
...
</ANY>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngKeyup|expression|Expression to evaluate upon Keyup.(Event object is available as $event and can be interrogated for keyCode,altKey, etc.)|

######Example:

<p data-height="268" data-theme-id="0" data-slug-hash="gaZpOM" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/gaZpOM/'>gaZpOM</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

The keyup event is fired when a key is released.So the count gets updated by '+1' whenever a  key is released or say a text in entered in the box.

#####ng-keypress

The ngKeypress directive allows you to specify custom behavior on keypress event.

######Usage:

as attribute:

`<ANY
	ng-Keypress="expression">
...
</ANY>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngKeypress|expression|Expression to evaluate upon Keypress.(Event object is available as $event and can be interrogated for keyCode,altKey, etc.)|


######Example:

<p data-height="268" data-theme-id="0" data-slug-hash="dYwoPb" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/dYwoPb/'>dYwoPb</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

The keypress event is fired when a key is pressed down and that key normally produces a character value.So the count gets updated by '+1' whenever a  key is pressed down in the box.

#####ng-change

The ngChange directive evaluates the given expression when the user changes the input. The expression is evaluated immediately, unlike the JavaScript onchange event which only triggers at the end of a change (usually, when the user leaves the form element or presses the return key).

The ngChange expression is only evaluated when a change in the input value causes a new value to be committed to the model.

It will not be evaluated:

if the value returned from the $parsers transformation pipeline has not changed.
if the input has continued to be invalid since the model will stay null.
if the model is changed programmatically and not by a change to the input value.


`💡 Note: this directive requires ngModel to be present.`


######Usage:

as attribute:

`<input
	ng-change="expression">
...
</input>`

######Arguments:

|Param|	Type|	Details|
|----|----|----|
|ngChange|expression|Expression to evaluate upon change in input values.|


######Example:

<p data-height="268" data-theme-id="0" data-slug-hash="qOLdZe" data-default-tab="result" data-user="walkingtree" class='codepen'>See the Pen <a href='http://codepen.io/walkingtree/pen/qOLdZe/'>qOLdZe</a> by Walking Tree (<a href='http://codepen.io/walkingtree'>@walkingtree</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

######Explanation:

The ngChange expression is only evaluated when a change in the input value causes a new value to be committed to the model.

