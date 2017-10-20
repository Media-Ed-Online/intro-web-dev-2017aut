---
title: CSS Applied
module: 07
---

## CSS Applied:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

Lets look at some applied CSS, to start understanding how it will effect our webpages.

You'll see in the example below that the `<h1>`, `<p>`, `<strong>`, and `<em>` elements are selected. Except for the first instance with the line containing `.main-content`, the elements are selected using "element" or "type" selectors. "Main Content" uses a class selector (`.className`), which will be discussed in a few pages.

Within each declaration block, there are multiple style rules, each effecting a specific aspect. Each of the declarations, for each selector, either effects border or background color.

Notice that in the displayed HTML sample below how the code creates borders make it easier to visually identify the individual elements.

### Altogether Now

<p data-height="600" data-theme-id="30567" data-slug-hash="boZEEy" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-07: CSS Applied" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

<div class="pen-result displayed_code_example_pen">
  <style>
    .main-container {
        border-style: solid;
        border-width: 2px;
        border-color: limegreen;
        padding: 10px;
        background: #373E42;
    }
    .h1 {
        border-style: solid;
        border-color: orange;
        /* Set a unique background color. */
        background: #f1f1f1;
    }
    .p {
        border-style: solid;
        border-color: gold;
        background: #f1f1f1;
    }
    .p>strong {
        border-style: solid;
        border-width: 2px;
        border-color: tomato;
    }
    .p>em {
        border-style: solid;
        border-width: 2px;
        border-color: tomato;
    }
  </style>
  <div class="main-container">
    <h1 class="h1">This Heading 1 is quite stylish.</h1>
    <p class="p">A stylish paragraph of <strong>happiness</strong> within a div element.</p>
    <p class="p">Another stylish paragraph, that's not <em> as happy,</em> as it follows the other paragraph.</p>
  </div>
</div>

# { TODO: }
Please [click here](https://codepen.io/Media-Ed-Online/pen/boZEEy) to edit the above Pen:
1. Change the color of some text.
2. Changed the background of the main `<div>` to "silver".
3. Change all the boarders to "#5e001d".
4. Add another `<p>` with both an `<em>` and `<strong>` element. How does it look?
5. Feeling adventurous? Add some paragraphs to the secondary `<div>` and add your own style elements to `.secondary-container` in the CSS - whatever you can come up with!
