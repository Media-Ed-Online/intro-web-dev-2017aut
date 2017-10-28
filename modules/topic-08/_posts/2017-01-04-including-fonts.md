---
title: Including Fonts
module: 08
---

## It's All In the Family:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

To specify a font, use the `font-family: ` property. This is followed with a comma-delineated, list of fonts for the browser to _try_ and load.

At a minimum, every browser will be able to render something when passed one of three default values:

- `sans-serif`
- `serif`
- `monospace`

<div class="pen-group">
  <p data-height="200" data-theme-id="30567" data-slug-hash="RLzBbm" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Including Fonts, Pt. 1" class="codepen"></p>
  <script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

  <div class="pen-result displayed_code_example_pen">
      <style>
          .p1 {
              font-family: sans-serif;
          }
          .p2 {
              font-family: serif;
          }
          .p3 {
              font-family: monospace;
          }
      </style>
      <p class="p1">sans-serif</p>
      <p class="p2">serif</p>
      <p class="p3">monospace</p>
  </div>
</div>

Instead of using generic font class names, developers may also use specific font family names. When a specific font family is listed, the browser will try to load the font from the client computers font library.

For example, the following will cause the browser to first try and load "Comic Sans MS". If the client computer (yours in this case) does not have a font matching that name, it will then try "Comic Sans", then "Garamond", then "Times", then finally the default 'serif' font. The browser will do this by asking the client for the font. If the client doesn't have the font, then the browser will try the next listed font.

<div class="pen-group">
  <p data-height="300" data-theme-id="30567" data-slug-hash="WZqKxo" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Including Fonts, Pt. 2" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen">
    <style>
        #heading-1 {
            font-family: 'Comic Sans MS', 'Comic Sans', Garamond Times, serif;
        }
    </style>
    <h1 id="heading-1">Displayed Font</h1>
  </div>
</div>


### Web-Safe Fonts

Fonts that developers can count on being available by the system are known as "web-safe" fonts. These include font families that both Windows and Mac should have.

Web-safe fonts include:

- <p style="font-family: Arial; font-size:1.5em;">Arial</p>
- <p style="font-family: Georgia; font-size:1.5em;">Georgia</p>
- <p style="font-family: Times; font-size:1.5em;">Times New Roman</p>
- ...as well as these other [web safe fonts](http://www.ampsoft.net/webdesign-l/WindowsMacFonts.html).

The advantage of using fonts from this list is that the client computer will already have the font. This reduces load times and may increase performance.


# { TODO: }
Read page 269-273 of Chapter 12 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
