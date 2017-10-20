---
title: Background Color
module: 07
---

## Background Color:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

The first CSS property we will officially look at is "background color."

The background color property allows developers to specify the background color of elements.

As with all CSS multi-word properties, each word is separated with a hyphen, `background-color:`.

The background color property takes a color as its value. This can be a hex (i.e. `#ae34ff`) value, or an rgb value (i.e. `rgb(174, 52, 245)`).

**NOTE:** I am also including the CSS property `padding`. These will force the page to render block-level elements, even when they have no text content. Padding is the amount of space between the element content, and the edge of the element. In the case of no content, it is the amount of space between the edge and the center of the element.


<div id="code-heading">HTML</div>
```html
<style>
    div.main-container {
        background-color: rgb(127, 172, 200);
        padding: 100px;
    }
</style>

<div class="main-container">

</div>
```

<div class="displayed_code_example">
<style>
    .main-container {
        background-color: rgb(127, 172, 200);
        padding: 100px;
    }
</style>

<div class="main-container">
</div>
</div>


### Background Color of the Entire Page

There are two easy ways to set the background color for a page.

<p>1. Set the background color of the <code>&lt;body&gt;</code> element.</p>

<div id="code-heading">CSS</div>
```css
body {
    background-color: #ee12ff;
}
```
<br/>

<p>2. Wrap the entire page contents in a <code>&lt;div&gt;</code> element with an appropriate class name (i.e. <code>&lt;div class="main-container"&gt;</code>), and set the background color of that element.</p>

**NOTE:** You will also need to set the elements height property in this case `{ height: 100%; }`.

<div id="code-heading">CSS</div>
```css
.main-container {
    background-color: #ffee12;
}
```

### Inner Elements

When setting the background color of inner elements, you should do choose colors that encourage readability, and complement the main color schemes of the site.

<p data-height="400" data-theme-id="30567" data-slug-hash="ZXPeQW" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07] Background Color" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

<div class="pen-result displayed_code_example_pen">
    <div class="embed-responsive" style="padding-bottom:560px;"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/07/background-color/" frameborder="0" allowfullscreen></iframe></div>
</div>


# { TODO: }
Read pages 250-253 of Chapter 11 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
