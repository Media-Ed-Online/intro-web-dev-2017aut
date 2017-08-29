---
title: First Letter & First Line
module: 8
---

# First Letter & First Line

CSS includes a number of _pseudo_ things. The first type of pseudo thing we will discuss are "pseudo-elements".

Pseudo-elements allow for the selection of content, as if it were a separate element, without having to mark it up as such in the HTML.

Two pseudo elements that are made available with CSS are "first letter" and "first line". Respectively, these allow for the selection of the first letter or first line, in an element's text. This selection can then be used to alter the appearance or display of just the first letter or line.

The selectors for first letter and line are;

<div id="code-heading">CSS</div>

```css
selector::first-letter {}
selector::first-line {}
```

The word selector in the above is replaced with the normal CSS selectors used to identify elements.

## Example 1

In the following, the first letter and line of a div element are selected and altered.

<div id="code-heading">CSS</div>

```css
.text-element::first-letter {
    color: #ff19a3;
}
.text-element::first-line {
    background-color: #00baff;
}
```

<div class="displayed_code_example">
    <style>
        .text-element::first-letter {
            color: #ff19a3;
        }
        .text-element::first-line {
            background-color: #00baff;
        }
    </style>
    <div class="text-element">
    Do voluptate velit officia et voluptate cupidatat eiusmod nostrud consequat. Est dolore laborum eiusmod culpa ut exercitation nostrud Lorem in sint et tempor ea incididunt. In non irure pariatur in mollit id fugiat tempor dolore ut nisi minim irure aliqua anim. Irure dolore et cillum non culpa quis amet. </div>
</div>


## Example 2

In the following example, the same technique of using the first letter selector is applied to create a large letter, like might occur in a children's book.

<div id="code-heading">CSS</div>

```css
@import url('https://fonts.googleapis.com/css?family=Gentium+Book+Basic:400,700');

body {
    background-color: rgb(147, 12, 76);
}

.parent-container {
    padding: 1em;
}

.text-block {
    font-family: 'Gentium Book Basic', serif;
    font-weight: 400;
    font-size: 1.5em;
    padding: 1em;
    margin: 1em;
    background-color: #fff;
    text-indent: 1.5em;
    line-height: 1.5em;
}

/* Select the first paragraph child of .text-block */
.text-block p:first-child {
    text-indent: 0;
}

/* Select the first letter that occurs in the .text-block */
.text-block::first-letter {
    font-size: 4em;
    font-weight: 700;
    color: rgb(11, 44, 126);
    /*padding: 0.1em;*/
}
```


<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<div class="parent-container">
<div class="text-block">
    <p>Once upon a time, there was a great princess. She was fierce and protected the realm from the evils that be. Her name was Whataka GoGo. Along with her trusty sidekick, Pete the chocolate lab.</p>
    <p>One day the strong princess was attending a party, hosted by her dear friend Aspen. At this party all of the villages most enjoyable people had showed up.</p>
    <p> The Mayor was currently talking to Pete about his latest adventures with Whataka. Pete was boisterously regaling the mayor about their adventures to free a neighboring village from the attacking DerDarDuh's ...</p>
</div>
</div>
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:800px;"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/08/first-letter-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/first-letter-01/first-letter-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/first-letter-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/first-letter-01/) |
