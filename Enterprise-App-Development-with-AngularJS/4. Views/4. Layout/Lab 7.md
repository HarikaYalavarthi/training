####Overview:

Angular Material's responsive CSS layout is built on flexbox.

The layout system is based upon element attributes rather than CSS classes. Attributes provide an easy way to set a value (eg. layout="row") and help us separate concerns: attributes define layout, and classes define styling.

####Usage:

Use the layout attribute on an element to arrange its children horizontally in a row (layout="row") or vertically in a column (layout="column"). Row layout is the default if you specify the layout attribute without a value.

######Row -
Items arranged horizontally. max-height = 100% and max-width is the width of the items in the container.
######Column - 
Items arranged vertically. max-width = 100% and max-height is the height of the items in the container.

####Layout-Options:

To make our layout change depending upon the device screen size, there are other layout attributes available:

|Layout|	Features|
|----|----|----|
|layout | Sets the default layout on all devices.|
|Layout-sm|Sets the layout on devices less than 600px wide(phones).|
|Layout-gt-sm|Sets the layout on devices greater than 600px wide(bigger than phones).|
|Layout-md|Sets the layout on devices between 600px and 960px wide(tablets in portrait).|
|Layout-gt-md|Sets the layout on devices greater than 960px wide(bigger than tablets in portrait).|
|Layout-lg|Sets the layout on devices between 960px and 1200px wide(tablets in landscape).|
|Layout-gt-lg|Sets the layout on devices grater than 1200px wide(computers and large screens).|

* `layout-margin`  adds margin around each flex child. It also adds a margin to the layout container itself. 

* `layout-padding` adds padding inside each flex child. It also adds padding to the layout container itself. 

* `layout-fill` forces the layout element to fill its parent container.

* `layout-wrap` allows flex children to wrap within the container if the elements use more than 100%. 
