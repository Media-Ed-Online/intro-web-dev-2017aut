---
title: Selector Types
module: 7
---

# Selector Types

There are multiple ways of selecting elements from an HTML page. This allows developers to use general selectors when a rule should apply to many elements, and specific selectors when a rule should only apply to a few or one element.

## Universal Selector

The Universal selector is used to style _every_ element on a page. The universal selector is the star (`*`). (The star is often used in computer science to mean "all").

```html
<style>

    * {
        font-family: monospace;
        background-color: pink;
    }

</style>

<div>An element</div>
<p>A paragraph element</p>
```

<div class="displayed_code_example all">
<style>

    .all, #all {
        font-family: monospace;
        background-color: pink;
    }

</style>

<div class="all">An element</div>
<p class="all">A paragraph element</p>
<h1 class="all" id="all">A Heading</h1>
</div>



## Element Selectors

The element selector is used to select all elements of a certain type. This selector is applied by simply using an element name (the reserved keyword placed in the opening tag of an element).

NOTE: This is the selector type that has been demonstrated the most so far in the last few pages.

So to select all level 2 headings we write `h2`. Then we could turn their text blue and make them quite large with style rules in the declaration block.


```html
<style>

    h2 {
        color: blue;
        font-size: 4em;
    }

</style>


<h1>Heading 1</h1>
<h2>BLUE HEADING</h2>
<h3>boring heading</h3>
<p>boring text</p>
<h2>EXCITING BLUE HEADING</h2>
```
<div class="displayed_code_example">
<style>
    .h2 {
        color: blue;
        font-size: 4em;
    }
</style>

<h1>Heading 1</h1>
<h2 class="h2">BLUE HEADING</h2>
<h3>boring heading</h3>
<p>boring text</p>
<h2 class="h2">EXCITING BLUE HEADING</h2>
</div>


## Class Selectors

Class names assigned to HTML elements via the `class=""` attribute can also be used to style elements. To select class elements, prepend a dot (`.`) to the front of the class name in the CSS.

Using class selectors is a great way to select elements that serve the same function.

```html
<style>

    .rad-info {
        color: #ff00fc;
        background-color: black;
        font-weight: bolder;
    }

    .boring-info {
        color: #6a6656;
        background-color: #b4a086;
    }

</style>

<div class="boring-info">
    Hey diddle diddle,
    The cat and the fiddle,
</div>
<div class="rad-info">
    The cow jumped over the moon.
</div>
<div class="wrong-info">
    The little dog laughed,
    To see such craft,<br />
    And the dish ran away with the spoon.
</div>
<div class="rad-info">
    The dish ran away with the spoon.
</div>
```

<div class="displayed_code_example">
<style>
    /*
    Notice that the class name matches the one given to
    two div elements below.
    Its prepended with a single dot. */
    .rad-info {
        color: #ff00fc;
        background-color: black;
        font-weight: bolder;
    }

    .boring-info {
        color: #6a6656;
        background-color: #b4a086;
    }

</style>

<div class="boring-info">
    Hey diddle diddle,
    The cat and the fiddle,
</div>
<div class="rad-info">
    The cow jumped over the moon.
</div>
<div class="wrong-info">
    The little dog laughed,
    To see such craft,<br />
    And the dish ran away with the spoon.
</div>
<div class="rad-info">
    The dish ran away with the spoon.
</div>
</div>


## ID Selector

Just like the class selector, the ID selector allows developers to define style rules for a specific element by calling its unique ID.

ID names are prepended with a number sign (`#`).

```html
<style>
    #para-3 {
        font-family: "Comic Sans MS" "Comic Sans" sans-serif;
        font-weight: bolder;
    }
</style>

<div class="car" id="para-1">I like cars</div>
<div class="car" id="para-2">No, I like trucks</div>
<div class="car" id="para-3">I like driving aimlessly</div>
```
<div class="displayed_code_example">
<style>
    #para-3 {
        font-family: "Comic Sans MS" "Comic Sans" sans-serif;
        font-weight: bolder;
    }
</style>

<div class="car" id="para-1">I like cars</div>
<div class="car" id="para-2">No, I like trucks</div>
<div class="car" id="para-3">I like driving aimlessly</div>
</div>
