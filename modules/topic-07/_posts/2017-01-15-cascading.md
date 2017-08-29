---
title: Cascading
module: 7
---

# Cascading in CSS Rules

In CSS, it is possible and common to have two or more selectors that cause declarations to apply to the same element. CSS implements specific rules and algorithms to determine which rules ultimately apply to the specific element.

This is known as _cascading_, and is fundamental to the idea of CSS (hence why it is part of the name for the language).


## Order

The first cascading rule can be referred to as Order or The Last Rule. Essentially, if two or more selectors are the same, than the last one will take precedence.

In the following example, the second rule overwrites the aspects duplicated in the first. (i.e. the border specification applies from the first rule, but the color and background-color specs are overwritten.)

<div id="code-heading">CSS</div>

```css
.class-one {
    color: grey;
    background-color: grey;
    border: 3px dashed yellow;
}

.class-one{
    color: pink;
    background-color: black;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<div class="class-one">
    Div element of class type: "class-one".
</div>
```

<div class="displayed_code_example">
<style>
    .class-one {
        color: grey;
        background-color: grey;
        border: 3px dashed yellow;
    }

    .class-one{
        color: pink;
        background-color: black;
    }
</style>
<div class="class-one">
    Div element of class type: "class-one".
</div>
</div>

This may seem like a funny idea right now that may lead to poorly written code. However, it is common for a developer to use pre-made CSS "frameworks" that they load in as separate documents. They may then want to customize their site by overwriting specific rules. Rather than try to change the declarations, they will create a new CSS document, that keeps track of their specific changes and rules. To ensure these rules take precedence, the developer then simply needs to load in their sheet last.

In the following example, two documents are brought in, but notice the developers is brought in last.

```html
<head>
    <link rel="stylesheet" href="/css/bootstrap.css">
    <link rel="stylesheet" href="/css/my-custom-styles.css">
</head>
```

## Specificity

Rules which are more specific will take precedence over less specific rules. This is true even if the less specific rule is defined last.

For example;
- `h1 p` is more specific than `p` alone.
- `.box-two` is more specific than `<div>`.
- `#first-paragraph-id` is more specific than `.box-two`

<div id="code-heading">CSS</div>

```css
.box-one p {
    padding: 20%;
    font-weight: bolder;
    color: blue;
}

p {
    color: pink;
}

.box-two {
    background-color: orange;
}

#first-paragraph-id {
    background-color: pink;
    color: white;
}

div {
    padding: 5%;
    background-color: grey;
    color: black;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<div class="container-box">
    <div class="box-one">
        <p>I like dogs.</p>
    </div>
    <div class="box-two">
        <p id="first-paragraph-id">I like dogs alot.</p>
        <p>I like big dogs...</p>
    </div>
</div>
```

<div class="displayed_code_example">
<style>
    .box-one .p {
        padding: 10%;
        font-weight: bolder;
        color: blue;
    }

    .p {
        color: pink;
    }

    div .box-two {
        background-color: orange;
    }

    #first-paragraph-id {
        background-color: pink;
        color: white;
    }

    .div-code {
        padding: 5%;
        background-color: grey;
        color: black;
    }
</style>

<div class="container-box div-code">
    <div class="box-one div-code">
        <p class="p">I like dogs.</p>
    </div>
    <div class="box-two div-code">
        <p class="p" id="first-paragraph-id">I like dogs alot.</p>
        <p class="p">I like big dogs...</p>
    </div>
</div>
</div>


## !Important

If a developer believes it is necessary to force a rule, and is worried about it being overwritten, they can append the keyword `!important` after the CSS property value. This tells the browser to give precedence to "this" rule.

NOTE: Be careful using the `!important` keyword, as it can cause you to forget why a rule is not working when otherwise it should be. Often times, it is the use of important in another rule.

<div id="code-heading">CSS</div>

```css
p {
    color: blue !important;
}
.para-one {
    color: yellow;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<p class="para-one">Hank Williams!</p>
```

<div class="displayed_code_example">
<style>
    .p {
        color: blue !important;
    }
    .para-one {
        color: yellow;
    }
</style>

<p class="p para-one">Hank Williams!</p>
</div>





## { TODO: }

[- Read info on Cascading from the Mozilla Developer Network.](https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade)
