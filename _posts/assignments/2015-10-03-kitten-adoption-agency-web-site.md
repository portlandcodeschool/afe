---
layout: post
title: "04 Kitten Adoption Agency web site"
modified: 2015-10-03 14:21:12 -0700
category: assignments
tags: []
image:
  feature:
  credit:
  creditlink:
comments:
share:
---

The final project brings together most of the material we learned during the class:

* You use the entire front end toolchain.
* You customize bootstrap using Sass
* you interpret a website design and implement it in code

Earlier exercises laid the groundwork for this project:

* Our work with Sass allows us to structure our CSS style sheets more specifically, more expressively, and higher-quality due to the constant checking and linting of our code
* Our work with a website designer to understand how to implement her visual design helped us recognize potential problems in implementation and communicate these issues to the designer to influence the design and improve the quality of the implementation
* Our work analyzing the customer goals through user stories helped us map out the flow of the user interface and focus on what needs to be implemented first
* Our work with front end tool chains set up a development environment which will allow you to use sass, auto prefixing, and yeoman scaffolding to make development faster, higher quality, and more streamlined

# Phase One: Review the site design

0. Examine the Design materials at the bottom of the page to orient on user and client goals
0. Examine the prioritized user stories that are in scope.
0 Examine the site design mockups to analyze how to structure your HTML & SCSS to implement the design
    - There is no mobile design mockup!! So, you must create a simple wireframe with content blocks. Remember, you must code using mobile-first with progressive enhancement technique
    - How will you use the Bootstrap grid system to manage the layout? Write down your thoughts.
    - What Bootstrap components and plugins will be useful? Write down your thoughts.
    - What Bootstrap style classes will you need to control to implement the look? Write down a beginning list.

# Phase Two: Set up your development environment

This should already be done due to earlier class work. Make sure it includes the following

- Git
- Node
- Gulp
- Sass
- Autoprefixer
- Bower
- Yeoman

# Phase Three: Scaffold the site

0. Follow the generic instructions to scaffold a bootstrap/sass site with yo. (link)
0. Update the appropriate manifest files with information specific to this project.
0. Initialize the project as a git repo
    - Make sure your .gitignore file is set up correctly to ignore node modules and any temporary files created by your tool chain
    - initialize the project to create a local git repo and make your first commit
    - create a github repo and connect your local repo, making your first push
    - Create a gh-pages branch and make sure you can deploy the site with the scaffold boilerplate page

# Phase Four: Iterate on implementation

Perform this phase in iterations. An example series of iterations is listed below, but you can choose your own path.

0. Create the basic layout of the landing page; commit and push your changes
0. Add the cards from the earlier assignment for the kitten list.
0. Add the donation form. Please code it by hand don't use google forms, wufoo or other service. It does not have to store information anywhere but you can use the following link in your form tag to test the operation of the form: (URL to form-echo.herokuapp.com)
0. Add the kitten detail page. Create the page for just the first kitten. You do not have to create any additional pages. In a data-driven website, you would create the template for the page and then he would use programming to fill in that template from a database. That is beyond the scope of this class. So, just create one page and fill it with with the information from the first kitten.
0. At the adoption form. Again, code this by hand.

# Design elements

## Client brief

This web site is for a small kitten adoption agency. Client is a no-kill shelter

*Time deadline:* 1 week

*Client goals:*

1. Place animals in forever homes
2. Get funding for operations

*Budget:*

* Two person-weeks for developers (two people for one week)
* Two person-weeks for designer (already spent)
* No budget for hosting (use gh-pages)

## Roles & User stories

Roles that have been identified include:
Roles

* Adopter - a person that wants a kitten
* Donor - a person that needs a kitten

Others roles that are out of scope are:

* Volunteer
* Sponsor
* Marketer
* Janitor
* Staff
* Vet

#### User Stores in scope

These are user stories that we think we can accomplish in the budgeted time. Because we don't have copy from the client, the user story about getting information will have to be limited or not implemented.

As an Adopter  
In order to find a forever friend  
I want to see what's available  

As an Adopter  
In order to find a forever friend  
I want to choose an animal  

As an Adopter  
In order to find a forever friend  
I want to learn about each animal  

As an Adopter  
In order to find a forever friend  
I want to fill out an application  

As an Adopter  
In order to find a forever friend  
I want to learn about the process and shelter  

As a Donor  
In order to find a home for my animal  
I want to provide information about my animal  

As a Donor  
In order to find a home for my animal  
I want to provide information about my animal  


#### User Stores not in scope

These were identified during brainstorming but cannot be implemented in the available budget.

As an Adopter  
In order to find a forever friend  
I want to learn about the status of my application  

As an Adopter  
In order to find a forever friend  
I want to be notified when my application is decided  

As an Adopter  
In order to find a forever friend  
I want to find an animal with specific characteristic  

As an Adopter  
In order to find a forever friend  
I want to schedule time to meet an animal and introduce my pets  

As an Adopter  
In order to find a forever friend  
I want to pay fees and take an animal home  

As a Donor  
In order to find a home for my animal  
I want to learn about the process and shelter  

As a Donor  
In order to find a home for my animal  
I want to bring my animal to the shelter  

## Style Guide

You are required to have a live style guide for this class. Make a quick/easy static guide by going to

http://www.poormansstyleguide.com/

0. Create a new file called <kdb>styleguide.html</kbd> in the root of your app.
0. Paste the HTML from this site and bam! You've got your own style guide!
0. Set up your styleguide with the same classes that you will use in your Bootstrap customizations.
0. Define your Sass variables to make your live style guide mimic the styles given by the web designer.

![cat-adoption-styleguide](/afe/images/cat-adoption-styleguide.png)

## Mockups

Here are the mockups for the site design. Try to make your site as close as possible. However, it is better to finish all the pages and have a few things that aren't exactly correct. Don't get stuck trying to match the design exactly and miss your deadline!

### Home page

![cat-adoption-home-v1](/afe/images/cat-adoption-home-v1.png)

### Individual cat page, form closed

![cat-adoption-page-v1](/afe/images/cat-adoption-page-v1.png)

### Individual cat page, form open

![cat-adoption-page-form-open-v1](/afe/images/cat-adoption-page-form-open-v1.png)
