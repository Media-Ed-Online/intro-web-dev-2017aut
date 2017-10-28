---
title: Text Decoration
module: 08
---

## Text Decoration
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

The `text-decoration: ` accepts the following declaration keywords;

- `underline`
    - Underline text.
    - This is the default decoration browsers apply to links.
- `overline`
    - Place a line over text.
- `line-through`
    - Place a line through text.
    - This is often used to show text that no longer applies in content. (Also known as "strike through").
- `none`
    - Remove any decoration of text.
    - This is used by developers to remove default browser link decoration.

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="dZyXzK" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Text Decoration" class="codepen"></p>
  <script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

  <div class="pen-result displayed_code_example_pen">
    <style>
    .text {
        background-color: rgb(55, 62, 66);
        color: turquoise;
        padding: 0.75em;
        text-align: center;
    }
    .text-1 {
        text-decoration: none;
    }
    .text-2 {
        text-decoration: underline;
    }
    .text-3 {
        text-decoration: overline;
    }
    .text-4 {
        text-decoration: line-through;
    }
    </style>
    <h2 class="text text-1">Some text to decorate.</h2>
    <h2 class="text text-2">Some text to decorate.</h2>
    <h2 class="text text-3">Some text to decorate.</h2>
    <h2 class="text text-4">Some text to decorate.</h2>
  </div>
</div>


# { TODO: }
Read page 282 of Chapter 12 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
