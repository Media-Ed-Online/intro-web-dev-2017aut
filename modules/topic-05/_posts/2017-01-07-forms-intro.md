---
title: Intro to Forms
module: 05
---

## Forms:<br />How to Collect Information from Visitors
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />
Forms and form elements are used by web developers to collect data & information from users on websites. This can include:

- drop down boxes (multiple choices)
- text entry (usernames, real names, phone numbers, e-mails, etc)
- radio checkmarks/buttons (select all-that-apply)
- password input (hidden text)
- buttons (used for submitting information and navigating to new pages)
- file uploads

We will not use forms very much this semester, as they inherently require a more robust language to handle their collection and transmission. This is one of the roles of **JavaScript**, which will be discussed more in the second Web course ("Web Technologies"). However, there are services which will allow us to create forms for websites that can do the front-end and back-end lifting/handling of the data.

The most common example of a form in use is a searchbox, such as Google or Bing.
![Example of the google homescreen and their infamous search box. Overlay text says: "A Google Search starts by placing data in a 'text box'."](../imgs/googleSearchBox.png "Example of the google homescreen and their infamous search box.")

### The Form Element
<p style="font-size: x-large"><span style="color: #79AF33; font-weight: bold;"><form</span> <span style="color: #999">action="#" method="..." id="..." class="..."</span> <span style="color: #79AF33; font-weight: bold;">></span> <span style="color: #999;">...</span> <span style="color: #79AF33; font-weight: bold;"></form></span></p>

To include a form in a webpage we must declare a form element section. This is simply accomplished by using the `<form>...</form>` tags.

Between these tags will be separate "form elements" such as "text boxes" and "buttons" that we will discuss in the proceeding pages.

### Form Attributes

The following are attributes that you should always include in a form element tag.

#### action
<p style="font-size: x-large"><span style="color: #999"><form</span> <span style="color: #79AF33; font-weight: bold;">action="#"</span> <span style="color: #999">method="..." id="..." class="..."> ... </form></span></p>

The `action` attribute is a link to a server-side script (i.e. a file on another computer, not the users computer). Typically this file is code file (php, javascript, python, java, etc) on a server that will do 'something' with the user data before returning information back to the browser.

The value of the action attribute will always be an URL.

#### method
<p style="font-size: x-large"><span style="color: #999"><form action="#"</span> <span style="color: #79AF33; font-weight: bold;">method="..."</span> <span style="color: #999">id="..." class="..."> ... </form></span></p>

Forms can be sent using one of two methods; '`get`' or '`post`'.

With the '`get`' method, values are added to the end of the specified action URL.

This methods is ideal for searches, or for _retrieving_ data from a server (as opposed to sending data that will be stored in a database).

With the '`post`' method, values are sent in what are known as 'HTTP headers'. As a rule of thumb, use the '`post`' method when;

- users are uploading a file.
- the data will be very long
- the data is sensitive (ie. contains passwords)
- The data is intended to alter or access a database on the server.

#### id & class
<p style="font-size: x-large"><span style="color: #999"><form action="#" method="..."</span> <span style="color: #79AF33; font-weight: bold;">id="..." class="..."</span><span style="color: #999">> ... </form></span></p>
As with many other elements in HTML, you should assign a unique element `id` and `class` that can be used by other languages to refer to the specific form.

### Altogether Now
<div id="code-heading">HTML</div>
```html
<form action="http://www.example.com/subscribe.php" method="get" id="subscribe-form" class="basic-forms">
    <!-- This is where the related form elements and controls will appear. -->
</form>
```


# { TODO: }
1. Read "[How does an HTML form work?](http://www.simfatic.com/forms/help/v40/how_does_an_html_form_work_.html)"
2. Read pages 144-150 of Chapter 07 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
