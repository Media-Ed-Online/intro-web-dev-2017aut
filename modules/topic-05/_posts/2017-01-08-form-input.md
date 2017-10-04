---
title: Form Input Elements
module: 05
---

## Input Elements of Forms:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />
The "Input Element" is used to collect data from users. This is an element that you will likely use often as a web developer. The data collected by this element can be sent as part of a bunch of data in a form element to a server. This element can also be accessed through client-side JavaScript, allowing developers to create ways of getting data they can process on the client-computer.

### Attributes
<p style="font-size: x-large"><span style="color: #79AF33; font-weight: bold;"><input</span> <span style="color: #999">type="..." name="..." id="..."</span> <span style="color: #79AF33; font-weight: bold;">/></span></p>

The "input" element is an **empty elemen**t. Therefore, the element only requires a single tag (`<input />`).

#### type
<p style="font-size: x-large"><span style="color: #999"><input</span> <span style="color: #79AF33; font-weight: bold;">type="..."</span> <span style="color: #999">name="..." id="..." /></span></p>

By itself, the "input element" will not do anything. The input element requires the `type=""` to define the type of data it will collect, as well as how it will be displayed.

#### name
<p style="font-size: x-large"><span style="color: #999"><input type="..."</span> <span style="color: #79AF33; font-weight: bold;">name="..."</span> <span style="color: #999">id="..." /></span></p>

Each form control requires a `name=""` attribute. This information is sent as part of a "name:value" pair to the server.

For example, an "input element" with the name attribute set to "username" (i.e. `name="username"`) might collect the data "Justine", which would then be sent to the server as `username:Justine`.

#### id
<p style="font-size: x-large"><span style="color: #999"><input type="..." name="..."</span> <span style="color: #79AF33; font-weight: bold;">id="..."</span> <span style="color: #999">/></span></p>

As with many other elements in HTML, you should assign a unique element ID that can be used by other languages to refer to the specific form.

This `id` attribute allows JavaScript to use data from a form element. (This is of course in addition to the use of the `id` attribute by the styling engine; discussed later in the course.)

### Altogether Now
The following code shows an "input" element, wrapped in a "form" element, along with the three _required_ attributes.

<div id="code-heading">HTML</div>
```html
<form action="http://www.example.com/login.php" method="post" id="sign-in" class="basic-forms">
    <input type="text" name="username" id="username_input" />
</form>
```

# { TODO: }
Read page 151 of Chapter 07 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
