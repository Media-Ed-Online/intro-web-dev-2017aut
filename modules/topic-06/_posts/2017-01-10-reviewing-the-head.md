---
title: Review the Head Element
module: 06
---

## More on the `<head>`:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

### The Language Reference

According to the World Wide Consortiums standards, you should include a language attribute (`lang=""`) inside the opening html tag of a document. This specifies the primary language of the site.

<div id="code-heading">HTML</div>
```html
<html lang="en">
```

You can view a list of [language codes on W3Schools](https://www.w3schools.com/tags/ref_language_codes.asp).


### Review the Head Element

Now that we are wrapping up our section on HTML, lets review the basic structure of the document and the elements that should populate the HTML page's head element.

#### Above `<head>`

As a reminder, the first line in your document should be a doctype declaration, in most cases, this should specify that the document is in HTML5.

<div id="code-heading">HTML</div>
```html
<!DOCTYPE html>
```

#### `<html>`

The next line in your document should be the opening `<html lang="en">` tag along with the ISO (International Organization for Standards) language code.

<div id="code-heading">HTML</div>
```html
<!DOCTYPE html>
<html lang="en">
  <!-- Head Elements -->
</html>
```

#### `<head>`

Following these, should be the `<head>` element. This should contain at a minimum a:

- `<meta charset="utf-8">`
- `<meta name="author" content="">`
- `<meta name="description" content="">`
- `<title>...</title>`


<h2 id="full-review">All Together Now</h2>

So the basic structure of your document along with metadata should look something like...

<div id="code-heading">HTML</div>
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="author" content="Justine Evans">
    <meta name="description" content="A Basic HTML Template">
    <title>Your Site's Title</title>
  </head>
  <body>
    <!-- Page Content -->
  </body>
</html>
```


# { TODO: }
Return to your Project 2 pages, and alter your beginning `<html>` tags to `<html lang=en">`. You should do this for:
- index.html
- instructions.html
- form.html
- about.html (upcoming)
- more-info.html (upcoming)
