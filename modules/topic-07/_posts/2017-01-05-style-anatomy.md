---
title: Selectors and Declarations
module: 7
---

# Selectors and Declarations

To "style" content in your HTML document you write style "rules" that apply to elements. These rules will always follow the same patterns.

## Selector

The first part of every rule is a "selector" which tells the browser what element/s the rule applies to. This is followed by a space, then a block, delineated with curly brackets.

```css
/*
⬇ selector - selects all h1 elements */
h1 {
    /* Style declarations go inside curly brackets. */
}
```

## Declaration

The portion of the rule delineated by the curly brackets is known as the declaration. This tells the browser what to do to the selected element/s.


## Multiple Selectors with different rules

When applying different rules to elements, you simply need to write another selector/declaration set. The closing curly bracket (`}`) tells the browser the rule is finished.

NOTE: CSS is not whitespace dependent. In other words, you do not need to include extra lines between rules. However, this shown style increases readability of your code.

```css
/* Rule 1. Applied to all h1 elements */
h1 {
    /* Style declarations */
}

/* Rule 2. Applied to all paragraphs */
p {
    /* Style declarations */
}
```

## Multiple Selectors with the Same Rules

If you need to apply the same rules to more than one element, you can select multiple elements in a single style rule. To do so, separate each selector element with a comma (`,`).

You can then still go on to apply additional, unique style rules to an already styled element. These rules will simply be cumulative.

```css
h1, h2, p {
    /* Style Rules applied to all h1, h2, and paragraph elements. */
}

p {
    /* Additional style rules applied only to paragraph elements. */
}
```
