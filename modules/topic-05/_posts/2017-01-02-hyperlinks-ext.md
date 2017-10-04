---
title: External Hyperlinks
module: 05
---

## Hyperlinks:<br />Introduction and Linking to External Sites
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />
One of the primary reasons for the Internet was to be able to easily reference research when citing others, with an ability to directly “link” to their work.

In computing, a hyperlink, or simply a link, is a reference to data that the reader can directly follow either by clicking, tapping, or hovering. A hyperlink points to a whole document or to a specific element within a document. Hypertext is text with hyperlinks. The text that is linked is called _anchor text_. A software system that is used for viewing and creating hypertext is a hypertext system, and to create a hyperlink is to hyperlink (or simply to link). A user following hyperlinks is said to navigate or browse the hypertext. [<sup>\[1]</sup>](https://en.wikipedia.org/wiki/Hyperlink "Wikipedia - Hyperlink")

#### Using Links
With links being such a basic and historical part of the Internet, they  also have a very simple tag; `<a>...</a>`. Any text between a hyperlink element’s tags will display as “hypertext”. Traditionally, this has been blue, underlined text, visually signifying to the user that the text is a <a href="#" style="color: blue; text-decoration: underline">link</a>.

In order to link to another document, the author must include a hyper-reference attribute within the opening tag. This attribute is signified with `href=""`.

<p data-height="200" data-theme-id="30567" data-slug-hash="aLWJpd" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-05: Links" class="codepen"></p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

#### A Word About Style
Link text should be specific about where the user will be going if they click a link. This means that links **should not** be simple text such as "[Click Me!](#)" Instead, good style would dictate that the link text be a description of the site, name, or information that informs the user.

#### Opening Links in a New Window
The `target` attribute provides us a way of specifying to a browser that a link should be opened in a new window.
In this case, the attributes value should be set to `"_blank".`

<p data-height="200" data-theme-id="30567" data-slug-hash="yzbMvB" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="Topic-05: Links Pt. 2" class="codepen"></p>

---

### External: Links to Other Sites
If you remember from [Topic-02](https://media-ed-online.github.io/intro-web-dev/modules/topic-02/urls/), links that include the “`http/https`” as part of the entire URL are known as **absolute URLs**.

Notice in the above link that it includes “`https`”. The “`https`” is required to signify to the browser that this is an ‘external’ link outside of the current document’s directory/server. **You must include either “`http`” or “`https`”.**

 The former is a older, established, version of the “hypertext transfer protocol”, which specified how data was sent between clients. The latter, is a “secure” version of this protocol. Whenever possible, you should provide “`https`” links (just check that they work first), as it provides a safer browsing experience.

 <p data-height="400" data-theme-id="30567" data-slug-hash="zEwMLb" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Intro-Web-Dev] Topic-05: Links Pt. 3" class="codepen"></p>

### E-mail
A very common type of hyperlinking is to create an e-mail link within a page. This is accomplished by prepending “`mailto:`” to the desired e-mail address. So, to create a hyperlink that e-mails me:

<p data-height="200" data-theme-id="30567" data-slug-hash="gGWQZm" data-default-tab="html,result" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Intro-Web-Dev] Topic-05: Links Pt. 4" class="codepen"></p>

Clicking on such a link in a webpage will cause the webpage to try and open the users default e-mail application.

For this reason, it is also good practice to write the full e-mail address out. That way a user can easily copy the address from the browser into the e-mail client of their choice.


# { TODO: }
Read pages 74-79 of Chapter 04 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
