---
title: Including Fonts
module: 8
---

# Including Fonts

To specify a font, use the `font-family: ` property. This is followed with a comma-delineated, list of fonts for the browser to _try_ and load.

At a minimum, every browser will be able to render something when passed one of three default values;

- `sans-serif`
- `serif`
- `monospace`

<div id="code-heading">CSS</div>

```css
.p1 {
    font-family: sans-serif;
}
.p2 {
    font-family: serif;
}
.p2 {
    font-family: monospace;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<p class="p1">sans-serif</p>
<p class="p2">serif</p>
<p class="p3">monospace</p>
```

<div class="displayed_code_example">
    <style>
        .p1 {
            font-family: sans-serif;
        }
        .p2 {
            font-family: serif;
        }
        .p3 {
            font-family: monospace;
        }
    </style>
    <p class="p1">sans-serif</p>
    <p class="p2">serif</p>
    <p class="p3">monospace</p>
</div>


Instead of using generic font class names, developers may also use specific font family names. When a specific font family is listed, the browser will try to load the font from the client computers font library.

For example, the following will cause the browser to first try and load "Comic Sans MS". If the client computer (yours in this case) does not have a font matching that name, it will then try "Comic Sans", then "Garamond", then "Times", then finally the default 'serif' font. The browser will do this by asking the client for the font. If the client doesn't have the font, then the browser will try the next listed font.

<div id="code-heading">CSS</div>

```css
#heading-1 {
    font-family: 'Comic Sans MS', 'Comic Sans', Garamond, Times, serif;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<h1 id="heading-1">Displayed Font</h1>
```

<div class="displayed_code_example">
<style>
    #heading-1 {
        font-family: 'Comic Sans MS', 'Comic Sans', Garamond Times, serif;
    }
</style>
<h1 id="heading-1">Displayed Font</h1>
</div>


# Web-Safe Fonts

Fonts that developers can count on being available by the system are known as "web-safe" fonts. These include font families that both Windows and Mac should have.

A list of these fonts is available from:

- [Web Safe Fonts](http://www.ampsoft.net/webdesign-l/WindowsMacFonts.html)

The advantage of using fonts from this list is that the client computer will already have the font. This reduced load times and may increase performance. 
