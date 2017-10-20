---
title: Selector Types
module: 07
---

## Selector Types:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

There are multiple ways of selecting elements from an HTML page. This allows developers to use general selectors when a rule should apply to many elements, and specific selectors when a rule should only apply to a few or one element.

### Universal Selector

The Universal selector is used to style _every_ element on a page. The universal selector is the star (`*`). (The star is often used in computer science to mean "all").

<p data-height="400" data-theme-id="30567" data-slug-hash="QqoNLG" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  CSS Selectors, Pt. 1" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


### Element Selectors

The element selector is used to select all elements of a certain type. This selector is applied by simply using an element name (the reserved keyword placed in the opening tag of an element).

So to select all level 2 headings we write `h2`. Then we could turn their text blue and make them quite large with style rules in the declaration block.

**NOTE:** This is the selector type that has been demonstrated the most so far in the last few pages.

<p data-height="400" data-theme-id="30567" data-slug-hash="oGVxXV" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  CSS Selectors, Pt. 2" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


### Class Selectors

Class names assigned to HTML elements via the `class=""` attribute can also be used to style elements. To select class elements, prepend a dot (`.`) to the front of the class name in the CSS.

Using class selectors is a great way to select elements that serve the same function.

<p data-height="400" data-theme-id="30567" data-slug-hash="eGXZZM" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  CSS Selectors, Pt. 2" class="codepen"></p>


### ID Selector

Just like the class selector, the ID selector allows developers to define style rules for a specific element by calling its unique ID.

ID names are prepended with a number sign (`#`).

<p data-height="400" data-theme-id="30567" data-slug-hash="EwMKNd" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  CSS Selectors, Pt. 3" class="codepen"></p>


# { TODO: }
Read page 237 of Chapter 10 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
