---
title: Escape Characters
module: 06
---

## Escape Characters:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

As you may have discovered, HTML specifies that certain are "reserved" or serve a special purpose for browsers. The most obvious conflicts are the greater than and less than characters (`<`, `>`), since these identify tags to browsers in HTML. Any character that may be accidentally interpreted as markup by the browser _should_ be replaced with its escape code equivalent. There are also characters that have no easy "keyboard" equivalent, (such as the copyright symbol - &#169; ) in which case an escape code must be used.

<p style="margin-left: 30px;"><b>Question:</b> So what is a developer to do if they need to write some math (or something else less stressful than including comparison operators in their page)?</p>

<p style="margin-left: 30px;"><b>Answer:</b> Use special codes, known as escape characters, that the browser can use to render the intended character!</p>

This is not a fun process, but one that is necessary since HTML is a language.

**NOTE:** Also, for those of you who are more "security" minded or wanting to protect yourself and your client from "middle-man" attacks, using escape characters is critical, as evidence by [some discussions around the web](http://wonko.com/post/html-escaping).

### How-To

Escape codes always start with an ampersand (`&`) character followed by the individual code and finished with a semicolon (`;`).

### Character Code

All characters have a numerical, [decimal-based](https://www.w3schools.com/charsets/ref_utf_basic_latin.asp) (in addition to hexadecimal), value. In HTML, prepend decimal this value with the ampersand identifier as well as a number sign (`&#`).

Using escape character codes in HTML text is straight forward. Simply replace the character you want with its escape code equivalent in the text.

For example, we could write the word "CAT", by wrapping the individual letter's decimal values (67, 65, and 84) in the escape code values as;

<div id="code-heading">HTML</div>
```html
<h1>Where is the &#67;&#65;&#84; ?</h1>
```

<div class="displayed_code_example">
    <h1>Where is the &#67;&#65;&#84;?</h1>
</div>


### Entity Name

There are two ways of including an escape character in your HTML text. The first, mentioned above, simply utilizes the decimal based character code. This of course can be difficult to remember for the characters you may need.

Characters used often have special codes that are more "human readable", known as "entity names". For example, the less than and greater than characters (`<` & `>`) have entity names 'lt' and 'gt', respectively. To use an entity name, prepend it with the ampersand and appended with a semicolon. So to use `<` & `>` as actual characters in HTML write `&lt;` and `&gt;`.


### Common Escape Character Codes

These are some of the more commonly used escape code characters, along with their entity name and decimal code.

Symbol  | Name  | Entity Name   | Code
:------: | :----: | :-----------: | :----:
&#169; | Copyright | `&copy;` | `&#169;`
&#174; | Registered trademark | `&reg;` | `&#174;`
&#8482; | Trademark | `&trade;` | `&#8482;`
&#60; | Less than | `&lt;` | `&#60;`
&#62; | Greater than | `&gt;` | `&#62;`
&#38; | Ampersand | `&amp;` | `&#38;`
&#34; | Quotation mark | `&quot;` | `&#34;`
&cent; | Cent | `&cent;` | `&162;`
&pound; | Pound | `&pound;` | `&163;`
&curren; | Currency | `&curren;` | `&164;`
&yen; | Yen | `&yen;` | `&165;`
&euro; | Euro | `&euro;` | `&8364;`


#### Resources

- [List of Escape Character Codes](http://www.escapecodes.info)


# { TODO: }
Read pages 194-199 of Chapter 08 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
