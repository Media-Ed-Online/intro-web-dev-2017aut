---
title: External Fonts from the Web
module: 8
---

# External Fonts from the Web

Sometimes, as with embedding movies and audio, it is easier and more efficient to utilize a service that will deliver the fonts via their servers.

This type of service will allow you to not worry about font-package types. As the service will often query the browser and deliver the appropriate type. Additionally, this means that you do not have to manage the fonts on your server space.

Google Fonts, in addition to allowing for font downloads, also provides a font server service.

There are embed links from the same pop-up window that allows you to download a font-package. Simply copy the HTML or CSS embed code from their site into the appropriate place. Then specify the font in CSS rules.

# Example

As an example, lets do the same thing as the previous page, but instead, use Google's embed code.

To do this, we will pick up after step 4. (NOTE: Make sure you have still selected a font, and gone into the CUSTOMIZE tag to select any additional font styles you may need.)

![Select additional font styles from the CUSTOMIZE tag](../imgs/gfonts-04.png "Select additional fonts")

### 5. Embed

Instead of downloading the fonts, select the "EMBED" tag next to "CUSTOMIZE".
![Select the EMBED tag](../imgs/gfonts-07.png "Select EMBED tag")

Then depending on whether you want to include the embed code in your HTML _OR_ CSS, select the "STANDARD" tag _OR_ "@IMPORT" tag.

Then copy the code below in the gray box.

##### STANDARD

![Standard Embed Code](../imgs/gfonts-08.png "Example of selecting the 'STANDARD' embed code")

This would go in the `<head>` element of `index.html`;

<div id="code-heading">HTML</div>

```html
<link href="https://fonts.googleapis.com/css?family=Arvo:400,400i,700,700i" rel="stylesheet">
```


##### @IMPORT

!['@IMPORT' Embed Code](../imgs/gfonts-09.png "Example of selecting the '@IMPORT' embed code")

This could be placed either in;

1. a CSS file, such as at the top of your `style.css` file.
2. the `index.html` file inside a `<style>...</style>` element.

NOTE: Where ever you place it, you must make sure it appears before you try to assign the font.

If we placed this in our css file, it would appear at the top like;

<div id="code-heading">CSS</div>

```css
@import url('https://fonts.googleapis.com/css?family=Arvo:400,400i,700,700i');
```

### Use the Font

At this point, the font is ready for use. We could pick up from [[step 10 on the previous page]]({{base.url}}/modules/week-8/get-fonts/#apply-in-css).

To accomplish the same thing as the previous page, our final code would look like the following;

NOTE: We are using the "HTML link" method from Google fonts for embedding the font code. As such, this is placed in our HTML.

<div id="code-heading">Directory</div>
```bash
.
├── index.html
└── css
    └── style.css
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Download Google Fonts</title>

        <!-- The Google Font Embed Code -->
        <link href="https://fonts.googleapis.com/css?family=Arvo:400,400i,700,700i" rel="stylesheet">
        <!-- Our Style Sheet -->
        <link rel="stylesheet" href="./css/style.css">
    </head>
    <body>

        <header>
            <h1>I Think Arvo is a Cool Font!</h1>
        </header>

        <main>
            <p>This is some plain ol' text, in a paragraph.</p>
            <p>This is a paragraph with <em>emphasized</em> or <em>italic</em> content.</p>
            <p>This is a paragraph with some <strong>strong</strong> content.</p>
            <p>This is a paragraph with both <strong>strong</strong> and <em>emphasized</em> text <strong><em>TOGETHER!!!!</em></strong></p>
        </main>

    </body>
</html>
```

<div id="code-ruler"></div>
<div id="code-heading">CSS (style.css)</div>

```css
* {
    font-family: 'Arvo', serif;
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:250px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/08/embed-gfonts" frameborder="0" allowfullscreen></iframe></div>
</div>

Follow these links to download, view on GitHub, or view the page;

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/embed-gfonts/embed-gfonts.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/embed-gfonts/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/embed-gfonts/) |


## { TODO: }

Please read;

- ["Avoiding Faux Weights And Styles With Google Web Fonts", by Laura Franz]( https://www.smashingmagazine.com/2012/07/avoiding-faux-weights-styles-google-web-fonts/)
