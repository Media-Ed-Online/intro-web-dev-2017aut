---
title: Text Decoration
module: 8
---

# Text Decoration

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

<div id="code-heading">CSS</div>

```css
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
.text {
    background-color: rgb(186, 186, 186);
    padding: 0.75em;
    text-align: center;
}
```


<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<h2 class="text text-1">Some text to decorate.</h2>
<h2 class="text text-2">Some text to decorate.</h2>
<h2 class="text text-3">Some text to decorate.</h2>
<h2 class="text text-4">Some text to decorate.</h2>
```

<div class="displayed_code_example">
    <style>
    .text {
        background-color: rgb(186, 186, 186);
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
