---
title: Text Alignment
module: 8
---

# Text Alignment

Alignment properties allows developers to specify how text should be positioned within an element. We will focus purely on the `text-align: ` property, which specifies horizontal placement of text in an element.

#### Values

This property should only be passed keywords. The possible values are;

- `left`
- `center`
- `right`
- `justify`


## Example

In the following code, a simple paragraph with Lorem Ipsum text is aligned using the above property declaration values.

<div id="code-heading">CSS</div>

```css
.parent-1 {
    height: 200px;
    background-color: #12f388;
}
.parent-1 p {
    background-color: #fff;
}
.left {
    text-align: left;
}
.right {
    text-align: right;
}
.center {
    text-align: center;
}
.justify {
    text-align: justify;
}
```

<div class="displayed_code_example">
    <style>
    .parent-1 {
        background-color: #12f388;
        padding: 1em;
        margin: 1em;
    }
    .parent-1 div {
        background-color: #fff;
        padding: 2em;
        margin: 1em;
    }
    .left {
        text-align: left;
    }
    .right {
        text-align: right;
    }
    .center {
        text-align: center;
    }
    .justify {
        text-align: justify;
    }
    </style>
    <div class="parent-1">
        <div class="left">
            <h2>Left</h2>
            <p>Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.</p> </div>
        <div class="right">
            <h2>Right</h2>
            <p>Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.</p> </div>
        <div class="center">
            <h2>Center</h2>
            <p>Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.</p> </div>
        <div class="justify">
            <h2>Justified</h2>
            <p>Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.Ex voluptate id veniam minim tempor deserunt adipisicing in nisi fugiat non laboris reprehenderit amet reprehenderit.</p> </div>
    </div>
</div>


| [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/tree/master/lectureCode/08/text-align-01/index.html) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/text-align-01/) |
