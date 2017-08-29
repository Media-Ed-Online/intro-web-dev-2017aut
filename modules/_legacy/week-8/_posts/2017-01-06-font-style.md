---
title: Font Style
module: 8
---

# Font Style

Font style typically refers to whether a font is "italicized" or not.

**NOTE:** As with "font weight", the "font style" property will try to find an appropriate, and dedicated, italic font family. If it is unable to do so, it will try to "italicize" the font itself. When a browser slants a font to achieve an italic effect (assuming it was unable to find a truly italic equivalent), this is actually known as an "oblique" style.

##### Example

In the following example, I have set it up, so that each element uses the same font family, but I have made it so that the true, "italicized" version is not available to the `#heading-2` element.

Notice the difference between the second and third elements. Depending on the browser, the second version is either a simple slanted version of the first or the same as the first (again different browsers display things differently). BUT, the third includes unique serifs (look at the capital 'T's) that are part of the italic version of the font.

<div id="code-heading">CSS</div>

```css
h1 {
    font-family: serif;
}
#heading-1 {
    font-style: normal;
}
#heading-2 {
    font-style: oblique;
}
#heading-3 {
    font-style: italic;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<h1 id="heading-1">I am Normal "Style"</h1>
<h1 id="heading-2">I am fake ITALIC; I am "oblique", if at all...</h1>
<h1 id="heading-3">I am a true "ITALIC" style! AM I NOT BEAUTIFUL?</h1>
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:300px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/08/font-style-example-01" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/font-style-example-01/font-style-example-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/font-style-example-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/font-style-example-01/) |


Assuming your fonts are loaded correctly (next few pages), this will not be an issue for you. Specifying an elements style as "italic" should select the correct font-family. If it is not, then you know you need to check your font loading.
