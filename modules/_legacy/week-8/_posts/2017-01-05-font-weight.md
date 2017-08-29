---
title: Font Weight
module: 8
---

# Font Weight

Before we look at how to include external fonts, lets discuss font weight and font style. These are used to determine if a font is "bold" and/or "italic".


Within CSS, the `font-weight` property, in its most basic use, specifies whether a font is "normal", or "bold".

<div id="code-heading">CSS</div>

```css
#heading-1 {
    font-family: sans-serif;
    font-weight: normal;
}
#heading-2 {
    font-family: sans-serif;
    font-weight: bold;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<h1 id="heading-1">I am Normal "Weight"</h1>
<h1 id="heading-2">My Weight is "Bold"</h1>
```

<div class="displayed_code_example">
<style>
#heading-1 {
    font-family: sans-serif;
    font-weight: normal;
}
#heading-2 {
    font-family: sans-serif;
    font-weight: bold;
}
</style>
<h1 id="heading-1">I am Normal "Weight"</h1>
<h1 id="heading-2">My Weight is "Bold"</h1>
</div>

When we wrap words with the `<strong>...</strong>` element, the browser is trying to find a "bold" version of the font. If none exists for the specified font, then they browser _may try_ to bold the selected words on its own. (This assumes we have not overwritten the strong elements rules in our CSS)

<div id="code-heading">CSS</div>

```css
h1 {
    font-family: sans-serif;
    font-weight: normal;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<h1 id="heading-1">I am Normal "Weight"</h1>
<h1 id="heading-2"><strong>I am STRONG!</strong></h1>
```

<div class="displayed_code_example">
<style>
.displayCodeExample h1 {
    font-family: sans-serif;
    font-weight: normal;
}
</style>
<h1 id="heading-1">I am Normal "Weight"</h1>
<h1 id="heading-2"><strong>I am STRONG!</strong></h1>
</div>

In addition to the "bold" font weight, depending on the font-family superclass, it is possible to also specify varying weights using;

- **Terms**
    - `bolder`
    - `bold`
    - `normal`
    - `lighter`
- **Number Values**
    - `100` through `900`

**NOTE:** For these font weights to work, the equivalent font-family for each font weight (i.e. "Times-Regular.otf" & "Times-ExtraBold.otf") must be loaded on the clients computer. Otherwise, the browser will 'round' to the nearest font weight. At the end of the day, this means you always need to check you site on multiple devices, to ensure it is being displayed as you intend it to be.

<div id="code-heading">CSS</div>

```css
h2 {
    font-family: "Source Sans Pro";
    text-align: center;
}
#w1 {
    font-weight: bolder;
}
#w2 {
    font-weight: bold;
}
#w3 {
    font-weight: normal;
}
#w4 {
    font-weight: lighter;
}
#t1 {
    font-weight: 100;
}
#t2 {
    font-weight: 200;
}
#t3 {
    font-weight: 300;
}
#t4 {
    font-weight: 400;
}
#t5 {
    font-weight: 500;
}
#t6 {
    font-weight: 600;
}
#t7 {
    font-weight: 700;
}
#t8 {
    font-weight: 800;
}
#t9 {
    font-weight: 900;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<!-- This is an external link to load the font-family. -->
<!-- You will learn more about how to do this in a few pages. -->
<link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:100,200,300,400,500,600,700,800,900" rel="stylesheet">

<h2 id="w1">Bolder</h2>
<h2 id="w2">Bold</h2>
<h2 id="w3">Normal</h2>
<h2 id="w4">Lighter</h2>
<hr>
<h2 id="t1">Weight: 100...</h2>
<h2 id="t2">Weight: 200...</h2>
<h2 id="t3">Weight: 300...</h2>
<h2 id="t4">Weight: 400...</h2>
<h2 id="t5">Weight: 500...</h2>
<h2 id="t6">Weight: 600...</h2>
<h2 id="t7">Weight: 700...</h2>
<h2 id="t8">Weight: 800...</h2>
<h2 id="t9">Weight: 900...</h2>
```

<div class="displayed_code_example">
    <link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:100,200,300,400,500,600,700,800,900" rel="stylesheet">
    <style>
        .displayed_code_example h2 {
            font-family: "Source Sans Pro";
            text-align: center;
        }
        #w1 {
            font-weight: bolder;
        }
        #w2 {
            font-weight: bold;
        }
        #w3 {
            font-weight: normal;
        }
        #w4 {
            font-weight: lighter;
        }
        #t1 {
            font-weight: 100;
        }
        #t2 {
            font-weight: 200;
        }
        #t3 {
            font-weight: 300;
        }
        #t4 {
            font-weight: 400;
        }
        #t5 {
            font-weight: 500;
        }
        #t6 {
            font-weight: 600;
        }
        #t7 {
            font-weight: 700;
        }
        #t8 {
            font-weight: 800;
        }
        #t9 {
            font-weight: 900;
        }
    </style>

    <h2 id="w1">Bolder</h2>
    <h2 id="w2">Bold</h2>
    <h2 id="w3">Normal</h2>
    <h2 id="w4">Lighter</h2>
    <hr>
    <h2 id="t1">Weight: 100...</h2>
    <h2 id="t2">Weight: 200...</h2>
    <h2 id="t3">Weight: 300...</h2>
    <h2 id="t4">Weight: 400...</h2>
    <h2 id="t5">Weight: 500...</h2>
    <h2 id="t6">Weight: 600...</h2>
    <h2 id="t7">Weight: 700...</h2>
    <h2 id="t8">Weight: 800...</h2>
    <h2 id="t9">Weight: 900...</h2>
</div>
