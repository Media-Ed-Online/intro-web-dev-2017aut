---
title: External Fonts
module: 8
---

# External Fonts

As a developer you will want to include specific fonts for certain sites. These fonts may be part of the brand, add personality, be integral to the overall design aesthetic, or be serve a special purpose.

Developers can include external fonts a number of ways. However, when including external fonts, you should keep in mind that this is an additional resource the client computer will have to download. This may impact speed and performance. Therefore you should only include external fonts with purpose, and ensure that you only include fonts you are actually using.


# Fonts from Your Server

One way to include an external font is to place its resource files in a sub-directory, similar to how images, style sheets, and other external resources are handled.

## @font-face

To include an external font, you first must tell the browser to load the font and what to refer to it as. To do this, use the `@font-face` rule in your CSS.

This rule is formatted like other CSS selectors, but instead of being used to alter HTML elements, it is used to load in data for CSS to use.

The `@font-face` rule takes three properties.

#### src: url and format

The source property (`src: url() format()`) tells the browser where to load the font from via the `url()` function, and what type of font it is via the `format()` function.

As with audio and video, not every browser is capable of reading and using every type/format of font. Therefore, you will need to include multiple types of fonts in order to cover support for all browsers.

For information on what browsers support what types of font formats please read:

- [Web-Font Formats](https://transfonter.org/formats)
- [w3schools web font info](https://www.w3schools.com/css/css3_fonts.asp)

As you can see, you will need to include multiple versions of every font you want to use in order to ensure compatibility.

<br />


#### Directory Structure

As mentioned above, your font files should be placed in a child-directory, labeled something along the lines of `fonts/`.

Lets assume, we have two fonts, to be used for headings and paragraphs, respectively;

- ['monoton'](https://fonts.google.com/specimen/Monoton)
- ['Source Code Pro'](https://github.com/adobe-fonts/source-code-pro/releases/tag/2.030R-ro/1.050R-it)

We will have the following directory structure.

<div id="code-heading">Directory</div>

```bash
├── index.html
├── css
│   └── style.css
└── fonts
    ├── SourceCodePro-Light.otf
    ├── SourceCodePro-Light.ttf
    ├── SourceCodePro-Light.woff
    ├── SourceCodePro-Light.woff2
    ├── monoton-regular.ttf
    ├── monoton-regular.woff
    └── monoton-regular.woff2
```

To use these fonts we would include an `@font-face` for each font, along with relative url's for each font type. This allows us to ensure compatibility with all browsers.

NOTE: This css is applying the `monoton` font to the heading and `Source Code Pro` to the paragraphs.

<div id="code-heading">CSS</div>

```css
@font-face {
    /* Declare the name that we will reference the font by. */
    font-family: 'monoton';
    /* Load the font, in decreasing order of compatibility. */
    src:
        /* Specifying both the relative url and font type. */
        url('../fonts/monoton-regular.woff2') format('woff2'),
        url('../fonts/monoton-regular.woff') format('woff'),
        url('../fonts/monoton-regular.ttf') format('truetype');
}

@font-face {
    font-family: 'Source Code Pro';
    src:
        url('../fonts/SourceCodePro-Light.woff') format('woff'),
        url('../fonts/SourceCodePro-Light.woff2') format('woff2'),
        url('../fonts/SourceCodePro-Light.otf') format('opentype'),
        url('../fonts/SourceCodePro-Light.ttf') format('truetype');
}

.main-heading {
    /* Apply the font, using the name specified above. */
    /* Always include a backup font, incase ours does not load. */
    font-family: 'monoton', sans-serif;
    font-size: 3em;
}

.content {
    font-family: 'Source Code Pro', serif;
}
```
<div id="code-ruler"></div>

<div id="code-heading">HTML</div>

```html
<h1 class="main-heading">I Love This Font!!!</h1>
<p class="content">
    It is <strong>interesting</strong> how two fonts can compliment or distract from one another. You should try to choose fonts that easily flow and delineate the content of your webpage.
</p>
```


<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:250px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/08/font-example-01" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/font-example-01/font-example-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/font-example-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/font-example-01/) |

# Font Weights and Styles

Notice in the example above, that in the code, the inline syntax element "<strong>...</strong>" has been placed around the word "interesting". Depending on the browser you are using, this word may or may not have appereard in bold, like we asked it to.

This relates to the discussion of font weight and font stye had in the last few pages. We have only imported one type of the 'Source Code Pro' family; the 'light' type. When we ask the browser to display the text as "strong"/"bold", it tries to look for the specific font package, with the name 'Source Code Pro', that has been identified as the 'bold' version. Since none has been specified as such, the browser decides if it will try and make the font bold itself, or just display the text as is.

This little example shows that if you intend to make more than one version of a font available, such as bold, or true italic, you will have to also include these font packages and tell the browser as much.

When importing a font with `@font-face`, there are two additional properties that can be set, `font-weight: ` and `font-style: `. Setting these during font import makes them available to the browser.

To use the font, then simply specify the weight and/or style in the css element rule, (as discussed in the last few pages) matching what you specified during font import.


##### Example

In the following example, six types of the font-family 'Playfair' are imported. There are three weights of this font;

- regular
- **bold**
- **900 (Also known as 'Black' or 'extra-bold')**

Each weight has a 'regular' and _'italic'_ version.

When selecting the font for use, the CSS specifies the `font-weight:` and `font-style:` which then allows the browser to call the correct font package.

For this example, the font import statements have also been moved into their own css file; `fonts.css`. These allows the main css style file to be cleaner in appearance. Notice that the `fonts.css` file is linked in the html file before the `style.css` file. This is important in allowing the latter file to 'see' the fonts. 

<div id="code-heading">Directory</div>

```bash
.
├── index.html
├── css/
│   ├── fonts.css
│   └── style.css
└── fonts/
    ├── PlayfairDisplay-Black.ttf
    ├── PlayfairDisplay-BlackItalic.ttf
    ├── PlayfairDisplay-Bold.ttf
    ├── PlayfairDisplay-BoldItalic.ttf
    ├── PlayfairDisplay-Italic.ttf
    └── PlayfairDisplay-Regular.ttf
```

<div id="code-ruler"></div>
<div id="code-heading">CSS (fonts.css)</div>

```css
@font-face {
    font-family: 'Playfair';
    src:
        url('../fonts/PlayfairDisplay-Regular.ttf') format('opentype');
    font-weight: normal;
    font-style: normal;
}
@font-face {
    font-family: 'Playfair';
    src:
        url('../fonts/PlayfairDisplay-Italic.ttf') format('opentype');
    font-weight: normal;
    font-style: italic;
}
@font-face {
    font-family: 'Playfair';
    src:
        url('../fonts/PlayfairDisplay-Bold.ttf') format('opentype');
    font-weight: bold;
    font-style: normal;
}
@font-face {
    font-family: 'Playfair';
    src:
        url('../fonts/PlayfairDisplay-BoldItalic.ttf') format('opentype');
    font-weight: bold;
    font-style: italic;
}
@font-face {
    font-family: 'Playfair';
    src:
        url('../fonts/PlayfairDisplay-Black.ttf') format('opentype');
    font-weight: 900;
    font-style: normal;
}
@font-face {
    font-family: 'Playfair';
    src:
        url('../fonts/PlayfairDisplay-BlackItalic.ttf') format('opentype');
    font-weight: 900;
    font-style: italic;
}
```

<div id="code-ruler"></div>
<div id="code-heading">CSS (style.css)</div>

```css

.one {
    font-family: 'Playfair', sans-serif;
    font-weight: normal;
}
.two {
    font-family: 'Playfair', sans-serif;
    font-weight: normal;
    font-style: italic;
}
.three {
    font-family: 'Playfair', sans-serif;
    font-weight: bold;
}
.four {
    font-family: 'Playfair', sans-serif;
    font-weight: bold;
    font-style: italic;
}
.five {
    font-family: 'Playfair', sans-serif;
    font-weight: 900;
}
.six {
    font-family: 'Playfair', sans-serif;
    font-weight: 900;
    font-style: italic;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>Font Example</title>
    <link rel="stylesheet" href="./css/fonts.css">
    <link rel="stylesheet" href="./css/style.css">
</head>

<body>
    <h1 class="one">Testing This Font, YO!</h1>
    <h1 class="two">Testing This Font, YO!</h1>
    <h1 class="three">Testing This Font, YO!</h1>
    <h1 class="four">Testing This Font, YO!</h1>
    <h1 class="five">Testing This Font, YO!</h1>
    <h1 class="six">Testing This Font, YO!</h1>
</body>
</html>
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:420px;"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/08/font-example-02/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/font-example-01/font-example-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/font-example-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/font-example-01/) |
