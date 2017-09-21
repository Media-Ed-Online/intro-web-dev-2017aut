---
title: Describing Structure
module: 04
---

## How HTML Describes the Structure of Pages:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

With HTML, a browser’s processor identifies _elements_ of the document by looking for _tags_ embedded directly in the text. These elements are then parsed into the _Document Object Model (DOM)_.

### Review of Elements and Tags

_Remember?_ An HTML document is composed of a tree of HTML **elements**. An element is an individual component of an HTML document. Elements denote to the processor structure and semantic meaning of the document. Elements may also be nested or encapsulated within other elements. Elements are identified through **tags**.

<div id="code-heading">HTML</div>
 ```html
 <p>This is a paragraph element, made with "<p>" tags.</p>
 ```

### <span style="color: #EF4A36; font-weight: bold">New!</span> Attributes

Attributes provide additional information about an HTML element. This may include information such as languages (US-English vs. French), URL links for text, the size to display a picture, or ways of identifying specific elements.

Attributes are always placed inside the opening tag for the element they refer to. Attributes are always provided in a key=“value” pair. The key is an identifier the the browser processor will recognize. These keys are defined by the W3 Consortium that defined HTML5 specification. The value provides information about the attribute.

The value is always surrounded by double quotations. One reason for this is that it allows for spaces to be used within the value for an attribute. Furthermore, the attribute will have one space placed between the tag label and the attribute, as well as between any subsequent attributes.

<div id="code-heading">HTML</div>
```html
<p lang="en-us">This is a paragraph element, made with "<p>" tags.<br/>
It is written in US-style English.</p>
```


# { TODO: }
1. Read pages 23-26 of Chapter 01 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
2. If you need a refresher, please review the _Elements_ and _Tags_ pages of [Topic-03](https://media-ed-online.github.io/intro-web-dev/modules/topic-03/basic-html/).
