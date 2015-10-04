---
layout: post
title: "03 Scaffold a Boostrap/Sass site with Yeoman"
modified: 2015-10-03 16:22:17 -0700
category: assignments
tags: []
image:
  feature:
  credit:
  creditlink:
comments:
share:
---
# Theme: tools

Reference: http://slides.com/auraelius/style-guides-11

# Goals

Our tools goal is always: less work & more quality. Specifically:

0. **More quality** - script it, debug it, control it, forget it. Until you have to change it. Then put the whole thing under version control just like any other code. This gives us...
0. **More certainty** in our projects - it would be great to know that we always start with the best possible setup or at least the one we want. Don't forget anything. And we need to do all this with...
0. **Less work** - setting up the files, the templates, the tool chain for each project has lots of details and steps. Once we figure it out, we should script it so that we don't have to do the same work over and over.

# Tools we will use in this module:

0. **Node package manager** - the way we get JavaScript components for our tool chain or our product
0. **Bower package manager** - the way we get components for our product
0. **Gulp** - task automation for our tool chain
0. **Yeoman** - scaffolding tool - specialized task automation that assembles all the files, tools, and components for a web application.

Yeoman uses "generators" - plugins that assemble and install specific combinations of components and tools. Choosing a generator involves the same selection and vetting process of any tool choice. Basically, you ask,

Is it

* Appropriate?
* Well-documented?
* Supported by a healthy community?
* Up-to-date?

Check the [yoeman generator site](http://yeoman.io/generators/) site for lots of examples.

# Exercise:

Scaffold a site that has the following major parts

- Bootstrap
- Sass
- Gulp

We'll use [gulp-webapp](https://github.com/yeoman/generator-gulp-webapp#readme) (It has the appropriate functionality, high search rankings, good documentation, and recent project activity. Besides, a test install and examination of the results showed that the generated files looked ok.)

## Steps to scaffold the site:

1. Install node packages: gulp, bower, yo
2. To make sure that yeoman is installed, test with the commands: <kbd>$ yo -- help; bower --help</kbd>
3. Install a generator (Notice the naming convention and refer to [the Readme.md file](https://github.com/yeoman/generator-gulp-webapp#readme) for details)  
<kbd>$ npm install generator-gulp-webapp</kbd>
4. Run yo  
<kbd>$ yo gulp-webapp</kbd>
5. Include all suggested components: Sass, Bootstrap, Modernizer.
6. Watch it work and be amazed at how little work you are doing. Yay!
7. Examine the results
    * Notice the .gitignore file
    * Notice where components are installed and the resulting file paths in the html and sass files.
8. Fire up the toolchain  
<kbd>$ gulp serve</kbd>
9. Notice the live update feature
10. Edit bower.json project definition file with appropriate information

## Steps to set up your live style guide

If you are lucky enough to have a designer that created a style guide for you, consider yourself blessed. Your next step is to map that styleguide to the Bootstrap Sass variables that you must override.

0. Make a quick/easy static guide by going to  
<kbd>http://www.poormansstyleguide.com/</kbd>
0. Create a new file called <kdb>styleguide.html</kbd> in the root of your app.
0. Paste the HTML from this site <kdb>styleguide.html</kbd>
0. Modify <kdb>styleguide.html</kbd> to include your compiled CSS file. Check <kdb>index.html</kbd> if you don't know the name of the CSS file.
0. Read the bootstrap documentation (URL) for which components, classes, and variables to use
0. Set up your styleguide with the same classes that you will use in your Bootstrap customizations.
0. Override the appropriate variables to customize styles and components. When your style guide looks good, then start building the site pages.

# Helpful hints

* Watch to make sure your Sass files are included and extended, etc, in the right order to override the bower components bootstrap SCSS files.
* You should avoid modifying the distribution versions of bower components.
* You should not source control anything that is installed, configured, or created by your tool chain. There are exceptions, but this is the general concept.
