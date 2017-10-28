---
title: Alignment
module: 08
---

## Text Alignment
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

Alignment properties allows developers to specify how text should be positioned within an element.


### Horizontal

The `text-align: ` property specifies horizontal placement of text in an element.

#### Values

This property should only be passed by keywords. The possible values are:

- `left`
- `center`
- `right`
- `justify`

#### Example

In the following code, a simple paragraph with _Lorem Ipsum_ text is aligned using the above property declaration values.

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="rYNLdw" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Alignment, Pt. 1" class="codepen"></p>
  <script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

  <div class="pen-result displayed_code_example_pen">
      <style>
      .parent-1 {
          background-color: saddlebrown;
          padding: 1em;
          margin: 1em;
      }
      .parent-1 div {
          background-color: #fff;
          padding: 2em;
          margin: 1em;
      }
      .left {
          text-align: left;
      }
      .right {
          text-align: right;
      }
      .center {
          text-align: center;
      }
      .justify {
          text-align: justify;
      }
      </style>
      <div class="parent-1">
          <div class="left">
              <h2>Left</h2>
              <p>Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.</p> </div>
          <div class="right">
              <h2>Right</h2>
              <p>Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.</p> </div>
          <div class="center">
              <h2>Center</h2>
              <p>Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.</p> </div>
          <div class="justify">
              <h2>Justified</h2>
              <p>Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.</p> </div>
      </div>
  </div>
</div>


### Vertical

The `vertical-align: ` property specifies vertical placement of text in relation to an inline element, usually images.

#### Values

The property should only be passed by keywords. The most common used inlcude:

- `top`
- `text-top`
- `middle`
- `bottom`
- `text-bottom`

#### Example

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="Bmazqa" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Alignment, Pt. 2" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen">
		<style type="text/css">
      #jpg-ex {
        vertical-align: text-top;
        display: inline;
        border: 0px;
        margin: 0px !important;
      }
      #png-ex {
        vertical-align: middle;
        display: inline;
        border: 0px;
        margin: 0px !important;
      }
      #gif-ex {
        vertical-align: text-bottom;
        display: inline;
        border: 0px;
        margin: 0px !important;
      }
      </style>
    <body>
      <h1>Common Image File Types for Web</h1>
      <p><img src="../imgs/jpg.svg" width="75" height="75" alt="JPG file type" id="jpg-ex" /> JPEG/JPG</p>
      <p><img src="../imgs/png.svg" width="75" height="75" alt="PNG file type" id="png-ex" /> PNG</p>
      <p><img src="../imgs/gif.svg" width="75" height="75" alt="GIF file type" id="gif-ex" /> GIF</p>
    </body>
  </div>
</div>


# { TODO: }
Read pages 285-286 of Chapter 12 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
