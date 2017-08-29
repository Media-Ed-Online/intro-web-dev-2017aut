---
title: Where to Style
module: 7
---

# Where to Style

There are three general ways to specify CSS style rules, within a CSS Style element in an HTML document, in a separate css document, or as an attribute within each element.

# The Style Element

Within an HTML document, (for example `index.html`), you can place CSS within a Style Element (`<style>...</style>`).

NOTE: You should usually place, your style element inside the head element, as one of the last entries.
<br />


```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Style Example</title>
        <style>
            /* CSS GOES HERE */
        </style>
    </head>
    <body>
        <!-- Content you are styling. -->
    </body>
</html>
```


# CSS Documents

It is perfectly acceptable to place CSS within the HTML document, if the CSS is minimal. Usually however, you should place CSS in one or more external "style sheets".

A CSS document is given the `.css` extension. As with images and media, it is considered best practice to place your CSS documents in a separate child directory labeled either css or style.

```bash
.
├── index.html
└── css
    ├── fonts.css
    └── style.css
```

It is also necessary to tell the browser to use the style defined within the document. To do this, you will add the "link element" (`<link />`) inside the document's head element. Just like the style element, the link element is typically placed near or at the end of the head element. The link element is an empty element, so it only requires a single tag.

NOTE: You may link more than one CSS document by simply including multiple link elements. This is common for larger sites.

### Attributes

#### href

Provide the relative or absolute URL as the value to the `href=""` attribute. This tells the browser where the document is located at.

#### rel

The relationship (`rel=""`) attribute describes the relationship of the linked document to the html document. When linking to a css document, the value for this attribute should "stylesheet" (i.e. `rel="stylesheet"`). You should always include this attribute.

#### type

The type attribute tells the browser what type of document you are linking to. This should always be passed as `type="text/css"` when linking to a CSS document.

<br />


To link to an external style sheet located in the directory structure discussed above you would include the following line in your head element.

```html
<link rel="stylesheet" type="text/css" href="/css/style.css">
```


# The style attribute

The last way of specifying style is to include the rule as the value for a style attribute in any HTML element.

As with the global `class` and `id` attributes, every HTML element can be passed a global `style` attribute. This value takes a string, formatted as valid CSS. (NOTE: Valid CSS will be discussed over the next few pages.)

```html
<div class="content-para" style="background-color:#59ff00;color:#fff">
    <p style="border:'solid 3px #ff0063'">Duis nulla id dolor cupidatat
        dolor consectetur id aute eu non eu voluptate culpa minim qui esse.</p>
    <p style="color:#00d9ff">Duis nulla id dolor cupidatat dolor consectetur
         id aute eu non eu voluptate culpa minim qui esse.</p>
</div>
```
<div class="displayed_code_example">
<div class="content-para" style="background-color:#59ff00;color:#fff">
    <p style="border:3px solid #ff0063;">Duis nulla id dolor cupidatat
    dolor consectetur id aute eu non eu voluptate culpa minim qui esse.</p>
    <p style="color:#00d9ff">Duis nulla id dolor cupidatat dolor consectetur
     id aute eu non eu voluptate culpa minim qui esse.</p>
</div>
</div>
