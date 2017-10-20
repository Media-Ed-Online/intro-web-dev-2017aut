---
title: Chaining Selectors
module: 07
---

## Chaining Selectors:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

In addition to using a single selector, developers can also chain selectors to increase the specificity of their request.

### Direct Chaining

You can create a direct chain in CSS that tells the browser to grab a specific element. To do this, you simply place selectors together, without any spaces.

In the following example, the rule tells the browser to select all paragraph (`<p>`) elements with the class "secondary-description".

**NOTE:** The use of the dot (`.`) in the class selector.

<div id="code-heading">CSS</div>
```css
p.secondary-description {

}
```

### Descendant Selector

The descendant selector tells the browser to select all elements that are a descendant of the first.

To create a descendant selector, place spaces between each subsequent selector.

**NOTE:** The sub-level does not matter, only that the element is hierarchically related to the first.

In the following example, only paragraph elements in the second div block are selected.

<p data-height="400" data-theme-id="30567" data-slug-hash="MExyrG" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  Chaining Selectors, Pt. 1" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


### Child Selector

The child selector tells the browser to select only the direct children of the parent element. To create a child selector chain, use the "greater than" operator between elements (`>`).

In the following example, the browser should only select the paragraph elements that are direct children of the div element "my-block". It ignores the paragraph element inside the div block "inner-block".

<p data-height="400" data-theme-id="30567" data-slug-hash="PJLNQG" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  Chaining Selectors, Pt. 2" class="codepen"></p>


### Adjacent Sibling Selector

Use the plus sign (`+`) to create an adjacent sibling selector chain. This tells the browser to select the next element (and only the next element) that matches the search criteria.

<p data-height="400" data-theme-id="30567" data-slug-hash="OxqNvW" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  Chaining Selectors, Pt. 3" class="codepen"></p>


### General Sibling Selector

Use the tilda (`~`) sign to create a "general sibling" relationship between elements. This selects any elements that are siblings (i.e. at the same indention level) as the first element.

<p data-height="400" data-theme-id="30567" data-slug-hash="EwMKLr" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-07]  Chaining Selectors, Pt. 4" class="codepen"></p>


# { TODO: }
Read page 238 of Chapter 10 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
