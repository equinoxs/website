---
layout: docs
title: Generating CSS | Pattern Lab
---
# Generating CSS

As of v0.6.0 the PHP version of Pattern Lab includes support for the [CSS Rule Saver](https://github.com/dmolsen/css-rule-saver) library. When used, Pattern Lab can display only those CSS rules that affect a given pattern on the pattern detail view. This might be useful if you have a large Sass-generated CSS file or framework but only need a sub-set of styles that may affect a small piece of mark-up or pattern.

## How to Generate the CSS

To generate your Pattern Lab site with CSS support on Mac OS X you can do the following:

1. Open `scripts/`
2. Double-click `generateSiteWithCSS.command`
3. Refresh the Pattern Lab site

You can also start the service from the command line. To do so open Terminal and navigate to the root of the patternlab-php directory. Type:

    php builder/builder.php -gc

## Important Note About Performance

It may take several seconds for the PHP version of Pattern Lab to generate a site when it's also calculating the CSS rules. Be patient.

