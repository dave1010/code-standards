# Code Standards

This repository contains a set of code standards and guidelines, along with a few helpful resources.
These standards are part of the [@wearebase](https://github.com/wearebase) code quality assurance process.

Please note: This document is biased towards PHP and JavaScript, which are the most common languages we currently use. Much of it should apply to other languages (such as Objective-C, Java, Python and Ruby) however if an existing industry standard is in widespread use then it should be preferred. Wherever possible we try to follow industry standards.

Content is licensed under the Creative Commons - CC BY 3.0 license.

## General

* Save files as UTF-8
* UNIX-style line endings. (`git` should take care of this for you if you use Windows)
* Comment what is not obvious
* Indent using 4 spaces. This is the standard for PHP. Your editor can make this seamless for you.
* Large changes to whitespace should be in their own commit

## PHP

* PHP code must have no syntax errors (check with `php -l filename.php`)
* Use [PSR-0](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md) or the framework’s class autoloader when loading classes
* Follow [PSR-1](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md) to the letter with all new code and when updating legacy code
* Follow [PSR-2](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md), except when working with legacy files
* Try not to mix PHP with HTML

## JavaScript

* JavaScript code must not show errors on [JSHint](http://www.jshint.com/)
* 4 spaces, not tabs (to be consistent with PHP)

## CSS (and SCSS/Less)

* Formatting
    * 4 spaces, not tabs (to be consistent with PHP)
    * A space to the left of `{` and a newline after
    * Rules on new lines, with a space after `:`
    * `}` on its own
* SASS comments (`//`) instead of CSS comments (`/* ... */`)
* Prefer class selectors (`.`) and avoid id selectors (`#`)
* Comment where styles are used if it is not obvious
* CSS hacks should be avoided and documented if they are ever used (use [conditional classes on the html element](http://paulirish.com/2008/conditional-stylesheets-vs-css-hacks-answer-neither/) instead)

## HTML

* `.class-names-lowercase-with-dashes`
* `#ids-lowercase-with-dashes`
* HTML5 doctype: `<!doctype html>`
* HTML should be mostly valid
