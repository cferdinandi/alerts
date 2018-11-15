# Alerts [![Build Status](https://travis-ci.org/cferdinandi/alerts.svg)](https://travis-ci.org/cferdinandi/alerts)
Simple alert messages.

[Download Alerts](https://github.com/cferdinandi/alerts/archive/master.zip) / [View the demo](http://cferdinandi.github.io/alerts/)



## Getting Started

Compiled and production-ready code can be found in the `dist` directory. The `src` directory contains development code.

### 1. Include Alerts on your site.

If you'd like to be able to dismiss alerts, also include `alerts.js`. For basic alerts, it can be excluded.

```html
<link rel="stylesheet" href="dist/css/alerts.css">
<script src="dis/js/alerts.js"></script>
```

### 2. Add the markup to your HTML.

Create an alert by adding the `.alert` class to a `<div>` element. Add optional `.alert-success`, `.alert-danger`, or `.alert-warning` classes for additional colors, and to convey meaning.

```html
<div class="alert">...</div>
<div class="alert alert-success">...</div>
<div class="alert alert-danger">...</div>
<div class="alert alert-warning">...</div>
```

For dismissable alerts, also add an element with the `.alert-dismiss` class and `[data-alert-dismiss]` attribute. By default, dismissed alerts remain in the DOM but are hidden. To remove them entirely give `[data-alert-dismiss]` a value of `remove`.

```html
<div class="alert">
	<span class="alert-dismiss" data-alert-dismiss>X</span>
	This is a dismissable alert. It will be hidden in the DOM.
</div>

<div class="alert">
	<span class="alert-dismiss" data-alert-dismiss="remove">X</span>
	This is a dismissable alert. It will be removed from the DOM entirely.
</div>
```

And that's it, you're done. Nice work!



## Installing with Package Managers

You can install Alerts with your favorite package manager.

* **NPM:** `npm install cferdinandi/alerts`
* **Bower:** `bower install https://github.com/cferdinandi/alerts.git`
* **Component:** `component install cferdinandi/alerts`



## Working with the Source Files

If you would prefer, you can work with the development code in the `src` directory using the included [Gulp build system](http://gulpjs.com/). This compiles, lints, and minifies code, and runs unit tests.

### Dependencies
Make sure these are installed first.

* [Node.js](http://nodejs.org)
* [Gulp](http://gulpjs.com) `sudo npm install -g gulp`

### Quick Start

1. In bash/terminal/command line, `cd` into your project directory.
2. Run `npm install` to install required files.
3. When it's done installing, run one of the task runners to get going:
	* `gulp` manually compiles files.
	* `gulp watch` automatically compiles files and applies changes using [LiveReload](http://livereload.com/).
	* `gulp test` compiles files and runs unit tests.



## Options and Settings

Alerts includes smart defaults and works right out of the box. But if you want to customize things, it also has a robust API that provides multiple ways for you to adjust the default options and settings.

### Global Settings

You can pass options and callbacks into Alerts through the `init()` function:

```javascript
alerts.init({
	alert: '.alert', // The alert selector
	dismiss: '[data-alert-dismiss]', // The dismiss button selector
	initClass: 'js-alerts', // Class added to `<html>` element when initiated
	callback: function () {} // Function that's run after content is expanded or collapsed
});
```

### Use Alerts events in your own scripts

You can also call Alerts events in your own scripts.

#### dismissAlert()
Dismisses an alert.

```javascript
alerts.dismissAlert(
	alert,  // The alert to dismiss
	remove, // [Boolean] If true, remove the alert from the DOM entirely (optional)
	options // Selectors and callbacks. Same options as those passed into the init() function.
);
```

**Example**

```javascript
var alert = document.querySelector( '#some-alert' );
alerts.dismissAlert( alert );
```

#### destroy()
Destroy the current `alerts.init()`. This is called automatically during the `init` function to remove any existing initializations.

```javascript
alerts.destroy();
```



## Browser Compatibility

Alerts works with all modern browsers, including IE 6 and above. Dismissable alerts work in IE 9 and above. In unsupported browsers, the dismiss icon will not display.



## How to Contribute

In lieu of a formal style guide, take care to maintain the existing coding style. Please apply fixes to both the development and production code. Don't forget to update the version number, and when applicable, the documentation.



## License

The code is available under the [MIT License](LICENSE.md).
