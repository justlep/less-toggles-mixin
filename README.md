# less-toggles-mixin [![Build Status](https://travis-ci.org/justlep/less-toggles-mixin.svg?branch=master)](https://travis-ci.org/justlep/less-toggles-mixin)
A LESS mixin for nice-looking toggles instead of default browser checkboxes.  
Inspired originally by http://callmenick.com/_development/css-toggle-switch/

[Live Demo](http://justlep.github.io/less-toggles-mixin/)

### How to use
In your .less file, import the mixin and use it to build your custom toggle classes:  
```less
@import "toggles-mixin";

.myRoundToggle {
    .createRoundToggle();
}
.myRoundInsetToggle {
    .createRoundInsetToggle();
}
```
Then use the classes in your HTML like so
```html
<span class="myRoundToggle">
    <input type="checkbox" id="cb1"/>
    <label for="cb1"><!-- This label MUST be empty --></label>
</span>
<label for="cb1"> Visible label for cb1 </label>

<span class="myRoundInsetToggle">
    <input type="checkbox" id="cb2"/>
    <label for="cb2"><!-- This label MUST be empty --></label>
</span>
<label for="cb3"> Visible label for cb2 </label>
```
## Hints
- Remove the line-break between the span and the visible label for better control over spacing between the two.
- See [toggles-mixin.less](./src/toggles-mixin.less) for optional parameters of the mixin.
