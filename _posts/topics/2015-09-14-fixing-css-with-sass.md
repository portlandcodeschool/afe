---
layout: post
title: "Fixing CSS with Sass"
modified: 2015-09-14 16:53:15 -0700
category: topics
---

See [the slide deck, "Fixing CSS with Sass"](http://slides.com/auraelius/fixing-css)

Required reading: http://sass-lang.com/guide


# Notes


## Introductory/conceptual
* SCSS syntax is a superset of CSS - everything you know still works, you just get to add new & cool techniques
* Sass is more efficient (it does more with less code) and expressive (it is better at describing what is going on)
* The Sass `@import` directive and partials allow well-structured file organization. (http://thesassway.com/beginner/how-to-structure-a-sass-project). This, like many of the techniques taught in this class, is overkill for small projects but a matter of survival in larger projects.
* ["Directive"](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#directives) is a vocabulary word that you should understand and be able to give examples of.

## Variables
* **Variables** are a way to store things (colors, font stacks, other CSS values) that you want to reuse many places.
* They also make things more understandable by allowing you to name things (like `$warning-color`) instead of just the hex value.
* The naming things is very important

## Nesting and hierarchy
* **Nesting** lets you take advantage of hierarchy.
* You can structure your stylesheets like you structure your HTML.
* It makes complicated things easier to understand.
* When you are writing nested rules, use the parent selector (`&`) to refer back up the hierarchy
* You can nest properties as well as selectors (http://sass-lang.com/documentation/file.SASS_REFERENCE.html#nested_properties)

## Partials and modularity
* **Partials** are Sass files with little snippets of code.
* A good partial is focused on one thing and very modular.
* Partials _can_ make it a little harder to find things when you are new to a project, but good file naming conventions fix that.  
* A partial file name starts with a leading underscore.
* Names with leading underscores are not converted to CSS by themselves, they are imported into the primary Sass file using the @import directive.

## Importing partials
* The `@import` directive lets you modularize your code.
* It's better than the CSS `@import` directive because it happens in the development environment, not as the page loads (causing additional HTTP requests and delays).
* The `@import` directive just takes the name without the underscore and no extension

## Mixins DRY up your code
* The `@mixin` directive lets you make groups of CSS declarations and reuse them many places.
* Mixins save time, improving quality and, with good naming, makes your code easier to understand.
* They kind of look like JavaScript functions -- they can take parameters, too. But they don't return values.
* Some Sass tutorials use the example of using mixins to make vendor prefixes tolerable, but we have a better method with auto-prefixer.
* To use a mixin, use the `@include` directive.

## @extends and inheritance
* The `@extend` directive share CSS properties from one selector to another.
* It implements _inheritance_, where one selector takes on the properties of another selector and, well, _extends_ it.
* Mixins allow you to naturally implement a design that has visual consistency and cohesiveness (visual elements have common characteristics, so their classes have common code)
* You write less code and you don't repeat yourself. Again, higher quality, better design.
* This can get pretty complicated, especially when you start doing things like [@extend-Only Selectors](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#placeholders) so it's important to analyze your web design prior to starting to code so you can take full advantage of what Sass can do.

## SassScript
* You can use operators, parentheses, functions, and other language features in CSS directives using a set of extensions called [SassScript](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#sassscript).
* As you learn JavaScript and SassScript together, you will notice many similarities (and a few differences).
* Operators let you do simple math in your CSS directives, which can make your code easier to understand.
* [**Functions**](http://sass-lang.com/documentation/Sass/Script/Functions.html) provide lots of useful little behaviors that make working with colors, opacity, strings, numbers, lists, and other more esoteric things fun and easy.

##Screencasts
Treehouse has an introductory sequence of Sass classes.

* http://teamtreehouse.com/library/sass-basics
* http://teamtreehouse.com/library/advanced-sass
* http://teamtreehouse.com/library/modular-css-with-sass

If we get into Compass, watch this. There are lots of cool things in there.
http://teamtreehouse.com/library/compass-basics

# Textbooks

There's a short, cheap one here: http://abookapart.com/products/sass-for-web-designers

I have a copy you can look at if you like.

# Online resources

* [The main Sass site] http://sass-lang.com/
* [Sass Guidelines](http://sass-guidelin.es/)
* [Sass Style Guide](https://css-tricks.com/sass-style-guide/)
