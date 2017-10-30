---
title: Pseudo-Classes
module: 08
---

## Psuedo-Classes
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

In CSS, a "**pseudo-class**" is an event or state that can be triggered by the browser. When this event is triggered, additional CSS rules can be applied to a page.

The horribly obnoxious ["Wrap-Up" page from Topic-07]({{site.baseurl}}/modules/topic-07/wrap-up/), utilized CSS pseudo-classes.

This is the same technology that allows browsers to alter the appearance of links when you hover over them, click them, or after you have visited them.

Like pseudo-elements, pseudo-classes are appended after a CSS selector.

**NOTE:** Pseudo classes are preceded by only a single colon, as opposed to a set.

<div id="code-heading">CSS</div>

```css
/* A CSS Pseudo-Element Selector: */
p::first-letter {}

/* A CSS Pseudo-Class Selector: */
p:hover {}
```


### Common Pseudo-Classes

**NOTE:** Any pseudo-class that relies upon mouse information (such as the ones below) will not translate to mobile devices.

#### `:hover`

The `:hover` class is triggered whenever a users mouse "hovers over" the selected element.

<div class="pen-group">
<p data-height="400" data-theme-id="30567" data-slug-hash="bYNpEY" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Pseudo-Classes, Pt. 1" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>
  <div class="pen-result displayed_code_example_pen">
    <style>
    .hover-element {
        font-size: 1em;
        background-color: #545454;
        color: #c4c8c4;
        padding: 1em;
        text-align: right;
    }
    .hover-element:hover {
        font-size: 4em;
        background-image: url(../imgs/puppy.jpg);
        background-position: center center;
        background-size: cover;
        color: gold;
        text-transform: uppercase;
        font-weight: bold;
        text-align: justify;
        letter-spacing: 0.2em;
        padding: 0em;
        height: 75%;
    }
    </style>
    <div class="hover-element">
      Don't hover over me, please...
    </div>
  </div>
</div>


Hover is more often used to specify how link text will appear when a user hovers over it.

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="KywzgB" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Pseudo-Classes, Pt. 2" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen">
    <style>
      .element-1 {
        font-size: 1.5em;
        font-family: sans-serif;
      }
      .element-1 a {
        color: #79AF33;
        text-decoration: none;
      }
      .element-1 a:hover {
        color: #1CCDCA;
        font-style: italic;
      }
    </style>
    <div class="element-1">
        You should visit the <a href="https://en.wikipedia.org/wiki/The_Garden_of_One_Thousand_Buddhas">Garden of a Thousand Buddhas</a> in Montana sometime. It is beautiful.
    </div>
  </div>
</div>


#### `:active`

The `:active` pseudo-class is applied when a user is clicking on an element.

Often this is used to make a button feel more real by slightly changing the color when the user presses it. But this can be used for any pressed effect.

<div class="pen-group">
  <p data-height="600" data-theme-id="30567" data-slug-hash="OOPNgx" data-default-tab="css,html" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Pseudo-Classes, Pt. 3" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen">
    <style>
      .parent-element {
        min-height: 10em;
      }
      .button-1 {
        font-size: 1.5em;
        color: white;
        font-weight: 600;
        background-color: rgb(28,205,202);
        border-color: #8f8b8b #383636 #383636 #8f8b8b;
        border-width: 9px 15px 15px 9px;
        border-style: solid;
        position: relative;
        margin: auto;
        top: .5em;
        padding: 1em;
        width: 9em;
        text-align: center !important;
      }
      .button-1:hover {
        color: #383636;
        font-style: italic;
      }
      .button-1:active {
        color: #fff;
        background-color: rgb(17, 127, 126);
        border-color: #383636 #8f8b8b #8f8b8b #383636;
        border-width: 15px 9px 9px 15px;
      }
      .link-button {
        text-decoration: none !important;
        color: inherit !important;
      }
    </style>
    <div class="parent-element">
       <center><a href="https://google.com" class="link-button"><div class="button-1">
          Press me...<br />
          <span style="font-size: small; text-transform:uppercase;">(I link to Google)</span>
       </div></a></center>
    </div>
  </div>
</div>


# { TODO: }
1. Read pages 290-298 of Chapter 12 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
2. Explore this area on our "[Go Further With Fonts](../going-further#pseudo-classes)" page.
