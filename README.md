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

If you would prefer, you can work with the development code in the `src` directory using the included [Gulp build system](http://gulpjs.com/). This compiles, lints, and minifies code, and runs unit tests. It's the same build system that's used by [Kraken](http://cferdinandi.github.io/kraken/), so it includes some unnecessary tasks and Sass variables but can be dropped right in to the boilerplate without any configuration.

### Dependencies
Make sure these are installed first.

* [Node.js](http://nodejs.org)
* [Gulp](http://gulpjs.com) `sudo npm install -g gulp`

### Quick Start

1. In bash/terminal/command line, `cd` into your project directory.
2. Run `npm install` to install required files.
3. When it's done installing, run one of the task runners to get going:
	* `gulp` manually compiles files.
	* `gulp watch` automatically compiles files when changes are made and applies changes using [LiveReload](http://livereload.com/).



## Browser Compatibility

Alerts works with all modern browsers, including IE 6 and above.



## How to Contribute

In lieu of a formal style guide, take care to maintain the existing coding style. Please apply fixes to both the development and production code. Don't forget to update the version number, and when applicable, the documentation.



## License

The code is available under the [MIT License](LICENSE.md).