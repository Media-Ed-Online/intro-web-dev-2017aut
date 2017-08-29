---
title: Text Color
module: 7
---

# Text Color

In addition to background color, CSS also provides developers the ability to specify the color of text. The property name for this is simply `color: `.

The color property is an "inherited" property. This means a developer can define a color property value in a top level element, and it will be "inherited" by all children elements.

<div id="code-heading">CSS</div>

```css
body {
    color: rgb(255, 255, 255);
    background-color: rgb(43, 44, 48);
}
.color-text {
    color: rgb(49, 186, 172);
}
```
<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<body>
    <h1>Text Color Examples</h1>
    <p>Notice how the text color, defined in the body element
        selector, is inherited by the h1 element and this paragraph
        element.</p>
    <h2 class="color-text">New Colors</h2>
    <p class="color-text">Whereas, we can define a different color for
        the elements that are part of the "color-text" class.</p>
</body>
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:250px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/07/color-text/" frameborder="0" allowfullscreen ></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/07/color-text/color-text.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/07/color-text/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/07/color-text/) |
