---
title: Body Elements
module: 04
---

## Elements in the Body:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

The _body element_ is where all of the “meat & potatoes” (if you will) of the site gets placed. This is the data that is rendered by the browser and displayed on the client's local computer.

Within the body there will generally be 2 types of markup used;

1. Structural markup
2. Semantic markup

### Structural Markup
Structural markup embeds information about the structure of a document. Structure includes elements such as:

- Headings
- Paragraphs
- Breaks
- Lists

These elements will help guide a user visually and provide information about the type of content through a document. These elements are also used by the browser and DOM to understand the content of a document. A browser will use this structural markup to assist [screen readers](http://www.afb.org/prodBrowseCatResults.aspx?CatID=49) and other accessibility-based software.


### Reveiw of Basic Structure and the Body
_Remember?_ The most basic of structured documents should include tags identifying headings and paragraphs. These two markup elements are used in almost every document editing application and are crucial in authoring web content.

##### Headings
Headings are defined with the `<h1>` to `<h6>` tags, and are written `<h1>...</h1>`.

`<h1>` defines the most important heading. `<h6>` defines the least important heading. `<h1` headings are considered to be _Main Headings_. While, `<h2>` headings are usually considered _sub-headings_ and so forth through `<h6>`.


##### Basic Paragraph
Any text between the paragraph tags `<p>...</p>` belongs to the same paragraph.

Almost all non-heading text will be placed within a paragraph element in a web document.

<p data-height="600" data-theme-id="30567" data-slug-hash="LzpqLO" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-04: HTML Body Elements" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


### Semantic Markup
Semantic markup us used to reinforce the [semantics](https://en.wikipedia.org/wiki/Semantics), or meaning, of the information in a document. Semantic markup might be used to place _emphasis_ on a word or phrase, identify a word as being **strong**, provide <cite>citations</cite> or <q>quotations</q>, link to <dfn>definitions</dfn>, or distinguish <del>editorial changes</del>.

More on semantic markup on the next page.


# { TODO: }
1. Read pages 26-39 of Chapter 01 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
2. Read pages 40-44 of Chapter 02 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
