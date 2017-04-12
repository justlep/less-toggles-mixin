# less-toggles-mixin [![Build Status](https://travis-ci.org/justlep/less-toggles-mixin.svg?branch=master)](https://travis-ci.org/justlep/less-toggles-mixin)
A LESS mixin for nice-looking toggles instead of default browser checkboxes.
Originally inspired by http://callmenick.com/_development/css-toggle-switch/

See Demo:
[http://justlep.github.io/less-toggles-mixin/](http://justlep.github.io/less-toggles-mixin/)

**How to use**
First generate one or more CSS classes for your checkboxes by calling the mixins:
```less
@import (reference) "toggles-mixin";
.roundToggle {
    .createRoundToggle();
}
```
Then use the generated classes in your HTML like so
```html
<span class="roundToggle">
    <input type="checkbox" id="cb1"/>
    <label for="cb1"></label>
</span>
<label for="cb1"> Visible label for cb1 </label>
```

