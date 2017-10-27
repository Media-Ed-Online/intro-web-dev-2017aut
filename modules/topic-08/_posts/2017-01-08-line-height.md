---
title: Leading
module: 8
---

# Leading

As with any text based rendering engine, it is also possible to adjust many additional properties of how the text is displayed. We will examine a few of these over the next couple pages.

The first in question is known as _"leading"_ in typography. _Leading_ is the space between the top x-height of a font and the line of text above it.

We will refer to this more simply as "line height", as that is the css property which sets it (`line-height: `). The line hight property in CSS sets the vertical spacing between the lines of text.

As with font size, you can set the line height through a number of units; including absolute and relative. If desires, one can set the line height as an absolute pixel (px) value. However, you are encouraged to use a number, percent, or ems.


<br />


When you include a number, without any unit attached, the browser multiplies the current font size to set the line height.

This is equivalent to calling a percentage or em. So, the following are all the same;

```
line-height: 2;
line-height: 200%;
line-height: 2em;
```

For an example of using numbers, percentages, or ems visit;

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/line-height-01/line-height-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/line-height-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/line-height-01/) |



## What is an appropriate line height?

An appropriate line height, at its simplest, is one that encourages readability and understanding of the content.

However, in general, ideal leading ratios tend to be mentioned in the range of 1.2 - 1.45 times the text size. This is typically larger than the size of a horizontal space between words, which encourages the eyes movement along the line. But, not so large as to make text look separate from each other.

## Example

In the following example, each div element contains a h1 heading and paragraph, so that the line height can be evaluated. Each paragraph's first sentance mentiones that line height, then continues with [Lorem Ipsum](http://www.lipsum.com) (or dummy text).

Each paragraph is similar to;

<div id="code-heading">HTML</div>

```html
<div class="parent-1">
    <h1>1.45em</h1>
    <p class="p1">This is suppose to be the ideal line height at 1.45em. Ad nisi ea culpa cillum aliquip ad sit. Minim aliquip culpa occaecat consequat anim aute voluptate commodo dolore culpa nulla tempor ut. Irure sint incididunt nulla laborum occaecat sit labore nulla irure. Amet do exercitation proident in esse anim id velit proident dolore magna. Magna sit in voluptate commodo duis cupidatat esse duis ut exercitation deserunt mollit aliqua nulla.</p>
</div>
```

There are 6 paragraphs, with the following values for `line-height: `;

- 1.45em
- 1.0em
- 0.75em
- 0.1em
- 2.0em
- 4.0em

The result is as follows;

<!-- <div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:2000px;"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/08/line-height-02" frameborder="0" allowfullscreen></iframe></div>
</div> -->

<div class="displayed_code_example">
    <style>
    .main-container div {
        font-size: 1em;
        background-color: #dfc0ed;
        margin: 1em;
        padding: 1em;
    }
    .main-container div p {
        background-color: #fff;
        /*margin: 1em;*/
        padding: 1em;
    }
    .parent-1 .p1 {
        line-height: 1.45em;
    }

    .parent-2 .p1 {
        line-height: 1.0em;
    }

    .parent-3 .p1 {
        line-height: 0.75em;
    }

    .parent-4 .p1 {
        line-height: 0.1em;
    }

    .parent-5 .p1 {
        line-height: 2.0em;
    }

    .parent-6 .p1 {
        line-height: 4.0em;
    }
    </style>

    <div class="main-container">

        <div class="parent-1">
            <h1>1.45em</h1>
            <p class="p1">This is suppose to be the ideal line height at 1.45em. Ad nisi ea culpa cillum aliquip ad sit. Minim aliquip culpa occaecat consequat anim aute voluptate commodo dolore culpa nulla tempor ut. Irure sint incididunt nulla laborum occaecat sit labore nulla irure. Amet do exercitation proident in esse anim id velit proident dolore magna. Magna sit in voluptate commodo duis cupidatat esse duis ut exercitation deserunt mollit aliqua nulla.</p>
        </div>

        <div class="parent-2">
            <h1>1em</h1>
            <p class="p1">This is too tight at 1em. But is readable still. Ad nisi ea culpa cillum aliquip ad sit. Minim aliquip culpa occaecat consequat anim aute voluptate commodo dolore culpa nulla tempor ut. Irure sint incididunt nulla laborum occaecat sit labore nulla irure. Amet do exercitation proident in esse anim id velit proident dolore magna. Magna sit in voluptate commodo duis cupidatat esse duis ut exercitation deserunt mollit aliqua nulla.</p>
        </div>

        <div class="parent-3">
            <h1>0.75em</h1>
            <p class="p1">This is illegible at 0.75em. Ad nisi ea culpa cillum aliquip ad sit. Minim aliquip culpa occaecat consequat anim aute voluptate commodo dolore culpa nulla tempor ut. Irure sint incididunt nulla laborum occaecat sit labore nulla irure. Amet do exercitation proident in esse anim id velit proident dolore magna. Magna sit in voluptate commodo duis cupidatat esse duis ut exercitation deserunt mollit aliqua nulla.</p>
        </div>

        <div class="parent-4">
            <h1>0.1em</h1>
            <p class="p1">This is illegible at 0.1em. Ad nisi ea culpa cillum aliquip ad sit. Minim aliquip culpa occaecat consequat anim aute voluptate commodo dolore culpa nulla tempor ut. Irure sint incididunt nulla laborum occaecat sit labore nulla irure. Amet do exercitation proident in esse anim id velit proident dolore magna. Magna sit in voluptate commodo duis cupidatat esse duis ut exercitation deserunt mollit aliqua nulla.</p>
        </div>

        <div class="parent-5">
            <h1>2em</h1>
            <p class="p1">This is slightly too large at 2em. It is appropriate for some instances, but does not direct the eye in the same way. Ad nisi ea culpa cillum aliquip ad sit. Minim aliquip culpa occaecat consequat anim aute voluptate commodo dolore culpa nulla tempor ut. Irure sint incididunt nulla laborum occaecat sit labore nulla irure. Amet do exercitation proident in esse anim id velit proident dolore magna. Magna sit in voluptate commodo duis cupidatat esse duis ut exercitation deserunt mollit aliqua nulla.</p>
        </div>

        <div class="parent-6">
            <h1>4em</h1>
            <p class="p1">This is too large at 4em. It is appropriate for some instances, but does not direct the eye in the same way. Ad nisi ea culpa cillum aliquip ad sit. Minim aliquip culpa occaecat consequat anim aute voluptate commodo dolore culpa nulla tempor ut. Irure sint incididunt nulla laborum occaecat sit labore nulla irure. Amet do exercitation proident in esse anim id velit proident dolore magna. Magna sit in voluptate commodo duis cupidatat esse duis ut exercitation deserunt mollit aliqua nulla.</p>
        </div>
    </div>
</div>



To view this in a separate window, or to view the code;

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/line-height-02/line-height-02.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/08/line-height-02/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/line-height-02/) |
