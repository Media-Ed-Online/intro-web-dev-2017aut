---
title: Font Variant & Transform
module: 8
---

# Font Variant & Transform

There are two properties that allow developers to set the capitalization of text.

# Font Variant

The `font-variant: ` property allows developers to specify whether text should appear in all caps, with 'non-capitalized' letters being displayed as small caps.


In a small-caps font, all lowercase letters are converted to uppercase letters. However, the converted uppercase letters appears in a smaller font size than the original uppercase letters in the text.

<div id="code-heading">CSS</div>

```css
.content-p {
    font-variant: small-caps;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<p class="content-p">
    An example of the font-variant property.
    Notice how the first letters of each sentence
    are still full size. But, the rest of the
    characters are "small-caps".</p>
```

<div class="displayed_code_example">
    <style>
        .content-p {
            font-variant: small-caps;
        }
    </style>
    <p class="content-p"> An example of the font-variant property. Notice how the first letters of each sentence are still full size. But, the rest of the characters are "small-caps".</p>
</div>

# Text Transform

The second property that allows for the control of capitalization is `text-transform: `.

Text transform takes one of four keyword values;

- `none`; Do nothing.
- `uppercase`; Make all characters uppercase.
- `lowercase`; Make all characters lowercase.
- `capitalize`; Capitalize the first letter of each word. (Sometimes also known as "Title Case")

<div id="code-heading">CSS</div>

```css
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
```


<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<h2 class="text-1">Some text, WITH crAzY capitaLIZATION.</h2>
<h2 class="text-2">Some text, WITH crAzY capitaLIZATION.</h2>
<h2 class="text-3">Some text, WITH crAzY capitaLIZATION.</h2>
<h2 class="text-4">Some text, WITH crAzY capitaLIZATION.</h2>
```

<div class="displayed_code_example">
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
