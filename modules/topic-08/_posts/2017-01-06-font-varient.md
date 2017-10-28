---
title: Caps & Cases
module: 08
---

## Font Variant & Transform:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

There are two properties that allow developers to set the capitalization of text.

### Font Variant

The `font-variant: ` property allows developers to specify whether text should appear in all caps, with 'non-capitalized' letters being displayed as small caps.

In a small-caps font, all lowercase letters are converted to uppercase letters. However, the converted uppercase letters appears in a smaller font size than the original uppercase letters in the text.

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="zPYBow" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Caps & Cases, Pt. 1" class="codepen"></p>
  <script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

  <div class="pen-result displayed_code_example_pen">
    <style>
        .content-p {
            font-variant: small-caps;
            font-size: 2em;
        }
    </style>
    <p class="content-p"> An example of the font-variant property. Notice how the first letters of each sentence are still full size. But, the rest of the characters are "small-caps".</p>
  </div>
</div>


### Text Transform

The second property that allows for the control of capitalization is `text-transform: `.

Text transform takes one of four keyword values;

- `none`; Do nothing.
- `uppercase`; Make all characters uppercase.
- `lowercase`; Make all characters lowercase.
- `capitalize`; Capitalize the first letter of each word. (Sometimes also known as "Title Case")


<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="KyKMWd" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Caps & Cases, Pt. 2" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen">
    <style>
    .text-1 {
        text-transform: none;
    }
    .text-2 {
        text-transform: uppercase;
    }
    .text-3 {
        text-transform: lowercase;
    }
    .text-4 {
        text-transform: capitalize;
    }
    </style>
    <h2 class="text-1">Some text, wiTH crAzY capitaLIZATION.</h2>
    <h2 class="text-2">Some text, wiTH crAzY capitaLIZATION.</h2>
    <h2 class="text-3">Some text, wiTH crAzY capitaLIZATION.</h2>
    <h2 class="text-4">Some text, wiTH crAzY capitaLIZATION.</h2>
  </div>
</div>

# { TODO: }
Read page 281 of Chapter 12 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
