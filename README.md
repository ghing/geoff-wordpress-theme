geoff
=====

A WordPress theme for http://blogs.terrorware.com/geoff/.

It's based on the [Timber starter theme](https://github.com/timber/starter-theme).

Installation
------------

Install this theme as you would any other, and be sure the Timber plugin is activated. But hey, let's break it down into some bullets:

1. Make sure you have installed the plugin for the [Timber Library](https://wordpress.org/plugins/timber-library/) (and Advanced Custom Fields - they [play quite nicely](http://timber.github.io/timber/#acf-cookbook) together). 
2. Download the zip for this theme (or clone it) and move it to `wp-content/themes` in your WordPress installation. 
4. Activate the theme in Appearance >  Themes.

Directory structure
-------------------

`static/` is where you can keep your static front-end scripts, styles, or images. In other words, your Sass files, JS files, fonts, and SVGs would live here.

`static/src/` is where source JavaScript and SCSS files live.  Yarn scripts will compile these 

`templates/` contains all of your Twig templates. These pretty much correspond 1 to 1 with the PHP files that respond to the WordPress template hierarchy. At the end of each PHP template, you'll notice a `Timber::render()` function whose first parameter is the Twig file where that data (or `$context`) will be used. Just an FYI.

`bin/` and `tests/` These are parts of the Timber Starter Theme. Don't worry about (or remove) these unless you know what they are and want to.

Assumptions
-----------

* Yarn

Building front-end assets
-------------------------

    yarn run build
