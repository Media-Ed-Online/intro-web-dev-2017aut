---
title: Alignment & Indents
module: 08
---

## Alignment & Indentation
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

Aligning your headers or captions can help draw the eye visually to new text events on the page. Likewise, indents can be used to breakup points introduced under a common topic, or delineate new paragraphs.

### Text Alignment

Alignment properties allows developers to specify how text should be positioned within an element.

#### Horizontal

The `text-align: ` property specifies horizontal placement of text in an element.

##### Values

This property should only be passed by keywords. The possible values are:

- `left`
- `center`
- `right`
- `justify`

##### Example

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


#### Vertical

The `vertical-align: ` property specifies vertical placement of text in relation to an inline element, usually images.

#### Values

The property should only be passed by keywords. The most common used inlcude:

- `top`
- `text-top`
- `middle`
- `bottom`
- `text-bottom`

##### Example

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="wPvjgW" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Alignment, Pt. 2" class="codepen"></p>

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
      <p><img src="../imgs/jpg.png" width="64" height="64" alt="JPG file type" id="jpg-ex" /> JPEG/JPG</p>
      <p><img src="../imgs/png.png" width="64" height="64" alt="PNG file type" id="png-ex" /> PNG</p>
      <p><img src="../imgs/gif.png" width="64" height="64" alt="GIF file type" id="gif-ex" /> GIF</p>
    </body>
  </div>
</div>


<div style="border-top: 5px dotted #1CCDCA; width: 100%; margin-top: 150px"></div>
<div style="border-top: 5px dotted #1CCDCA; width: 100%; margin-top: 20px"></div>


### Text Indent

First line indents are another typesetting property that CSS allows for the manipulation of. This property is controlled via `text-indent: `.

This property controls how much the first line of a paragraph is indented.

As with many text properties, this once can be passed absolute values with pixels (`px`) or points (`pt`). It can also be passed relative values, such as `em`s.

##### Example

In the following example, the text-indent property adjusts the indentations of three paragraph elements inside a "parent" (`.parent-1`) div element.

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="RjwyEa" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Alignment, Pt. 3" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen">
    <style media="screen">
    .parent-2 {
        text-indent: 1.5em;
        background-color: saddlebrown;
        color: white;
        padding: 1em;
    }
    </style>

    <div class="parent-2">
    <p>Ex reprehenderit officia pariatur mollit aliquip eu cillum magna quis. Labore officia incididunt quis laboris veniam quis veniam ad sunt. Minim fugiat consectetur ad consectetur eiusmod quis nostrud do. Deserunt laboris est commodo id Lorem mollit nostrud. Cupidatat culpa officia consequat proident duis nostrud quis nostrud incididunt commodo dolore sit velit.</p>
    <p>Laboris excepteur amet incididunt cupidatat tempor non veniam reprehenderit aute minim qui quis ullamco mollit officia nostrud duis. Ut do nulla excepteur ex magna labore labore commodo. Lorem laborum minim occaecat tempor veniam ad consectetur adipisicing magna.</p>
    <p>Et et commodo veniam do do enim nisi aliquip enim. Elit nisi officia esse aute ea mollit cillum exercitation. In in mollit laboris officia commodo pariatur mollit ipsum do est do.</p>
    </div>
  </div>
</div>


# { TODO: }
Read pages 285-288 of Chapter 12 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
