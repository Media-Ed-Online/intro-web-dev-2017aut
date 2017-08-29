---
title: Media Queries
module: 10
---

# Media Queries

## Intro to Responsive Design Patterns

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/aNW9IUaSE7c" frameborder="0" allowfullscreen></iframe></div>

## Intro to Media Queries

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/xvBbwVQqDWE" frameborder="0" allowfullscreen></iframe></div>

#### Linked Style Sheet Media Query

In this first video, you will learn about using the link tag in HTML to import style sheets when a certain condition is true about the media in question.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/KtqM_xH-pLY" frameborder="0" allowfullscreen></iframe></div>

So, following from their examples, the below HTML code for a linked style sheet media query would only load that style sheet when the screens width was larger than 500px.

<div id="code-heading">HTML</div>

```html
<link rel="stylesheet" media="screen and (min-width: 600px)" href="style-min-600.css">
```

Likewise, the following would only load the `style-499-max.css` stylesheet when the screen size is less than or equal to 499px.

<div id="code-heading">HTML</div>

```html
<link rel="stylesheet" media="screen and (max-width: 499px)" href="style-max-499.css">
```

### Most Common Media Queries
The most common media queries are

#### `min-width: `
Which is executed with the pixel amount is greater than the set number.

#### `max-width: `
Which is executed when the browser is less than the number of pixels specified.


#### Media Query Example 1

In the following example, there are three style sheets;

- `main.css`
    - Always loaded and active
    - This sets the font family to `sans-serif`
    - And makes the body elements default background-color white.
- `499-max.css`
    - This is only loaded if the window width is less than 500 pixels.
    - This changes the background color to red.
- `600-max.css`
    - This is only loaded and active if the window width is greater than 600 pixels.
    - This changes the background color to blue.

Notice how they allow the examples background color to change, based on the screen size of the iframe. You should also [open this example in a separate tab](https://montana-media-arts.github.io/341-work/lectureCode/10/media-query-01/) to explore it in your own browser directly.

<div id="code-heading">HTML</div>

```html
<head>
    <meta charset="utf-8">
    <title>Media Query Example 1</title>

    <!-- Main CSS Style Sheet -->
    <link rel="stylesheet" href="./css/main.css">

    <!-- CSS Style Sheets loaded via media queries -->
    <link rel="stylesheet" media="(min-width:600px)" href="./css/600-min.css">
    <link rel="stylesheet" media="(max-width:499px)" href="./css/499-max.css">

</head>
<body>
    <h2>Media Query Example.</h2>
    <h3>Please resize your browser. You Should see the background color change.</h3>
    <h3>You might also open the example in a seperate tab, via the link below.</h3>
</body>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS (main.css)</div>

```css
body {
    font-family: sans-serif;
    background-color: #fff;
}
```

<div id="code-ruler"></div>
<div id="code-heading">CSS (499-max.css)</div>

```css
body {
    background-color: #ff0000;
}
```

<div id="code-ruler"></div>
<div id="code-heading">CSS (600-min.css)</div>

```css
body {
    background-color: #0000ff;
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:300px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/10/media-query-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/media-query-01/media-query-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/media-query-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/10/media-query-01/) |
