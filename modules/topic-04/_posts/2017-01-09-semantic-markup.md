---
title: Semantic Markup
module: 04
---

## Its all in the Semantics:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

As discussed earlier, semantic markup changes the meaning and emphasis of written text. Just as with the structural markup elements just presented, semantic elements are included directly in the text document and are signified by tags that surround the text they apply to.

### Bold & Strong
One of the most common types of semantic markup is to **“bold”** some text. The element used for identifying bold text is `<b>...</b>`.

However, it is important to recognize that the use of **bold** text does not imply any extra meaning. For this reason, you are encouraged to use the **strong** element.

The use of a **strong** ( `<strong>...</strong>` ) element indicates that its content has strong importance. By default, browsers will show the contents of strong elements in bold.

<p data-height="300" data-theme-id="30567" data-slug-hash="rGOPKj" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-04: HTML Semantics Pt. 1" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


### Italic & Emphasis
Just like bold, another very common semantic alteration is the use of _italicized text_. Text can be marked up as italicized with the use of `<i>...</i>`.

As with bold/strong, italicized text does not necessarily imply semantically different meaning. Instead, you are encouraged to use the _”emphasis”_ element instead ( `<em>...</em>` ). The _emphasis_ element indicates subtle changes in the meaning of a sentence. By default the browser will show these elements in italic.

<p data-height="300" data-theme-id="30567" data-slug-hash="zEveXE" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-04: Semantic HTML Pt. 1" class="codepen"></p>


### Superscript & Subscript
The superscript ( `<sup>...</sup>` ) & subscript ( `<sub>...</sub>` ) elements are used to raise or lower text relative to normal text.

The superscript element is used to denote characters that should appear as 'superscript'; such as date suffixes or mathematical powers.

The subscript element is commonly used with footnotes or in mathematical and chemical formulas.

<p data-height="300" data-theme-id="30567" data-slug-hash="gGaqyJ" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-04: Semantic HTML Pt. 3" class="codepen"></p>


<h3 id="markup-list"> Other </h3>
Read the rest of Chapter 02 as asked in the **{ TODO: }** below. Please pay particular attention to the remaining semantic markup elements presented there that we are not discussing here. These include:

- <q>Block Quotes & Quotations</q> ( `<blockquote cite="">...</blockquote>`, `<q>...</q>` )
- <abbr title="Abbreviations and Acronyms take up too much space">Abbreviations & Acronyms</abbr> ( `<abbr title="">...</abbr>` )
- <cite>Citations</cite> ( `<cite>...</cite>` )
- <dfn>Definitions</dfn> ( `<dfn>...</dfn>` )
- Address ( `<address>... </address>` )
- <ins>Insert</ins> & <del>Delete</del> ( `<del>...</del> <ins>...</ins>` )
- <s>Strike-through</s>  ( `<s>...</s>` )

You are responsible for all of these in Project 2.


# { TODO: }
Read pages 45-61 of Chapter 02 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
