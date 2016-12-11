Zepto Slide Transition
======================

This is an updated version of the zepto slide transitions. 

The original and other forks have a bug which forces the animated elements retain a fixed size after the animation is completed.

In addition, the original `.slideToggle()` wasn't passing duration to `.slideUp()` or `.slideDown()`

There's now a callback for the animation completion.

Zepto Slide Transitions plugin adds the following functions to Zepto.js:

* slideDown();
* slideUp();
* slideToggle();

# Requirements:

This Zepto.js plugin requires Zepto.js to run (duh)

# Usage

* Include Zepto.js and this plugin:

```html
<script src="zepto.min.js"></script>
<script src="zepto-slide-transition.js"></script>
```

* The function is similar to jQuery: it takes `duration` and `callback` arguments:

```javascript
$('element').slideUp(1500, function callback(elem) { console.log('Finished with', elem); });
$('element').slideDown(250, do_something);
$('element').slideToggle(350, do_something_else);
```

# TODO

* Prevent the functions from working on an element that is already undergoing a transition