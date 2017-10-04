---
title: Text Input
module: 05
---

## Text Input:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

The most common, and basic, "input" element type is `type="text"`.

This creates a "text box" where users can type in information that is available to the browser.

<p>
  <span style="color: #79AF33; font-weight: bold;">Type in this example text input element! </span>
  <input type="text" name="autofocus" id="test-autofocus" autofocus />
</p>


#### Plain Text Input Element

This following code demonstrates how to create an input element of `type="text"`. Please notice the use of the `<p>...</p>` element to display information text in front of the text box.

**NOTE:** Technically, you can omit the "type" from the input element if you want a text box. But good style dictates that you should be explicit in your code so as to prevent errors. So don't.

<p>
  <span style="color: #79AF33; font-weight: bold;">Your first name is:</span>
  <input type="text" name="name" id="test-text" />
</p>


#### Password Input Element

The `type="password"` for input elements creates a "password input box".

This attribute creates a single line text entry field where the characters are hidden with `*`s.

**NOTE:** You would never use this type of field to send sensitive data such as SSN's. For such situations, a site should create a web socket or use an Secure Socket Layer (SSL) connection with a server to guarantee secure delivery of data.

<p>
   <span style="color: #79AF33; font-weight: bold;">What's the magic word?</span>
   <input type="password" name="password" id="test-password" maxlength="5"/>
</p>


#### Textarea Input Element

The `textarea` input type can be used to create an input field element where users can enter longer responses.

**NOTE:** This field uses an opening and closing tag pair. Any text between these tags will initially inhabit the box.

<p style="color: #79AF33; font-weight: bold;">How are you feeling today?</p>
  <textarea name="comments" id="test-textarea" style="min-width:100%">
    I feel...
  </textarea>


### Altogether Now
<p data-height="600" data-theme-id="30567" data-slug-hash="pWPMzx" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Intro-Web-Dev] Topic-05: Text Input Elements" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

___

## Additional Elements

## autofocus

The `autofocus` attribute is used to set the "focus" of a browser to the specified form element after the page loads.

**NOTE:** Unlike most attributes, there is no "value" to assign. Therefore the attribute it passed in alone.

Refresh the page. See how the cursor is blinking inside the first example input box? This means it is "focused," and can take input right away.


### maxlength

The 'maxlength' attribute is used to limit the number of characters a user may enter into a text field. As an example, a text field that expects a year, may be limited to `maxlength="4"` characters.

**NOTE:** Type in the below text box. You will find (at least in most browsers) that you cannot type more than 4 characters.

<p>
  <span style="color: #79AF33; font-weight: bold;">Enter the last 4 digits of your Student ID:</span>
  <input type="text" name="dob" id="test-maxlength" maxlength="4" />
</p>


### cols & rows

You can specify the number of `cols` and `rows` through the appropriate attributes. This changes the size of the displayed element, as well as how text will look when typed.

- `cols` is the width of the textarea in character widths (i.e. this is the number of characters that will fit from left to right).
- `rows` is the number of visible lines.

**NOTE:** Typically, and as is the case with many size parameters that you can set in HTML, you should override these parameters with CSS. See the following code example.

<p>
  <span style="color: #79AF33; font-weight: bold;">Why should we consider you for the job?</span>
  <textarea name="comments" id="test-cols-rows" cols="20" rows="4" style="min-width:100%">
  Include qualifications, past experience, and references.
  </textarea>
</p>


### placeholder

The `placeholder` attribute can be used to place grey text in a text field. This text will disappear when the user focuses the element by clicking in it.

This text can be used to offer hints about the _type of text that is expected_ or to _encourage the user to type in the field_.

**NOTE:** Notice how the text box has grey text (should work in most browsers), and that when you click in there or begin typing it goes away.

<p>
  <span style="color: #79AF33; font-weight: bold;">What do you do for fun?</span>
  <input type="text" name="interests" id="test-placeholder" placeholder="Skiing, cooking, painting, juggling, etc." />
</p>


### size

You can use the `size` attribute to set the display (in character widths) for the text input box.

<p>
  <span style="color: #79AF33; font-weight: bold;">What do you do for fun?</span>
  <input type="text" name="interests" id="test-placeholder" placeholder="Skiing, cooking, painting, juggling, etc." size="30"/>
</p>


### value

The `value` attribute can be used to "pre-fill" a text box. Unlike `placeholder`, when you click in the text box, the "pre-filled" text is not replaced. Instead, the user can edit it freely, remove it, or keep it.

**NOTE:** This can be used to fill in "input" elements with data that would be used "most of the time".

<p>
  <span style="color: #79AF33; font-weight: bold;">What year were you born?</span>
  <input type="text" name="dob" id="test-maxlength" maxlength="4" value="19"/>
</p>


### Altogether Now, but _Better_
<p data-height="600" data-theme-id="30567" data-slug-hash="xXdvRw" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Intro-Web-Dev] Topic-05: Text Input Elements Pt. 2" class="codepen"></p>




# { TODO: }
Read pages 152-154 of Chapter 07 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
