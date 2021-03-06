---
layout: docs
title: Watching for Changes and Auto Regenerating Patterns | Pattern Lab
---

# Watching for Changes and Auto Regenerating Patterns
The PHP version of Pattern Lab has the ability to watch for changes to patterns and select files. When these files change, it will automatically rebuild the entire Pattern Lab website. You simply make your changes, save the file, and the PHP version of Pattern Lab will take care of the rest.

## How to Start the Watch

To set-up the watch on Mac OS X you can do the following:

1. Open `scripts/`
2. Double-click `startWatcher.command`

You can also start the watch from the command line. To do so open Terminal and navigate to the root of the `patternlab-php` directory. Type:

    php builder/builder.php -w

## How to Stop the Watch

To stop watching files on Mac OS X you can press`CTRL+C` in the Terminal window where the process is running. 

## The Default Files That Are Watched

By default, the PHP version of Pattern Lab monitors the following files:

* all of the patterns under `source/_patterns`
* all of the JSON files under `source/_data/` 
* any directory in `source/` without an `_` (underscore) or that doesn't match a directory name found in the `id` variable in `config/config.ini`
* any file in `source/` with a file extension that doesn't match one found in the `ie` variable in `config/config.ini`

## Ignoring Other Directories & File Extensions 

Instructions on how to ignore assets in other directories or with other file extensions can be found in "[Managing Assets for a Pattern](https://github.com/pattern-lab/patternlab-php/wiki/Managing-Assets-for-a-Pattern)".