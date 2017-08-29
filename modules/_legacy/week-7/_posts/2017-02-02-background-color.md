---
title: Background Color
module: 7
---

# Background Color

The first CSS property we will officially look at is "background color".

The background color property allows developers to specify the background color of elements.

As with all CSS multi-word properties, each word is separated with a hyphen. `background-color:`

The background color property takes a color as its value. This can be a hex (i.e. `#ae34ff`) value, or an rgb value (i.e. `rgb(174, 52, 245)`).

NOTE: I am also including the CSS property `padding`. These will force the page to render block-level elements, even when they have no text content. Padding is the amount of space between the element content, and the edge of the element. In the case of no content, it is the amount of space between the edge and the center of the element.


```html
<style>
    div.main-container {
        background-color: rgb(127, 172, 200);
        padding: 100px;
    }
</style>

<div class="main-container">

</div>
```

<div class="displayed_code_example">
<style>
    .main-container {
        background-color: rgb(127, 172, 200);
        padding: 100px;
    }
</style>

<div class="main-container">
</div>
</div>


## Background Color of the Entire Page

There are two easy ways to set the background color for a page.

1. Set the background color of the `<body>` element.

```css
body {
    background-color: #ee12ff;
}
```

2. Wrap the entire page contents in a `<div>` element with an appropriate class name (i.e. `<div class="main-container">`), and set the background color of that element. (NOTE: You will also need to set the elements height property in this case `{ height: 100%; }`)

```css
.main-container {
    background-color: #ffee12;
}
```

## Inner Elements

When setting the background color of inner elements, you should do choose colors that encourage readability, and complement the main color schemes of the site.

<div id="code-heading">CSS</div>

```css
body {
    background-color: #dddfd4;
}

header {
    background-color: #3fb0ac;
    padding: 75px;
}

.content {
    display: flex;
    flex-direction: row;
    width: 100%;
}

main {
    background-color: #173e43;
    flex: 1 3 auto;
    padding: 200px;
}

aside {
    background-color: #fae596;
    flex: 1 1 auto;
    padding: 10px;
}

footer {
    background-color: #3fb0ac;
    padding: 75px;
}
```

<div id="code-ruler"></div>

<div id="code-heading">HTML</div>

```html
<body>
    <header></header>
    <div class="content">
        <main></main>
        <aside></aside>
    </div>
    <footer></footer>
</body>
</div>
```



<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:560px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/07/background-color/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/07/background-color/background-color.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/07/background-color/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/07/background-color/) |
