# Alerts
Simple alert messages. [View the demo](http://cferdinandi.github.io/alerts/).

**In This Documentation**

1. [Getting Started](#getting-started)
2. [Browser Compatibility](#browser-compatibility)
3. [How to Contribute](#how-to-contribute)
4. [License](#license)
5. [Changelog](#changelog)



## Getting Started

### 1. Include Alerts on your site.

```html
<link rel="stylesheet" href="css/alerts-css.css">
```

Alerts is [built with Sass](http://sass-lang.com/) for easy customization. If you don't use Sass, that's ok. The `css` folder contains compiled vanilla CSS.

The `_config.scss` and `_mixins.scss` files are the same ones used in [Kraken](http://cferdinandi.github.io/kraken/), so you can drop the `_alerts.css` file right into Kraken without making any updates. Or, adjust the variables to suit your own project.

### 2. Add the markup to your HTML.

```html
<div class="alert">...</div>
<div class="alert alert-success">...</div>
<div class="alert alert-danger">...</div>
<div class="alert alert-warning">...</div>
```

Create an alert by adding the `.alert` class to a `<div>` element. Add optional `.alert-success`, `.alert-danger`, or `.alert-warning` classes for additional colors, and to convey meaning.

And that's it, you're done. Nice work!



## Browser Compatibility

Alerts works with all modern browsers, including IE 6 and above.



## How to Contribute

In lieu of a formal style guide, take care to maintain the existing coding style. Don't forget to update the version number, the changelog (in the `readme.md` file), and when applicable, the documentation.



## License

Alerts is licensed under the [MIT License](http://gomakethings.com/mit/).



## Changelog

* v2.0 - December 2, 2013
	* Added Sass support.
	* Broke old namespacing. Moved from color-based names to action-based names.
* v1.0 - June 7, 2013
	* Switched to MIT license.
* v1.0 - May 18, 2013
	* Initial release.