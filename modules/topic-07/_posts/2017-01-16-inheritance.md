---
title: Inheritance
module: 7
---

# Inheritance

Another crucial idea and concept in CSS is that or "inheritance".

Inheritance allows rules for certain aspects that are defined in parent elements to apply to all children elements.

For example, defining the text color and font family in the all selector (`* {}`) or HTML element selector (`html {}`), will define a base text color and font for the entire page (or until another more specific rule overwrites it).

<div id="code-heading">CSS</div>


```css
html {
    font-family: sans-serif;
    color: pink;
}
#other-paragraph {
    font-family: serif;
    color: black;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>


```html
<div class="container-box">
    <h1>A Heading, that is pink and without serifs.</h1>
    <p>
        Some Text, that is also pink and without serifs.
        <p>
            You should not nest paragraphs in other paragraphs.
            <p>
            But notice how the text color and font apply to all sub-children.
            </p>
        </p>
    </p>
    <h1>Another heading, so forth and so on.</h1>
    <p id="other-paragraph">
        A more Specific Selector overwrite this paragraph.
    </p>
</div>
```

<div class="displayed_code_example">
<style>
    .container-box {
        font-family: sans-serif;
        color: pink;
    }
    #other-paragraph {
        font-family: serif;
        color: black;
    }
</style>

<div class="container-box">
    <h1>A Heading, that is pink and without serifs.</h1>
    <p>
        Some Text, that is also pink and without serifs.
        <p>
            You should not nest paragraphs in other paragraphs.
            <p>
            But notice how the text color and font apply to all sub-children.
            </p>
        </p>
    </p>
    <h1>Another heading, so forth and so on.</h1>
    <p id="other-paragraph">
        A more Specific Selector overwrote this paragraph.
    </p>
</div>
</div>



## What Inherits

Not all properties will inherent their value from the parent element.

Text properties tend to inherit values from their parents, however, some properties do not. As with many things in web development, this is partly browser specific.

## Forcing Inheritance

If you are worried, or find a property that is not inheriting, you can for inheritance with the `inherit` keyword as the properties value.

<div id="code-heading">CSS</div>

```css
.parent-container {
    color: pink;
    background-color: black;
}
.child-container {
    background-color: inherit;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<div class="parent-container">
    <div class="child-container">
        <p>Notice that the black background color
            only applies to the outer &lt;div&gt; element.
            Not the child paragraph elements.</p>
        <p>Yet, the text color applies all...</p>
    </div>
</div>
```

<div class="displayed_code_example">
<style>
    .parent-container {
        color: pink;
        background-color: black;
    }
    .child-container {
        background-color: inherit;
    }
</style>

<div class="parent-container">
    <div class="child-container">
        <p>We are forcing the child-container &lt;div&gt; element to inherit whatever value its parent element has for background-color.
        </p>
        <p>We know, that the text color applies to all...</p>
    </div>
</div>
</div>



# { TODO: }

[- Read info on Inheritance and Cascading from w3.org](https://www.w3.org/wiki/Inheritance_and_cascade)

ALSO: Read Chapter 10 from the Duckett "Introducing CSS", which will re-cover everything discussed so far.
