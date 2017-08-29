---
title: Background Images
module: 11
---

# Background Images

In addition to including images in your age with the `<img>` HTML element, you can specify that elements use images for the background. This would serve as a replacement for `background-color:`.

To set an elements background as an image, use the `background-image:` property. You will then need to supply this property with a valid URL as the value. To do so, you should supply the URL within a `url()` function.

<div id="code-heading">CSS</div>

```css
.my-element {
    background-image: url("path-to-my-image.png");
}
```

NOTE: Be mindful with the size of file you use for background images, as these can slow your page load times.

## Repeating Images

You can use the `background-repeat:` property to specify if a background image should repeat, or only occur one time. This property takes the following possible values;

- `repeat` -- The background image will be repeated both vertically and horizontally. This is the default.
- `repeat-x` -- The background image will be repeated only horizontally.
- `repeat-y` -- The background image will be repeated only vertically.
- `no-repeat` -- The background-image will not be repeated.
- `round` -- The background image will be scaled to fit fill the element, without hangovers.
- `space` -- The background image will be positioned with space between repetitions.

<div id="code-heading">HTML</div>

```html
<div class="container">
    <p>Eu officia sint in dolor minim aliquip deserunt officia eu officia. Magna eiusmod qui consectetur dolore deserunt ea amet Lorem amet labore in amet id occaecat. Esse dolor reprehenderit laboris occaecat voluptate laborum aute magna fugiat tempor cillum aute quis sit ipsum. Proident ullamco magna ullamco velit adipisicing aliquip elit. Occaecat consectetur duis deserunt sint elit cupidatat id sit consectetur eu. Ad excepteur nisi fugiat incididunt do pariatur voluptate pariatur aute irure ea veniam consectetur amet.</p>
</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
.container {
    background-image: url("./imgs/instructorIsLost.jpg");
    background-repeat: round;
    height: 700px;
    color: #fff;
    text-align: center;
    display: flex;
}

.container p {
    margin: auto;
    width: 80%;
    min-width: 200px;
    font-size: 18pt;
    align-content: center;
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:700px;"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/11/bg-image-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/11/bg-image-01/bg-image-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/11/bg-image-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/11/bg-image-01/) |

## Background Size

Using the `background-size:` property allows a developer to specify how an image should be scaled in relation to the containing element. This property takes the following values ([These were taken from w3schools](https://www.w3schools.com/cssref/css3_pr_background-size.asp));

- `auto`
    - Default value. The background-image contains its width and height.
- `length`
    - Sets the width and height of the background image. The first value sets the width, the second value sets the height. If only one value is given, the second is set to "auto".
- `percentage`
    - Sets the width and height of the background image in percent of the parent element. The first value sets the width, the second value sets the height. If only one value is given, the second is set to "auto".
- `cover`
    - Scale the background image to be as large as possible so that the background area is completely covered by the background image. Some parts of the background image may not be in view within the background positioning area.
- `contain`
    - Scale the image to the largest size such that both its width and its height can fit inside the content area.

NOTE: Resize the page to see how the various values behave.

<div id="code-heading">HTML</div>

```html
<div class="container bg-1"><p></p></div>
<div class="container bg-2"><p></p></div>
<div class="container bg-3"><p></p></div>
<div class="container bg-4"><p></p></div>
<div class="container bg-5"><p></p></div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
.container {
    background-image: url("./imgs/instructorIsLost.jpg");
    background-repeat: no-repeat;
    background-color: #000;
    height: 300px;
}

.bg-1 { background-size: auto; }
.bg-2 { background-size: 700px 100px; }
.bg-3 { background-size: 90% 80%; }
.bg-4 { background-size: cover; }
.bg-5 { background-size: contain; }
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:1600px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/11/bg-image-04" frameborder="0" allowfullscreen></iframe></div>
</div>



## Background Position

You can use the `background-position:` property to specify where an image should be placed in relationship to the elements.

If the image is smaller than the element, then it will be positioned where you tell it.

If the image is larger than the element, then this property is used to specify the anchor point of the image in the element.

This property takes the following values;

- `left top`
- `left center`
- `left bottom`
- `center top`
- `center center`
- `center bottom`
- `right top`
- `right center`
- `right bottom`

<div id="code-heading">CSS</div>

```css
.container {
    background-image: url("./imgs/instructorIsLost.jpg");
    background-repeat: no-repeat;
    background-position: right bottom;
    background-color: #000;
    height: 400px;
    color: #fff;
    text-align: center;
    display: flex;
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:80%"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/11/bg-image-02/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/11/bg-image-02/bg-image-02.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/11/bg-image-02/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/11/bg-image-02/) |


## Background Attachment

The `background-attachment:` property specifies to a browser whether a background image is "scrollable" or "fixed" in relation to the page.

Per the [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/background-attachment), this property takes three possible values;

- `fixed`
    - This keyword means that the background is fixed with regard to the viewport. Even if an element has a scrolling mechanism, a ‘fixed’ background doesn't move with the element.
- `local`
    - This keyword means that the background is fixed with regard to the element's contents: if the element has a scrolling mechanism, the background scrolls with the element's contents, and the background painting area and background positioning area are relative to the scrollable area of the element rather than to the border framing them.
- `scroll`
    - This keyword means that the background is fixed with regard to the element itself and does not scroll with its contents. (It is effectively attached to the element's border.) (This is the default value.)


## { TODO: }

Please read:

- Chapter 16 from the Duckett for more on images.
