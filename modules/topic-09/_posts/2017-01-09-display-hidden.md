---
title: Display Hidden
module: 09
---

## Hide with Display
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

The display property can also be used to 'hide' elements. At first, it may seem difficult to understand why it would be useful to hide an element, but this is done often in order to create "drop-down menus" or "hidden tips" type content.

To hide an element, set the `display` properties value to `none`. To get it to appear, you create a selector made up of the parent container and element in question, with the `:hover` pseudo-class added to the parent.

<div id="code-heading">CSS</div>
```css
.child-class-to-unhide {
    display: none;
}
.parent-container:hover .child-class-to-unhide {
    display: block;
}
```

In the following example, this exact technique is used to create an "additional information" type box.

<div class="pen-group">
  <p data-height="600" data-theme-id="30567" data-slug-hash="LOxMya" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-09] Display Hidden, Pt. 1" class="codepen"></p>
  <script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

  <div class="pen-result displayed_code_example_pen">
    <style>
      .example-container {
        font-family: sans-serif;
        font-size: 16pt;
        width: 100%;
        min-width: 200px;
        max-width: 500px;
        background-color: #BCD799;
        margin: auto;
        padding: 0;
      }
      .tip-header {
        height: inherit;
        font-size: 1.5em;
        padding: 1em;
        text-align: center;
        color: #fff;
        background-color: #79AF33;
      }
      .example-container .hidden-content {
        display: none;
        font-size: 1em;
        font-style: italic;
        padding: 1em;
      }
      .example-container:hover .hidden-content {
        display: block;
      }
    </style>
    <div class="example-container">
        <div class="tip-header">
            Hover over me for more information...
        </div>
        <div class="hidden-content">
            This is some hidden information,
            that serves to further enlighten your end-user.
        </div>
    </div>
  </div>
</div>


### Used for Dropdown Menus

This same technique can be used for to create dropdown menus.

The following code is one solution to creating a horizontal menu with a dropdown. Notice in line 33, that the content is hidden. Lines 47-49, cause the menu to be displayed, and lines 32-62 are used to present and style the dropdown menu.

Please study the following code to understand it better. You should also download the code and play with it via the links under the example.

<div class="pen-group">
  <p data-height="600" data-theme-id="30567" data-slug-hash="OOWrdp" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-09] Dropdown Menu" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen">
    <style>
      /* Set your header design: */
      header {
          background-color: #26272b;
          font-family: sans-serif;
          font-size: 12pt;
          text-transform: uppercase;
          margin: 0;
          height: 2.15em;
          text-align: right;
      }

      /* Set the layout of the menu: */
      .menu-item {
          display: inline-block;
          margin: -1px 1px 0 0;
          min-width: 8em;
          text-align: center;
          background-color: #26272b;
          padding: 0.5em 0;
      }

      /* Style the links: */
      .menu-item a {
          color: #fff;
          text-decoration: none;
      }
      .menu-item:hover {
          background-color: #1CCDCA;
      }

      /* Add a dropdown feature: */
      .dropdown {
          display: inline-block;
      }
      .dropdown-content {
          display: none;
          min-width: 8em;
          position: absolute;
          border: 1px solid #000;
          margin: 0;
          margin-top: 0.5em;
          color: #000;
          background-color: #fff;
          z-index: 1;
      }
      .dropdown-content a {
          color: #000;
      }
      .dropdown:hover .dropdown-content {
          display: block;
      }

      /* Style dropdown item display: */
      .dropdown-item {
          display: block;
          text-align: left;
          margin: -2px 0;
          padding: 0.5em;
          min-width: 7em;
      }
      .dropdown-item:hover, .dropdown-item:hover a {
          color: #baf0ef;
          background-color: #a2a2a2;
      }
    </style>
    <header class="">
       <div class="menu-item">
          <a href="#">Home</a></div>
       <div class="menu-item">
          <a href="#">About</a></div>
       <div class="menu-item dropdown">
          <a href="#">Dropdown</a>
          <div class="dropdown-content">
             <div class="dropdown-item">
                <a href="#">Services</a></div>
             <div class="dropdown-item">
                <a href="#">Press</a></div>
             <div class="dropdown-item">
                <a href="#">Careers</a></div>
             <div class="dropdown-item">
                <a href="#">Contact</a></div>
          </div>
       </div>
     </header>
     <div id="main">
      <h2>Page Title</h2>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam nisi quam, iaculis porta faucibus a, pharetra at purus. Nam sed elit erat. In in consectetur ipsum. Vestibulum vestibulum convallis purus, vestibulum egestas lectus consequat nec. Nullam malesuada, lorem nec blandit accumsan, lectus ante eleifend est, eu dictum nisl diam nec quam. Nunc hendrerit varius sagittis. Cras faucibus semper sapien, tincidunt consequat dolor condimentum sit amet. Donec rhoncus, risus gravida suscipit finibus, nisi ipsum luctus lacus, in mattis arcu sem nec tortor. Phasellus et rhoncus turpis. Donec nec nunc vehicula nisl luctus ultricies a et metus. Nam id nisl feugiat, porta lacus in, euismod diam.</p>
    </div>
  </div>
</div>


# { TODO: }
1. Study W3School's fantastic examples of [CSS Navigation Bars](https://www.w3schools.com/css/css_navbar.asp).
2. Read pages 318-329 of Chapter 13 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
