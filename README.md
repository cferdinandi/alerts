# Alerts [![Build Status](https://travis-ci.org/cferdinandi/alerts.svg)](https://travis-ci.org/cferdinandi/alerts)
Simple alert messages.

[Download Alerts](https://github.com/cferdinandi/alerts/archive/master.zip) / [View the demo](http://cferdinandi.github.io/alerts/).

**In This Documentation**

1. [Getting Started](#getting-started)
2. [Installing with Package Managers](#installing-with-package-managers)
3. [Working with the Source Files](#working-with-the-source-files)
4. [Browser Compatibility](#browser-compatibility)
5. [How to Contribute](#how-to-contribute)
6. [License](#license)
7. [Changelog](#changelog)



## Getting Started

Compiled and production-ready code can be found in the `dist` directory. The `src` directory contains development code.

### 1. Include Alerts on your site.

```html
<link rel="stylesheet" href="dist/css/alerts.css">
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



## Installing with Package Managers

You can install Alerts with your favorite package manager.

* **[NPM](https://www.npmjs.org/):** `npm install cferdinandi/alerts`
* **[Bower](http://bower.io/):** `bower install https://github.com/cferdinandi/alerts.git`
* **[Component](http://component.io/):** `component install cferdinandi/alerts`



## Working with the Source Files

If you would prefer, you can work with the development code in the `src` directory using the included [Gulp build system](http://gulpjs.com/). This compiles, lints, and minifies code, and runs unit tests.

### Dependencies
Make sure these are installed first.

* [Node.js](http://nodejs.org)
* [Ruby Sass](http://sass-lang.com/install)
* [Gulp](http://gulpjs.com) `sudo npm install -g gulp`
* [PhantomJS](http://phantomjs.org)

### Quick Start

1. In bash/terminal/command line, `cd` into your project directory.
2. Run `npm install` to install required files.
3. When it's done installing, run `gulp` to get going.

Every time you want to run your tasks, run `gulp`.



## Browser Compatibility

Alerts works with all modern browsers, including IE 6 and above.



## How to Contribute

In lieu of a formal style guide, take care to maintain the existing coding style. Don't forget to update the version number, the changelog (in the `readme.md` file), and when applicable, the documentation.



## License

Alerts is licensed under the [MIT License](http://gomakethings.com/mit/).



## Changelog

Alerts uses [semantic versioning](http://semver.org/).

* v2.2.1 - October 3, 2014
	* Updated `gulpfile.js`.
	* Updated readme.
	* Updated travis config.
* v2.2.0 - August 25, 2014
	* Switched from Sass Lib to Ruby Sass.
* v2.1.0 - June 23, 2014
	* Converted to gulp.js workflow.
	* Updated naming conventions.
	* Added minified versions of files.
	* Updated to three number versioning system.
* v2.0 - December 2, 2013
	* Added Sass support.
	* Broke old namespacing. Moved from color-based names to action-based names.
* v1.0 - June 7, 2013
	* Switched to MIT license.
* v1.0 - May 18, 2013
	* Initial release.