---
title: Selection Input
module: 05
---

## Selection Input Types:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

Text can get messy. There are many ways to ask questions that allow users to select one or more of a handful of predetermined choices.

### Radio Buttons

Radio Buttons (`type="radio"`) allow users to select **one** item.

Radio buttons need to be grouped together. This tells the browser that only "one of the choices" of this group can be selected. To group radio button elements together the developer provides the same `name=""` attribute value for each possible choice. As with all elements, this name attribute will be sent along with the returned data.

Notice in the code example below, that this element, like the text box, will likely be placed in a `<p>...</p>`. This makes it easy to add information or "choice" text around the elements.

**NOTE:** A radio button set cannot be 'deselected'.

#### value (Required)

Unlike text boxes, where the user enters unique data, radio buttons provide discrete options/data. To set the data that might be returned from this element, use the `value=""` attribute. This is a required attribute for the checkbox element.

#### checked (Optional)

The `checked="checked"` attribute can be used with one of the radio button elements to 'pre-select' an option that will be displayed when the page loads.

<p data-height="400" data-theme-id="30567" data-slug-hash="oGwNqv" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Intro-Web-Dev] Topic-05: Selection Input Elements, Pt. 1" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

---

### The Checkbox Element
A `type="checkbox"` allows users to select (or deselect) zero, one, or more options.

#### value (Required)
When grouping checkboxes, as with 'radio buttons' the `name=""` should be the same for each element option, while the `value=""` should be unique to each element.

**NOTE:** Displayed text should appear AFTER each checkbox element.

#### checked (Optional)
As with radio buttons, you can use the `checked` attrubite to pre-select checkboxes.

<p data-height="400" data-theme-id="30567" data-slug-hash="wrevjd" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Intro-Web-Dev] Topic-05: Selection Input Elements, Pt. 1" class="codepen"></p>

---

### The Select Box (aka. Dropdown Select)

A select box allows a user to select one option from a dropdown list.

Unlike the other form elements we have been looking at, this element has its own name and uses opening and closing tags: `<select>...</select>`.

Dropdown lists are very similar to radio buttons. However, these are more appropriate when a large amount of selections is possible (i.e. "select a state").


#### The Option Element

The option element (`<option>...</option>`) is used within select elements to indicate each possible option. Any text between the option tags will be displayed in the dropdown box.

As with other form types, the `value=""` attribute should be unique for each option element. This will be sent back with the select elements name attribute.

#### selected (optional)
The `selected` attribute can be used to pre-select an option. If this attribute is omitted then the first option will be pre-selected.

<p data-height="400" data-theme-id="30567" data-slug-hash="WZONgX" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Intro-Web-Dev] Topic-05: Selection Input Elements, Pt. 3" class="codepen"></p>

# { TODO: }
Read pages 155-158 of Chapter 07 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
