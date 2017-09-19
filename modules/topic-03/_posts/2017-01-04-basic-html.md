---
title: Basic HTML
module: 03
---

## Beginning in HTML
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

Let's just touch on using HTML or the **HyperText Markup Language.**

HTML is the standard markup language for creating web pages and web applications. HTML is a markup language that web browsers use to interpret and compose text, images, and other material into visual or audible web pages. HTML was first proposed in 1990 by Tim Berners-Lee, then a contract physicist at CERN.

For more info, quickly read [Amy Hisson's "History of HTML"](http://amyhissom.com/HTML5-CSS3/history.html#1).

### Elements & Tags
We will begin working in-depth with HTML in the next Topic. For now, I want you to just have basic understanding of how HTML renders.

HTML is a language that describes the structure of a document intended for viewing through a browser. The browser’s processor identifies _elements_ of the document by looking for _tags_ embedded directly in the text. These elements are then parsed into the _Document Object Model (DOM)_.

We can compare the basic structure of HTML to Markdown in the hierarchy of its elements. However, HTML is much more robust, and therefore needs more information to compile correctly.

#### Elements
An HTML document is composed of a tree of HTML elements. An **element** is an individual component of an HTML document. Elements denote to the processor structure and semantic meaning of the document. Elements may also be nested or encapsulated within other elements.

<div id="code-heading">HTML</div>
 ```html
 <p>This is a paragraph element.</p>
 ```

#### Tags
Elements are identified in a document through tags. A **tag** is code that is syntactically unique from the text content of the document. In HTML, all tags include a less-than (**<**) and greater-than (**>**) sign, with the tag typed between.

Most elements include an “opening” and “closing” tag that the processor uses to identify the beginning and end of the element with. Closing tags are identical to opening tags, except that they contain a forward-slash (**/**) between the less-than (**>**) sign and the tag text.

<div id="code-heading">HTML</div>
```html
<p>This is a paragraph element.
This element is created with an opening "<p>" tag and a closing "</p>" tag.
We call this wrapping.</p>
```

### Basic Structure and the Body
The most basic of structured documents should include tags identifying headings and paragraphs. These two markup elements are used in almost every document editing application and are crucial in authoring web content.

Everything a user sees on a web page lives in the **body element**. We'll get further into this soon, but for this _My First Web Page!_ just know you'll be working between the `<body>...</body>` tags.

##### Headings
Headings are defined with the `<h1>` to `<h6>` tags, and are written `<h1>...</h1>`.

`<h1>` defines the most important heading. `<h6>` defines the least important heading. `<h1` headings are considered to be _Main Headings_. While, `<h2>` headings are usually considered _sub-headings_ and so forth through `<h6>`.

By default, browsers will display headings with decreasing font size. Although, headings should instead be explicitly styled using CSS rules and definitions. This prevents any _un-expected_ rendering of the web document content.

##### Basic Paragraph
Any text between the paragraph tags `<p>...</p>` belongs to the same paragraph.

Almost all non-heading text will be placed within a paragraph element in a web document.

<p data-height="400" data-theme-id="30567" data-slug-hash="ZJZEXa" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-02: HTML Headings" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


# { TODO: }
Edit this Pen showing some basic HTML structure.

<p data-height="600" data-theme-id="30567" data-slug-hash="NvmWQv" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-02: HTML Structure Example" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>
