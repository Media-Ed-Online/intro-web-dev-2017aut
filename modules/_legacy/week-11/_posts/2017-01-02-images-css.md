---
title: Images & CSS
module: 11
---

# Images & CSS

Back, during our modules in HTML, you learned how to include images, and specify their size in your HTML. We discussed a need to specify size for images, so that a browser could reserve the correct amount of space, even if the image took longer to load than the rest of the page.

As I am sure you can guess, we can also specify the size of images with CSS. This is accomplished by using the same `width:` and `height:` properties that we use for other box elements.

In an order to preserve the responsive pages we are working on, a good practice to get into is to set the initial width and height of your image via HTML attributes.

<div id="code-heading">HTML</div>

```html
<img src="relative-path.jpg" width="460" height="345">
```

Then to set the width via CSS to `100%` and height to `auto`. This allows the image to take up the full width of its container element and to resize with the browser window.

<div id="code-heading">CSS</div>

```css
img {
    width: 100%;
    height: auto;
}
```

In some situations, this will cause the height of the image to get skewed. In which case, you should set the height of the image to the a percentage. This percentage should be the ratio of width:height. So if you image is 4:3, you would set the height to `75%`;

<div id="code-heading">CSS</div>

```css
img {
    width: 100%;
    height: 75%;
}
```


We can then place this inside of another parent element.

For an example, lets create a container, with two elements, a text block, and an accompanying image, set side-by-side. We can set the image to take up 66.66666%, and the text to take up 33.33333% (More specifically, the text element is set to 30.33333% with a padding of 1.5%. This sets the total to 33.33333%, because 30.33333 plus 1.5% on the left, plus 1.5% on the right, equals 33.33333%). We will set these widths using a media query, so that by default, our page is "mobile ready", and reflows as the display gets wider.

<div id="code-heading">HTML</div>

```html
<div class="container">
    <img src="./imgs/musick_algo_art_ex1.png" alt="algorithmic art example" title="algorithmic art example" width="1200px" height="750px">
    <div class="content-1">
        <h2>Algorithmic Art</h2>
        <p>Ut aliquip consectetur elit id ad amet eiusmod quis nisi ea velit minim elit ad. Eu elit amet fugiat adipisicing sint veniam laborum elit voluptate. Non aute excepteur incididunt Lorem est ullamco deserunt do. Est laboris quis qui mollit eiusmod aliqua deserunt adipisicing nulla laborum.</p>
    </div>
</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
body {
    padding: 0;
    margin: 0;
    font-size: 20px;
}
.container {
    display: flex;
    flex-flow: wrap;
    align-items: center;
    background-color: black;
}

.container img {
    width: 100%;
    height: 62.5%;
}

.container .content-1 {
    width: 100%;
    padding: 1.5%;
    color: #fff;
    background-color: #404040;
    text-align: justify;
}

@media (min-width: 650px) {
    .container img {
        width: 66.66666%;
    }
    .container .content-1 {
        width: 30.33333%;
        height: 100%;
    }
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:500px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/11/images-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/11/images-01/images-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/11/images-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/11/images-01/) |
