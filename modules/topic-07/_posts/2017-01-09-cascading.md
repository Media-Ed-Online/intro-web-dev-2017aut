---
title: Cascading
module: 07
---

## Cascading in CSS Rules:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

In CSS, it is possible and common to have two or more selectors that cause declarations to apply to the same element. CSS implements specific rules and algorithms to determine which rules ultimately apply to the specific element.

This is known as _cascading_, and is fundamental to the idea of CSS (hence why it is part of the name for the language).


### Order

The first cascading rule can be referred to as "Order" or "The Last Rule."" Essentially, if two or more selectors are the same, than the last one will take precedence.

In the following example, the second rule overwrites the aspects duplicated in the first. (i.e. the border specification applies from the first rule, but the color and background-color specs are overwritten.)

<p data-height="400" data-theme-id="30567" data-slug-hash="vePKWJ" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  Cascading, Pt. 1" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

<div class="pen-result displayed_code_example_pen">
  <style>
    .class-one {
        color: grey;
        background-color: grey;
        border: 3px dashed gold;
    }

    .class-one{
        color: hotpink;
        background-color: black;
    }
  </style>
  <div class="class-one">
      Div element of class type: "class-one".
  </div>
</div>

This may seem like a funny idea right now that may lead to poorly written code. However, it is common for a developer to use pre-made CSS "frameworks" that they load in as separate documents. They may then want to customize their site by overwriting specific rules. Rather than try to change the declarations, they will create a new CSS document, that keeps track of their specific changes and rules. To ensure these rules take precedence, the developer then simply needs to load in their sheet last.

In the following example, two documents are brought in, but notice the developer's is brought in last.

<div id="code-heading">HTML</div>
```html
<head>
    <link rel="stylesheet" href="/css/bootstrap.css">
    <link rel="stylesheet" href="/css/my-custom-styles.css">
</head>
```

### Specificity

Rules which are more specific will take precedence over less specific rules. This is true even if the less specific rule is defined last.

For example;
- `h1 p` is more specific than `p` alone.
- `.box-two` is more specific than `<div>`.
- `#first-paragraph-id` is more specific than `.box-two`

<p data-height="400" data-theme-id="30567" data-slug-hash="XeGKGd" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  Cascading, Pt. 2" class="codepen"></p>

<div class="pen-result">
  <style>
      .box-one .p {
          padding: 20%;
          font-weight: bolder;
          color: tomato;
      }
      .p {
          color: turquoise;
      }

      div .box-two {
          background-color: saddlebrown;
      }

      #first-paragraph-id {
          background-color: gold;
          color: black;
      }

      .div-code {
          padding: 5%;
          background-color: #f1f1f1;
          color: black ;
      }
  </style>
  <div class="container-box div-code">
      <div class="box-one div-code">
          <p class="p">I like dogs.</p>
      </div>
      <div class="box-two div-code">
          <p class="p" id="first-paragraph-id">I like dogs a lot.</p>
          <p class="p">I like big dogs...</p>
      </div>
  </div>
</div>


### !Important

If a developer believes it is necessary to force a rule, and is worried about it being overwritten, they can append the keyword `!important` after the CSS property value. This tells the browser to give precedence to "this" rule.

**NOTE:** Be careful using the `!important` keyword, as it can cause you to forget why a rule is not working when otherwise it should be. Often times, it is the use of important in another rule.

<p data-height="200" data-theme-id="30567" data-slug-hash="aLMmMG" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07] !Important" class="codepen"></p>

<div class="displayed_code_example_pen pen-result">
  <style>
      .p-imp {
          color: blue !important;
          font-size: x-large;
      }
      .para-one {
          color: yellow;
      }
  </style>
  <p class="p-imp para-one">Hank Williams!</p>
</div>


# { TODO: }
1. Read page 239 of Chapter 10 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3.
2. [Read information on Cascading from the Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade).
