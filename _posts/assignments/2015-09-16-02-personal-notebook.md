---
layout: post
title: "02 Personal Notebook"
modified: 2015-09-16 14:52:48 -0700
category: assignments
tags: []
image:
  feature:
  credit:
  creditlink:
comments:
share:
---

# Objectives

* Create an maintain an online notebook to record key concepts and vocabulary terms
* Use the notebook to demonstrate proficiency in SCSS and other technologies
* Use the notebook to awareness of design languages and to demonstrate the ability to translate a design language to code.


# Iteration 1
This assignment has students use SCSS to style some cards according to the Google Material Design language. It starts with a template with obsolete or missing styling.



## Preparation

0. Fork this repo: [https://github.com/portlandcodeschool/afe-cards](https://github.com/portlandcodeschool/afe-cards) and clone it to your machine.  We will do this as a code-along in class as a review for students and to make sure everybody gets it ok.

0. Verify that you can build the SCSS files using your tool chain's Sass preprocessor. You don't need autoprefixer yet because we only require that the site work on Chrome for now.

0. Watch this video: [https://design.google.com/videos/making-material-design/](https://design.google.com/videos/making-material-design/)
0. Read this introduction: [https://www.google.com/design/spec/material-design/introduction.html](https://www.google.com/design/spec/material-design/introduction.html)
0. Review the [Material Design section on cards](https://www.google.com/design/spec/components/cards.html#cards-usage)
0. (Optional/Extra) Read the background information at
    * [Environment](https://www.google.com/design/spec/what-is-material/environment.html),
    * [Material Properties](https://www.google.com/design/spec/what-is-material/material-properties.html)
    * [Elevation Shadows](https://www.google.com/design/spec/what-is-material/elevation-shadows.html)
0. (Optional/Extra) For a series of videos about Material Design, see the YouTube playlist
    * [Intro to Material Design](https://youtu.be/p4gmvHyuZzw?list=PLOU2XLYxmsIJFcNKpAV9B_aQmz2h68fw_)
    * [Material Design in the Google I/O App](https://youtu.be/XOcCOBe8PTc?list=PLOU2XLYxmsIJFcNKpAV9B_aQmz2h68fw_)
    * [Paper and Ink: The Materials that Matter](https://youtu.be/YaG_ljfzeUw?list=PLOU2XLYxmsIJFcNKpAV9B_aQmz2h68fw_)
    * [Density-independent Pixels](https://youtu.be/zhszwkcay2A?list=PLOU2XLYxmsIJFcNKpAV9B_aQmz2h68fw_)

## Design and style cards

0. Design a "card" HTML & SCSS component that has the following characteristics (We will do this as a discussion in class)
    * It must contain an image. You can use a placeholder image from [placehold.it](https://placehold.it/), a colored banner whose color relates to the overall topic (HTML, CSS, etc.), or an image that evokes the specific topic of the card.
    * It must have a title that overlays the image/banner
    * It must have a summary that is always visible.
    * It must have a description that only appears when requested. Note Material Design does not allow flipping, so review the specification to see what sort of animation is legal within the language.
    * It must have at least one action that reveals the description.
    * It may optionally have a second action that links to an authoritative site (like MDN or sass-lang) that explains the item in more detail.
0. Make sure you use variables, `@include`, `@mixins` and `@extends`  directives to implement your design.
0. Create at least three cards with real content in each topic area (HTML, CSS, JS, Tools, Learning).

## Create and style glossary

0. Update the glossary with all the terms you learned this week. Use the definition list (`<dl>`) for semantic markup. Do not add any HTML for styling whatsoever.
0. Design and style the glossary to use the Material design language. There is more freedom here, but be ready to defend your choices. You may want to:
  * Use the [Material Design List guidelines](https://www.google.com/design/spec/components/lists.html)
  * Put a colored dot in front of the term that matches the overall topic color used in your cards

# Optional/Extra

You do not need to do these steps this week in Iteraton 1. You should consider doing them sooner or later to make your notebook into a portfolio piece demonstrating your understanding of Material Design.

0. Convert the existing `main.css` and other CSS files to SCSS so that you can start to remove obsolete style rules instead of overriding them.
0. Adjust your `.gitignore` file to ignore CSS files
0. Update the existing color palette to put the color values in variables and to use the new colors in the navigation menu, glossary, and footer.
0. Convert the navigation to the Material Design language, using the button styling described here: [https://www.google.com/design/spec/components/buttons.html](https://www.google.com/design/spec/components/buttons.html)


# Other resources

To see how others are implementing Material Design, check out:

* [Material Design Lite](https://github.com/google/material-design-lite)
* [Materialize](http://materializecss.com/)

But do not use these in your code.
