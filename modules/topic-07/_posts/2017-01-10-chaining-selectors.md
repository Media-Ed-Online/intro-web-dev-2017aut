---
title: Chaining Selectors
module: 7
---

# Chaining Selectors

In addition to using a single selector, developers can also chain selectors to increase the specificity of their request.

## Direct Chaining

You can create a direct chain in CSS that tells the browser to grab a specific element. To do this, you simply place selectors together, without any spaces.

In the following example, the rule tells the browser to select all paragraph (`<p>`) elements with the class "secondary-description". NOTE: The use of the dot in the class selector.

```css
p.secondary-description {

}
```

## Descendant Selector

The descendant selector tells the browser to select all elements that are a descendant of the first.

To create a descendant selector, place spaces between each subsequent selector.

NOTE: The sub-level does not matter, only that the element hierarchically related to the first.

In the following example, only paragraph elements in the second div block are selected.

```html
<style>
    .block-two p {
        background-color: purple;
    }
</style>

<div class="block-one">
    <h1>A Heading</h1>
    <p>Some Text</p>
    <p>Some More Text</p>
</div>
<div class="block-two">
    <h1>Another Heading</h1>
    <p>Some Text</p>
    <h2>A Subheading</h2>
    <p>Some More Text</p>
    <p>M o o o r r r e e e e e . . . . .     text.</p>
</div>
```
<div class="displayed_code_example">
<style>
    .block-two p {
        color: white;
        background-color: purple;
    }
</style>

<div class="block-one">
    <h1>A Heading</h1>
    <p>Some Text</p>
    <p>Some More Text</p>
</div>
<div class="block-two">
    <h1>Another Heading</h1>
    <p>Some Text</p>
    <h2>A Subheading</h2>
    <p>Some More Text</p>
    <p>M o o o r r r e e e e e . . . . .     text.</p>
</div>
</div>



## Child Selector

The child selector tells the browser to select only the direct children of the parent element. To create a child selector chain, use the "greater than" operator between elements (`>`).

In the following example, the browser should only select the paragraph elements that are direct children of the div element "my-block". It ignores the paragraph element inside the div block "inner-block".

```html
<style>
    .my-block>p {
        color: white;
        background-color: purple;
    }
</style>

<div class="my-block">
    <p>Paragraph 1</p>
    <div class="inner-block">
        <p>Paragraph 2.1</p>
    </div>
    <p>Paragraph 3</p>
</div>
```

<div class="displayed_code_example">
<style>
    .my-block>p {
        color: white;
        background-color: purple;
    }
</style>

<div class="my-block">
    <p>Paragraph 1</p>
    <div class="inner-block">
        <p>Paragraph 2.1</p>
    </div>
    <p>Paragraph 3</p>
</div>
</div>


## Adjacent Sibling Selector

Use the plus sign (`+`) to create an adjacent sibling selector chain. This tells the browser to select the next element (and only the next element) that matches the search criteria.

```html
<style>
    h1+p {
        border: 1px solid purple;
    }
</style>

<p>Some text</p>
<h1>A Heading 1</h1>
<p>The selected element</p>
<p>Just a paragraph</p>
<h1>Another Heading 1</h1>
<p>Another selected element</p>
```

<div class="displayed_code_example">
<style>
    .h1+p {
        border: 1px solid purple;
    }
</style>

<p>Some text</p>
<h1 class="h1">A Heading 1</h1>
<p>The selected element</p>
<p>Just a paragraph</p>
<p>not selected</p>
<h1 class="h1">Another Heading 1</h1>
<p>Another selected element</p>
</div>


## General Sibling Selector

Use the tilda (`~`) sign to create a "general sibling" relationship between elements. This selects any elements that are siblings (i.e. at the same indention level) as the first element.

```html
<style>
    input~p {
        border: 2px dashed purple;
        background-color: yellow;
    }
</style>

<p>Some Text</p>
<p>Some Text</p>
<p>Some Text</p>
<input type="text" name="text1">
<p>Some Text</p>
<p>Some Text</p>
<p>Some Text</p>
<p>Some Text</p>
<input type="text" name="text2">
<p>Some Text</p>
```

<div class="displayed_code_example">
<style>
    input~p {
        border: 2px dashed purple;
        background-color: yellow;
    }
</style>

<p>Some Text</p>
<p>Some Text</p>
<p>Some Text</p>
<input type="text" name="text1">
<p>Some Text</p>
<p>Some Text</p>
<p>Some Text</p>
<p>Some Text</p>
<input type="text" name="text2">
<p>Some Text</p>
</div>
