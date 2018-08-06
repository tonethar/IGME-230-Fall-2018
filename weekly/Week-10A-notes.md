# Week 10A - Frameworks and Libraries

## I. Topics
- CSS Frameworks
- JavaScript Libraries and Plugins
- HTML templates
- Code minification
- Single-page sites

This week, it's back to some Web design! We've talked about responsive design a fair amount, and been focused on hand-building our own pages. But in the real world, more and more developers are coming to rely on various resources of existing code that do a lot of the heavy lifting for them, and streamline the design and development process.

## II. Frameworks
A [CSS framework](https://en.wikipedia.org/wiki/CSS_framework) is a set of CSS that can be applied as a starting point for designing a responsive page or site. The big one right now is Bootstrap, which was originally developed as Twitter's underlying responsive CSS. There are a lot of them out there, though, including:
- [Bootstrap](https://getbootstrap.com/)
- [Skeleton](http://getskeleton.com/)
- [Materialize](http://materializecss.com/)
- [Bulma](https://bulma.io/)

One thing you'll notice in all these frameworks is that they provide both readable and [minified](https://en.wikipedia.org/wiki/Minification_(programming)) code. This serves the purpose of decreasing our file sizes (and thus our download times), as well as making production code harder to decipher and copy.

## III. Libraries
There are also a ton of JS libraries in common use nowadays, giving us external JS files with access to new functions and functionality. We've already seen jQuery for processing AJAX and handling some other issues. Some of these libraries help streamline our processes, like jQuery, some help us build JS-based responsive sites, like Angular and React, some even add additional capabilities, like Node.js which lets us do server-side JS programming.
- [jQuery](https://jquery.com/)
- [Angular](https://angularjs.org/)
- [React](https://reactjs.org/)
- [PixiJS](http://www.pixijs.com/)
- [Node.js](https://nodejs.org/en/)

You'll note once again that libraries like jQuery provide minified code, which can have a significant impact on file sizes.

## IV. Plugins
In addition to libraries, there are tons of plugins and other code snippets available on the Web to add functionality quickly. jQuery's site lists a ton of these. Another great example, useful for portfolios, is [Fancybox](http://fancyapps.com/fancybox/3/), a jQuery "lightbox" plugin for adding interactive galleries to your pages.

## V. Templates
While we're at it, let's talk about HTML templates (also known as HTML themes). There are a lot of options to choose from, most of which use both a CSS framework and a JS library in addition to their own custom HTML and CSS. Templates are a quick and easy way to take pre-fab pages, populate them with your own content, and have a responsive site up and running in potentially a matter of minutes. Of course, on your assignments you need to build your own pages, not use templates, but they are a great resource for future work! There are a lot of these online, but here are some random examples:
- [TemplateMo](http://www.templatemo.com/)
- [tooplate](http://www.tooplate.com/)
- [Templated](https://templated.co/)
- [Theme Forest](https://themeforest.net/category/site-templates)

Take a look at what they provide, and what frameworks/libraries they use.

## VI. Single-page Sites
Single-page sites are becoming more and more popular, especially in the age of responsive design. These include sites like the "endless scrollers" we see in social media like Tumblr and Facebook, the sectioned "whole site on one scrolling page" like many portfolios, and web-app sites where all the content is changed on one page via JavaScript.

[What are the advantages and disadvantages of single-page sites?](https://www.uxpin.com/studio/blog/single-page-vs-multi-page-ui-design-pros-cons/)

Here are some cool examples:
- https://www.epicgames.com/paragon/
- https://www.airbnb.com/belong-anywhere
- http://www.ginventory.co/  
- http://www.dds.mu/

Implementation:
- Some sites are simply a single page, nothing more.
- Some allow some in-page navigation, linking to IDs on the page
```html
<a href="#section1">Section 1</a>
```
- Some use JS to manipulate the DOM, hiding or showing different elements when navigation is clicked, or rewriting innerHTML

## VII. Helpful Exercises
- [CSS Frameworks](../exercises/week-11/frameworks-ice.md) - this is an extra credit exercise (see dropbox)
- [Lynda.com Bootstrap Tutorial](https://www.lynda.com/Bootstrap-tutorials/What-well-build/186538/371577-4.html) - this takes about 2 hours, and walks you through creating a template that you can build on when creating your portfolio mini-project.
- [Lynda.com Skeleton Tutorial](https://www.lynda.com/CSS-tutorials/Welcome/372808/413142-4.html) - another nice option, with a slightly simpler layout.

## VIII. Demo
Together we will build a responsive web page using the [Skeleton](http://getskeleton.com) framework. This will be a simplified version of the page created in the Skeleton Tutorial linked above.
1. First we will look at the completed version of the demo (and the Skeleton Tutorial) in class. The Skeleton Tutorial has some nice features such as LightBox that you will likely want to use on your project.
1. Next we will download the start files from mycourses (we will use the image files are from the Skeleton Tutorial above)
1. Now head to http://getskeleton.com, look over the docs and download the skeleton framework
1. Copy the *css* folder from the Skeleton download into our *start* folder
1. Link to *css/normalize.css* & *css/skeleton.css*
1. Head to https://fonts.google.com and copy the link to the *Abel* and *Satisfy* fonts
1. Walk through *skeleton.css*:
    - change max-width of container to 1000
    - skeleton uses a 12-column layout
    - *container* class
    - *columns* class
    - *row* class
1. Build container &lt;div>
1. Add &lt;header>
1. Use CSS to style up the header. We will make it 12 columns wide (the full 1000px width) and give it a green background color.
1. Add rows, columns, and images - wow those images are big!
1. Add CSS to fix things.
1. Resize the window to see how the framework is automatically responsive.
1. Make even more responsive with media queries



## IX. Assignment
- [Portfolio Mini-Project](../projects/portfolio-mini-project.md)

<hr><hr>

[<-- Back to IGME-230 Schedule](../schedule.md)
