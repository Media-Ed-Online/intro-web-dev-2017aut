---
title: Step-by-Step Guide
module: 09
---

## Using CSS:<br/>A Step-by-Step Tutorial
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

On the previous page you got a taste of layouts with the "Shoping Site" product page. Here, we'll explore how we could build a blog page in under 3 hours, all with the power of CSS.

<iframe src="https://embed.plnkr.co/plunk/UOgE6A?show=style.css,preview" frameborder="0" width="130%" height="600px" style="margin: 100px 100px 100px -100px; border: 30px solid #F49626;"></iframe>

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/243960837?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>

If you're still a little uncertain how all this code comes together, please complete this tutorial using the files found in the "follow-along" folder:

1. [View the completed site]({{site.baseurl}}/modules/topic-09/layout-ex4/) in a new tab.
2. [Download the example files]({{site.baseurl}}/modules/topic-09/files/layout-ex4.zip), which includes 2 folders:
    - "completed" contains the full site
    - "follow-along" contains the templates and materials for this guide

This guide is broken up into 10 areas, so you can just view what you need help on:
1. <a href="#tut-1">Project Overview</a> (files, linking, stucture)
2. <a href="#tut-2">Calling Fonts</a> (downloaded and through Google API)
3. <a href="#tut-3">General Styling</a> (backgrounds, creating selectors)
4. <a href="#tut-4">Main Layout Areas</a> (the basic pieces)
5. <a href="#tut-5">Site Heading and Slogan</a> (display, alignment)
6. <a href="#tut-6">Interactive Site Logo</a> (hovers, placement, position)
7. <a href="#tut-7">Large Content Areas</a> (typographical styling, pseudo elements)
8. <a href="#tut-8">Small Content Areas</a> ("pull quotes" or asides)
9. <a href="#tut-9">Buttons</a> (pseudo classes)
10. <a href="#tut-10">Menus</a> (navigation bars and dropdowns)


<h3 id="tut-1">Step 1: Project Overview</h3>
Flies, linking, and site structure.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244068008?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-2">Step 2: Calling Fonts</h3>
Using fonts you've downloaded, and ones you're importing from Google Fonts.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244075708?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-3">Step 3: General Styling</h3>
Applying fonts, creating selectors, and adding background images and colors.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244098332?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-4">Step 4: Main Layout Areas</h3>
Styling the basic pieces, and an intro to DIVs and classes.

**NOTE:** At 09:00, I gave you the wrong property. It should be `max-value: 700px;` not `min-value: 700px;`.<br />

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244104033?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-5">Step 5: Site Heading and Slogan</h3>
Creating a site information area at the top of your page, which displays the site's title, slogan, and...

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244108602?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-6">Step 6: Interactive Site Logo</h3>
...a site logo that changes on hover.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244114956?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-7">Step 7: Large Content Area(s)</h3>
First creating a big box for a large body of text, then adding typographical styling and pseudo elements to make it visually interesting.

**NOTE:** `:first-letter` is a pseudo-element, not a pseudo-class.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244120327?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-8">Step 8: Small Content Area(s)</h3>
Using divs and floats to "pull" quotes out from the main body.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244154043?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-9">Step 9: Button</h3>
Creating a linking button using pseudo classes.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244158069?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


<h3 id="tut-10">Step 10: Menu</h3>
Creating a navigation bar to house links to your site pages and social media accounts, as well as adding a dropdown menu to organize content.

**NOTE:** At 27:00, I mispelled "width" which is why my `.menu-item` selections weren't sizing or centering. The element should look like

```
#site-links .menu-item {
  width: 6em;
  padding: .5em 1em;
  display: inline-block;
```

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/244167503?color=F49626&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>


# { TODO: }
1. <a href="{{site.baseurl}}/modules/topic-09/layout-ex4/" target="_blank">Open the example in a separate tab</a> to see it in full. Be sure to view the source code!
2. Try this tutorial out for yourself, and then try again without me. How'd it go?
