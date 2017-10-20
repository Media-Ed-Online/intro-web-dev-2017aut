---
title: Inheritance
module: 07
---

## Inheritance:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

Another crucial idea and concept in CSS is that of "inheritance."

Inheritance allows rules for certain aspects that are defined in parent elements to apply to all children elements.

For example, defining the text color and font family in the all selector (`* {}`) or HTML element selector (`html {}`), will define a base text color and font for the entire page (or until another more specific rule overwrites it).

<p data-height="400" data-theme-id="30567" data-slug-hash="JrzbYe" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07] Inheritance, Pt. 1" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

<div class="pen-result displayed_code_example_pen">
  <style>
    .h1-inher {
      font-size: 2em;
      margin: 0;
    }
    .container-box {
        background-color: #f1f1f1;
        font-family: sans-serif;
        color: hotpink;
    }
    #other-paragraph {
        font-family: serif;
        color: black;
    }
  </style>
  <div class="container-box">
      <h1 class="h1-inher">A Heading, that is pink and without serifs.</h1>
      <p>Some Text, that is also pink and without serifs.
          <p>You should not nest paragraphs in other paragraphs.
              <p>But notice how the text color and font apply to all sub-children.</p>
          </p>
      </p>
      <br />
      <h1 class="h1-inher">Another heading, so forth and so on.</h1>
      <p id="other-paragraph">A more Specific Selector can overwrite this paragraph.</p>
  </div>
</div>



### What Inherits

Not all properties will inherent their value from the parent element.

Text properties tend to inherit values from their parents, however, some properties do not. As with many things in web development, this is partly browser specific.

### Forcing Inheritance

If you are worried, or find a property that is not inheriting, you can for inheritance with the `inherit` keyword as the properties value.

<p data-height="400" data-theme-id="30567" data-slug-hash="EwMNeM" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07] Inheritance, Pt. 2" class="codepen"></p>

<div class="pen-result displayed_code_example_pen">
  <style>
    .parent-container {
        color: #f1f1f1;
        background-color: hotpink;
    }
    .child-container {
        background-color: inherit;
    }
  </style>
  <div class="parent-container">
      <div class="child-container">
          <p>Notice that the black background color only applies to the outer &lt;div&gt; element. Not the child paragraph elements.</p>
          <p>Yet, the text color applies all...</p>
      </div>
  </div>
</div>




# { TODO: }
1. Read pages 240-245 of Chapter 10 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
2. [Skim information on Inheritance and Cascading from w3.org](https://www.w3.org/wiki/Inheritance_and_cascade).
